# Comparing `tmp/T3SF-2.5rc2.tar.gz` & `tmp/T3SF-2.5rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "T3SF-2.5rc2.tar", last modified: Tue Aug  1 20:39:07 2023, max compression
+gzip compressed data, was "T3SF-2.5rc3.tar", last modified: Tue Aug  1 20:55:15 2023, max compression
```

## Comparing `T3SF-2.5rc2.tar` & `T3SF-2.5rc3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.362268 T3SF-2.5rc2/
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.5rc2/LICENSE
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       33 2023-08-01 20:26:56.000000 T3SF-2.5rc2/MANIFEST.in
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6508 2023-08-01 20:39:07.362268 T3SF-2.5rc2/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5855 2023-07-18 16:44:35.000000 T3SF-2.5rc2/README.md
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-08-01 20:39:07.362268 T3SF-2.5rc2/setup.cfg
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-08-01 20:38:57.000000 T3SF-2.5rc2/setup.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.354268 T3SF-2.5rc2/src/
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.354268 T3SF-2.5rc2/src/T3SF/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14998 2023-07-14 15:39:52.000000 T3SF-2.5rc2/src/T3SF/T3SF.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-06-27 20:32:45.000000 T3SF-2.5rc2/src/T3SF/__init__.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.354268 T3SF-2.5rc2/src/T3SF/discord/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-06-07 19:56:31.000000 T3SF-2.5rc2/src/T3SF/discord/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7356 2023-06-07 19:56:31.000000 T3SF-2.5rc2/src/T3SF/discord/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10481 2023-07-14 15:49:41.000000 T3SF-2.5rc2/src/T3SF/discord/discord.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.354268 T3SF-2.5rc2/src/T3SF/gui/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-06-07 19:56:31.000000 T3SF-2.5rc2/src/T3SF/gui/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    15747 2023-08-01 20:37:30.000000 T3SF-2.5rc2/src/T3SF/gui/core.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.354268 T3SF-2.5rc2/src/T3SF/gui/static/
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.354268 T3SF-2.5rc2/src/T3SF/gui/static/imgs/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6417 2023-07-11 23:06:46.000000 T3SF-2.5rc2/src/T3SF/gui/static/imgs/icon.png
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6790 2023-06-27 17:01:48.000000 T3SF-2.5rc2/src/T3SF/gui/static/imgs/logo-dark.png
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7387 2023-06-27 17:01:32.000000 T3SF-2.5rc2/src/T3SF/gui/static/imgs/logo-light.png
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.358268 T3SF-2.5rc2/src/T3SF/gui/static/js/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1310 2023-06-27 20:44:06.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/bootstrap_toasts.js
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      784 2023-06-09 19:28:29.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/copy.js
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     2133 2023-07-18 17:02:36.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/theme_switcher.js
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.362268 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)    91322 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/CHANGELOG.md
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)      740 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/LICENSE.md
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)     7034 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/README.md
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)      210 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/SECURITY.md
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)   752111 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/index.d.ts
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)  1305579 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)  5701941 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js.map
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)     1031 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/package.json
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.362268 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)     4197 2023-06-27 19:55:09.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-dark.css
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)     6561 1985-10-26 08:15:00.000000 T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-default.css
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)   217088 2023-07-11 00:15:04.000000 T3SF-2.5rc2/src/T3SF/gui/t3sf.sqlite3
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.362268 T3SF-2.5rc2/src/T3SF/gui/templates/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    16629 2023-07-24 20:40:01.000000 T3SF-2.5rc2/src/T3SF/gui/templates/base.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5069 2023-06-28 00:10:12.000000 T3SF-2.5rc2/src/T3SF/gui/templates/env_creation.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14588 2023-07-11 23:14:57.000000 T3SF-2.5rc2/src/T3SF/gui/templates/index.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    27402 2023-07-14 15:40:11.000000 T3SF-2.5rc2/src/T3SF/gui/templates/msel_playground.html
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.362268 T3SF-2.5rc2/src/T3SF/logger/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-06-07 19:56:31.000000 T3SF-2.5rc2/src/T3SF/logger/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1348 2023-07-14 15:39:57.000000 T3SF-2.5rc2/src/T3SF/logger/logger.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.362268 T3SF-2.5rc2/src/T3SF/slack/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-06-07 19:56:31.000000 T3SF-2.5rc2/src/T3SF/slack/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7129 2023-06-27 14:42:45.000000 T3SF-2.5rc2/src/T3SF/slack/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    11866 2023-07-14 15:49:05.000000 T3SF-2.5rc2/src/T3SF/slack/slack.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      749 2023-07-11 22:09:12.000000 T3SF-2.5rc2/src/T3SF/utils.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:39:07.354268 T3SF-2.5rc2/src/T3SF.egg-info/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6508 2023-08-01 20:39:07.000000 T3SF-2.5rc2/src/T3SF.egg-info/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1490 2023-08-01 20:39:07.000000 T3SF-2.5rc2/src/T3SF.egg-info/SOURCES.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-08-01 20:39:07.000000 T3SF-2.5rc2/src/T3SF.egg-info/dependency_links.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-08-01 20:39:07.000000 T3SF-2.5rc2/src/T3SF.egg-info/requires.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-08-01 20:39:07.000000 T3SF-2.5rc2/src/T3SF.egg-info/top_level.txt
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.109807 T3SF-2.5rc3/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.5rc3/LICENSE
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       33 2023-08-01 20:26:56.000000 T3SF-2.5rc3/MANIFEST.in
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6508 2023-08-01 20:55:15.109807 T3SF-2.5rc3/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5855 2023-07-18 16:44:35.000000 T3SF-2.5rc3/README.md
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-08-01 20:55:15.109807 T3SF-2.5rc3/setup.cfg
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-08-01 20:54:19.000000 T3SF-2.5rc3/setup.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/T3SF/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14998 2023-07-14 15:39:52.000000 T3SF-2.5rc3/src/T3SF/T3SF.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-06-27 20:32:45.000000 T3SF-2.5rc3/src/T3SF/__init__.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/T3SF/discord/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-06-07 19:56:31.000000 T3SF-2.5rc3/src/T3SF/discord/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7356 2023-06-07 19:56:31.000000 T3SF-2.5rc3/src/T3SF/discord/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10481 2023-07-14 15:49:41.000000 T3SF-2.5rc3/src/T3SF/discord/discord.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/T3SF/gui/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-06-07 19:56:31.000000 T3SF-2.5rc3/src/T3SF/gui/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    15747 2023-08-01 20:37:30.000000 T3SF-2.5rc3/src/T3SF/gui/core.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/T3SF/gui/static/
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/T3SF/gui/static/imgs/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6417 2023-07-11 23:06:46.000000 T3SF-2.5rc3/src/T3SF/gui/static/imgs/icon.png
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6790 2023-06-27 17:01:48.000000 T3SF-2.5rc3/src/T3SF/gui/static/imgs/logo-dark.png
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7387 2023-06-27 17:01:32.000000 T3SF-2.5rc3/src/T3SF/gui/static/imgs/logo-light.png
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/T3SF/gui/static/js/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1310 2023-06-27 20:44:06.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/bootstrap_toasts.js
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      784 2023-06-09 19:28:29.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/copy.js
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     2133 2023-07-18 17:02:36.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/theme_switcher.js
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.109807 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)    91322 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/CHANGELOG.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)      740 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/LICENSE.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     7034 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/README.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)      210 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/SECURITY.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)   752111 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/index.d.ts
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)  1305579 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)  5701941 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js.map
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     1031 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/package.json
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.109807 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     4197 2023-06-27 19:55:09.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-dark.css
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     6561 1985-10-26 08:15:00.000000 T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-default.css
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)   217088 2023-07-11 00:15:04.000000 T3SF-2.5rc3/src/T3SF/gui/t3sf.sqlite3
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.109807 T3SF-2.5rc3/src/T3SF/gui/templates/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    16635 2023-08-01 20:54:53.000000 T3SF-2.5rc3/src/T3SF/gui/templates/base.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5069 2023-06-28 00:10:12.000000 T3SF-2.5rc3/src/T3SF/gui/templates/env_creation.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14588 2023-07-11 23:14:57.000000 T3SF-2.5rc3/src/T3SF/gui/templates/index.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    27402 2023-07-14 15:40:11.000000 T3SF-2.5rc3/src/T3SF/gui/templates/msel_playground.html
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.109807 T3SF-2.5rc3/src/T3SF/logger/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-06-07 19:56:31.000000 T3SF-2.5rc3/src/T3SF/logger/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1348 2023-07-14 15:39:57.000000 T3SF-2.5rc3/src/T3SF/logger/logger.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.109807 T3SF-2.5rc3/src/T3SF/slack/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-06-07 19:56:31.000000 T3SF-2.5rc3/src/T3SF/slack/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7129 2023-06-27 14:42:45.000000 T3SF-2.5rc3/src/T3SF/slack/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    11866 2023-07-14 15:49:05.000000 T3SF-2.5rc3/src/T3SF/slack/slack.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      749 2023-07-11 22:09:12.000000 T3SF-2.5rc3/src/T3SF/utils.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:55:15.101807 T3SF-2.5rc3/src/T3SF.egg-info/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6508 2023-08-01 20:55:15.000000 T3SF-2.5rc3/src/T3SF.egg-info/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1490 2023-08-01 20:55:15.000000 T3SF-2.5rc3/src/T3SF.egg-info/SOURCES.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-08-01 20:55:15.000000 T3SF-2.5rc3/src/T3SF.egg-info/dependency_links.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-08-01 20:55:15.000000 T3SF-2.5rc3/src/T3SF.egg-info/requires.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-08-01 20:55:15.000000 T3SF-2.5rc3/src/T3SF.egg-info/top_level.txt
```

### Comparing `T3SF-2.5rc2/LICENSE` & `T3SF-2.5rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/PKG-INFO` & `T3SF-2.5rc3/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.5rc2
+Version: 2.5rc3
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.5rc2 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.5rc3 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
```

### Comparing `T3SF-2.5rc2/README.md` & `T3SF-2.5rc3/README.md`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/setup.py` & `T3SF-2.5rc3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="T3SF",
-    version="2.5-rc2",
+    version="2.5-rc3",
     author="BASE4 Security",
     author_email="jlanfranconi@base4sec.com",
     description="Technical Tabletop Exercises Simulation Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Base4Security/T3SF",
     project_urls={
```

### Comparing `T3SF-2.5rc2/src/T3SF/T3SF.py` & `T3SF-2.5rc3/src/T3SF/T3SF.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/discord/bot.py` & `T3SF-2.5rc3/src/T3SF/discord/bot.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/discord/discord.py` & `T3SF-2.5rc3/src/T3SF/discord/discord.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/core.py` & `T3SF-2.5rc3/src/T3SF/gui/core.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/imgs/icon.png` & `T3SF-2.5rc3/src/T3SF/gui/static/imgs/icon.png`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/imgs/logo-dark.png` & `T3SF-2.5rc3/src/T3SF/gui/static/imgs/logo-dark.png`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/imgs/logo-light.png` & `T3SF-2.5rc3/src/T3SF/gui/static/imgs/logo-light.png`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/bootstrap_toasts.js` & `T3SF-2.5rc3/src/T3SF/gui/static/js/bootstrap_toasts.js`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/copy.js` & `T3SF-2.5rc3/src/T3SF/gui/static/js/copy.js`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/theme_switcher.js` & `T3SF-2.5rc3/src/T3SF/gui/static/js/theme_switcher.js`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/CHANGELOG.md` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/LICENSE.md` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/LICENSE.md`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/README.md` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/README.md`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/index.d.ts` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/index.d.ts`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js.map` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js.map`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/package.json` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/package.json`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-dark.css` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-dark.css`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-default.css` & `T3SF-2.5rc3/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-default.css`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/t3sf.sqlite3` & `T3SF-2.5rc3/src/T3SF/gui/t3sf.sqlite3`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/templates/base.html` & `T3SF-2.5rc3/src/T3SF/gui/templates/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 						<h5 class="modal-title" id="DiscordServerModalLabel">Set Discord Server ID</h5>
 						<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
 					</div>
 					<div class="modal-body">
 						<form id="discordForm">
 							<div class="mb-3">
 								<label for="serverId" class="form-label">Server ID:</label>
-								<input type="text" class="form-control" id="serverId" required pattern="\d{18}">
+								<input type="text" class="form-control" id="serverId" required pattern="\d{18,19}">
 								<small class="form-text text-muted d-block">Don't know how to get it? <a href="https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID" target="_blank">Go here!</a></small>
 								<small id="validationMessage" class="form-text text-danger d-block"></small>
 
 							</div>
 						</form>
 					</div>
 					<div class="modal-footer d-flex justify-content-between">
@@ -295,15 +295,15 @@
 	<script>
 		function saveServerId() {
 			var serverIdInput = document.getElementById("serverId");
 			var serverId = serverIdInput.value;
 			var validationMessage = document.getElementById("validationMessage");
 
 			// Define the regex pattern for server ID validation
-			var serverIdPattern = /^\d{19}$/;
+			var serverIdPattern = /^\d{18,19}$/;
 
 			if (serverIdPattern.test(serverId)) {
 				localStorage.setItem("discordServerId", serverId);
 				validationMessage.innerHTML = "";
 				$('#DiscordServerModal').modal('hide');
 				b5toast.show("success", "Discord's server ID stored!", "We stored the server ID", 3000);
 			} else {
```

### Comparing `T3SF-2.5rc2/src/T3SF/gui/templates/env_creation.html` & `T3SF-2.5rc3/src/T3SF/gui/templates/env_creation.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/templates/index.html` & `T3SF-2.5rc3/src/T3SF/gui/templates/index.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/gui/templates/msel_playground.html` & `T3SF-2.5rc3/src/T3SF/gui/templates/msel_playground.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/logger/logger.py` & `T3SF-2.5rc3/src/T3SF/logger/logger.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/slack/bot.py` & `T3SF-2.5rc3/src/T3SF/slack/bot.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/slack/slack.py` & `T3SF-2.5rc3/src/T3SF/slack/slack.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF/utils.py` & `T3SF-2.5rc3/src/T3SF/utils.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.5rc2/src/T3SF.egg-info/PKG-INFO` & `T3SF-2.5rc3/src/T3SF.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.5rc2
+Version: 2.5rc3
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.5rc2 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.5rc3 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
```

### Comparing `T3SF-2.5rc2/src/T3SF.egg-info/SOURCES.txt` & `T3SF-2.5rc3/src/T3SF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

