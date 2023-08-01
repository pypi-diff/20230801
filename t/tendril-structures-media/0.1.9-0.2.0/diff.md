# Comparing `tmp/tendril-structures-media-0.1.9.tar.gz` & `tmp/tendril-structures-media-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-structures-media-0.1.9.tar", last modified: Tue Jul 25 12:00:40 2023, max compression
+gzip compressed data, was "tendril-structures-media-0.2.0.tar", last modified: Tue Aug  1 15:40:10 2023, max compression
```

## Comparing `tendril-structures-media-0.1.9.tar` & `tendril-structures-media-0.2.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.890595 tendril-structures-media-0.1.9/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.1.9/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-25 12:00:40.890595 tendril-structures-media-0.1.9/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.874595 tendril-structures-media-0.1.9/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.874595 tendril-structures-media-0.1.9/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.1.9/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-25 12:00:40.890595 tendril-structures-media-0.1.9/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.1.9/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.870595 tendril-structures-media-0.1.9/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.9/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/routers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    11648 2023-07-06 20:23:55.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/templates/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.1.9/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/common/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.1.9/src/tendril/common/content/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.1.9/src/tendril/common/content/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.1.9/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.1.9/src/tendril/config/media.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.9/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.1.9/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5991 2023-07-22 21:26:24.000000 tendril-structures-media-0.1.9/src/tendril/db/controllers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.9/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7326 2023-07-25 11:56:15.000000 tendril-structures-media-0.1.9/src/tendril/db/models/content.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4118 2023-07-23 04:19:22.000000 tendril-structures-media-0.1.9/src/tendril/db/models/content_formats.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.1.9/src/tendril/db/models/content_thumbnails.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.1.9/src/tendril/interests/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.1.9/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17585 2023-07-25 12:00:04.000000 tendril-structures-media-0.1.9/src/tendril/interests/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.1.9/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.1.9/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1015 2023-07-14 16:11:05.000000 tendril-structures-media-0.1.9/src/tendril/libraries/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/structures/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.1.9/src/tendril/structures/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/structures/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.2.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.141319 tendril-structures-media-0.2.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.2.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.2.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.137319 tendril-structures-media-0.2.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/routers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11648 2023-07-06 20:23:55.000000 tendril-structures-media-0.2.0/src/tendril/apiserver/templates/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.2.0/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/common/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.2.0/src/tendril/common/content/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.2.0/src/tendril/common/content/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.2.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.2.0/src/tendril/config/media.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.0/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.2.0/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5991 2023-07-22 21:26:24.000000 tendril-structures-media-0.2.0/src/tendril/db/controllers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.2.0/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7474 2023-08-01 15:34:46.000000 tendril-structures-media-0.2.0/src/tendril/db/models/content.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4112 2023-07-26 19:25:19.000000 tendril-structures-media-0.2.0/src/tendril/db/models/content_formats.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.2.0/src/tendril/db/models/content_thumbnails.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.2.0/src/tendril/interests/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.2.0/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17742 2023-08-01 15:38:36.000000 tendril-structures-media-0.2.0/src/tendril/interests/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.2.0/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.2.0/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1015 2023-07-14 16:11:05.000000 tendril-structures-media-0.2.0/src/tendril/libraries/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/structures/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.2.0/src/tendril/structures/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/structures/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.145319 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.2.0/src/tendril/structures/content/providers/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-01 15:40:10.000000 tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 15:40:10.149319 tendril-structures-media-0.2.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.2.0/tox.ini
```

### Comparing `tendril-structures-media-0.1.9/.gitignore` & `tendril-structures-media-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/.readthedocs.yml` & `tendril-structures-media-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/.travis.yml` & `tendril-structures-media-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/LICENSE` & `tendril-structures-media-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/PKG-INFO` & `tendril-structures-media-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.1.9
+Version: 0.2.0
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.1.9/README.rst` & `tendril-structures-media-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/Makefile` & `tendril-structures-media-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/_static/custom.css` & `tendril-structures-media-0.2.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/_static/favicon.ico` & `tendril-structures-media-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/_static/logo.png` & `tendril-structures-media-0.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/_static/logo_packed.png` & `tendril-structures-media-0.2.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/_templates/about.html` & `tendril-structures-media-0.2.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/conf.py` & `tendril-structures-media-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/index.rst` & `tendril-structures-media-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/docs/installation.rst` & `tendril-structures-media-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/setup.py` & `tendril-structures-media-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/apiserver/templates/content.py` & `tendril-structures-media-0.2.0/src/tendril/apiserver/templates/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/common/content/exceptions.py` & `tendril-structures-media-0.2.0/src/tendril/common/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/config/__init__.py` & `tendril-structures-media-0.2.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/config/media.py` & `tendril-structures-media-0.2.0/src/tendril/config/media.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/db/controllers/content.py` & `tendril-structures-media-0.2.0/src/tendril/db/controllers/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/db/models/content.py` & `tendril-structures-media-0.2.0/src/tendril/db/models/content.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import List
 from typing import Union
 from typing import Optional
 from sqlalchemy import Column
 from sqlalchemy import String
 from sqlalchemy import Integer
 from sqlalchemy import ForeignKey
-from sqlalchemy import UniqueConstraint
 from sqlalchemy.orm import Mapped
 from sqlalchemy.orm import mapped_column
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy_json import mutable_json_type
 
@@ -78,15 +77,15 @@
     sequence_usages: Mapped[List["SequenceContentAssociationModel"]] = relationship()
 
     __mapper_args__ = {
         "polymorphic_identity": type_name,
         "polymorphic_on": content_type
     }
 
-    def export(self, full=False):
+    def export(self, full=False, explicit_durations_only=False):
         rv = {'content_type': self.content_type,
               'estimated_duration': self.estimated_duration()}
         if self.bg_color:
             rv['bg_color'] = self.bg_color
         return rv
 
     def is_usable(self):
@@ -107,16 +106,16 @@
     def formats(cls):
         return relationship(MediaContentFormatModel, back_populates="content", lazy="selectin")
 
     __mapper_args__ = {
         "polymorphic_identity": type_name
     }
 
-    def export(self, full=False):
-        rv = super(MediaContentModel, self).export(full=full)
+    def export(self, full=False, explicit_durations_only=False):
+        rv = super(MediaContentModel, self).export(full=full, explicit_durations_only=explicit_durations_only)
         rv['formats'] = [x.export(full=full) for x in self.formats]
         for fmt in self.formats:
             if len(fmt.thumbnails):
                 rv['thumbnails'] = fmt.export_thumbnails()
                 break
         return rv
 
@@ -126,15 +125,15 @@
         step_durations = [x for x in durations if x < 0]
         if not len(simple_durations) and not len(step_durations):
             return 0
         if not len(step_durations):
             return max(simple_durations)
         if not len(simple_durations):
             return min(step_durations)
-        step_durations = [x * -1 * 10000 for x in step_durations]
+        step_durations = [x * -1 * 10 for x in step_durations]
         return max(simple_durations + step_durations)
 
     def is_usable(self):
         return len(self.formats) > 0
 
 
 class StructuredContentModel(ContentModel):
@@ -145,16 +144,16 @@
     path = Column(String(64))
     args = Column(mutable_json_type(dbtype=JSONB))
 
     __mapper_args__ = {
         "polymorphic_identity": type_name
     }
 
-    def export(self, full=False):
-        rv = super(StructuredContentModel, self).export(full=full)
+    def export(self, full=False, explicit_durations_only=False):
+        rv = super(StructuredContentModel, self).export(full=full, explicit_durations_only=explicit_durations_only)
         rv['path'] = self.path
         if self.args:
             rv['args'] = self.args
         return rv
 
     def estimated_duration(self):
         return None
@@ -165,44 +164,40 @@
 
 
 class SequenceContentModel(ContentModel):
     type_name = 'sequence'
     type_description = "Sequence of other content types"
 
     id = Column(Integer, ForeignKey("Content.id"), primary_key=True)
-    default_duration = Column(Integer, nullable=False, default=10000)
+    default_duration = Column(Integer, nullable=False, default=10)
 
     contents: Mapped[List["SequenceContentAssociationModel"]] = \
         relationship(order_by="SequenceContentAssociationModel.position")
 
     __mapper_args__ = {
         "polymorphic_identity": type_name
     }
 
-    def export(self, full=False):
-        rv = super(SequenceContentModel, self).export(full=full)
+    def export(self, full=False, explicit_durations_only=False):
+        rv = super(SequenceContentModel, self).export(full=full, explicit_durations_only=explicit_durations_only)
         rv['default_duration'] = self.default_duration
-        rv['contents'] = [x.export(full=full) for x in self.contents]
+        rv['contents'] = [x.export(full=full, explicit_durations_only=explicit_durations_only) for x in self.contents]
         return rv
 
     def estimated_duration(self):
         durations = [x.duration or x.content.estimated_duration() for x in self.contents]
         actual_durations = []
         for duration in durations:
             if duration < 0:
-                padding = 0
-                if duration != -1:
-                    padding = (-1 - duration) * 1000
-                duration = self.default_duration * -1 * duration + padding
-
+                duration = self.default_duration * -1 * duration
             actual_durations.append(duration)
-        return sum(actual_durations) + 1000 * len(durations)
+        return sum(actual_durations) + len(durations)
 
     def is_usable(self):
-        return len(self.contents) > 0 and all([x.is_usable() for x in self.contents])
+        return len(self.contents) > 0 and all([x.content.is_usable() for x in self.contents])
 
 
 class SequenceContentAssociationModel(DeclBase):
     __tablename__ = "SequenceContentAssociation"
     sequence_id: Mapped[int] = mapped_column(ForeignKey("SequenceContent.id"), primary_key=True)
     content_id: Mapped[int] = mapped_column(ForeignKey("Content.id"))
     position: Mapped[int] = mapped_column(primary_key=True)
```

### Comparing `tendril-structures-media-0.1.9/src/tendril/db/models/content_formats.py` & `tendril-structures-media-0.2.0/src/tendril/db/models/content_formats.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,18 +84,18 @@
         if full:
             rv['thumbnails'] = self.export_thumbnails()
         return rv
 
     def estimated_duration(self):
         if self.duration:
             if self.duration < 0:
-                return self.duration * -10000
+                return self.duration * -10
             return self.duration
         else:
-            return 10000
+            return 10
 
     __mapper_args__ = {
         "polymorphic_identity": format_class_name,
         "polymorphic_on": format_class
     }
```

### Comparing `tendril-structures-media-0.1.9/src/tendril/db/models/content_thumbnails.py` & `tendril-structures-media-0.2.0/src/tendril/db/models/content_thumbnails.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/interests/mixins/content.py` & `tendril-structures-media-0.2.0/src/tendril/interests/mixins/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
         if not self.model_instance.status == LifecycleStatus.ACTIVE:
             return result, msg
 
         publishable = self.publishable()
 
         if background_tasks:
-            background_tasks.add_task(self._publish_files(publishable))
+            background_tasks.add_task(self._publish_files, publishable)
         else:
             asyncio.ensure_future(self._publish_files(publishable))
         return result, msg
 
     async def _publish_files(self, stored_files):
         for stored_file in stored_files:
             logger.info(f"Publishing file {stored_file.filename}")
@@ -389,18 +389,21 @@
 
         # Get Content and Verify Access
         content = get_interest(content_id, type=self.type_name, session=session).actual
         if not content.check_user_access(auth_user, 'read', session=session):
             raise PermissionError("User does not seem to have access to the underlying content. "
                                   "Cannot add to sequence.")
 
-        if not duration:
-            duration = content.estimated_duration(auth_user=auth_user, session=session)
+        if not content.status == LifecycleStatus.ACTIVE:
+            raise ValueError("The content must be active before it can be added to a sequence.")
 
         if not duration:
+            _duration = content.estimated_duration(auth_user=auth_user, session=session)
+
+        if not _duration:
             raise ValueError("We need a duration, however none is provided and the content does "
                              "not provide it intrinsically.")
 
         # Create and commit Association Model
         sequence_add_content(id=self.model_instance.content_id,
                              content=content.model_instance.content_id,
                              position=position,
```

### Comparing `tendril-structures-media-0.1.9/src/tendril/libraries/mixins/content.py` & `tendril-structures-media-0.2.0/src/tendril/libraries/mixins/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/structures/content/providers/base.py` & `tendril-structures-media-0.2.0/src/tendril/structures/content/providers/base.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril/structures/content/providers/manager.py` & `tendril-structures-media-0.2.0/src/tendril/structures/content/providers/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/PKG-INFO` & `tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.1.9
+Version: 0.2.0
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/SOURCES.txt` & `tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/requires.txt` & `tendril-structures-media-0.2.0/src/tendril_structures_media.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/tests/coveralls.py` & `tendril-structures-media-0.2.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.9/tox.ini` & `tendril-structures-media-0.2.0/tox.ini`

 * *Files identical despite different names*

