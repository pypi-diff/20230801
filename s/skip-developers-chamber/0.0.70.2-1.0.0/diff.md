# Comparing `tmp/skip-developers-chamber-0.0.70.2.tar.gz` & `tmp/skip-developers-chamber-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-developers-chamber-0.0.70.2.tar", last modified: Tue Jul  4 13:39:21 2023, max compression
+gzip compressed data, was "skip-developers-chamber-1.0.0.tar", last modified: Tue Aug  1 11:24:05 2023, max compression
```

## Comparing `skip-developers-chamber-0.0.70.2.tar` & `skip-developers-chamber-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/bin/pydev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/bitbucket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/click/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/click/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25338 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/ecs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/gitlab_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/jira_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/project_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/qa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/qa/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/qa/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/init_aliasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/sh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/slack_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/toggle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.403693 skip-developers-chamber-1.0.0/developers_chamber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.403693 skip-developers-chamber-1.0.0/developers_chamber/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/bin/pydev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/bitbucket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.407693 skip-developers-chamber-1.0.0/developers_chamber/click/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/click/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25338 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/ecs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/gitlab_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/jira_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/project_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.407693 skip-developers-chamber-1.0.0/developers_chamber/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/qa/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/qa/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.407693 skip-developers-chamber-1.0.0/developers_chamber/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/init_aliasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/scripts/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/slack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/toggle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/developers_chamber/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 11:23:56.000000 skip-developers-chamber-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:05.411693 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:24:05.000000 skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/top_level.txt
```

### Comparing `skip-developers-chamber-0.0.70.2/LICENSE` & `skip-developers-chamber-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/README.md` & `skip-developers-chamber-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,14 @@
 
 #### Commands
 * `pydev qa all` - run all QA checks
 * `pydev qa missing-migrations` - run a missing Django migrations QA check. It will try to generate a Django migrations if there is one or more missing check is failed
 * `pydev qa migration-filenames` - run migration filenames QA check. Migration name should be in format "[0-9]{4}_migration.py" (ex. 0001_migration.py)
 * `pydev qa missing-translations` - run missing translations QA check. It will try to generate a Django `makemessages` if there is one or more missing check is failed
 * `pydev qa import-order` - run import order QA check. It will check if all the new python code imports have the right order defined with isort command
-* `pydev qa unused-imports` - run unused imports QA check. It will check if the new python code does not contain unused imports
 * `pydev qa test-method-names` - runs test method names QA check. It will check if the new test methods has the right name in format defined in `QA_DISALLOWED_TEST_METHOD_REGEXP` setting
 
 #### Configuration
 * `QA_DISALLOWED_TEST_METHOD_REGEXP` - your disallowed test method regex. Example: `"def (test_should_[^\(]+)\("` 
 
 ### Version
```

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/bin/pydev.py` & `skip-developers-chamber-1.0.0/developers_chamber/bin/pydev.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/bitbucket_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/bitbucket_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/click/options.py` & `skip-developers-chamber-1.0.0/developers_chamber/click/options.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/ecs_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/git_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/git_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/gitlab_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/jira_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/jira_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/project_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/project_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/qa/base.py` & `skip-developers-chamber-1.0.0/developers_chamber/qa/base.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/qa/checks.py` & `skip-developers-chamber-1.0.0/developers_chamber/qa/checks.py`

 * *Files 11% similar despite different names*

```diff
@@ -100,33 +100,14 @@
                     '\n'.join(wrong_import_order_files) +
                     '\n\n' +
                     'To fix it run: "isort {}"'.format(' '.join(wrong_import_order_files))
                 )
             )
 
 
-class UnusedImportsQACheck(QACheck):
-    """
-    Checks that there are no unused imports among changed files.
-    """
-    name = 'Check unused imports'
-
-    def _run_check(self):
-        changed_files = [diff.b_path for diff in self._get_diffs()
-                         if diff.b_path and self._is_python_file(diff.b_path)]
-        if changed_files:
-            output = self._run_command(
-                'flake8 --count --exit-zero --select=F401'
-                ' --per-file-ignores="__init__.py:F401"'
-                ' {}'.format(' '.join(changed_files))
-            )
-            if output != '0':
-                raise QAError('Found unused import(s):', output)
-
-
 class RegexPyQACheck(QACheck):
     """
     Helper for writing QAChecks which finds invalid regex patterns in python code.
     """
 
     pattern = None
 
@@ -162,21 +143,7 @@
 
     def _found_invalid_patterns(self, invalid_patterns):
         raise QAError(
             'Found disallowed test method name(s):',
             '\n'.join(('{}: {}'.format(file, value) for file, value in invalid_patterns))
         )
 
-
-class PrintStatementsQACheck(RegexPyQACheck):
-    """
-    Checks if changes do not contain print statements.
-    """
-    name = 'Checking for print statements'
-
-    pattern = r'(?:^|[^a-zA-Z0-9_])(print *\([^\)]*\))'
-
-    def _found_invalid_patterns(self, invalid_patterns):
-        raise QAError(
-            'Found print statement(s):',
-            '\n'.join(('{}: {}'.format(file, value) for file, value in invalid_patterns))
-        )
```

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/bitbucket.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/bitbucket.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/docker.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/docker.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/ecs.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/ecs.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/git.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/git.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/gitlab.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/gitlab.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/init_aliasses.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/init_aliasses.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/jira.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/jira.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/project.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/project.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/qa.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/qa.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from developers_chamber.qa.base import QACheck, QACheckRunner
 from developers_chamber.qa.checks import (ImportOrderQACheck,
                                           MigrationFilenamesQACheck,
                                           MissingMigrationsQACheck,
                                           MissingTranslationsQACheck,
-                                          TestMethodNamesQACheck,
-                                          PrintStatementsQACheck,
-                                          UnusedImportsQACheck)
+                                          TestMethodNamesQACheck)
 from developers_chamber.scripts import cli
 
 
 @cli.group()
 def qa():
     """Helpers for python project quality assurance."""
 
@@ -20,17 +18,15 @@
     Run all defined QA checks.
     """
     QACheckRunner(
         MissingMigrationsQACheck(),
         MigrationFilenamesQACheck(),
         MissingTranslationsQACheck(),
         ImportOrderQACheck(),
-        UnusedImportsQACheck(),
         TestMethodNamesQACheck(),
-        PrintStatementsQACheck(),
     ).run()
 
 
 @qa.command()
 def missing_migrations():
     """
     Run a missing Django migrations QA check. It will try to generate a Django migrations
@@ -63,29 +59,13 @@
     Run import order QA check. It will check if all the new python code imports have the right order
     defined with isort command.
     """
     QACheckRunner(ImportOrderQACheck()).run()
 
 
 @qa.command()
-def unused_imports():
-    """
-    Run unused imports QA check. It will check if the new python code does not contain unused imports and prints it.
-    """
-    QACheckRunner(UnusedImportsQACheck()).run()
-
-
-@qa.command()
 def test_method_names():
     """
     Runs test method names QA check. It will check if the new test methods has the right name in format defined in
     QA_DISALLOWED_TEST_METHOD_REGEXP setting.
     """
     QACheckRunner(TestMethodNamesQACheck()).run()
-
-
-@qa.command()
-def print_statements():
-    """
-    Runs print statements names QA check. It will check if the new test methods do not have python print statements.
-    """
-    QACheckRunner(PrintStatementsQACheck()).run()
```

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/slack.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/slack.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/toggle.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/toggle.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/version.py` & `skip-developers-chamber-1.0.0/developers_chamber/scripts/version.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/slack_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/slack_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/toggle_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/toggle_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/types.py` & `skip-developers-chamber-1.0.0/developers_chamber/types.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/developers_chamber/version_utils.py` & `skip-developers-chamber-1.0.0/developers_chamber/version_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.2/setup.py` & `skip-developers-chamber-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import find_packages, setup
 
 setup(
     name='skip-developers-chamber',
-    version='0.0.70.2',
+    version='1.0.0',
     description='A small plugin which help with development, deployment, git',
     keywords='django, skripts, easy live, git, bitbucket, Jira',
     author='Druids team',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/developers-chamber',
     license='MIT',
     package_dir={'developers_chamber': 'developers_chamber'},
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
         'boto3<2',
         'click>=7.0',
         'click-completion==0.5.2',
         'coloredlogs==10.0',
-        'flake8>=4.0.1',
         'gitpython==3.1.30',
         'isort>=5.12.0',
         'jira==2.0.0',
         'oauthlib==3.1.0',
         'pip-tools==6.13.0',
         'python-dotenv==0.14.0',
         'python-hosts==0.4.6',
```

### Comparing `skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/SOURCES.txt` & `skip-developers-chamber-1.0.0/skip_developers_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

