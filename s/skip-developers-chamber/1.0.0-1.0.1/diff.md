# Comparing `tmp/skip-developers-chamber-1.0.0.tar.gz` & `tmp/skip-developers-chamber-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-developers-chamber-1.0.0.tar", last modified: Tue Aug  1 11:24:05 2023, max compression
+gzip compressed data, was "skip-developers-chamber-1.0.1.tar", last modified: Tue Aug  1 12:37:03 2023, max compression
```

## Comparing `skip-developers-chamber-1.0.0.tar` & `skip-developers-chamber-1.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.403693 skip-developers-chamber-1.0.0/developers_chamber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.403693 skip-developers-chamber-1.0.0/developers_chamber/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/bin/pydev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/bitbucket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.407693 skip-developers-chamber-1.0.0/developers_chamber/click/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/click/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25338 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/ecs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/gitlab_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/jira_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/project_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.407693 skip-developers-chamber-1.0.0/developers_chamber/qa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/qa/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/qa/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.407693 skip-developers-chamber-1.0.0/developers_chamber/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/init_aliasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/sh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/slack_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/toggle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:03.255281 skip-developers-chamber-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 12:37:03.255281 skip-developers-chamber-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:03.251280 skip-developers-chamber-1.0.1/developers_chamber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:03.251280 skip-developers-chamber-1.0.1/developers_chamber/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/bin/pydev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/bitbucket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:03.255281 skip-developers-chamber-1.0.1/developers_chamber/click/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/click/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25338 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/ecs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/gitlab_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/jira_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/project_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:03.255281 skip-developers-chamber-1.0.1/developers_chamber/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/qa/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/qa/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:03.255281 skip-developers-chamber-1.0.1/developers_chamber/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/init_aliasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/scripts/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/slack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/toggle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/developers_chamber/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:37:03.255281 skip-developers-chamber-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 12:36:53.000000 skip-developers-chamber-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:03.255281 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 12:37:03.000000 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 12:37:03.000000 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:37:03.000000 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 12:37:03.000000 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:37:03.000000 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 12:37:03.000000 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 12:37:03.000000 skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/top_level.txt
```

### Comparing `skip-developers-chamber-1.0.0/LICENSE` & `skip-developers-chamber-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/README.md` & `skip-developers-chamber-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/bin/pydev.py` & `skip-developers-chamber-1.0.1/developers_chamber/bin/pydev.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/bitbucket_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/bitbucket_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/click/options.py` & `skip-developers-chamber-1.0.1/developers_chamber/click/options.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/ecs_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/git_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/git_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/gitlab_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/jira_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/jira_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/project_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/project_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/qa/base.py` & `skip-developers-chamber-1.0.1/developers_chamber/qa/base.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/qa/checks.py` & `skip-developers-chamber-1.0.1/developers_chamber/qa/checks.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/bitbucket.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/bitbucket.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/docker.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/docker.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/ecs.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/ecs.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/git.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/git.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/gitlab.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/gitlab.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/init_aliasses.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/init_aliasses.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/jira.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/jira.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/project.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/project.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/qa.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/qa.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/slack.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/slack.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/toggle.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/toggle.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/scripts/version.py` & `skip-developers-chamber-1.0.1/developers_chamber/scripts/version.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/slack_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/slack_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/toggle_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/toggle_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/types.py` & `skip-developers-chamber-1.0.1/developers_chamber/types.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/developers_chamber/version_utils.py` & `skip-developers-chamber-1.0.1/developers_chamber/version_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.0.0/setup.py` & `skip-developers-chamber-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='skip-developers-chamber',
-    version='1.0.0',
+    version='1.0.1',
     description='A small plugin which help with development, deployment, git',
     keywords='django, skripts, easy live, git, bitbucket, Jira',
     author='Druids team',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/developers-chamber',
     license='MIT',
     package_dir={'developers_chamber': 'developers_chamber'},
```

### Comparing `skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/SOURCES.txt` & `skip-developers-chamber-1.0.1/skip_developers_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

