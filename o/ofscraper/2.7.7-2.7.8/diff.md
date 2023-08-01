# Comparing `tmp/ofscraper-2.7.7.tar.gz` & `tmp/ofscraper-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.7.7.tar", max compression
+gzip compressed data, was "ofscraper-2.7.8.tar", max compression
```

## Comparing `ofscraper-2.7.7.tar` & `ofscraper-2.7.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-08-01 13:59:00.508663 ofscraper-2.7.7/LICENSE
--rw-r--r--   0        0        0     2859 2023-08-01 13:59:00.508663 ofscraper-2.7.7/README.md
--rw-r--r--   0        0        0      607 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/__init__.py
--rw-r--r--   0        0        0     1016 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8591 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9690 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1060 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/init.py
--rw-r--r--   0        0        0     7357 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/labels.py
--rw-r--r--   0        0        0     3246 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/me.py
--rw-r--r--   0        0        0     9415 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9499 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5645 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     4393 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3294 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9141 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/api/timeline.py
--rw-r--r--   0        0        0        0 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/classes/__init__.py
--rw-r--r--   0        0        0      804 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8491 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/classes/media.py
--rw-r--r--   0        0        0     7278 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3737 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/classes/posts.py
--rw-r--r--   0        0        0     4656 2023-08-01 13:59:00.516663 ofscraper-2.7.7/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    29810 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/classes/table.py
--rw-r--r--   0        0        0    14593 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5353 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    14111 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6936 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10059 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4891 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      730 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     5794 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0     6695 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7834 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    29433 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1583 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    12404 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/args.py
--rw-r--r--   0        0        0    10197 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    13774 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/console.py
--rw-r--r--   0        0        0     1080 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    28038 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5564 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     7367 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/logger.py
--rw-r--r--   0        0        0    10686 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7013 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1211 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     5638 2023-08-01 13:59:00.520663 ofscraper-2.7.7/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1967 2023-08-01 13:59:42.121894 ofscraper-2.7.7/pyproject.toml
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 ofscraper-2.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-01 13:58:44.537582 ofscraper-2.7.8/LICENSE
+-rw-r--r--   0        0        0     2859 2023-08-01 13:58:44.537582 ofscraper-2.7.8/README.md
+-rw-r--r--   0        0        0      607 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/__init__.py
+-rw-r--r--   0        0        0     1016 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8591 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9690 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1060 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7357 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     3246 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9415 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9499 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5645 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4393 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3294 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9141 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/classes/__init__.py
+-rw-r--r--   0        0        0      804 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8491 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     7278 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3737 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4656 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29810 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14593 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5353 2023-08-01 13:58:44.545582 ofscraper-2.7.8/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    14111 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6936 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10059 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4891 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      730 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     5794 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0     6695 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7834 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    29433 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1583 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    12404 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/args.py
+-rw-r--r--   0        0        0    10197 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    13774 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    28038 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5564 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     7367 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0    10686 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7013 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1211 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5638 2023-08-01 13:58:44.549582 ofscraper-2.7.8/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1967 2023-08-01 13:59:23.661998 ofscraper-2.7.8/pyproject.toml
+-rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 ofscraper-2.7.8/PKG-INFO
```

### Comparing `ofscraper-2.7.7/LICENSE` & `ofscraper-2.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/README.md` & `ofscraper-2.7.8/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/__init__.py` & `ofscraper-2.7.8/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/__version__.py` & `ofscraper-2.7.8/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/__version__.pye` & `ofscraper-2.7.8/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/archive.py` & `ofscraper-2.7.8/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/highlights.py` & `ofscraper-2.7.8/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/init.py` & `ofscraper-2.7.8/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/labels.py` & `ofscraper-2.7.8/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/me.py` & `ofscraper-2.7.8/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/messages.py` & `ofscraper-2.7.8/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/paid.py` & `ofscraper-2.7.8/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/pinned.py` & `ofscraper-2.7.8/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/profile.py` & `ofscraper-2.7.8/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/subscriptions.py` & `ofscraper-2.7.8/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/api/timeline.py` & `ofscraper-2.7.8/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/classes/labels.py` & `ofscraper-2.7.8/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/classes/media.py` & `ofscraper-2.7.8/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/classes/placeholder.py` & `ofscraper-2.7.8/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/classes/posts.py` & `ofscraper-2.7.8/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/classes/sessionbuilder.py` & `ofscraper-2.7.8/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/classes/table.py` & `ofscraper-2.7.8/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/commands/check.py` & `ofscraper-2.7.8/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/commands/manual.py` & `ofscraper-2.7.8/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/commands/scraper.py` & `ofscraper-2.7.8/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/constants.py` & `ofscraper-2.7.8/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/db/operations.py` & `ofscraper-2.7.8/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/db/queries.py` & `ofscraper-2.7.8/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/interaction/like.py` & `ofscraper-2.7.8/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/prompts/keybindings.py` & `ofscraper-2.7.8/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/prompts/promptConvert.py` & `ofscraper-2.7.8/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.7.8/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.7.8/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/prompts/prompts.py` & `ofscraper-2.7.8/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/start.py` & `ofscraper-2.7.8/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/args.py` & `ofscraper-2.7.8/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/auth.py` & `ofscraper-2.7.8/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/binaries.py` & `ofscraper-2.7.8/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/config.py` & `ofscraper-2.7.8/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/dates.py` & `ofscraper-2.7.8/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/download.py` & `ofscraper-2.7.8/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/encoding.py` & `ofscraper-2.7.8/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/exit.py` & `ofscraper-2.7.8/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/filters.py` & `ofscraper-2.7.8/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/logger.py` & `ofscraper-2.7.8/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/of.py` & `ofscraper-2.7.8/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/paths.py` & `ofscraper-2.7.8/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/profiles.py` & `ofscraper-2.7.8/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/separate.py` & `ofscraper-2.7.8/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/stdout.py` & `ofscraper-2.7.8/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/ofscraper/utils/userselector.py` & `ofscraper-2.7.8/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.7/pyproject.toml` & `ofscraper-2.7.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.7.7"
+version = "2.7.8"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
@@ -26,17 +26,17 @@
 dunamai = "^1.17.0"
 poetry-dynamic-versioning = "^0.22.0"
 textual = "^0.27.0"
 aiohttp = {extras = ["speedups"], version = "^3.8.4"}
 faust-cchardet = "^2.1.18"
 certifi = "^2023.5.7"
 aiosqlite = "^0.19.0"
-pycryptodome = "^3.18.0"
 pywidevine = "^1.6.0"
 aiomultiprocess = "^0.9.0"
+pycryptodome = "^3.18.0"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
```

### Comparing `ofscraper-2.7.7/PKG-INFO` & `ofscraper-2.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.7.7
+Version: 2.7.8
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

