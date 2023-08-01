# Comparing `tmp/django-versionator-0.2.0b0.tar.gz` & `tmp/django-versionator-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-versionator-0.2.0b0.tar", last modified: Fri Jul 28 19:08:07 2023, max compression
+gzip compressed data, was "django-versionator-1.0.0b0.tar", last modified: Tue Aug  1 17:26:16 2023, max compression
```

## Comparing `django-versionator-0.2.0b0.tar` & `django-versionator-1.0.0b0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.606867 django-versionator-0.2.0b0/
--rw-r--r--   0 acl        (501) staff       (20)      395 2023-07-28 19:08:07.606681 django-versionator-0.2.0b0/PKG-INFO
--rw-r--r--   0 acl        (501) staff       (20)       38 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/README.md
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.599297 django-versionator-0.2.0b0/django_versionator.egg-info/
--rw-r--r--   0 acl        (501) staff       (20)      395 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/PKG-INFO
--rw-r--r--   0 acl        (501) staff       (20)     1898 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/SOURCES.txt
--rw-r--r--   0 acl        (501) staff       (20)        1 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/dependency_links.txt
--rw-r--r--   0 acl        (501) staff       (20)      108 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/requires.txt
--rw-r--r--   0 acl        (501) staff       (20)       12 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/top_level.txt
--rw-r--r--   0 acl        (501) staff       (20)       38 2023-07-28 19:08:07.606927 django-versionator-0.2.0b0/setup.cfg
--rw-r--r--   0 acl        (501) staff       (20)     1161 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/setup.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.600084 django-versionator-0.2.0b0/tests/
--rw-r--r--   0 acl        (501) staff       (20)     4030 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/tests/test_changelog.py
--rw-r--r--   0 acl        (501) staff       (20)      652 2023-03-13 15:50:58.000000 django-versionator-0.2.0b0/tests/test_edited_by_versioning.py
--rw-r--r--   0 acl        (501) staff       (20)     6195 2023-03-13 15:50:58.000000 django-versionator-0.2.0b0/tests/test_versioning.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.601189 django-versionator-0.2.0b0/versionator/
--rw-r--r--   0 acl        (501) staff       (20)       64 2023-03-13 14:43:23.000000 django-versionator-0.2.0b0/versionator/__init__.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.602550 django-versionator-0.2.0b0/versionator/changelog/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     2433 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/arbitrary_version_pair_fetcher.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.602826 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/__init__.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.604085 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/
--rw-r--r--   0 acl        (501) staff       (20)      236 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     3720 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_entry.py
--rw-r--r--   0 acl        (501) staff       (20)     1949 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py
--rw-r--r--   0 acl        (501) staff       (20)     1162 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_page.py
--rw-r--r--   0 acl        (501) staff       (20)    10146 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/diff.py
--rw-r--r--   0 acl        (501) staff       (20)      753 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/version.py
--rw-r--r--   0 acl        (501) staff       (20)     2801 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py
--rw-r--r--   0 acl        (501) staff       (20)     3836 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/util.py
--rw-r--r--   0 acl        (501) staff       (20)     8109 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/consecutive_versions_fetcher.py
--rw-r--r--   0 acl        (501) staff       (20)     3279 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/diff_utils.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.605329 django-versionator-0.2.0b0/versionator/changelog/graphql/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     2364 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/dataloader.py
--rw-r--r--   0 acl        (501) staff       (20)     1758 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/graphiql_view_base.py
--rw-r--r--   0 acl        (501) staff       (20)      180 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/graphql_context.py
--rw-r--r--   0 acl        (501) staff       (20)     2741 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/internal_query_executor_base.py
--rw-r--r--   0 acl        (501) staff       (20)     1235 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/middleware.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.605649 django-versionator-0.2.0b0/versionator/changelog/graphql/testing/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/testing/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)      683 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/testing/fixtures.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.606090 django-versionator-0.2.0b0/versionator/changelog/graphql/types/
--rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/types/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)      634 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py
--rw-r--r--   0 acl        (501) staff       (20)      966 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/types/version.py
--rw-r--r--   0 acl        (501) staff       (20)     2535 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/utils.py
--rw-r--r--   0 acl        (501) staff       (20)     2850 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/simple_changelog.py
--rw-r--r--   0 acl        (501) staff       (20)      490 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/util.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.606435 django-versionator-0.2.0b0/versionator/changelog/views/
--rw-r--r--   0 acl        (501) staff       (20)       59 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/views/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)     2060 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/views/abstract_changelog_view.py
--rw-r--r--   0 acl        (501) staff       (20)    11348 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/core.py
--rw-r--r--   0 acl        (501) staff       (20)     1158 2023-03-13 14:43:23.000000 django-versionator-0.2.0b0/versionator/middleware.py
--rw-r--r--   0 acl        (501) staff       (20)      343 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/utils.py
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

### Comparing `django-versionator-0.2.0b0/django_versionator.egg-info/SOURCES.txt` & `django-versionator-1.0.0b0/django_versionator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/setup.py` & `django-versionator-1.0.0b0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-versionator",
-    version="0.2.0b",
+    version="1.0.0b",
     author="AlexCLeduc",
     # author_email="author@example.com",
     # description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexCleduc/django-versionator",
     packages=[
```

### Comparing `django-versionator-0.2.0b0/tests/test_changelog.py` & `django-versionator-1.0.0b0/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/tests/test_edited_by_versioning.py` & `django-versionator-1.0.0b0/tests/test_edited_by_versioning.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/tests/test_versioning.py` & `django-versionator-1.0.0b0/tests/test_versioning.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,106 +84,103 @@
 
     live_inst_1 = common.LiveModel.objects.create(name="v1", favorite_group=common.group1)
     assert live_inst_1.versions.count() == 1
     v1 = live_inst_1.versions.last()
     assert v1.eternal == live_inst_1
     assert v1.name == "v1"
     assert v1.favorite_group_id == common.group1.id
-    assert v1.groups == []
-
+    assert v1.get_m2m_ids("groups") == []
+    
     live_inst_1.reset_version_attrs()
     live_inst_1.groups.add(common.group1)
     live_inst_1.save()
     assert live_inst_1.versions.count() == 2
     v2 = live_inst_1.versions.last()
-    assert v2.groups == [common.group1.pk]
+    assert v2.get_m2m_ids("groups") == [common.group1.pk]
 
     v1.refresh_from_db()
-    assert v1.groups == []
+    assert v1.get_m2m_ids("groups") == []
 
 
 def test_m2m_add(common):
     obj = common.LiveModel.objects.create(name="v1", favorite_group=common.group1)
     obj.reset_version_attrs()
 
     obj.groups.add(common.group1)
 
     # check og version wasn't modified
     assert obj.versions.count() == 2
-    assert obj.versions.first().groups == []
-    assert obj.versions.last().groups == [common.group1.pk]
-
+    assert obj.versions.first().get_m2m_ids("groups") == []
+    assert obj.versions.last().get_m2m_ids("groups") == [common.group1.pk]
 
 def test_m2m_rm(common):
     obj = common.LiveModel.objects.create(name="v1", favorite_group=common.group1)
     obj.groups.add(common.group1)
 
     assert obj.versions.count() == 1
-    assert obj.versions.last().groups == [common.group1.pk]
+    assert obj.versions.last().get_m2m_ids("groups") == [common.group1.pk]
 
     obj.reset_version_attrs()
     obj.groups.remove(common.group1)
 
     # check og version wasn't modified
     assert obj.versions.count() == 2
-    assert obj.versions.first().groups == [common.group1.pk]
-    assert obj.versions.last().groups == []
-
+    assert obj.versions.first().get_m2m_ids("groups") == [common.group1.pk]
+    assert obj.versions.last().get_m2m_ids("groups") == []
 
 def test_m2m_add_and_rm(common):
     obj = common.LiveModel.objects.create(name="v1", favorite_group=common.group1)
     obj.groups.add(common.group1)
 
     assert obj.versions.count() == 1
-    assert obj.versions.last().groups == [common.group1.pk]
+    assert obj.versions.last().get_m2m_ids("groups") == [common.group1.pk]
 
     obj.reset_version_attrs()
     obj.groups.remove(common.group1)
     obj.groups.add(common.group2)
 
     assert obj.versions.count() == 2
-    assert obj.versions.first().groups == [common.group1.pk]
-    assert obj.versions.last().groups == [common.group2.pk]
-
+    assert obj.versions.first().get_m2m_ids("groups") == [common.group1.pk]
+    assert obj.versions.last().get_m2m_ids("groups") == [common.group2.pk]
 
 def test_create_then_m2m_edit_doesnt_add_version(common):
     obj = common.LiveModel.objects.create(name="v1", favorite_group=common.group1)
     obj.groups.add(common.group1)
     assert obj.versions.count() == 1
-    assert obj.versions.last().groups == [common.group1.pk]
+    assert obj.versions.last().get_m2m_ids("groups") == [common.group1.pk]
 
 
 def test_scalar_edit_then_m2m_edit_only_adds_one_version(common):
     obj = common.LiveModel.objects.create(name="name1", favorite_group=common.group1)
     obj.reset_version_attrs()
 
     obj.name = "name2"
     obj.save()
     obj.groups.add(common.group1)
 
     assert obj.versions.count() == 2
     assert obj.versions.first().name == "name1"
-    assert obj.versions.first().groups == []
+    assert obj.versions.first().get_m2m_ids("groups") == []
     assert obj.versions.last().name == "name2"
-    assert obj.versions.last().groups == [common.group1.pk]
+    assert obj.versions.last().get_m2m_ids("groups") == [common.group1.pk]
 
 
 def test_m2m_change_then_scalar_change_only_adds_one_version(common):
     obj = common.LiveModel.objects.create(name="name1", favorite_group=common.group1)
     obj.reset_version_attrs()
 
     obj.groups.add(common.group1)
     obj.name = "name2"
     obj.save()
 
     assert obj.versions.count() == 2
     assert obj.versions.first().name == "name1"
-    assert obj.versions.first().groups == []
+    assert obj.versions.first().get_m2m_ids("groups") == []
     assert obj.versions.last().name == "name2"
-    assert obj.versions.last().groups == [common.group1.pk]
+    assert obj.versions.last().get_m2m_ids("groups") == [common.group1.pk]
 
 
 def test_create_via_model_form(common):
     class Form(ModelForm):
         class Meta:
             model = common.LiveModel
             fields = [
@@ -199,8 +196,8 @@
     }
 
     obj = Form(form_data).save()
     assert obj.pk
     assert obj.versions.count() == 1
     v1 = obj.versions.last()
     assert v1.name == "v1"
-    assert v1.groups == [common.group1.pk]
+    assert v1.get_m2m_ids("groups") == [common.group1.pk]
```

### Comparing `django-versionator-0.2.0b0/versionator/changelog/arbitrary_version_pair_fetcher.py` & `django-versionator-1.0.0b0/versionator/changelog/arbitrary_version_pair_fetcher.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_entry.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_entry.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_page.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/changelog_page.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/diff.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import inspect
 
-from django.db.models import ForeignKey, JSONField, ManyToManyField
+from django.db.models import ForeignKey, ManyToManyField
 from django.utils.functional import cached_property
 from django.utils.html import escape
 
 import graphene
 
 from promise import Promise
 
+from versionator.core import M2MTextField
 from versionator.changelog.diff_utils import list_diff, text_compare_inline
 from versionator.changelog.graphql.dataloader import PrimaryKeyDataLoaderFactory
 from versionator.changelog.graphql.utils import NonSerializable, genfunc_to_prom, non_serializable_field
 
 
 # this is used by the parent resolver and fed to the below graphene type
 class DiffObject:
@@ -121,17 +122,16 @@
         diffs = yield self._get_diffs()
         return diffs[2]
 
 
 class M2MDiffObject(AsyncDiffObject):
     @genfunc_to_prom
     def _compute_diffs(self):
-        prev_id_list = self.previous_version.serializable_value(self.field.name)
-        current_id_list = self.current_version.serializable_value(self.field.name)
-
+        prev_id_list = self.previous_version.get_m2m_ids(self.field.name)
+        current_id_list = self.current_version.get_m2m_ids(self.field.name)
         related_model = self.field.related_model
         related_dataloader_cls = PrimaryKeyDataLoaderFactory.get_model_by_id_loader(
             related_model
         )
         related_dataloader = related_dataloader_cls(self.dataloader_cache)
 
         prev_instances, current_instances = yield Promise.all(
@@ -182,15 +182,15 @@
 
 
 def is_field_different_accross_versions(current_version, previous_version, field_name):
     current_db_value = current_version.serializable_value(field_name)
     prev_db_value = previous_version.serializable_value(field_name)
 
     field_obj = current_version._meta.get_field(field_name)
-    if isinstance(field_obj, JSONField):
+    if isinstance(field_obj, M2MTextField):
         return current_db_value != prev_db_value
 
     if current_db_value == prev_db_value or (
         # consider "" vs. None to be non-diff worthy
         {current_db_value, prev_db_value}.issubset({None, ""})
     ):
         return False
```

### Comparing `django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/version.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/version.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/util.py` & `django-versionator-1.0.0b0/versionator/changelog/changelog_graphql/util.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/consecutive_versions_fetcher.py` & `django-versionator-1.0.0b0/versionator/changelog/consecutive_versions_fetcher.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/diff_utils.py` & `django-versionator-1.0.0b0/versionator/changelog/diff_utils.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/dataloader.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/dataloader.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/graphiql_view_base.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/graphiql_view_base.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/internal_query_executor_base.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/internal_query_executor_base.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/middleware.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/middleware.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/testing/fixtures.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/types/version.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/types/version.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/graphql/utils.py` & `django-versionator-1.0.0b0/versionator/changelog/graphql/utils.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/simple_changelog.py` & `django-versionator-1.0.0b0/versionator/changelog/simple_changelog.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/changelog/views/abstract_changelog_view.py` & `django-versionator-1.0.0b0/versionator/changelog/views/abstract_changelog_view.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.2.0b0/versionator/core.py` & `django-versionator-1.0.0b0/versionator/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from django.db import models
 from django.db.models import F, Manager, OuterRef, QuerySet, Subquery
 from django.db.models.base import ModelBase
 from django.db.models.signals import m2m_changed, post_save
 from django.utils import timezone
 
 # other imports, to remove
@@ -10,14 +11,20 @@
 class VersioningException(Exception):
     pass
 
 
 class VersioningConfigException(VersioningException):
     pass
 
+class M2MTextField(models.TextField):
+    """
+        A 'nominal' type is used for convenience of distinguishing from plain text fields
+    """
+    pass
+
 
 def find_m2m_field(from_class, to_class):
     return next(
         rel
         for rel in from_class._meta.get_fields()
         if isinstance(rel, models.ManyToManyField) and rel.related_model is to_class
     )
@@ -106,14 +113,17 @@
 
         return self.model.objects.filter(
             eternal_id__in=eternal_ids
         ).only_most_recent_versions()
 
 
 def m2m_default_empty_list():
+    """
+        here for legacy reasons, referred to from older migrations
+    """
     return []
 
 
 def create_version_field_from_live_field(field):
     name = field.attname
 
     ## forces uses of id as the primary key
@@ -234,15 +244,15 @@
 
         return versioned_fields
 
     @staticmethod
     def _create_m2m_fields(version_cls, live_model):
         m2m_fields_to_add = {}
         for field in version_cls.get_m2m_fields_to_version():
-            new_field = models.JSONField(default=m2m_default_empty_list)
+            new_field = models.TextField(default="[]")
             m2m_fields_to_add[field.name] = new_field
 
         return m2m_fields_to_add
 
     @staticmethod
     def _attach_signals(live_model):
         post_save.connect(save_copy_post_save, live_model)
@@ -316,18 +326,18 @@
             if not f.name in ["id", "timestamp"]:
                 setattr(version, f.attname, instance.serializable_value(f.name))
 
         version.save()
 
     @staticmethod
     def serialize_m2m_ids(pk_list):
-        return sorted(pk_list)
+        return json.dumps(sorted(pk_list))
 
     def get_m2m_ids(self, key):
-        getattr(self, key)
+        return json.loads(getattr(self, key) or [])
 
     def set_m2m(self, field, pk_set):
         setattr(self, field.name, self.serialize_m2m_ids(pk_set))
         self.save()
 
     def recreate_original(self):
         live_fields = [f for f in self.live_model._meta.fields if f.name != "id"]
```

### Comparing `django-versionator-0.2.0b0/versionator/middleware.py` & `django-versionator-1.0.0b0/versionator/middleware.py`

 * *Files identical despite different names*

