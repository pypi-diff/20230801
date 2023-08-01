# Comparing `tmp/django-feed-reader-1.0.6.tar.gz` & `tmp/django-feed-reader-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-feed-reader-1.0.6.tar", last modified: Fri Jul 28 05:50:28 2023, max compression
+gzip compressed data, was "django-feed-reader-1.0.7.tar", last modified: Tue Aug  1 01:05:26 2023, max compression
```

## Comparing `django-feed-reader-1.0.6.tar` & `django-feed-reader-1.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.962802 django-feed-reader-1.0.6/
--rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django-feed-reader-1.0.6/LICENSE
--rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django-feed-reader-1.0.6/MANIFEST.in
--rw-r--r--   0 g          (501) staff       (20)     4513 2023-07-28 05:50:28.962852 django-feed-reader-1.0.6/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)     4074 2023-01-28 17:47:47.000000 django-feed-reader-1.0.6/README.md
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.960308 django-feed-reader-1.0.6/django_feed_reader.egg-info/
--rw-r--r--   0 g          (501) staff       (20)     4513 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)      997 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/SOURCES.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/dependency_links.txt
--rw-r--r--   0 g          (501) staff       (20)       74 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/requires.txt
--rw-r--r--   0 g          (501) staff       (20)        6 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/top_level.txt
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.961192 django-feed-reader-1.0.6/feeds/
--rw-r--r--   0 g          (501) staff       (20)      454 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     1520 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/admin.py
--rw-r--r--   0 g          (501) staff       (20)      139 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/apps.py
--rw-r--r--   0 g          (501) staff       (20)       17 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/cloudflare.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.961309 django-feed-reader-1.0.6/feeds/management/
--rw-r--r--   0 g          (501) staff       (20)        1 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/management/__init__.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.961510 django-feed-reader-1.0.6/feeds/management/commands/
--rw-r--r--   0 g          (501) staff       (20)        1 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/management/commands/__init__.py
--rw-r--r--   0 g          (501) staff       (20)      310 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/management/commands/refreshfeeds.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.962725 django-feed-reader-1.0.6/feeds/migrations/
--rw-r--r--   0 g          (501) staff       (20)     3384 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0001_initial.py
--rw-r--r--   0 g          (501) staff       (20)      395 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0002_auto_20190604_0845.py
--rw-r--r--   0 g          (501) staff       (20)      407 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0003_post_image_url.py
--rw-r--r--   0 g          (501) staff       (20)      513 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0004_webproxy.py
--rw-r--r--   0 g          (501) staff       (20)      385 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0005_source_description.py
--rw-r--r--   0 g          (501) staff       (20)      921 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0006_auto_20190901_1644.py
--rw-r--r--   0 g          (501) staff       (20)     1098 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0007_auto_20210502_0716.py
--rw-r--r--   0 g          (501) staff       (20)      419 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0008_allow_longer_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)      576 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
--rw-r--r--   0 g          (501) staff       (20)      626 2023-07-28 05:42:06.000000 django-feed-reader-1.0.6/feeds/migrations/0010_enclosure_description_enclosure_medium.py
--rw-r--r--   0 g          (501) staff       (20)        0 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     6322 2023-07-28 05:42:06.000000 django-feed-reader-1.0.6/feeds/models.py
--rw-r--r--   0 g          (501) staff       (20)    16817 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/tests.py
--rw-r--r--   0 g          (501) staff       (20)    33338 2023-07-28 05:42:06.000000 django-feed-reader-1.0.6/feeds/utils.py
--rw-r--r--   0 g          (501) staff       (20)       63 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/views.py
--rw-r--r--   0 g          (501) staff       (20)       38 2023-07-28 05:50:28.962999 django-feed-reader-1.0.6/setup.cfg
--rw-r--r--   0 g          (501) staff       (20)      869 2023-07-28 05:45:12.000000 django-feed-reader-1.0.6/setup.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-08-01 01:05:26.416102 django-feed-reader-1.0.7/
+-rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django-feed-reader-1.0.7/LICENSE
+-rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django-feed-reader-1.0.7/MANIFEST.in
+-rw-r--r--   0 g          (501) staff       (20)     4513 2023-08-01 01:05:26.416169 django-feed-reader-1.0.7/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)     4074 2023-01-28 17:47:47.000000 django-feed-reader-1.0.7/README.md
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-08-01 01:05:26.411815 django-feed-reader-1.0.7/django_feed_reader.egg-info/
+-rw-r--r--   0 g          (501) staff       (20)     4513 2023-08-01 01:05:26.000000 django-feed-reader-1.0.7/django_feed_reader.egg-info/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)      997 2023-08-01 01:05:26.000000 django-feed-reader-1.0.7/django_feed_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 g          (501) staff       (20)        1 2023-08-01 01:05:26.000000 django-feed-reader-1.0.7/django_feed_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 g          (501) staff       (20)       74 2023-08-01 01:05:26.000000 django-feed-reader-1.0.7/django_feed_reader.egg-info/requires.txt
+-rw-r--r--   0 g          (501) staff       (20)        6 2023-08-01 01:05:26.000000 django-feed-reader-1.0.7/django_feed_reader.egg-info/top_level.txt
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-08-01 01:05:26.413540 django-feed-reader-1.0.7/feeds/
+-rw-r--r--   0 g          (501) staff       (20)      454 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     1520 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/admin.py
+-rw-r--r--   0 g          (501) staff       (20)      139 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/apps.py
+-rw-r--r--   0 g          (501) staff       (20)       17 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/cloudflare.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-08-01 01:05:26.413645 django-feed-reader-1.0.7/feeds/management/
+-rw-r--r--   0 g          (501) staff       (20)        1 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/management/__init__.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-08-01 01:05:26.414048 django-feed-reader-1.0.7/feeds/management/commands/
+-rw-r--r--   0 g          (501) staff       (20)        1 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/management/commands/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)      310 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/management/commands/refreshfeeds.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-08-01 01:05:26.416020 django-feed-reader-1.0.7/feeds/migrations/
+-rw-r--r--   0 g          (501) staff       (20)     3384 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0001_initial.py
+-rw-r--r--   0 g          (501) staff       (20)      395 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0002_auto_20190604_0845.py
+-rw-r--r--   0 g          (501) staff       (20)      407 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0003_post_image_url.py
+-rw-r--r--   0 g          (501) staff       (20)      513 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0004_webproxy.py
+-rw-r--r--   0 g          (501) staff       (20)      385 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0005_source_description.py
+-rw-r--r--   0 g          (501) staff       (20)      921 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0006_auto_20190901_1644.py
+-rw-r--r--   0 g          (501) staff       (20)     1098 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0007_auto_20210502_0716.py
+-rw-r--r--   0 g          (501) staff       (20)      419 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0008_allow_longer_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)      576 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
+-rw-r--r--   0 g          (501) staff       (20)      626 2023-07-28 05:42:06.000000 django-feed-reader-1.0.7/feeds/migrations/0010_enclosure_description_enclosure_medium.py
+-rw-r--r--   0 g          (501) staff       (20)        0 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/migrations/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     6322 2023-07-28 05:42:06.000000 django-feed-reader-1.0.7/feeds/models.py
+-rw-r--r--   0 g          (501) staff       (20)    16817 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/tests.py
+-rw-r--r--   0 g          (501) staff       (20)    33290 2023-08-01 00:33:31.000000 django-feed-reader-1.0.7/feeds/utils.py
+-rw-r--r--   0 g          (501) staff       (20)       63 2023-07-27 22:04:19.000000 django-feed-reader-1.0.7/feeds/views.py
+-rw-r--r--   0 g          (501) staff       (20)       38 2023-08-01 01:05:26.416357 django-feed-reader-1.0.7/setup.cfg
+-rw-r--r--   0 g          (501) staff       (20)      869 2023-08-01 01:03:31.000000 django-feed-reader-1.0.7/setup.py
```

### Comparing `django-feed-reader-1.0.6/LICENSE` & `django-feed-reader-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/PKG-INFO` & `django-feed-reader-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 1.0.6
+Version: 1.0.7
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-feed-reader-1.0.6/README.md` & `django-feed-reader-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/django_feed_reader.egg-info/PKG-INFO` & `django-feed-reader-1.0.7/django_feed_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 1.0.6
+Version: 1.0.7
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-feed-reader-1.0.6/django_feed_reader.egg-info/SOURCES.txt` & `django-feed-reader-1.0.7/django_feed_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/admin.py` & `django-feed-reader-1.0.7/feeds/admin.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/migrations/0001_initial.py` & `django-feed-reader-1.0.7/feeds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/migrations/0004_webproxy.py` & `django-feed-reader-1.0.7/feeds/migrations/0004_webproxy.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/migrations/0006_auto_20190901_1644.py` & `django-feed-reader-1.0.7/feeds/migrations/0006_auto_20190901_1644.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/migrations/0007_auto_20210502_0716.py` & `django-feed-reader-1.0.7/feeds/migrations/0007_auto_20210502_0716.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py` & `django-feed-reader-1.0.7/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/migrations/0010_enclosure_description_enclosure_medium.py` & `django-feed-reader-1.0.7/feeds/migrations/0010_enclosure_description_enclosure_medium.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/models.py` & `django-feed-reader-1.0.7/feeds/models.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/tests.py` & `django-feed-reader-1.0.7/feeds/tests.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.6/feeds/utils.py` & `django-feed-reader-1.0.7/feeds/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,31 +205,32 @@
         #errors, impossible return codes
         source_feed.interval += 120
         source_feed.last_result = "Server error fetching feed (%d)" % ret.status_code
     elif ret.status_code == 404:
         #not found
         source_feed.interval += 120
         source_feed.last_result = "The feed could not be found"
-    elif ret.status_code == 403 or ret.status_code == 410: #Forbidden or gone
-
+    elif ret.status_code == 410: # Gone
+        source_feed.last_result = "Feed has gone away and says it isn't coming back."
+        source_feed.live = False
+    elif ret.status_code == 403:  # Forbidden
         if "Cloudflare" in ret.text or ("Server" in ret.headers and "cloudflare" in ret.headers["Server"]):
 
             if source_feed.is_cloudflare and proxy is not None:
                 # we are already proxied - this proxy on cloudflare's shit list too?
                 proxy.delete()
                 output.write("\nProxy seemed to also be blocked, burning")
                 source_feed.interval /= 2
                 source_feed.last_result = "Proxy kind of worked but still got cloudflared."
             else:            
                 source_feed.is_cloudflare = True
                 source_feed.last_result = "Blocked by Cloudflare (grr)"
         else:
             source_feed.last_result = "Feed is no longer accessible."
             source_feed.live = False
-            
 
     elif ret.status_code >= 400 and ret.status_code < 500:
         #treat as bad request
         source_feed.live = False
         source_feed.last_result = "Bad request (%d)" % ret.status_code
     elif ret.status_code == 304:
         #not modified
@@ -479,30 +480,25 @@
         #output.write(entries)
         entries.reverse() # Entries are typically in reverse chronological order - put them in right order
         for e in entries:
         
 
             # we are going to take the longest
             body = ""
-            
-            if hasattr(e, "content"):
-                for c in e.content:
-                    if len(c.value) > len(body):
-                        body = c.value
-            
+                        
             if hasattr(e, "summary"):
                 if len(e.summary) > len(body):
                     body = e.summary
 
             if hasattr(e, "summary_detail"):
-                if len(e.summary_detail.value) > len(body):
+                if len(e.summary_detail.value) >= len(body):
                     body = e.summary_detail.value
 
             if hasattr(e, "description"):
-                if len(e.description) > len(body):
+                if len(e.description) >= len(body):
                     body = e.description
 
 
             body = fix_relative(body, source_feed.site_url)
             
             try:
                 guid = e.guid
```

### Comparing `django-feed-reader-1.0.6/setup.py` & `django-feed-reader-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('readme.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='django-feed-reader',
-    version='1.0.6',
+    version='1.0.7',
     description='An RSS feed reading library for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Gareth Simpson',
     author_email='g@xurble.org',
     url='https://github.com/xurble/django-feed-reader',
     license='MIT',
```

