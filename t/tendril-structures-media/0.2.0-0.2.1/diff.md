# Comparing `tmp/tendril-structures-media-0.2.0.tar.gz` & `tmp/tendril-structures-media-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-structures-media-0.2.0.tar", last modified: Tue Aug  1 15:40:10 2023, max compression
+gzip compressed data, was "tendril-structures-media-0.2.1.tar", last modified: Tue Aug  1 18:10:27 2023, max compression
```

## Comparing `tendril-structures-media-0.2.0.tar` & `tendril-structures-media-0.2.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.2.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.141319 tendril-structures-media-0.2.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.2.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.2.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.137319 tendril-structures-media-0.2.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/routers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    11648 2023-07-06 20:23:55.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/templates/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.2.0/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/common/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.2.0/src/tendril/common/content/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.2.0/src/tendril/common/content/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.2.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.2.0/src/tendril/config/media.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.0/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.2.0/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5991 2023-07-22 21:26:24.000000 tendril-structures-media-0.2.0/src/tendril/db/controllers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.0/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7474 2023-08-01 15:34:46.000000 tendril-structures-media-0.2.0/src/tendril/db/models/content.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4112 2023-07-26 19:25:19.000000 tendril-structures-media-0.2.0/src/tendril/db/models/content_formats.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.2.0/src/tendril/db/models/content_thumbnails.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.2.0/src/tendril/interests/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.2.0/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17742 2023-08-01 15:38:36.000000 tendril-structures-media-0.2.0/src/tendril/interests/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.2.0/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.2.0/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1015 2023-07-14 16:11:05.000000 tendril-structures-media-0.2.0/src/tendril/libraries/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/structures/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.2.0/src/tendril/structures/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/structures/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.726333 tendril-structures-media-0.2.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.2.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-08-01 18:10:27.726333 tendril-structures-media-0.2.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.2.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-01 18:10:27.726333 tendril-structures-media-0.2.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.2.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.718334 tendril-structures-media-0.2.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.2.1/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.2.1/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.2.1/src/tendril/apiserver/routers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.2.1/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11648 2023-07-06 20:23:55.000000 tendril-structures-media-0.2.1/src/tendril/apiserver/templates/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.2.1/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/common/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.2.1/src/tendril/common/content/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.2.1/src/tendril/common/content/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.2.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.2.1/src/tendril/config/media.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.1/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.2.1/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5991 2023-07-22 21:26:24.000000 tendril-structures-media-0.2.1/src/tendril/db/controllers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.1/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7505 2023-08-01 18:10:02.000000 tendril-structures-media-0.2.1/src/tendril/db/models/content.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4112 2023-07-26 19:25:19.000000 tendril-structures-media-0.2.1/src/tendril/db/models/content_formats.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.2.1/src/tendril/db/models/content_thumbnails.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.2.1/src/tendril/interests/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.2.1/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17742 2023-08-01 15:38:36.000000 tendril-structures-media-0.2.1/src/tendril/interests/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.2.1/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.2.1/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1015 2023-07-14 16:11:05.000000 tendril-structures-media-0.2.1/src/tendril/libraries/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/structures/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.2.1/src/tendril/structures/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.722334 tendril-structures-media-0.2.1/src/tendril/structures/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.2.1/src/tendril/structures/content/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.726333 tendril-structures-media-0.2.1/src/tendril/structures/content/providers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.2.1/src/tendril/structures/content/providers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.2.1/src/tendril/structures/content/providers/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.2.1/src/tendril/structures/content/providers/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.726333 tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-08-01 18:10:27.000000 tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-08-01 18:10:27.000000 tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-01 18:10:27.000000 tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-08-01 18:10:27.000000 tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-01 18:10:27.000000 tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 18:10:27.726333 tendril-structures-media-0.2.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.1/tox.ini
```

### Comparing `tendril-structures-media-0.2.0/.gitignore` & `tendril-structures-media-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/.readthedocs.yml` & `tendril-structures-media-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/.travis.yml` & `tendril-structures-media-0.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/LICENSE` & `tendril-structures-media-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/PKG-INFO` & `tendril-structures-media-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.2.0
+Version: 0.2.1
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.2.0/README.rst` & `tendril-structures-media-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/Makefile` & `tendril-structures-media-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/_static/custom.css` & `tendril-structures-media-0.2.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/_static/favicon.ico` & `tendril-structures-media-0.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/_static/logo.png` & `tendril-structures-media-0.2.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/_static/logo_packed.png` & `tendril-structures-media-0.2.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/_templates/about.html` & `tendril-structures-media-0.2.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/conf.py` & `tendril-structures-media-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/index.rst` & `tendril-structures-media-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/docs/installation.rst` & `tendril-structures-media-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/setup.py` & `tendril-structures-media-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/apiserver/templates/content.py` & `tendril-structures-media-0.2.1/src/tendril/apiserver/templates/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/common/content/exceptions.py` & `tendril-structures-media-0.2.1/src/tendril/common/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/config/__init__.py` & `tendril-structures-media-0.2.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/config/media.py` & `tendril-structures-media-0.2.1/src/tendril/config/media.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/db/controllers/content.py` & `tendril-structures-media-0.2.1/src/tendril/db/controllers/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/db/models/content.py` & `tendril-structures-media-0.2.1/src/tendril/db/models/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,13 +201,13 @@
     sequence_id: Mapped[int] = mapped_column(ForeignKey("SequenceContent.id"), primary_key=True)
     content_id: Mapped[int] = mapped_column(ForeignKey("Content.id"))
     position: Mapped[int] = mapped_column(primary_key=True)
     duration: Mapped[Optional[int]]
     sequence: Mapped[SequenceContentModel] = relationship(back_populates="contents", foreign_keys=[sequence_id], lazy='selectin')
     content: Mapped[ContentModel] = relationship(back_populates="sequence_usages", foreign_keys=[content_id], lazy='joined')
 
-    def export(self, full=False):
+    def export(self, full=False, explicit_durations_only=False):
         return {
             'position': self.position,
             'duration': self.duration,
             'content': self.content.export(full=full)
         }
```

### Comparing `tendril-structures-media-0.2.0/src/tendril/db/models/content_formats.py` & `tendril-structures-media-0.2.1/src/tendril/db/models/content_formats.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/db/models/content_thumbnails.py` & `tendril-structures-media-0.2.1/src/tendril/db/models/content_thumbnails.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/interests/mixins/content.py` & `tendril-structures-media-0.2.1/src/tendril/interests/mixins/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/libraries/mixins/content.py` & `tendril-structures-media-0.2.1/src/tendril/libraries/mixins/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/structures/content/providers/base.py` & `tendril-structures-media-0.2.1/src/tendril/structures/content/providers/base.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril/structures/content/providers/manager.py` & `tendril-structures-media-0.2.1/src/tendril/structures/content/providers/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/PKG-INFO` & `tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.2.0
+Version: 0.2.1
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/SOURCES.txt` & `tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/requires.txt` & `tendril-structures-media-0.2.1/src/tendril_structures_media.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/tests/coveralls.py` & `tendril-structures-media-0.2.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.2.0/tox.ini` & `tendril-structures-media-0.2.1/tox.ini`

 * *Files identical despite different names*

