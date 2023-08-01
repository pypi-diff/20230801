# Comparing `tmp/django-dingtalk-sit-1.0.0.tar.gz` & `tmp/django-dingtalk-sit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dingtalk-sit-1.0.0.tar", last modified: Mon Jul 31 10:17:57 2023, max compression
+gzip compressed data, was "django-dingtalk-sit-1.0.1.tar", last modified: Tue Aug  1 03:08:07 2023, max compression
```

## Comparing `django-dingtalk-sit-1.0.0.tar` & `django-dingtalk-sit-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 alias      (502) staff       (20)        0 2023-07-31 10:17:57.822132 django-dingtalk-sit-1.0.0/
--rw-r--r--   0 alias      (502) staff       (20)       63 2023-07-31 10:00:34.000000 django-dingtalk-sit-1.0.0/MANIFEST.in
--rw-r--r--   0 alias      (502) staff       (20)      252 2023-07-31 10:17:57.822016 django-dingtalk-sit-1.0.0/PKG-INFO
-drwxr-xr-x   0 alias      (502) staff       (20)        0 2023-07-31 10:17:57.820228 django-dingtalk-sit-1.0.0/django_dingtalk_sit.egg-info/
--rw-r--r--   0 alias      (502) staff       (20)      252 2023-07-31 10:17:57.000000 django-dingtalk-sit-1.0.0/django_dingtalk_sit.egg-info/PKG-INFO
--rw-r--r--   0 alias      (502) staff       (20)      320 2023-07-31 10:17:57.000000 django-dingtalk-sit-1.0.0/django_dingtalk_sit.egg-info/SOURCES.txt
--rw-r--r--   0 alias      (502) staff       (20)        1 2023-07-31 10:17:57.000000 django-dingtalk-sit-1.0.0/django_dingtalk_sit.egg-info/dependency_links.txt
--rw-r--r--   0 alias      (502) staff       (20)        7 2023-07-31 10:17:57.000000 django-dingtalk-sit-1.0.0/django_dingtalk_sit.egg-info/requires.txt
--rw-r--r--   0 alias      (502) staff       (20)        8 2023-07-31 10:17:57.000000 django-dingtalk-sit-1.0.0/django_dingtalk_sit.egg-info/top_level.txt
-drwxr-xr-x   0 alias      (502) staff       (20)        0 2023-07-31 10:17:57.821252 django-dingtalk-sit-1.0.0/message/
--rw-r--r--   0 alias      (502) staff       (20)        0 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.0/message/__init__.py
--rw-r--r--   0 alias      (502) staff       (20)      541 2023-07-28 07:37:07.000000 django-dingtalk-sit-1.0.0/message/admin.py
--rw-r--r--   0 alias      (502) staff       (20)      151 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.0/message/apps.py
--rw-r--r--   0 alias      (502) staff       (20)      306 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.0/message/tests.py
--rw-r--r--   0 alias      (502) staff       (20)      179 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.0/message/urls.py
--rw-r--r--   0 alias      (502) staff       (20)       38 2023-07-31 10:17:57.822178 django-dingtalk-sit-1.0.0/setup.cfg
--rw-r--r--   0 alias      (502) staff       (20)      488 2023-07-31 10:17:45.000000 django-dingtalk-sit-1.0.0/setup.py
+drwxr-xr-x   0 alias      (502) staff       (20)        0 2023-08-01 03:08:07.892453 django-dingtalk-sit-1.0.1/
+-rw-r--r--   0 alias      (502) staff       (20)       63 2023-07-31 10:00:34.000000 django-dingtalk-sit-1.0.1/MANIFEST.in
+-rw-r--r--   0 alias      (502) staff       (20)      579 2023-08-01 03:08:07.892315 django-dingtalk-sit-1.0.1/PKG-INFO
+-rw-r--r--   0 alias      (502) staff       (20)      286 2023-08-01 03:07:20.000000 django-dingtalk-sit-1.0.1/README.md
+drwxr-xr-x   0 alias      (502) staff       (20)        0 2023-08-01 03:08:07.890657 django-dingtalk-sit-1.0.1/django_dingtalk_sit.egg-info/
+-rw-r--r--   0 alias      (502) staff       (20)      579 2023-08-01 03:08:07.000000 django-dingtalk-sit-1.0.1/django_dingtalk_sit.egg-info/PKG-INFO
+-rw-r--r--   0 alias      (502) staff       (20)      330 2023-08-01 03:08:07.000000 django-dingtalk-sit-1.0.1/django_dingtalk_sit.egg-info/SOURCES.txt
+-rw-r--r--   0 alias      (502) staff       (20)        1 2023-08-01 03:08:07.000000 django-dingtalk-sit-1.0.1/django_dingtalk_sit.egg-info/dependency_links.txt
+-rw-r--r--   0 alias      (502) staff       (20)        7 2023-08-01 03:08:07.000000 django-dingtalk-sit-1.0.1/django_dingtalk_sit.egg-info/requires.txt
+-rw-r--r--   0 alias      (502) staff       (20)        8 2023-08-01 03:08:07.000000 django-dingtalk-sit-1.0.1/django_dingtalk_sit.egg-info/top_level.txt
+drwxr-xr-x   0 alias      (502) staff       (20)        0 2023-08-01 03:08:07.891926 django-dingtalk-sit-1.0.1/message/
+-rw-r--r--   0 alias      (502) staff       (20)        0 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.1/message/__init__.py
+-rw-r--r--   0 alias      (502) staff       (20)      541 2023-07-28 07:37:07.000000 django-dingtalk-sit-1.0.1/message/admin.py
+-rw-r--r--   0 alias      (502) staff       (20)      151 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.1/message/apps.py
+-rw-r--r--   0 alias      (502) staff       (20)      306 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.1/message/tests.py
+-rw-r--r--   0 alias      (502) staff       (20)      179 2023-07-11 07:15:51.000000 django-dingtalk-sit-1.0.1/message/urls.py
+-rw-r--r--   0 alias      (502) staff       (20)       38 2023-08-01 03:08:07.892505 django-dingtalk-sit-1.0.1/setup.cfg
+-rw-r--r--   0 alias      (502) staff       (20)      767 2023-08-01 03:07:54.000000 django-dingtalk-sit-1.0.1/setup.py
```

### Comparing `django-dingtalk-sit-1.0.0/message/admin.py` & `django-dingtalk-sit-1.0.1/message/admin.py`

 * *Files identical despite different names*

