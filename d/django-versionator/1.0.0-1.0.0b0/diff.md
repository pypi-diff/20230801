# Comparing `tmp/django-versionator-1.0.0.tar.gz` & `tmp/django-versionator-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-versionator-1.0.0.tar", last modified: Tue Aug  1 18:05:28 2023, max compression
+gzip compressed data, was "django-versionator-1.0.0b0.tar", last modified: Tue Aug  1 17:26:16 2023, max compression
```

## Comparing `django-versionator-1.0.0.tar` & `django-versionator-1.0.0b0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.594751 django-versionator-1.0.0/
--rw-r--r--   0 acl        (501) staff       (20)      393 2023-08-01 18:05:28.594597 django-versionator-1.0.0/PKG-INFO
--rw-r--r--   0 acl        (501) staff       (20)       38 2023-07-28 19:07:13.000000 django-versionator-1.0.0/README.md
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.586406 django-versionator-1.0.0/django_versionator.egg-info/
--rw-r--r--   0 acl        (501) staff       (20)      393 2023-08-01 18:05:28.000000 django-versionator-1.0.0/django_versionator.egg-info/PKG-INFO
--rw-r--r--   0 acl        (501) staff       (20)     1898 2023-08-01 18:05:28.000000 django-versionator-1.0.0/django_versionator.egg-info/SOURCES.txt
--rw-r--r--   0 acl        (501) staff       (20)        1 2023-08-01 18:05:28.000000 django-versionator-1.0.0/django_versionator.egg-info/dependency_links.txt
--rw-r--r--   0 acl        (501) staff       (20)      108 2023-08-01 18:05:28.000000 django-versionator-1.0.0/django_versionator.egg-info/requires.txt
--rw-r--r--   0 acl        (501) staff       (20)       12 2023-08-01 18:05:28.000000 django-versionator-1.0.0/django_versionator.egg-info/top_level.txt
--rw-r--r--   0 acl        (501) staff       (20)       38 2023-08-01 18:05:28.594799 django-versionator-1.0.0/setup.cfg
--rw-r--r--   0 acl        (501) staff       (20)     1160 2023-08-01 18:05:15.000000 django-versionator-1.0.0/setup.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.587365 django-versionator-1.0.0/tests/
--rw-r--r--   0 acl        (501) staff       (20)     4030 2023-07-28 19:07:13.000000 django-versionator-1.0.0/tests/test_changelog.py
--rw-r--r--   0 acl        (501) staff       (20)      652 2023-03-13 15:50:58.000000 django-versionator-1.0.0/tests/test_edited_by_versioning.py
--rw-r--r--   0 acl        (501) staff       (20)     6451 2023-08-01 17:25:18.000000 django-versionator-1.0.0/tests/test_versioning.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.588333 django-versionator-1.0.0/versionator/
--rw-r--r--   0 acl        (501) staff       (20)       64 2023-03-13 14:43:23.000000 django-versionator-1.0.0/versionator/__init__.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.589729 django-versionator-1.0.0/versionator/changelog/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     2433 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/arbitrary_version_pair_fetcher.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.590074 django-versionator-1.0.0/versionator/changelog/changelog_graphql/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/__init__.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.591727 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/
--rw-r--r--   0 acl        (501) staff       (20)      236 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     3720 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/changelog_entry.py
--rw-r--r--   0 acl        (501) staff       (20)     1949 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py
--rw-r--r--   0 acl        (501) staff       (20)     1162 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/changelog_page.py
--rw-r--r--   0 acl        (501) staff       (20)    10165 2023-08-01 17:25:18.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/diff.py
--rw-r--r--   0 acl        (501) staff       (20)      753 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/version.py
--rw-r--r--   0 acl        (501) staff       (20)     2801 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py
--rw-r--r--   0 acl        (501) staff       (20)     3836 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/changelog_graphql/util.py
--rw-r--r--   0 acl        (501) staff       (20)     8109 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/consecutive_versions_fetcher.py
--rw-r--r--   0 acl        (501) staff       (20)     3279 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/diff_utils.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.593053 django-versionator-1.0.0/versionator/changelog/graphql/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     2364 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/dataloader.py
--rw-r--r--   0 acl        (501) staff       (20)     1758 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/graphiql_view_base.py
--rw-r--r--   0 acl        (501) staff       (20)      180 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/graphql_context.py
--rw-r--r--   0 acl        (501) staff       (20)     2741 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/internal_query_executor_base.py
--rw-r--r--   0 acl        (501) staff       (20)     1235 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/middleware.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.593429 django-versionator-1.0.0/versionator/changelog/graphql/testing/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/testing/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)      683 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/testing/fixtures.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.593910 django-versionator-1.0.0/versionator/changelog/graphql/types/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/types/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)      634 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py
--rw-r--r--   0 acl        (501) staff       (20)      966 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/types/version.py
--rw-r--r--   0 acl        (501) staff       (20)     2535 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/graphql/utils.py
--rw-r--r--   0 acl        (501) staff       (20)     2850 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/simple_changelog.py
--rw-r--r--   0 acl        (501) staff       (20)      490 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/util.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 18:05:28.594330 django-versionator-1.0.0/versionator/changelog/views/
--rw-r--r--   0 acl        (501) staff       (20)       59 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/views/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     2060 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/changelog/views/abstract_changelog_view.py
--rw-r--r--   0 acl        (501) staff       (20)    11612 2023-08-01 17:43:06.000000 django-versionator-1.0.0/versionator/core.py
--rw-r--r--   0 acl        (501) staff       (20)     1158 2023-03-13 14:43:23.000000 django-versionator-1.0.0/versionator/middleware.py
--rw-r--r--   0 acl        (501) staff       (20)      343 2023-07-28 19:07:13.000000 django-versionator-1.0.0/versionator/utils.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.037182 django-versionator-1.0.0b0/
+-rw-r--r--   0 acl        (501) staff       (20)      395 2023-08-01 17:26:16.037039 django-versionator-1.0.0b0/PKG-INFO
+-rw-r--r--   0 acl        (501) staff       (20)       38 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/README.md
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.031406 django-versionator-1.0.0b0/django_versionator.egg-info/
+-rw-r--r--   0 acl        (501) staff       (20)      395 2023-08-01 17:26:16.000000 django-versionator-1.0.0b0/django_versionator.egg-info/PKG-INFO
+-rw-r--r--   0 acl        (501) staff       (20)     1898 2023-08-01 17:26:16.000000 django-versionator-1.0.0b0/django_versionator.egg-info/SOURCES.txt
+-rw-r--r--   0 acl        (501) staff       (20)        1 2023-08-01 17:26:16.000000 django-versionator-1.0.0b0/django_versionator.egg-info/dependency_links.txt
+-rw-r--r--   0 acl        (501) staff       (20)      108 2023-08-01 17:26:16.000000 django-versionator-1.0.0b0/django_versionator.egg-info/requires.txt
+-rw-r--r--   0 acl        (501) staff       (20)       12 2023-08-01 17:26:16.000000 django-versionator-1.0.0b0/django_versionator.egg-info/top_level.txt
+-rw-r--r--   0 acl        (501) staff       (20)       38 2023-08-01 17:26:16.037228 django-versionator-1.0.0b0/setup.cfg
+-rw-r--r--   0 acl        (501) staff       (20)     1161 2023-08-01 17:25:43.000000 django-versionator-1.0.0b0/setup.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.031860 django-versionator-1.0.0b0/tests/
+-rw-r--r--   0 acl        (501) staff       (20)     4030 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/tests/test_changelog.py
+-rw-r--r--   0 acl        (501) staff       (20)      652 2023-03-13 15:50:58.000000 django-versionator-1.0.0b0/tests/test_edited_by_versioning.py
+-rw-r--r--   0 acl        (501) staff       (20)     6451 2023-08-01 17:25:18.000000 django-versionator-1.0.0b0/tests/test_versioning.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.032490 django-versionator-1.0.0b0/versionator/
+-rw-r--r--   0 acl        (501) staff       (20)       64 2023-03-13 14:43:23.000000 django-versionator-1.0.0b0/versionator/__init__.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.033461 django-versionator-1.0.0b0/versionator/changelog/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     2433 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/arbitrary_version_pair_fetcher.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.033763 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/__init__.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.034895 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/
+-rw-r--r--   0 acl        (501) staff       (20)      236 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     3720 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_entry.py
+-rw-r--r--   0 acl        (501) staff       (20)     1949 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py
+-rw-r--r--   0 acl        (501) staff       (20)     1162 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_page.py
+-rw-r--r--   0 acl        (501) staff       (20)    10165 2023-08-01 17:25:18.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/diff.py
+-rw-r--r--   0 acl        (501) staff       (20)      753 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/version.py
+-rw-r--r--   0 acl        (501) staff       (20)     2801 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py
+-rw-r--r--   0 acl        (501) staff       (20)     3836 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/util.py
+-rw-r--r--   0 acl        (501) staff       (20)     8109 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/consecutive_versions_fetcher.py
+-rw-r--r--   0 acl        (501) staff       (20)     3279 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/diff_utils.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.035872 django-versionator-1.0.0b0/versionator/changelog/graphql/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     2364 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/dataloader.py
+-rw-r--r--   0 acl        (501) staff       (20)     1758 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/graphiql_view_base.py
+-rw-r--r--   0 acl        (501) staff       (20)      180 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/graphql_context.py
+-rw-r--r--   0 acl        (501) staff       (20)     2741 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/internal_query_executor_base.py
+-rw-r--r--   0 acl        (501) staff       (20)     1235 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/middleware.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.036131 django-versionator-1.0.0b0/versionator/changelog/graphql/testing/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/testing/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)      683 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/testing/fixtures.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.036545 django-versionator-1.0.0b0/versionator/changelog/graphql/types/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/types/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)      634 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py
+-rw-r--r--   0 acl        (501) staff       (20)      966 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/types/version.py
+-rw-r--r--   0 acl        (501) staff       (20)     2535 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/graphql/utils.py
+-rw-r--r--   0 acl        (501) staff       (20)     2850 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/simple_changelog.py
+-rw-r--r--   0 acl        (501) staff       (20)      490 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/util.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-08-01 17:26:16.036844 django-versionator-1.0.0b0/versionator/changelog/views/
+-rw-r--r--   0 acl        (501) staff       (20)       59 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/views/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     2060 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/changelog/views/abstract_changelog_view.py
+-rw-r--r--   0 acl        (501) staff       (20)    11616 2023-08-01 17:25:18.000000 django-versionator-1.0.0b0/versionator/core.py
+-rw-r--r--   0 acl        (501) staff       (20)     1158 2023-03-13 14:43:23.000000 django-versionator-1.0.0b0/versionator/middleware.py
+-rw-r--r--   0 acl        (501) staff       (20)      343 2023-07-28 19:07:13.000000 django-versionator-1.0.0b0/versionator/utils.py
```

### Comparing `django-versionator-1.0.0/django_versionator.egg-info/SOURCES.txt` & `django-versionator-1.0.0b0/django_versionator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/setup.py` & `django-versionator-1.0.0b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-versionator",
-    version="1.0.0",
+    version="1.0.0b",
     author="AlexCLeduc",
     # author_email="author@example.com",
     # description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexCleduc/django-versionator",
     packages=[
```

### Comparing `django-versionator-1.0.0/tests/test_changelog.py` & `django-versionator-1.0.0b0/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/tests/test_edited_by_versioning.py` & `django-versionator-1.0.0b0/tests/test_edited_by_versioning.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/tests/test_versioning.py` & `django-versionator-1.0.0b0/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/arbitrary_version_pair_fetcher.py` & `django-versionator-1.0.0b0/versionator/changelog/arbitrary_version_pair_fetcher.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/changelog_entry.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_entry.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/changelog_page.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_page.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/diff.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/diff.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/version.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/version.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/changelog_graphql/util.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/util.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/consecutive_versions_fetcher.py` & `django-versionator-1.0.0b0/versionator/changelog/consecutive_versions_fetcher.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/diff_utils.py` & `django-versionator-1.0.0b0/versionator/changelog/diff_utils.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/dataloader.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/dataloader.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/graphiql_view_base.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/graphiql_view_base.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/internal_query_executor_base.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/internal_query_executor_base.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/middleware.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/middleware.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/testing/fixtures.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/types/version.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/types/version.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/graphql/utils.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/utils.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/simple_changelog.py` & `django-versionator-1.0.0b0/versionator/changelog/simple_changelog.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/changelog/views/abstract_changelog_view.py` & `django-versionator-1.0.0b0/versionator/changelog/views/abstract_changelog_view.py`

 * *Files identical despite different names*

### Comparing `django-versionator-1.0.0/versionator/core.py` & `django-versionator-1.0.0b0/versionator/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
         return versioned_fields
 
     @staticmethod
     def _create_m2m_fields(version_cls, live_model):
         m2m_fields_to_add = {}
         for field in version_cls.get_m2m_fields_to_version():
-            new_field = M2MTextField(default="[]")
+            new_field = models.TextField(default="[]")
             m2m_fields_to_add[field.name] = new_field
 
         return m2m_fields_to_add
 
     @staticmethod
     def _attach_signals(live_model):
         post_save.connect(save_copy_post_save, live_model)
```

### Comparing `django-versionator-1.0.0/versionator/middleware.py` & `django-versionator-1.0.0b0/versionator/middleware.py`

 * *Files identical despite different names*

