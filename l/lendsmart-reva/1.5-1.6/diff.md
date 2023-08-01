# Comparing `tmp/lendsmart_reva-1.5.tar.gz` & `tmp/lendsmart_reva-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_reva-1.5.tar", last modified: Wed May 24 11:03:32 2023, max compression
+gzip compressed data, was "lendsmart_reva-1.6.tar", last modified: Tue Aug  1 06:40:20 2023, max compression
```

## Comparing `lendsmart_reva-1.5.tar` & `lendsmart_reva-1.6.tar`

### file list

```diff
@@ -1,75 +1,89 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2442 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/lendsmart_reva.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1743 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      448 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      158 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/autotest.py
--rw-rw-r--   0 user      (1000) user      (1000)     3528 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/cli.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/conf/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/conf/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/conf/reva.py
--rw-rw-r--   0 user      (1000) user      (1000)      953 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/exception.py
--rw-rw-r--   0 user      (1000) user      (1000)      954 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/info.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/lib/auto/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/auto/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3988 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/auto/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/lib/base/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/base/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1101 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/base/base.py
--rw-rw-r--   0 user      (1000) user      (1000)      948 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/base/run_query.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/client/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/client/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      399 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/client/builder.py
--rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/client/graphql_client.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/document_access_control/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/document_access_control/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      728 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/document_access_control/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/document_access_control/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/graphql_queries/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      806 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)      641 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)      944 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      590 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/site_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      802 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/workflow.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/loan_productus/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/loan_productus/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      642 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/loan_productus/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/loan_productus/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/roles_and_permissions/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/roles_and_permissions/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      687 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/roles_and_permissions/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/roles_and_permissions/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/site_settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/site_settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/site_settings/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/site_settings/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/filter_data_with_id.py
--rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/get_json_files.py
--rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/get_namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)     3463 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/get_paths.py
--rw-rw-r--   0 user      (1000) user      (1000)      236 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/list_files.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/workflow/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/workflow/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      608 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/workflow/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/workflow/update.py
--rw-rw-r--   0 user      (1000) user      (1000)      878 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)      933 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      853 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/site_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      820 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/workflow.py
--rw-rw-r--   0 user      (1000) user      (1000)       86 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2144 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2442 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/lendsmart_reva.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2109 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      531 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      158 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      907 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/advisor_profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/autotest.py
+-rw-rw-r--   0 user      (1000) user      (1000)      839 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/branch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3528 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/cli.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/conf/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/conf/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/conf/reva.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)      954 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/info.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/advisor_profile/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/advisor_profile/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9937 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/advisor_profile/create.py
+-rw-rw-r--   0 user      (1000) user      (1000)      483 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/advisor_profile/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/auto/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/auto/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3988 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/auto/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/base/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/base/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1840 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/base/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      950 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/base/run_query.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/branch/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/branch/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3452 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/branch/create.py
+-rw-rw-r--   0 user      (1000) user      (1000)      439 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/branch/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/client/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/client/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      684 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/client/builder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/client/graphql_client.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/document_access_control/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/document_access_control/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      728 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/document_access_control/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/document_access_control/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/graphql_queries/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1954 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/advisor_profiles.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/branch.py
+-rw-rw-r--   0 user      (1000) user      (1000)      806 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)      641 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)      386 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/namespace.py
+-rw-rw-r--   0 user      (1000) user      (1000)      944 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      590 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      802 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/workflow.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/loan_productus/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/loan_productus/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/loan_productus/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/loan_productus/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/roles_and_permissions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/roles_and_permissions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      687 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/roles_and_permissions/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/roles_and_permissions/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/site_settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/site_settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/site_settings/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/site_settings/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      507 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/address.py
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/filter_data_with_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2634 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/get_json_files.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/get_namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3463 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/get_paths.py
+-rw-rw-r--   0 user      (1000) user      (1000)      236 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/list_files.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/workflow/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/workflow/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      608 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/workflow/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/workflow/update.py
+-rw-rw-r--   0 user      (1000) user      (1000)      878 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)      933 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      853 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      820 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/workflow.py
+-rw-rw-r--   0 user      (1000) user      (1000)       86 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2257 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/setup.py
```

### Comparing `lendsmart_reva-1.5/PKG-INFO` & `lendsmart_reva-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart_reva
-Version: 1.5
+Version: 1.6
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.5/README.md` & `lendsmart_reva-1.6/README.md`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/lendsmart_reva.egg-info/PKG-INFO` & `lendsmart_reva-1.6/lendsmart_reva.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart-reva
-Version: 1.5
+Version: 1.6
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.5/lendsmart_reva.egg-info/SOURCES.txt` & `lendsmart_reva-1.6/lendsmart_reva.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,54 +5,66 @@
 lendsmart_reva.egg-info/PKG-INFO
 lendsmart_reva.egg-info/SOURCES.txt
 lendsmart_reva.egg-info/dependency_links.txt
 lendsmart_reva.egg-info/entry_points.txt
 lendsmart_reva.egg-info/requires.txt
 lendsmart_reva.egg-info/top_level.txt
 reva/__init__.py
+reva/advisor_profile.py
 reva/autotest.py
+reva/branch.py
 reva/cli.py
 reva/document_access_control.py
 reva/exception.py
 reva/info.py
 reva/loan_products.py
 reva/namespaces.py
 reva/roles_and_permissions.py
 reva/site_settings.py
 reva/workflow.py
 reva/conf/__init__.py
 reva/conf/reva.py
 reva/lib/__init__.py
+reva/lib/advisor_profile/__init__.py
+reva/lib/advisor_profile/create.py
+reva/lib/advisor_profile/main.py
 reva/lib/auto/__init__.py
 reva/lib/auto/main.py
 reva/lib/base/__init__.py
 reva/lib/base/base.py
 reva/lib/base/run_query.py
+reva/lib/branch/__init__.py
+reva/lib/branch/create.py
+reva/lib/branch/main.py
 reva/lib/client/__init__.py
 reva/lib/client/builder.py
 reva/lib/client/graphql_client.py
 reva/lib/document_access_control/__init__.py
 reva/lib/document_access_control/main.py
 reva/lib/document_access_control/update.py
 reva/lib/graphql_queries/__init__.py
+reva/lib/graphql_queries/advisor_profiles.py
+reva/lib/graphql_queries/branch.py
 reva/lib/graphql_queries/document_access_control.py
 reva/lib/graphql_queries/loan_products.py
+reva/lib/graphql_queries/namespace.py
 reva/lib/graphql_queries/roles_and_permissions.py
 reva/lib/graphql_queries/site_settings.py
 reva/lib/graphql_queries/workflow.py
 reva/lib/loan_productus/__init__.py
 reva/lib/loan_productus/main.py
 reva/lib/loan_productus/update.py
 reva/lib/roles_and_permissions/__init__.py
 reva/lib/roles_and_permissions/main.py
 reva/lib/roles_and_permissions/update.py
 reva/lib/site_settings/__init__.py
 reva/lib/site_settings/main.py
 reva/lib/site_settings/update.py
 reva/lib/utils/__init__.py
+reva/lib/utils/address.py
 reva/lib/utils/filter_data_with_id.py
 reva/lib/utils/get_json_files.py
 reva/lib/utils/get_namespaces.py
 reva/lib/utils/get_paths.py
 reva/lib/utils/list_files.py
 reva/lib/workflow/__init__.py
 reva/lib/workflow/main.py
```

### Comparing `lendsmart_reva-1.5/reva/autotest.py` & `lendsmart_reva-1.6/reva/autotest.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/cli.py` & `lendsmart_reva-1.6/reva/cli.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/conf/reva.py` & `lendsmart_reva-1.6/reva/conf/reva.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/document_access_control.py` & `lendsmart_reva-1.6/reva/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/exception.py` & `lendsmart_reva-1.6/reva/exception.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/info.py` & `lendsmart_reva-1.6/reva/info.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/auto/main.py` & `lendsmart_reva-1.6/reva/lib/auto/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/base/run_query.py` & `lendsmart_reva-1.6/reva/lib/base/run_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     This class will update the data
     """
 
     def run_query(self, query_data):
         """
         This function will run the query
         """
-        print("=======updating==>", query_data) # print will be removed after testing
+        #print("=======updating==>", query_data) # print will be removed after testing
         res = self.graphql_client.execute_query(query_data)
-        print("Response ==>", res) # print will be removed after testing
+        #print("Response ==>", res) # print will be removed after testing
         return res
 
     def excecute_for_single_query_data(self, query_data: dict):
         """
         This function will update the data
         single data : dict
         """
```

### Comparing `lendsmart_reva-1.5/reva/lib/client/graphql_client.py` & `lendsmart_reva-1.6/reva/lib/client/graphql_client.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/document_access_control/main.py` & `lendsmart_reva-1.6/reva/lib/document_access_control/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/document_access_control/update.py` & `lendsmart_reva-1.6/reva/lib/document_access_control/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/graphql_queries/document_access_control.py` & `lendsmart_reva-1.6/reva/lib/graphql_queries/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/graphql_queries/loan_products.py` & `lendsmart_reva-1.6/reva/lib/graphql_queries/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/graphql_queries/roles_and_permissions.py` & `lendsmart_reva-1.6/reva/lib/graphql_queries/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/graphql_queries/site_settings.py` & `lendsmart_reva-1.6/reva/lib/graphql_queries/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/graphql_queries/workflow.py` & `lendsmart_reva-1.6/reva/lib/graphql_queries/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/loan_productus/main.py` & `lendsmart_reva-1.6/reva/lib/loan_productus/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/loan_productus/update.py` & `lendsmart_reva-1.6/reva/lib/loan_productus/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/roles_and_permissions/main.py` & `lendsmart_reva-1.6/reva/lib/roles_and_permissions/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/roles_and_permissions/update.py` & `lendsmart_reva-1.6/reva/lib/roles_and_permissions/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/site_settings/main.py` & `lendsmart_reva-1.6/reva/lib/site_settings/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/site_settings/update.py` & `lendsmart_reva-1.6/reva/lib/site_settings/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/utils/get_namespaces.py` & `lendsmart_reva-1.6/reva/lib/utils/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/utils/get_paths.py` & `lendsmart_reva-1.6/reva/lib/utils/get_paths.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/workflow/main.py` & `lendsmart_reva-1.6/reva/lib/workflow/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/lib/workflow/update.py` & `lendsmart_reva-1.6/reva/lib/workflow/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/loan_products.py` & `lendsmart_reva-1.6/reva/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/namespaces.py` & `lendsmart_reva-1.6/reva/namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/roles_and_permissions.py` & `lendsmart_reva-1.6/reva/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/site_settings.py` & `lendsmart_reva-1.6/reva/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/reva/workflow.py` & `lendsmart_reva-1.6/reva/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.5/setup.py` & `lendsmart_reva-1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,12 +64,14 @@
             'ready = reva.info:ready',
             'workflow = reva.workflow:workflow',
             'sitesettings = reva.site_settings:site_settings',
             'namespace = reva.namespaces:namespaces',
             'autotest = reva.autotest:autotest',
             'loanproducts = reva.loan_products:loan_products',
             'documentaccesscontrol = reva.document_access_control:document_access_control',
-            'rolesandpermissions = reva.roles_and_permissions:roles_and_permissions'
+            'rolesandpermissions = reva.roles_and_permissions:roles_and_permissions',
+            'branch = reva.branch:branch',
+            'advisorprofiles = reva.advisor_profile:advisor_profile'
             ],
 
         },
     )
```

