# Comparing `tmp/afex-audit-trail-0.2.3.tar.gz` & `tmp/afex-audit-trail-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-audit-trail-0.2.3.tar", last modified: Mon Jul 31 11:08:01 2023, max compression
+gzip compressed data, was "afex-audit-trail-0.2.4.tar", last modified: Tue Aug  1 09:42:52 2023, max compression
```

## Comparing `afex-audit-trail-0.2.3.tar` & `afex-audit-trail-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:08:01.266276 afex-audit-trail-0.2.3/
--rw-rw-rw-   0        0        0     1062 2023-04-25 08:05:26.000000 afex-audit-trail-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6661 2023-07-31 11:08:01.266276 afex-audit-trail-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.2.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-31 11:08:00.978294 afex-audit-trail-0.2.3/afex_audit_trail.egg-info/
--rw-rw-rw-   0        0        0     6661 2023-07-31 11:07:59.000000 afex-audit-trail-0.2.3/afex_audit_trail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-07-31 11:08:00.000000 afex-audit-trail-0.2.3/afex_audit_trail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 11:07:59.000000 afex-audit-trail-0.2.3/afex_audit_trail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-31 11:07:59.000000 afex-audit-trail-0.2.3/afex_audit_trail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-31 11:07:59.000000 afex-audit-trail-0.2.3/afex_audit_trail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 11:08:01.137004 afex-audit-trail-0.2.3/audit_trails/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.3/audit_trails/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.3/audit_trails/admin.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:08:01.177121 afex-audit-trail-0.2.3/audit_trails/api/
--rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.2.3/audit_trails/api/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.2.3/audit_trails/api/serializers.py
--rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.2.3/audit_trails/api/urls.py
--rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.2.3/audit_trails/api/views.py
--rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.3/audit_trails/apps.py
--rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.2.3/audit_trails/logger.py
--rw-rw-rw-   0        0        0     3348 2023-07-21 17:11:44.000000 afex-audit-trail-0.2.3/audit_trails/middleware.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:08:01.186798 afex-audit-trail-0.2.3/audit_trails/migrations/
--rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.2.3/audit_trails/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1071 2023-07-06 08:42:58.000000 afex-audit-trail-0.2.3/audit_trails/migrations/0002_remove_notification_actor_and_more.py
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.3/audit_trails/migrations/__init__.py
--rw-rw-rw-   0        0        0     3725 2023-07-07 08:51:09.000000 afex-audit-trail-0.2.3/audit_trails/models.py
--rw-rw-rw-   0        0        0     1416 2023-06-06 11:17:58.000000 afex-audit-trail-0.2.3/audit_trails/signals.py
--rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.3/audit_trails/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.3/audit_trails/urls.py
--rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.3/audit_trails/views.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:08:01.266276 afex-audit-trail-0.2.3/main/
--rw-rw-rw-   0        0        0        0 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.3/main/__init__.py
--rw-rw-rw-   0        0        0      401 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.3/main/asgi.py
--rw-rw-rw-   0        0        0     3372 2023-07-06 08:42:12.000000 afex-audit-trail-0.2.3/main/settings.py
--rw-rw-rw-   0        0        0      767 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.3/main/urls.py
--rw-rw-rw-   0        0        0      401 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.3/main/wsgi.py
--rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      987 2023-07-31 11:08:01.282859 afex-audit-trail-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:42:52.863036 afex-audit-trail-0.2.4/
+-rw-rw-rw-   0        0        0     1062 2023-04-25 08:05:26.000000 afex-audit-trail-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6661 2023-08-01 09:42:52.863036 afex-audit-trail-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.2.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-01 09:42:52.721890 afex-audit-trail-0.2.4/afex_audit_trail.egg-info/
+-rw-rw-rw-   0        0        0     6661 2023-08-01 09:42:52.000000 afex-audit-trail-0.2.4/afex_audit_trail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-08-01 09:42:52.000000 afex-audit-trail-0.2.4/afex_audit_trail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:42:52.000000 afex-audit-trail-0.2.4/afex_audit_trail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-08-01 09:42:52.000000 afex-audit-trail-0.2.4/afex_audit_trail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-01 09:42:52.000000 afex-audit-trail-0.2.4/afex_audit_trail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 09:42:52.800530 afex-audit-trail-0.2.4/audit_trails/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.4/audit_trails/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.4/audit_trails/admin.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:42:52.816162 afex-audit-trail-0.2.4/audit_trails/api/
+-rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.2.4/audit_trails/api/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.2.4/audit_trails/api/serializers.py
+-rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.2.4/audit_trails/api/urls.py
+-rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.2.4/audit_trails/api/views.py
+-rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.4/audit_trails/apps.py
+-rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.2.4/audit_trails/logger.py
+-rw-rw-rw-   0        0        0     3348 2023-07-21 17:11:44.000000 afex-audit-trail-0.2.4/audit_trails/middleware.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:42:52.831788 afex-audit-trail-0.2.4/audit_trails/migrations/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.4/audit_trails/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3725 2023-07-07 08:51:09.000000 afex-audit-trail-0.2.4/audit_trails/models.py
+-rw-rw-rw-   0        0        0     1416 2023-06-06 11:17:58.000000 afex-audit-trail-0.2.4/audit_trails/signals.py
+-rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.4/audit_trails/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.4/audit_trails/urls.py
+-rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.4/audit_trails/views.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:42:52.863036 afex-audit-trail-0.2.4/main/
+-rw-rw-rw-   0        0        0        0 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.4/main/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.4/main/asgi.py
+-rw-rw-rw-   0        0        0     3372 2023-07-06 08:42:12.000000 afex-audit-trail-0.2.4/main/settings.py
+-rw-rw-rw-   0        0        0      767 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.4/main/urls.py
+-rw-rw-rw-   0        0        0      401 2023-07-06 08:38:09.000000 afex-audit-trail-0.2.4/main/wsgi.py
+-rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0      987 2023-08-01 09:42:52.863036 afex-audit-trail-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.2.4/setup.py
```

### Comparing `afex-audit-trail-0.2.3/LICENSE` & `afex-audit-trail-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/PKG-INFO` & `afex-audit-trail-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.2.3/afex_audit_trail.egg-info/PKG-INFO` & `afex-audit-trail-0.2.4/afex_audit_trail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.2.3/afex_audit_trail.egg-info/SOURCES.txt` & `afex-audit-trail-0.2.4/afex_audit_trail.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,13 @@
 audit_trails/tests.py
 audit_trails/urls.py
 audit_trails/views.py
 audit_trails/api/__init__.py
 audit_trails/api/serializers.py
 audit_trails/api/urls.py
 audit_trails/api/views.py
-audit_trails/migrations/0001_initial.py
-audit_trails/migrations/0002_remove_notification_actor_and_more.py
 audit_trails/migrations/__init__.py
 main/__init__.py
 main/asgi.py
 main/settings.py
 main/urls.py
 main/wsgi.py
```

### Comparing `afex-audit-trail-0.2.3/audit_trails/api/serializers.py` & `afex-audit-trail-0.2.4/audit_trails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/api/urls.py` & `afex-audit-trail-0.2.4/audit_trails/api/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/api/views.py` & `afex-audit-trail-0.2.4/audit_trails/api/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/logger.py` & `afex-audit-trail-0.2.4/audit_trails/logger.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/middleware.py` & `afex-audit-trail-0.2.4/audit_trails/middleware.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/models.py` & `afex-audit-trail-0.2.4/audit_trails/models.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/signals.py` & `afex-audit-trail-0.2.4/audit_trails/signals.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/urls.py` & `afex-audit-trail-0.2.4/audit_trails/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/audit_trails/views.py` & `afex-audit-trail-0.2.4/audit_trails/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/main/settings.py` & `afex-audit-trail-0.2.4/main/settings.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/main/urls.py` & `afex-audit-trail-0.2.4/main/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.2.3/setup.cfg` & `afex-audit-trail-0.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6665 782d 6175 6469 742d 7472   = afex-audit-tr
 00000020: 6169 6c0d 0a76 6572 7369 6f6e 203d 2030  ail..version = 0
-00000030: 2e32 2e33 0d0a 6465 7363 7269 7074 696f  .2.3..descriptio
+00000030: 2e32 2e34 0d0a 6465 7363 7269 7074 696f  .2.4..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6372 6561 7465 2073 6572 7665   to create serve
 00000060: 7220 6c6f 6773 2061 6e64 2075 7365 7273  r logs and users
 00000070: 2720 6e6f 7469 6669 6361 7469 6f6e 2e0d  ' notification..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 000000a0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
```

