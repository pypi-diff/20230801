# Comparing `tmp/motley_cue-0.5.3.tar.gz` & `tmp/motley_cue-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motley_cue-0.5.3.tar", last modified: Wed Jun 21 22:37:36 2023, max compression
+gzip compressed data, was "motley_cue-0.6.0.tar", last modified: Tue Aug  1 09:23:01 2023, max compression
```

## Comparing `motley_cue-0.5.3.tar` & `motley_cue-0.6.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-21 22:37:36.995091 motley_cue-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-21 22:37:26.000000 motley_cue-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/etc/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/bin/motley-cue
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/feudal_adapter.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/gunicorn.conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/etc/init.d/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2365 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/init.d/motley-cue
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/motley-cue.service
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/motley_cue.conf
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/motley_cue.env
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/nginx.motley_cue
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/privacystatement.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/etc/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.deploy.template
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.deploy.update.template
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.test.template
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.update.template
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/unknown.template
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/user.deploy.template
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/user.deploy.update.template
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/user.update.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/motley_cue/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/motley_cue/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/local_user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/motley_cue/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/routers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/motley_cue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 22:37:26.000000 motley_cue-0.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/selinux/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/motley-cue-gunicorn.te
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/motley-cue-nginx.te
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/motley-cue-sshd.te
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-21 22:37:36.995091 motley_cue-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_authorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_local_user_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.783117 motley_cue-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-01 09:23:01.783117 motley_cue-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-01 09:22:51.000000 motley_cue-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.779117 motley_cue-0.6.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.779117 motley_cue-0.6.0/etc/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/bin/motley-cue
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/feudal_adapter.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/gunicorn.conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.779117 motley_cue-0.6.0/etc/init.d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2365 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/init.d/motley-cue
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/motley-cue.service
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/motley_cue.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/motley_cue.env
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/nginx.motley_cue
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/privacystatement.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.783117 motley_cue-0.6.0/etc/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/admin.deploy.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/admin.deploy.update.template
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/admin.test.template
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/admin.update.template
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/unknown.template
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/user.deploy.template
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/user.deploy.update.template
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 09:22:51.000000 motley_cue-0.6.0/etc/templates/user.update.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.779117 motley_cue-0.6.0/motley_cue/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.779117 motley_cue-0.6.0/motley_cue/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/mapper/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/mapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/mapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/mapper/local_user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/mapper/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.779117 motley_cue-0.6.0/motley_cue/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/routers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 09:22:51.000000 motley_cue-0.6.0/motley_cue/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.783117 motley_cue-0.6.0/motley_cue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-01 09:23:01.000000 motley_cue-0.6.0/motley_cue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-01 09:23:01.000000 motley_cue-0.6.0/motley_cue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:23:01.000000 motley_cue-0.6.0/motley_cue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 09:23:01.000000 motley_cue-0.6.0/motley_cue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 09:23:01.000000 motley_cue-0.6.0/motley_cue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 09:23:01.000000 motley_cue-0.6.0/motley_cue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 09:22:51.000000 motley_cue-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.783117 motley_cue-0.6.0/selinux/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-01 09:22:51.000000 motley_cue-0.6.0/selinux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 09:22:51.000000 motley_cue-0.6.0/selinux/motley-cue-gunicorn.te
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-01 09:22:51.000000 motley_cue-0.6.0/selinux/motley-cue-nginx.te
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-01 09:22:51.000000 motley_cue-0.6.0/selinux/motley-cue-sshd.te
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-01 09:23:01.783117 motley_cue-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:23:01.779117 motley_cue-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/test_authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/test_local_user_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/test_token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-08-01 09:22:51.000000 motley_cue-0.6.0/tests/utils.py
```

### Comparing `motley_cue-0.5.3/PKG-INFO` & `motley_cue-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motley_cue
-Version: 0.5.3
+Version: 0.6.0
 Summary: Mapper Oidc To Local idEntitY with loCal User managEment
 Home-page: https://github.com/dianagudu/motley_cue
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dianagudu/motley_cue/issues
 Project-URL: Documentation, https://motley-cue.readthedocs.io
```

### Comparing `motley_cue-0.5.3/README.rst` & `motley_cue-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/feudal_adapter.conf` & `motley_cue-0.6.0/etc/feudal_adapter.conf`

 * *Files 8% similar despite different names*

```diff
@@ -272,14 +272,21 @@
 # Allows using ssh keys, when they are found in the deployment request
 deploy_user_ssh_keys = no
 
 # punch4nfdi -- default: no
 # If set to yes, we will use the punch4nfdi-specific method to translate group names
 # punch4nfdi = no
 
+## post_create_script -- default: None
+## A script to be executed after a user has been created
+# this script can be a shell script or a python script
+# and will be run with root privileges
+# the script will be called with the username as the first and only argument
+# post_create_script = /path/to/script.sh
+
 [backend.bwidm]
 # Configuration for the bwidm backend
 
 ### url
 # The base URL of the bwidm API
 url = https://bwidm-test.scc.kit.edu/rest
 
@@ -293,14 +300,21 @@
 # HTTP basic auth to connect to BWIDM API
 http_user = foo
 http_pass = bar
 
 # The name of the service the user should be added to on BWIDM:
 service_name = sshtest
 
+## post_create_script -- default: None
+## A script to be executed after a user has been created
+# this script can be a shell script or a python script
+# and will be run with root privileges
+# the script will be called with the username as the first and only argument
+# post_create_script = /path/to/script.sh
+
 [backend.ldap]
 # Configuration for the ldap backend
 
 # The ldap backend can function in 3 different modes:
 # - read_only (default): there is read only access to the LDAP, therefore the local accounts
 #       need to already be created in the LDAP and mapped to the federated accounts;
 #       read the docs for more on how to map local <-> federated accounts.
@@ -321,15 +335,16 @@
 # NEEDED for modifying the LDAP
 # when not provided, anonymous bind is used
 # admin user should be fully qualified
 # admin_user = cn=admin,dc=cesga,dc=es
 # admin_password = adminpassword
 
 # set to true if tls is enabled; default: False
-# not supported yet
+# if set to true, the protocol will be ldaps://
+# if set to false, the protocol will be ldap://
 # tls = False
 
 # ldap base for user namespace; default: ou=users,dc=example
 # can include any number of ou / o / dc entries separated by commas
 # user_base = ou=users,dc=example
 
 # user entry attributes containing uids for mapping a user; defaults: gecos & uid
@@ -354,7 +369,14 @@
 ## UID range -- default 1000 -> 60000
 # uid_min = 1000
 # uid_max = 60000
 
 ## GID range -- default 1000 -> 60000
 # gid_min = 1000
 # gid_max = 60000
+
+## post_create_script -- default: None
+## A script to be executed after a user has been created
+# this script can be a shell script or a python script
+# and will be run with root privileges
+# the script will be called with the username as the first and only argument
+# post_create_script = /path/to/script.sh
```

### Comparing `motley_cue-0.5.3/etc/gunicorn.conf.py` & `motley_cue-0.6.0/etc/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/init.d/motley-cue` & `motley_cue-0.6.0/etc/init.d/motley-cue`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/motley_cue.conf` & `motley_cue-0.6.0/etc/motley_cue.conf`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/nginx.motley_cue` & `motley_cue-0.6.0/etc/nginx.motley_cue`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/privacystatement.md` & `motley_cue-0.6.0/etc/privacystatement.md`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/templates/admin.deploy.template` & `motley_cue-0.6.0/etc/templates/admin.deploy.template`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/templates/admin.deploy.update.template` & `motley_cue-0.6.0/etc/templates/admin.deploy.update.template`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/etc/templates/admin.update.template` & `motley_cue-0.6.0/etc/templates/admin.update.template`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/api.py` & `motley_cue-0.6.0/motley_cue/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains the definition of motley_cue's REST API.
 """
 from fastapi import FastAPI, Depends, Request, Query, Header
-from fastapi.exceptions import RequestValidationError
+from fastapi.exceptions import RequestValidationError, ResponseValidationError
 from fastapi.responses import HTMLResponse
 from pydantic import ValidationError
 
 from .dependencies import mapper, Settings
 from .routers import user, admin
 from .models import Info, InfoAuthorisation, InfoOp, VerifyUser, responses, ClientError
 from .mapper.exceptions import (
@@ -24,14 +24,15 @@
     redoc_url=settings.redoc_url,
 )
 
 api.include_router(user.api, tags=["user"])
 api.include_router(admin.api, tags=["admin"])
 api.add_exception_handler(RequestValidationError, request_validation_exception_handler)
 api.add_exception_handler(ValidationError, validation_exception_handler)
+api.add_exception_handler(ResponseValidationError, validation_exception_handler)
 
 
 @api.get("/")
 async def read_root():
     """Retrieve general API information:
 
     * description
```

### Comparing `motley_cue-0.5.3/motley_cue/dependencies.py` & `motley_cue-0.6.0/motley_cue/dependencies.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Module containing global mapper object created from default configuration files.
 """
 from typing import Optional
-from pydantic import BaseSettings, validator
+from pydantic import field_validator
 
 from ._version import __version__
 from .mapper import Mapper, Config
+from pydantic_settings import BaseSettings
 
 
 class Settings(BaseSettings):
     """Settings class with default values for motley_cue API."""
 
     # pylint: disable=no-self-use, no-self-argument
     title: str = "motley_cue"
     description: str = "A service for mapping OIDC identities to local identities"
     version: str = __version__
     openapi_url: str = "/openapi.json"
     docs_url: Optional[str] = None
     redoc_url: Optional[str] = None
 
-    @validator("openapi_url", allow_reuse=True)
+    @field_validator("openapi_url")
+    @classmethod
     def must_start_with_slash(cls, url):
         """validate URLs: must start with a '/'"""
         if not url.startswith("/"):
             raise ValueError("Routed paths must start with '/'")
         return url
 
-    @validator("docs_url", "redoc_url", allow_reuse=True)
+    @field_validator("docs_url", "redoc_url")
+    @classmethod
     def must_start_with_slash_or_none(cls, url):
         """validate URLs: must start with a '/' or be None."""
         if url is not None and not url.startswith("/"):
             raise ValueError("Routed paths must start with '/'")
         return url
```

### Comparing `motley_cue-0.5.3/motley_cue/mapper/__init__.py` & `motley_cue-0.6.0/motley_cue/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/mapper/authorisation.py` & `motley_cue-0.6.0/motley_cue/mapper/authorisation.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/mapper/config.py` & `motley_cue-0.6.0/motley_cue/mapper/config.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/mapper/exceptions.py` & `motley_cue-0.6.0/motley_cue/mapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/mapper/local_user_management.py` & `motley_cue-0.6.0/motley_cue/mapper/local_user_management.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/mapper/token_manager.py` & `motley_cue-0.6.0/motley_cue/mapper/token_manager.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/models.py` & `motley_cue-0.6.0/motley_cue/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,110 +7,120 @@
 from .mapper.authorisation import AuthorisationType
 
 
 @dataclass
 class InfoOp:
     """Data model for responses on the /info/op endpoint."""
 
-    scopes: Optional[List[str]] = Field([], example=["openid", "profile", "email"])
-    audience: Optional[Union[str, List[str]]] = Field("", example="ssh_localhost")
+    scopes: Optional[List[str]] = Field([], examples=[["openid", "profile", "email"]])
+    audience: Optional[Union[str, List[str]]] = Field("", examples=["ssh_localhost"])
 
 
 @dataclass
 class Info:
     """Data model for responses on the /info endpoint."""
 
     login_info: dict = Field(
         ...,
-        example={
-            "description": "Local SSH Test Service",
-            "login_help": "Login via `mccli ssh {login_host}`.",
-            "ssh_host": "localhost",
-        },
+        examples=[
+            {
+                "description": "Local SSH Test Service",
+                "login_help": "Login via `mccli ssh {login_host}`.",
+                "ssh_host": "localhost",
+            }
+        ],
     )
     supported_OPs: list = Field(  # pylint: disable=invalid-name
         ...,
-        example=[
-            "https://aai.egi.eu/oidc",
-            "https://login.helmholtz.de/oauth2",
+        examples=[
+            [
+                "https://aai.egi.eu/oidc",
+                "https://login.helmholtz.de/oauth2",
+            ]
         ],
     )
     ops_info: Dict[str, InfoOp] = Field(
         {},
-        example={
-            "https://aai.egi.eu/oidc": {
-                "scopes": ["openid", "profile", "email"],
-                "audience": "ssh_localhost",
-            },
-            "https://login.helmholtz.de/oauth2": {
-                "scopes": ["openid", "profile", "email"],
-                "audience": "ssh_localhost",
-            },
-        },
+        examples=[
+            {
+                "https://aai.egi.eu/oidc": {
+                    "scopes": ["openid", "profile", "email"],
+                    "audience": "ssh_localhost",
+                },
+                "https://login.helmholtz.de/oauth2": {
+                    "scopes": ["openid", "profile", "email"],
+                    "audience": "ssh_localhost",
+                },
+            }
+        ],
     )
 
 
 @dataclass
 class InfoAuthorisation:
     """Data model for responses on the /info/authorisation endpoint."""
 
     OP: str = Field(
-        ..., example="https://wlcg.cloud.cnaf.infn.it/"
+        ..., examples=["https://wlcg.cloud.cnaf.infn.it/"]
     )  # pylint: disable=invalid-name
     authorisation_type: str = Field(
-        ..., example=AuthorisationType.VO_BASED.description()["authorisation_type"]
+        ..., examples=[AuthorisationType.VO_BASED.description()["authorisation_type"]]
     )
     authorisation_info: str = Field(
-        ..., example=AuthorisationType.VO_BASED.description()["authorisation_info"]
+        ..., examples=[AuthorisationType.VO_BASED.description()["authorisation_info"]]
     )
     supported_VOs: Optional[list] = Field(
-        [], example=["/wlcg"]
+        [], examples=[["/wlcg"]]
     )  # pylint: disable=invalid-name
-    audience: Optional[Union[str, List[str]]] = Field("", example="ssh_localhost")
+    audience: Optional[Union[str, List[str]]] = Field("", examples=["ssh_localhost"])
 
 
 @dataclass
 class VerifyUser:
     """Data model for responses on the /verify_user endpoint."""
 
-    state: str = Field(..., example="deployed")
-    verified: bool = Field(..., example=True)
+    state: str = Field(..., examples=["deployed"])
+    verified: bool = Field(..., examples=[True])
 
 
 @dataclass
 class FeudalResponse:
     """Data model for any responses coming from FeudalAdapter,
     on any /user/* and /admin/* endpoints.
     """
 
-    state: str = Field(..., example="deployed")
-    message: str = Field(..., example="User was created and was added to groups wlcg.")
+    state: str = Field(..., examples=["deployed"])
+    message: str = Field(
+        ..., examples=["User was created and was added to groups wlcg."]
+    )
     credentials: Optional[dict] = Field(
         {},
-        example={
-            "commandline": "ssh wlcg001@localhost",
-            "description": "Local SSH Test Service",
-            "login_help": "Login via `mccli ssh {login_host}`.",
-            "ssh_host": "localhost",
-            "ssh_user": "wlcg001",
-        },
+        examples=[
+            {
+                "commandline": "ssh wlcg001@localhost",
+                "description": "Local SSH Test Service",
+                "login_help": "Login via `mccli ssh {login_host}`.",
+                "ssh_host": "localhost",
+                "ssh_user": "wlcg001",
+            }
+        ],
     )
 
 
 @dataclass
 class OTPResponse:
     """Data model for any responses coming from TokenManager,
     on /user/generate_otp.
     Information on whether OTPs are supported, in which case also
     whether the OTP generation and storage succeeded.
     """
 
-    supported: bool = Field(..., example=True)
-    successful: bool = Field(False, example=True)
-    # message: Optional[str] = Field("", example="OTPs not supported.")
+    supported: bool = Field(..., examples=[True])
+    successful: bool = Field(False, examples=[True])
+    # message: Optional[str] = Field("", examples=["OTPs not supported.")
 
 
 @dataclass
 class ClientError:
     """Data model for responses on errors."""
 
     detail: str
```

### Comparing `motley_cue-0.5.3/motley_cue/routers/admin.py` & `motley_cue-0.6.0/motley_cue/routers/admin.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/routers/user.py` & `motley_cue-0.6.0/motley_cue/routers/user.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue/static.py` & `motley_cue-0.6.0/motley_cue/static.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/motley_cue.egg-info/PKG-INFO` & `motley_cue-0.6.0/motley_cue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motley-cue
-Version: 0.5.3
+Version: 0.6.0
 Summary: Mapper Oidc To Local idEntitY with loCal User managEment
 Home-page: https://github.com/dianagudu/motley_cue
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dianagudu/motley_cue/issues
 Project-URL: Documentation, https://motley-cue.readthedocs.io
```

### Comparing `motley_cue-0.5.3/motley_cue.egg-info/SOURCES.txt` & `motley_cue-0.6.0/motley_cue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/selinux/motley-cue-gunicorn.te` & `motley_cue-0.6.0/selinux/motley-cue-gunicorn.te`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/setup.cfg` & `motley_cue-0.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,24 @@
 
 [options.entry_points]
 console_scripts = 
 	motley_cue_uvicorn = motley_cue.__main__:main
 
 [options]
 install_requires = 
-	feudalAdapter>=0.5.3
-	flaat>=1.1.5
+	feudalAdapter>=0.6.0
+	flaat>=1.1.10
 	fastapi==0.*
 	uvicorn[standard]==0.*
 	gunicorn==20.*
 	sqlitedict==2.*
-	cryptography>=38.0.3
+	cryptography==41.*
 	markdown==3.*
+	pydantic-settings==2.*
+	pydantic==2.*
 package_dir = 
 	=.
 packages = find:
 include_package_data = True
 
 [options.package_data]
 motley_cue =
```

### Comparing `motley_cue-0.5.3/tests/configs.py` & `motley_cue-0.6.0/tests/configs.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/tests/conftest.py` & `motley_cue-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/tests/test_api.py` & `motley_cue-0.6.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/tests/test_authorisation.py` & `motley_cue-0.6.0/tests/test_authorisation.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/tests/test_config.py` & `motley_cue-0.6.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/tests/test_local_user_manager.py` & `motley_cue-0.6.0/tests/test_local_user_manager.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/tests/test_token_manager.py` & `motley_cue-0.6.0/tests/test_token_manager.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.3/tests/utils.py` & `motley_cue-0.6.0/tests/utils.py`

 * *Files identical despite different names*

