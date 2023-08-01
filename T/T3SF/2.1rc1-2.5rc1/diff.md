# Comparing `tmp/T3SF-2.1rc1.tar.gz` & `tmp/T3SF-2.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "T3SF-2.1rc1.tar", last modified: Fri Jun  2 16:39:23 2023, max compression
+gzip compressed data, was "T3SF-2.5rc1.tar", last modified: Tue Aug  1 20:08:26 2023, max compression
```

## Comparing `T3SF-2.1rc1.tar` & `T3SF-2.5rc1.tar`

### file list

```diff
@@ -1,37 +1,58 @@
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.1rc1/LICENSE
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       42 2023-04-05 17:28:50.000000 T3SF-2.1rc1/MANIFEST.in
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-06-02 16:39:23.409754 T3SF-2.1rc1/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4094 2023-05-30 14:58:35.000000 T3SF-2.1rc1/README.md
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-06-02 16:39:23.409754 T3SF-2.1rc1/setup.cfg
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-06-02 16:38:11.000000 T3SF-2.1rc1/setup.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.405754 T3SF-2.1rc1/src/
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.405754 T3SF-2.1rc1/src/T3SF/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14869 2023-06-02 16:18:59.000000 T3SF-2.1rc1/src/T3SF/T3SF.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/__init__.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/discord/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/discord/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7356 2023-06-02 15:53:09.000000 T3SF-2.1rc1/src/T3SF/discord/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10375 2023-06-02 16:23:53.000000 T3SF-2.1rc1/src/T3SF/discord/discord.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/gui/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4987 2023-06-02 16:22:50.000000 T3SF-2.1rc1/src/T3SF/gui/core.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/gui/templates/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4458 2023-05-30 15:48:00.000000 T3SF-2.1rc1/src/T3SF/gui/templates/base.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5575 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/templates/env_creation.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     8065 2023-06-02 16:23:01.000000 T3SF-2.1rc1/src/T3SF/gui/templates/index.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     3603 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/templates/msel_viewer.html
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/logger/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/logger/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1452 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/logger/logger.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/slack/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/slack/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7129 2023-05-30 16:20:25.000000 T3SF-2.1rc1/src/T3SF/slack/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    11646 2023-06-02 16:23:56.000000 T3SF-2.1rc1/src/T3SF/slack/slack.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      682 2023-06-02 16:25:20.000000 T3SF-2.1rc1/src/T3SF/utils.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF.egg-info/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      665 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/SOURCES.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/dependency_links.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/requires.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/top_level.txt
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.425623 T3SF-2.5rc1/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.5rc1/LICENSE
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       33 2023-08-01 20:08:17.000000 T3SF-2.5rc1/MANIFEST.in
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6508 2023-08-01 20:08:26.425623 T3SF-2.5rc1/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5855 2023-07-18 16:44:35.000000 T3SF-2.5rc1/README.md
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-08-01 20:08:26.425623 T3SF-2.5rc1/setup.cfg
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-08-01 18:13:53.000000 T3SF-2.5rc1/setup.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.409623 T3SF-2.5rc1/src/
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.413623 T3SF-2.5rc1/src/T3SF/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14998 2023-07-14 15:39:52.000000 T3SF-2.5rc1/src/T3SF/T3SF.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-06-27 20:32:45.000000 T3SF-2.5rc1/src/T3SF/__init__.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.413623 T3SF-2.5rc1/src/T3SF/discord/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-06-07 19:56:31.000000 T3SF-2.5rc1/src/T3SF/discord/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7356 2023-06-07 19:56:31.000000 T3SF-2.5rc1/src/T3SF/discord/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10481 2023-07-14 15:49:41.000000 T3SF-2.5rc1/src/T3SF/discord/discord.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.413623 T3SF-2.5rc1/src/T3SF/gui/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-06-07 19:56:31.000000 T3SF-2.5rc1/src/T3SF/gui/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    15576 2023-08-01 18:03:33.000000 T3SF-2.5rc1/src/T3SF/gui/core.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.413623 T3SF-2.5rc1/src/T3SF/gui/static/
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.413623 T3SF-2.5rc1/src/T3SF/gui/static/imgs/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6417 2023-07-11 23:06:46.000000 T3SF-2.5rc1/src/T3SF/gui/static/imgs/icon.png
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6790 2023-06-27 17:01:48.000000 T3SF-2.5rc1/src/T3SF/gui/static/imgs/logo-dark.png
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7387 2023-06-27 17:01:32.000000 T3SF-2.5rc1/src/T3SF/gui/static/imgs/logo-light.png
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.417623 T3SF-2.5rc1/src/T3SF/gui/static/js/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1310 2023-06-27 20:44:06.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/bootstrap_toasts.js
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      784 2023-06-09 19:28:29.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/copy.js
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     2133 2023-07-18 17:02:36.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/theme_switcher.js
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.421623 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)    91322 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/CHANGELOG.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)      740 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/LICENSE.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     7034 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/README.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)      210 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/SECURITY.md
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)   752111 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/index.d.ts
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)  1305579 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)  5701941 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/index.js.map
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     1031 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/package.json
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.421623 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     4197 2023-06-27 19:55:09.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-dark.css
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)     6561 1985-10-26 08:15:00.000000 T3SF-2.5rc1/src/T3SF/gui/static/js/vanilla-jsoneditor/themes/jse-theme-default.css
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.425623 T3SF-2.5rc1/src/T3SF/gui/templates/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    16629 2023-07-24 20:40:01.000000 T3SF-2.5rc1/src/T3SF/gui/templates/base.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5069 2023-06-28 00:10:12.000000 T3SF-2.5rc1/src/T3SF/gui/templates/env_creation.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14588 2023-07-11 23:14:57.000000 T3SF-2.5rc1/src/T3SF/gui/templates/index.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    27402 2023-07-14 15:40:11.000000 T3SF-2.5rc1/src/T3SF/gui/templates/msel_playground.html
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.425623 T3SF-2.5rc1/src/T3SF/logger/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-06-07 19:56:31.000000 T3SF-2.5rc1/src/T3SF/logger/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1348 2023-07-14 15:39:57.000000 T3SF-2.5rc1/src/T3SF/logger/logger.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.425623 T3SF-2.5rc1/src/T3SF/slack/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-06-07 19:56:31.000000 T3SF-2.5rc1/src/T3SF/slack/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7129 2023-06-27 14:42:45.000000 T3SF-2.5rc1/src/T3SF/slack/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    11866 2023-07-14 15:49:05.000000 T3SF-2.5rc1/src/T3SF/slack/slack.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      749 2023-07-11 22:09:12.000000 T3SF-2.5rc1/src/T3SF/utils.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-08-01 20:08:26.413623 T3SF-2.5rc1/src/T3SF.egg-info/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6508 2023-08-01 20:08:26.000000 T3SF-2.5rc1/src/T3SF.egg-info/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1464 2023-08-01 20:08:26.000000 T3SF-2.5rc1/src/T3SF.egg-info/SOURCES.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-08-01 20:08:26.000000 T3SF-2.5rc1/src/T3SF.egg-info/dependency_links.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-08-01 20:08:26.000000 T3SF-2.5rc1/src/T3SF.egg-info/requires.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-08-01 20:08:26.000000 T3SF-2.5rc1/src/T3SF.egg-info/top_level.txt
```

### Comparing `T3SF-2.1rc1/LICENSE` & `T3SF-2.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `T3SF-2.1rc1/PKG-INFO` & `T3SF-2.5rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.1rc1
+Version: 2.5rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,27 +13,31 @@
 Description-Content-Type: text/markdown
 Provides-Extra: Slack
 Provides-Extra: Discord
 License-File: LICENSE
 
 <p align="center">
   <a href="" rel="noopener">
- <img width=200px height=200px src="https://user-images.githubusercontent.com/103124157/164258966-7a049d6c-4012-49ca-8f7d-2bb814c24009.png" alt="WhaBot Logo"></a>
+ <img width=200px height=200px src="https://user-images.githubusercontent.com/103124157/164258966-7a049d6c-4012-49ca-8f7d-2bb814c24009.png" alt="T3SF Logo"></a>
 </p>
 
 <h3 align="center">T3SF</h3>
 
 <div align="center">
-
+  
   [![Status](https://img.shields.io/badge/status-active-success.svg)]() 
   [![PyPI version](https://badge.fury.io/py/T3SF.svg)](https://badge.fury.io/py/T3SF)
   [![Documentation Status](https://readthedocs.org/projects/t3sf/badge/?version=latest)](https://t3sf.readthedocs.io/en/latest/?badge=latest)
   [![License](https://img.shields.io/badge/license-GPL-blue.svg)](/LICENSE)
   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6519221.svg)](https://doi.org/10.5281/zenodo.6519221)
-
+</div>
+<div align="center">
+  
+  [![Docker Image for Discord](https://github.com/Base4Security/T3SF/actions/workflows/publish_discord.yml/badge.svg)](https://hub.docker.com/r/base4sec/t3sf)
+  [![Docker Image for Slack](https://github.com/Base4Security/T3SF/actions/workflows/publish_slack.yml/badge.svg)](https://hub.docker.com/r/base4sec/t3sf)
 </div>
 
 <p align="center"> Technical Tabletop Exercises Simulation Framework
     <br> 
 </p>
 
 ## Table of Contents
@@ -78,14 +82,47 @@
   - [Slack](https://t3sf.readthedocs.io/en/latest/Slack.html#installation)
   - [Telegram](https://t3sf.readthedocs.io/en/latest/Telegram.html#installation)
   - [WhatsApp](https://t3sf.readthedocs.io/en/latest/WhatsApp.html#installation)
 
 ## Usage <a name="Usage"></a>
 We created this framework to simplify all your work!
 
+
+<details>
+<summary>Using Docker</summary>
+
+### Supported Tags
+- slack → This image has all the requirements to perform an exercise in Slack.
+- discord → This image has all the requirements to perform an exercise in Discord.
+
+
+#### Using it with Slack
+
+```bash
+$ docker run --rm -t --env-file .env -v $(pwd)/MSEL.json:/app/MSEL.json base4sec/t3sf:slack
+```
+
+Inside your `.env` file you have to provide the `SLACK_BOT_TOKEN` and `SLACK_APP_TOKEN` tokens. Read more about it [here](https://t3sf.readthedocs.io/en/latest/Slack.html#providing-the-tokens).
+
+There is another environment variable to set, `MSEL_PATH`. This variable tells the framework in which path the MSEL is located. By default, the container path is `/app/MSEL.json`. If you change the mount location of the volume then also change the variable.
+
+
+#### Using it with Discord
+
+```bash
+$ docker run --rm -t --env-file .env -v $(pwd)/MSEL.json:/app/MSEL.json base4sec/t3sf:discord
+```
+
+Inside your `.env` file you have to provide the `DISCORD_TOKEN` token. Read more about it [here](https://t3sf.readthedocs.io/en/latest/Discord.html#providing-the-token).
+
+There is another environment variable to set, `MSEL_PATH`. This variable tells the framework in which path the MSEL is located. By default, the container path is `/app/MSEL.json`. If you change the mount location of the volume then also change the variable.
+
+---------------------
+</details>
+
 Once you have everything ready, use our template for the `main.py`, or modify the following code:
 
 Here is an example if you want to run the framework with the `Discord` bot and a `GUI`.
 
 ```python
 from T3SF import T3SF
 import asyncio
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.1rc1 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.5rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
 Provides-Extra: Discord License-File: LICENSE
-                                 [WhaBot Logo]
+                                  [T3SF Logo]
                                 **** T3SF ****
  [![Status](https://img.shields.io/badge/status-active-success.svg)]() [![PyPI
 version](https://badge.fury.io/py/T3SF.svg)](https://badge.fury.io/py/T3SF) [!
       [Documentation Status](https://readthedocs.org/projects/t3sf/badge/
    ?version=latest)](https://t3sf.readthedocs.io/en/latest/?badge=latest) [!
 [License](https://img.shields.io/badge/license-GPL-blue.svg)](/LICENSE) [![DOI]
   (https://zenodo.org/badge/DOI/10.5281/zenodo.6519221.svg)](https://doi.org/
                             10.5281/zenodo.6519221)
+  [![Docker Image for Discord](https://github.com/Base4Security/T3SF/actions/
+ workflows/publish_discord.yml/badge.svg)](https://hub.docker.com/r/base4sec/
+t3sf) [![Docker Image for Slack](https://github.com/Base4Security/T3SF/actions/
+workflows/publish_slack.yml/badge.svg)](https://hub.docker.com/r/base4sec/t3sf)
               Technical Tabletop Exercises Simulation Framework
 ## Table of Contents - [About](#About) - [Getting Things Ready](#Starting) -
 [TODO](./TODO.md) - [CHANGELOG](./CHANGELOG.md) - [Contributing](./
 CONTRIBUTING.md) ## About  T3SF is a framework that offers a modular structure
 for the orchestration of events based on a master scenario events list (MSEL)
 together with a set of rules defined for each exercise (optional) and a
 configuration that allows defining the parameters of the corresponding
@@ -44,17 +48,35 @@
 platform. Once the installation is complete, you can start using the framework
 with your platform of choice. We strongly recommend following the platform-
 specific guidance within our Read The Docs! Here are the links: - [Discord]
 (https://t3sf.readthedocs.io/en/latest/Discord.html#installation) - [Slack]
 (https://t3sf.readthedocs.io/en/latest/Slack.html#installation) - [Telegram]
 (https://t3sf.readthedocs.io/en/latest/Telegram.html#installation) - [WhatsApp]
 (https://t3sf.readthedocs.io/en/latest/WhatsApp.html#installation) ## Usage  We
-created this framework to simplify all your work! Once you have everything
-ready, use our template for the `main.py`, or modify the following code: Here
-is an example if you want to run the framework with the `Discord` bot and a
-`GUI`. ```python from T3SF import T3SF import asyncio async def main(): await
+created this framework to simplify all your work!  Using Docker ### Supported
+Tags - slack â This image has all the requirements to perform an exercise in
+Slack. - discord â This image has all the requirements to perform an exercise
+in Discord. #### Using it with Slack ```bash $ docker run --rm -t --env-file
+.env -v $(pwd)/MSEL.json:/app/MSEL.json base4sec/t3sf:slack ``` Inside your
+`.env` file you have to provide the `SLACK_BOT_TOKEN` and `SLACK_APP_TOKEN`
+tokens. Read more about it [here](https://t3sf.readthedocs.io/en/latest/
+Slack.html#providing-the-tokens). There is another environment variable to set,
+`MSEL_PATH`. This variable tells the framework in which path the MSEL is
+located. By default, the container path is `/app/MSEL.json`. If you change the
+mount location of the volume then also change the variable. #### Using it with
+Discord ```bash $ docker run --rm -t --env-file .env -v $(pwd)/MSEL.json:/app/
+MSEL.json base4sec/t3sf:discord ``` Inside your `.env` file you have to provide
+the `DISCORD_TOKEN` token. Read more about it [here](https://
+t3sf.readthedocs.io/en/latest/Discord.html#providing-the-token). There is
+another environment variable to set, `MSEL_PATH`. This variable tells the
+framework in which path the MSEL is located. By default, the container path is
+`/app/MSEL.json`. If you change the mount location of the volume then also
+change the variable. ---------------------  Once you have everything ready, use
+our template for the `main.py`, or modify the following code: Here is an
+example if you want to run the framework with the `Discord` bot and a `GUI`.
+```python from T3SF import T3SF import asyncio async def main(): await
 T3SF.start(MSEL="MSEL_TTX.json", platform="Discord", gui=True) if __name__ ==
 '__main__': asyncio.run(main()) ``` Or if you prefer to run the framework
 without `GUI` and with `Slack` instead, you can modify the arguments, and
 that's it! Yes, that simple! ```python await T3SF.start(MSEL="MSEL_TTX.json",
 platform="Slack", gui=False) ``` If you need more help, you can always check
 our documentation [here](https://t3sf.readthedocs.io/en/latest/)!
```

### Comparing `T3SF-2.1rc1/setup.py` & `T3SF-2.5rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="T3SF",
-    version="2.1-rc1",
+    version="2.5-rc1",
     author="BASE4 Security",
     author_email="jlanfranconi@base4sec.com",
     description="Technical Tabletop Exercises Simulation Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Base4Security/T3SF",
     project_urls={
```

### Comparing `T3SF-2.1rc1/src/T3SF/T3SF.py` & `T3SF-2.5rc1/src/T3SF/T3SF.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,17 @@
 def keyboard_interrupt_handler(signal_num, frame):
 	T3SF_Logger.emit(message=f"KeyboardInterrupt (ID: {signal_num}) has been caught. Exiting...", message_type="WARN")
 	os._exit(1)
 
 # Associate the signal handler function with SIGINT (keyboard interrupt)
 signal.signal(signal.SIGINT, keyboard_interrupt_handler)
 
-
 class T3SF(object):
 	def __init__(self, bot = None, app = None, platform = None):
 		self.response = None
-		self.process_wait = False
-		self.process_quit = False
 		self.regex_ready = None
 		self.incidents_running = False
 		self.poll_answered = False
 		self.ch_names_list = []
 		self.players_list = []
 		self.platform = platform.lower()
 		self.guild_id = None
@@ -81,16 +78,14 @@
 
 			if "Poll" in self._inject and self._inject['Poll'] != '' and self.poll_answered == False:
 				description = self._inject["Script"] + f"\n\n@channel Poll not answered within {self.diff} minute(s), Time's Up!"
 				await self.EditMessage(style="custom", variable="T3SF_instance.response_poll", color = "RED", title="Poll time ended!", description=description, response=self.response_poll)
 				await self.NotifyGameMasters(type_info="poll_unanswered", data={'msg_poll':self._inject["Script"]}) 
 
 		except Exception as e:
-			print("Get Time Difference")
-			print(e)
 			T3SF_Logger.emit("Get Time Difference", message_type="ERROR")
 			T3SF_Logger.emit(e, message_type="ERROR")
 			raise
 
 	def IncidentsFetcher(self, MSEL:str):
 		"""
 		Retrieves the incidents from the desired source, chosen in the config file.
@@ -109,15 +104,15 @@
 		else:
 			raise RuntimeError("Please set a method to retrieve the TTXs with the argument `MSEL` inside the `start` function.")
 
 	async def start(MSEL:str, platform, gui=False):
 		if gui == True:
 			T3SF_Logger.emit(message="Starting GUI", message_type="DEBUG")
 			gui_module = importlib.import_module("T3SF.gui.core")
-			gui_module.GUI(platform_run=platform, MSEL=MSEL)
+			gui_module.GUI(platform_run=platform, MSEL=MSEL, static_url_path='/static', static_folder='static')
 		
 		if platform.lower() == "slack":
 			bot_module = importlib.import_module("T3SF.slack.bot")
 
 		elif platform.lower() == "discord":
 			bot_module = importlib.import_module("T3SF.discord.bot")
 
@@ -168,16 +163,14 @@
 				description = f"Poll Question: {data['msg_poll']}\nNot answered by anyone."
 				# await self.SendMessage(title = title, description = description, color="RED", unique=True)
 
 			T3SF_Logger.emit(message=description, message_type="INFO")
 			return True
 
 		except Exception as e:
-			print("NotifyGameMasters")
-			print(e)
 			T3SF_Logger.emit("NotifyGameMasters", message_type="ERROR")
 			T3SF_Logger.emit(e, message_type="ERROR")
 			raise
 
 	async def ProcessIncidents(self, MSEL:str, ctx, function_type:str=None, itinerator:int=0):
 		"""
 		Process the incidents from the MSEL file.
@@ -195,20 +188,18 @@
 				await self.NotifyGameMasters(type_info="start_normal")  # Sends a message regarding the bot's start procedure.
 			else:
 				await self.NotifyGameMasters(type_info="start_resumed")  # Sends a message regarding the bot's restart procedure.
 			
 			bypass_time = True
 
 			for information in self.data:
-				if self.process_quit == True:
+				process_status = await self.check_status()
+
+				if process_status == 'break':
 					break
-				
-				if self.process_wait == True:
-					while self.process_wait == True:
-						await asyncio.sleep(5)
 
 				if itinerator == 0: # Set a variable to get the actual timestamp and the past one, after that checks for differences.
 					itinerator_loop = itinerator
 				else:
 					if function_type == "resume":
 						itinerator_loop = itinerator - 2
 					else:
@@ -244,41 +235,55 @@
 					else:
 						if bypass_time == True:
 							await self.NotifyGameMasters(type_info="started_resumed") # Informs that the bot succesfully restarted.
 							bypass_time = False
 
 					itinerator += 1
 			
+			await self.check_status(reset=True)
 			await self.NotifyGameMasters(type_info="finished_incidents") # Informs that the script is completed and there's no remaining incidents.
-			self.process_quit = False
-			self.process_wait = False
 			self.incidents_running = False
 
 		except Exception as e:
-			print("ProcessIncidents function")
-			print(e)
 			T3SF_Logger.emit("ProcessIncidents function", message_type="ERROR")
 			T3SF_Logger.emit(e, message_type="ERROR")
 			raise
 
+	async def check_status(self, reset:bool = False):
+		from .utils import process_wait, process_quit
+
+		if reset:
+			process_quit = False
+			process_wait = False
+			return True
+
+		if process_quit == True:
+			return 'break'
+
+		if process_wait == True:
+			# print(f"We are waiting, because the variable {process_wait} is set to True")
+			await asyncio.sleep(5)
+			await self.check_status()
+			return False
+
+		return True
+
 	async def SendIncident(self, inject):
 		try:
 			self._inject = inject
 
 			if self.platform == "discord":
 				await self.discord.InjectHandler(T3SF_instance=self)
 
 			elif self.platform == "slack":
 				await self.slack.InjectHandler(T3SF_instance=self)
 
 			return True
 
 		except Exception as e:
-			print("SendIncident")
-			print(e)
 			T3SF_Logger.emit("SendIncident", message_type="ERROR")
 			T3SF_Logger.emit(e, message_type="ERROR")
 			raise
 
 	async def SendPoll(self, inject):
 		try:
 			self._inject = inject
@@ -288,16 +293,14 @@
 
 			elif self.platform == "slack":
 				await self.slack.PollHandler(T3SF_instance=self)
 
 			return True
 
 		except Exception as e:
-			print("SendPoll")
-			print(e)
 			T3SF_Logger.emit("SendPoll", message_type="ERROR")
 			T3SF_Logger.emit(e, message_type="ERROR")
 			raise
 
 	async def InboxesAuto(self, message=None):
 		if self.platform == "discord":
 			await self.discord.InboxesAuto(T3SF_instance=self)
```

### Comparing `T3SF-2.1rc1/src/T3SF/discord/bot.py` & `T3SF-2.5rc1/src/T3SF/discord/bot.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1rc1/src/T3SF/discord/discord.py` & `T3SF-2.5rc1/src/T3SF/discord/discord.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import discord
 import asyncio
 import random
 import json
 import re 
-from T3SF import utils
+from T3SF import utils, T3SF_Logger
 
 class Discord(object):
 	def __init__(self, bot):
 		self.bot = bot
 
 	async def InboxesAuto(self, T3SF_instance):
 		mensaje_inboxes = ""
@@ -58,19 +58,22 @@
 								break
 					else:
 						player_itinerator += 1
 						channels_itinerator += 1
 						past_channel = category.name
 						pass
 
+			T3SF_Logger.emit(message=f'Please confirm the Regular Expression for the inboxes on the gm-chat!', message_type="INFO")
+
 			await T3SF_instance.response_auto.edit(embed=discord.Embed(
 			 title = "ℹ️ Regex detected!",
 			 description = f"Please confirm if the regex detected for the channels, is correct so we can get the inboxes!\n\nExample:\nGroup - Legal\nThe regex should be `Group -`\n\nDetected regex: `{regex}`",
 			 color = 0x77B255).set_image(url=image_example).set_footer(text="Please answer with [Yes(Y)/No(N)]"))
 
+
 			def check_regex_channels(msg):
 				if started_from_gui:
 					return msg.content.lower() in ["y", "yes", "n", "no"]
 
 				else:
 					return msg.author == T3SF_instance._ctx.author and msg.channel == T3SF_instance._ctx.channel and msg.content.lower() in ["y", "yes", "n", "no"]
 
@@ -116,14 +119,16 @@
 			json.dump(T3SF_instance.inboxes_all,open(f"inboxes_{T3SF_instance.platform}.json", "w"))
 
 			for player in T3SF_instance.inboxes_all:
 				mensaje_inboxes += f"**Inbox** {player}[{T3SF_instance.inboxes_all[player]}]\n"
 
 			await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="GREEN", title=f"📩  Inboxes fetched! [{len(T3SF_instance.inboxes_all)}]", description=mensaje_inboxes)
 
+			T3SF_Logger.emit(message=f'Confirmed! Inboxes ready', message_type="INFO")
+
 		return True
 
 	async def InjectHandler(self, T3SF_instance):
 		all_data = f'Date: {T3SF_instance._inject["Date"]}\n\n{T3SF_instance._inject["Script"]}'
 
 		player = T3SF_instance._inject['Player']
 
@@ -164,16 +169,16 @@
 		if diff < 0:
 			diff_no_real = int(actual_real_time) - int(next_real_time)
 			diff = 60 - diff_no_real 
 
 		diff_secs = diff * 60
 
 		view = discord.ui.View()
-		view.add_item(discord.ui.Button(style=discord.ButtonStyle.primary,label=poll_options[0], custom_id="poll|"+poll_options[0]))
-		view.add_item(discord.ui.Button(style=discord.ButtonStyle.primary,label=poll_options[1], custom_id="poll|"+poll_options[1]))
+		for option in poll_options:
+			view.add_item(discord.ui.Button(style=discord.ButtonStyle.primary, label=option, custom_id="poll|" + option))
 
 		all_data = all_data+ f"\n\nYou have {diff} minute(s) to answer this poll!"
 
 		player = T3SF_instance._inject['Player']
 
 		inbox = self.bot.get_channel(T3SF_instance.inboxes_all[player])
```

### Comparing `T3SF-2.1rc1/src/T3SF/gui/templates/env_creation.html` & `T3SF-2.5rc1/src/T3SF/gui/templates/env_creation.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,43 @@
 {% extends 'base.html' %}
 
-
 {% block title %} Environment creation {% endblock %}
 
 {% block extra_head %}
-<style type="text/css">
+	<style type="text/css">
 		#logs-content {
 			height: 500px;
 			overflow: auto;
-			white-space: pre-wrap;
 			flex-grow: 1;
 		}
 		@media (max-width: 991px) {
 			html, body, #logs-content {
 				height: 100%;
 				width: 100%;
 				max-width: none;
 			}
-
-			#logs-content {
-				margin-top: 0;
-			}
 		}
 
 		.log-type-DEBUG {
-			float: left;
 			color: blue;
 		}
 		.log-type-INFO {
-			float: left;
 			color: green;
 		}
 		.log-type-WARN {
-			float: left;
 			color: #FFC107;
 		}
 		.log-type-ERROR {
-			float: left;
 			color: red;
 		}
 
 		.log-timestamp {
 			font-size: 12px;
 			color: gray;
-			float: right;
-		}
-
-		#logs-level-dropdown {
-			border: 1px solid #ccc;
-			border-radius: 4px;
-			padding: 4px 8px;
-			font-size: 16px;
-			font-family: Arial, sans-serif;
-			color: #333;
-			background-color: #fff;
-			box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.1);
-			transition: border-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
-		}
-
-		#logs-level-dropdown:focus {
-			outline: none;
-			border-color: #007bff;
-			box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.1), 0 0 0 2px rgba(0, 123, 255, 0.5);
-		}
-
-		#logs-level-form label {
-			font-size: 16px;
-			font-family: Arial, sans-serif;
-			font-weight: bold;
-			margin-right: 8px;
-			color: #333;
 		}
-
-		#logs-level-form-container {
-			display: inline-block;
-		}
-
-		#logs-level-form,
-		#logs-level-dropdown {
-			display: inline-block;
-		}
-
-	}
 	</style>
 
 {% endblock %}
 {% block content %}
 <div class="container" id="content">
 	<div class="row align-items-center">
 		<div class="col">
@@ -108,73 +60,87 @@
 				<div class="col">
 					<h4>Channels for Game Masters:</h4>
 				</div>
 			</div>
 			<div class="row">
 				<div class="col">
 					{%- for player in T3SF.players_list -%}
-						<h5 class="text-muted">{{player}}<h5>
+						<h5 class="text-muted">{{player}}</h5>
 					{%- endfor -%}
 				</div>
 				<div class="col">
-					<h5 class="text-muted">Internal chat<h5>
-					<h5 class="text-muted">Inbox<h5>
-					<h5 class="text-muted">Decision log<h5>
+					<h5 class="text-muted">Internal chat</h5>
+					<h5 class="text-muted">Inbox</h5>
+					<h5 class="text-muted">Decision log</h5>
 					{%- if T3SF.platform == "discord" -%}
-						<h5 class="text-muted">Voice channel<h5>
+						<h5 class="text-muted">Voice channel</h5>
 					{%- endif -%}
 				</div>
 				<div class="col">
-					<h5 class="text-muted">Internal chat<h5>
-					<h5 class="text-muted">Logs<h5>
+					<h5 class="text-muted">Internal chat</h5>
+					<h5 class="text-muted">Logs</h5>
 					{%- if T3SF.platform == "discord" -%}
-						<h5 class="text-muted">Voice channel<h5>
+						<h5 class="text-muted">Voice channel</h5>
 					{%- endif -%}
 				</div>
 			</div>
 		</div>
 	</div>
-	<div class="row" style="visibility: hidden;" id="logs-container">
+	<div class="row d-none" id="logs-container">
 		<div class="col">
 			<hr>
-			<div class="bg-light rounded p-3" id="logs-content">
+			<div class="bg-light rounded mt-3 p-3" id="logs-content">
 			</div>
 		</div>
 	</div>
 </div>
 <script>
 	$('#create_env_button').click(function() {
 		{%- if T3SF.platform == "discord" -%}
-		var num = prompt("What's your Discord's server ID? ");
-		var url = "create?server=" + num;
+		var serverId = localStorage.getItem("discordServerId");
+
+		if (!serverId) {
+			// Server ID not stored, trigger modal to save it
+			$('#DiscordServerModal').modal('show');
+			return; // Stop execution until server ID is obtained
+		}
+		var url = "create?server=" + serverId;
 		{%- else -%}
 		var url = "create";
 		{%- endif -%}
 		$.ajax({ 
 			type: "GET",
 			url: url,
 			beforeSend: function() {
 				document.getElementById('create_env_button').disabled = true;
 				b5toast.show("warning", "Creating environment! ", "To check the status of the Environment creation check the logs below", 3000);
 				$('#logs-content').empty();
-				$("#logs-container").css("visibility", "visible");
+				$("#logs-container").removeClass("d-none");
 				
-				disclaimer = {% if T3SF.platform == "discord" %}'The server owner should see each created channel.'{% else %}'We will invite the Workspace owner to each created channel.'{% endif %}
+				disclaimer = {% if T3SF.platform == "discord" %}'The server owner should see each channel created.'{% else %}'We will invite the Workspace owner to each created channel.'{% endif %}
 
-				var logString = '<b>\<div>\
-				<span class="log-type-INFO">[INFO] </span>\
-				<span class="float-start"><b>' + disclaimer +'</b></span>\
-				</div></b>';
-				$('#logs-content').append(logString); },
+				var logString = '<div class="row">\
+					<div class="col-11">\
+						<span class="log-type-INFO">[INFO] </span>\
+						<span class="message">' + disclaimer + '</span>\
+					</div>\
+				</div>';
+				$('#logs-content').append(logString); 
+			},
 			success: function(data){
-				b5toast.show("success", "Environment created! ", "View the logs for more information", 3000);
+				if (data.status == "ok") {
+					b5toast.show("success", data.msg, "View the logs for more information", 3000);
+				}
+				else{
+					b5toast.show("danger", "An error ocurred", data.msg, 5000);
+				}
 			},
 			error: function(xhr){
 				document.getElementById('create_env_button').disabled = false;
-				b5toast.show("danger", "Error creating everything! ", "View the logs for more information", 5000);
+				b5toast.show("danger", "Error creating the environment!", "View the logs for more information", 5000);
 			}
 		});
 	});
 </script>
 
 <script>
 	let eventSource = new EventSource('/stream_news');
@@ -197,19 +163,23 @@
 		var messageId = message.id;
 
 		if (!historic_logs.includes(messageId)) {
 			// Store to the historics
 			historic_logs.push(messageId);
 
 			// Format the new log
-			var logString = '<div>\
-			<span class="log-type-'+message.type+'">[' + message.type + '] </span>\
-			<span class="float-start">' + message.content + '</span>\
-			<span class="log-timestamp">' + message.timestamp + '</span>\
-			</div>';
+			var logString = '<div class="row">\
+					<div class="col-11">\
+						<span class="log-type-'+message.type+'">[' + message.type + '] </span>\
+						<span class="message">' + message.content + '</span>\
+					</div>\
+					<div class="col-1 text-end">\
+						<span class="log-timestamp">' + message.timestamp + '</span>\
+					</div>\
+				</div>';
 
 			// Append the new log
 			$('#logs-content').append(logString);
 
 			// Scroll to latest message
 			var logsContent = document.getElementById("logs-content");
 			logsContent.scrollTop = logsContent.scrollHeight;
```

### Comparing `T3SF-2.1rc1/src/T3SF/slack/bot.py` & `T3SF-2.5rc1/src/T3SF/slack/bot.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1rc1/src/T3SF/slack/slack.py` & `T3SF-2.5rc1/src/T3SF/slack/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import Counter
-from T3SF import utils
+from T3SF import T3SF_Logger, utils
 import random
 import json
 import re 
 
 class Slack(object):
 	def __init__(self, app):
 		self.app = app
@@ -178,14 +178,16 @@
 			for player in T3SF_instance.inboxes_all:
 				mensaje_inboxes += f"Inbox {player} [{T3SF_instance.inboxes_all[player]}]\n"
 
 			T3SF_instance.response_auto = await self.EditMessage(response=T3SF_instance.response_auto, color="YELLOW", title = f"📩 Inboxes fetched! [{len(T3SF_instance.inboxes_all)}]", description=mensaje_inboxes)
 			
 			T3SF_instance.regex_ready = True
 
+			T3SF_Logger.emit(message=f'Confirmed! Inboxes ready', message_type="INFO")
+
 		elif T3SF_instance.fetch_inboxes == True:
 
 			T3SF_instance.response_auto = await self.SendMessage(channel = T3SF_instance._ctx['channel'], color="CYAN", title="💬 Fetching inboxes...", description=f"Please wait while we fetch all the inboxes in this server!")
 
 			channels = await T3SF_instance.app.client.conversations_list(types="public_channel,private_channel")
 
 			for channel in channels['channels']:
@@ -217,14 +219,15 @@
 						continue
 
 			image = {"image_url":"https://i.ibb.co/34rTqMH/image.png", "name": "regex"}
 			buttons = [{"text":"Yes!", "style": "primary", "value": regex, "action_id": "regex_yes"},{"text":"No.", "style": "danger", "value": "click_me_456", "action_id": "regex_no"}]
 			
 			T3SF_instance.response_auto = await self.EditMessage(response=T3SF_instance.response_auto, color="GREEN", title = "ℹ️ Regex detected!", description = f"Please confirm if the regex detected for the channels, is correct so we can get the inboxes!\n\nExample:\ninbox-legal\nThe regex should be `inbox-`\n\n*Detected regex:* `{regex}`\n\n\nPlease select your answer below.", image=image, buttons = buttons)
 			T3SF_instance.regex_ready = False
+			T3SF_Logger.emit(message=f'Please confirm the Regular Expression for the inboxes on the gm-chat!', message_type="INFO")
 
 		else:
 			mensaje_inboxes = ""
 			T3SF_instance.response_auto = await self.SendMessage(channel = T3SF_instance._ctx['channel'], color="CYAN", title="💬 Fetching inboxes...", description=f"Please wait while we fetch all the inboxes in this server!")
 
 			for player in T3SF_instance.inboxes_all:
 				mensaje_inboxes += f"Inbox {player} [{T3SF_instance.inboxes_all[player]}]\n"
@@ -287,15 +290,23 @@
 			diff_no_real = int(actual_real_time) - int(next_real_time)
 			diff = 60 - diff_no_real 
 
 		diff_secs = diff * 60
 
 		description = T3SF_instance._inject["Script"] + f"\n\nYou have {diff} minute(s) to answer this poll!"
 
-		buttons = [{"text": poll_options[0], "style": "primary", "value": 'option1', "action_id": "option1"},{"text":poll_options[1], "style": "primary", "value": "option2","action_id": "option2"}]
+		buttons = []
+
+		for i, option in enumerate(poll_options, start=1):
+			buttons.append({
+				"style": "primary",
+				"text": option,
+				"value": f"option{i}",
+				"action_id": f"option{i}"
+				})
 
 		T3SF_instance.response_poll = await self.SendMessage(channel = T3SF_instance.inboxes_all[player], title=T3SF_instance._inject['Subject'], description=description, image=image, buttons=buttons, color="YELLOW")
 
 		return True
 
 	async def PollAnswerHandler(self, T3SF_instance, body=None, payload=None):
 		poll_msg = body['message']['attachments'][0]['fallback']
```

### Comparing `T3SF-2.1rc1/src/T3SF/utils.py` & `T3SF-2.5rc1/src/T3SF/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from difflib import SequenceMatcher
 from collections import Counter
 import os
 
+process_wait = False
+process_quit = False
+process_started = False
+
 def is_docker():
 	"""
 	Detects if the script is running inside a docker environment.
 	"""
 	path = '/proc/self/cgroup'
 	return (
 		os.path.exists('/.dockerenv') or
```

### Comparing `T3SF-2.1rc1/src/T3SF.egg-info/PKG-INFO` & `T3SF-2.5rc1/src/T3SF.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.1rc1
+Version: 2.5rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,27 +13,31 @@
 Description-Content-Type: text/markdown
 Provides-Extra: Slack
 Provides-Extra: Discord
 License-File: LICENSE
 
 <p align="center">
   <a href="" rel="noopener">
- <img width=200px height=200px src="https://user-images.githubusercontent.com/103124157/164258966-7a049d6c-4012-49ca-8f7d-2bb814c24009.png" alt="WhaBot Logo"></a>
+ <img width=200px height=200px src="https://user-images.githubusercontent.com/103124157/164258966-7a049d6c-4012-49ca-8f7d-2bb814c24009.png" alt="T3SF Logo"></a>
 </p>
 
 <h3 align="center">T3SF</h3>
 
 <div align="center">
-
+  
   [![Status](https://img.shields.io/badge/status-active-success.svg)]() 
   [![PyPI version](https://badge.fury.io/py/T3SF.svg)](https://badge.fury.io/py/T3SF)
   [![Documentation Status](https://readthedocs.org/projects/t3sf/badge/?version=latest)](https://t3sf.readthedocs.io/en/latest/?badge=latest)
   [![License](https://img.shields.io/badge/license-GPL-blue.svg)](/LICENSE)
   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6519221.svg)](https://doi.org/10.5281/zenodo.6519221)
-
+</div>
+<div align="center">
+  
+  [![Docker Image for Discord](https://github.com/Base4Security/T3SF/actions/workflows/publish_discord.yml/badge.svg)](https://hub.docker.com/r/base4sec/t3sf)
+  [![Docker Image for Slack](https://github.com/Base4Security/T3SF/actions/workflows/publish_slack.yml/badge.svg)](https://hub.docker.com/r/base4sec/t3sf)
 </div>
 
 <p align="center"> Technical Tabletop Exercises Simulation Framework
     <br> 
 </p>
 
 ## Table of Contents
@@ -78,14 +82,47 @@
   - [Slack](https://t3sf.readthedocs.io/en/latest/Slack.html#installation)
   - [Telegram](https://t3sf.readthedocs.io/en/latest/Telegram.html#installation)
   - [WhatsApp](https://t3sf.readthedocs.io/en/latest/WhatsApp.html#installation)
 
 ## Usage <a name="Usage"></a>
 We created this framework to simplify all your work!
 
+
+<details>
+<summary>Using Docker</summary>
+
+### Supported Tags
+- slack → This image has all the requirements to perform an exercise in Slack.
+- discord → This image has all the requirements to perform an exercise in Discord.
+
+
+#### Using it with Slack
+
+```bash
+$ docker run --rm -t --env-file .env -v $(pwd)/MSEL.json:/app/MSEL.json base4sec/t3sf:slack
+```
+
+Inside your `.env` file you have to provide the `SLACK_BOT_TOKEN` and `SLACK_APP_TOKEN` tokens. Read more about it [here](https://t3sf.readthedocs.io/en/latest/Slack.html#providing-the-tokens).
+
+There is another environment variable to set, `MSEL_PATH`. This variable tells the framework in which path the MSEL is located. By default, the container path is `/app/MSEL.json`. If you change the mount location of the volume then also change the variable.
+
+
+#### Using it with Discord
+
+```bash
+$ docker run --rm -t --env-file .env -v $(pwd)/MSEL.json:/app/MSEL.json base4sec/t3sf:discord
+```
+
+Inside your `.env` file you have to provide the `DISCORD_TOKEN` token. Read more about it [here](https://t3sf.readthedocs.io/en/latest/Discord.html#providing-the-token).
+
+There is another environment variable to set, `MSEL_PATH`. This variable tells the framework in which path the MSEL is located. By default, the container path is `/app/MSEL.json`. If you change the mount location of the volume then also change the variable.
+
+---------------------
+</details>
+
 Once you have everything ready, use our template for the `main.py`, or modify the following code:
 
 Here is an example if you want to run the framework with the `Discord` bot and a `GUI`.
 
 ```python
 from T3SF import T3SF
 import asyncio
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.1rc1 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.5rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
 Provides-Extra: Discord License-File: LICENSE
-                                 [WhaBot Logo]
+                                  [T3SF Logo]
                                 **** T3SF ****
  [![Status](https://img.shields.io/badge/status-active-success.svg)]() [![PyPI
 version](https://badge.fury.io/py/T3SF.svg)](https://badge.fury.io/py/T3SF) [!
       [Documentation Status](https://readthedocs.org/projects/t3sf/badge/
    ?version=latest)](https://t3sf.readthedocs.io/en/latest/?badge=latest) [!
 [License](https://img.shields.io/badge/license-GPL-blue.svg)](/LICENSE) [![DOI]
   (https://zenodo.org/badge/DOI/10.5281/zenodo.6519221.svg)](https://doi.org/
                             10.5281/zenodo.6519221)
+  [![Docker Image for Discord](https://github.com/Base4Security/T3SF/actions/
+ workflows/publish_discord.yml/badge.svg)](https://hub.docker.com/r/base4sec/
+t3sf) [![Docker Image for Slack](https://github.com/Base4Security/T3SF/actions/
+workflows/publish_slack.yml/badge.svg)](https://hub.docker.com/r/base4sec/t3sf)
               Technical Tabletop Exercises Simulation Framework
 ## Table of Contents - [About](#About) - [Getting Things Ready](#Starting) -
 [TODO](./TODO.md) - [CHANGELOG](./CHANGELOG.md) - [Contributing](./
 CONTRIBUTING.md) ## About  T3SF is a framework that offers a modular structure
 for the orchestration of events based on a master scenario events list (MSEL)
 together with a set of rules defined for each exercise (optional) and a
 configuration that allows defining the parameters of the corresponding
@@ -44,17 +48,35 @@
 platform. Once the installation is complete, you can start using the framework
 with your platform of choice. We strongly recommend following the platform-
 specific guidance within our Read The Docs! Here are the links: - [Discord]
 (https://t3sf.readthedocs.io/en/latest/Discord.html#installation) - [Slack]
 (https://t3sf.readthedocs.io/en/latest/Slack.html#installation) - [Telegram]
 (https://t3sf.readthedocs.io/en/latest/Telegram.html#installation) - [WhatsApp]
 (https://t3sf.readthedocs.io/en/latest/WhatsApp.html#installation) ## Usage  We
-created this framework to simplify all your work! Once you have everything
-ready, use our template for the `main.py`, or modify the following code: Here
-is an example if you want to run the framework with the `Discord` bot and a
-`GUI`. ```python from T3SF import T3SF import asyncio async def main(): await
+created this framework to simplify all your work!  Using Docker ### Supported
+Tags - slack â This image has all the requirements to perform an exercise in
+Slack. - discord â This image has all the requirements to perform an exercise
+in Discord. #### Using it with Slack ```bash $ docker run --rm -t --env-file
+.env -v $(pwd)/MSEL.json:/app/MSEL.json base4sec/t3sf:slack ``` Inside your
+`.env` file you have to provide the `SLACK_BOT_TOKEN` and `SLACK_APP_TOKEN`
+tokens. Read more about it [here](https://t3sf.readthedocs.io/en/latest/
+Slack.html#providing-the-tokens). There is another environment variable to set,
+`MSEL_PATH`. This variable tells the framework in which path the MSEL is
+located. By default, the container path is `/app/MSEL.json`. If you change the
+mount location of the volume then also change the variable. #### Using it with
+Discord ```bash $ docker run --rm -t --env-file .env -v $(pwd)/MSEL.json:/app/
+MSEL.json base4sec/t3sf:discord ``` Inside your `.env` file you have to provide
+the `DISCORD_TOKEN` token. Read more about it [here](https://
+t3sf.readthedocs.io/en/latest/Discord.html#providing-the-token). There is
+another environment variable to set, `MSEL_PATH`. This variable tells the
+framework in which path the MSEL is located. By default, the container path is
+`/app/MSEL.json`. If you change the mount location of the volume then also
+change the variable. ---------------------  Once you have everything ready, use
+our template for the `main.py`, or modify the following code: Here is an
+example if you want to run the framework with the `Discord` bot and a `GUI`.
+```python from T3SF import T3SF import asyncio async def main(): await
 T3SF.start(MSEL="MSEL_TTX.json", platform="Discord", gui=True) if __name__ ==
 '__main__': asyncio.run(main()) ``` Or if you prefer to run the framework
 without `GUI` and with `Slack` instead, you can modify the arguments, and
 that's it! Yes, that simple! ```python await T3SF.start(MSEL="MSEL_TTX.json",
 platform="Slack", gui=False) ``` If you need more help, you can always check
 our documentation [here](https://t3sf.readthedocs.io/en/latest/)!
```

