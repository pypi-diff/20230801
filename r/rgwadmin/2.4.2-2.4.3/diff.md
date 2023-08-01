# Comparing `tmp/rgwadmin-2.4.2.tar.gz` & `tmp/rgwadmin-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgwadmin-2.4.2.tar", last modified: Thu May 11 14:16:20 2023, max compression
+gzip compressed data, was "rgwadmin-2.4.3.tar", last modified: Tue Aug  1 13:41:44 2023, max compression
```

## Comparing `rgwadmin-2.4.2.tar` & `rgwadmin-2.4.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/
--rw-rw-rw-   0 root         (0) root         (0)    26443 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3359 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.242102 rgwadmin-2.4.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.243101 rgwadmin-2.4.2/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/api.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.245102 rgwadmin-2.4.2/docs/source/apipages/
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/apipages/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/apipages/rgw.rst
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/apipages/user.rst
--rw-rw-rw-   0 root         (0) root         (0)     5460 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.245102 rgwadmin-2.4.2/docs/source/rgwadmin/
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/rgwadmin/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)    14356 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/rgwadmin/user-guide.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.247102 rgwadmin-2.4.2/rgwadmin/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21585 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/rgw.py
--rw-rw-rw-   0 root         (0) root         (0)     9589 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/user.py
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.249101 rgwadmin-2.4.2/rgwadmin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3359 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1444 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/test/
--rwxrwxrwx   0 root         (0) root         (0)     2683 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/test/test_metadata.py
--rwxrwxrwx   0 root         (0) root         (0)     6327 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/test/test_rgw.py
--rwxrwxrwx   0 root         (0) root         (0)     1461 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/test/test_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.604767 rgwadmin-2.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)    26443 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-08-01 13:41:44.603767 rgwadmin-2.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.585767 rgwadmin-2.4.3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.587767 rgwadmin-2.4.3/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/api.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.589767 rgwadmin-2.4.3/docs/source/apipages/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/apipages/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/apipages/rgw.rst
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/apipages/user.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5460 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.591767 rgwadmin-2.4.3/docs/source/rgwadmin/
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/rgwadmin/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14356 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/docs/source/rgwadmin/user-guide.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.595767 rgwadmin-2.4.3/rgwadmin/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/rgwadmin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/rgwadmin/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/rgwadmin/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21554 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/rgwadmin/rgw.py
+-rw-rw-rw-   0 root         (0) root         (0)     9589 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/rgwadmin/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/rgwadmin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.600767 rgwadmin-2.4.3/rgwadmin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-08-01 13:41:44.000000 rgwadmin-2.4.3/rgwadmin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      695 2023-08-01 13:41:44.000000 rgwadmin-2.4.3/rgwadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:41:44.000000 rgwadmin-2.4.3/rgwadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:41:44.000000 rgwadmin-2.4.3/rgwadmin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-01 13:41:44.000000 rgwadmin-2.4.3/rgwadmin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-01 13:41:44.000000 rgwadmin-2.4.3/rgwadmin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 13:41:44.604767 rgwadmin-2.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:41:44.602767 rgwadmin-2.4.3/test/
+-rwxrwxrwx   0 root         (0) root         (0)     2683 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/test/test_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     6327 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/test/test_rgw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1461 2023-08-01 13:41:36.000000 rgwadmin-2.4.3/test/test_user.py
```

### Comparing `rgwadmin-2.4.2/LICENSE` & `rgwadmin-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/PKG-INFO` & `rgwadmin-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgwadmin
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python Rados Gateway Admin API
 Home-page: https://github.com/UMIACS/rgwadmin
 Author: Derek Yarnell
 Author-email: derek@umiacs.umd.edu
 Maintainer: UMIACS Staff
 Maintainer-email: github@umiacs.umd.edu
 License: LGPL v2.1
```

### Comparing `rgwadmin-2.4.2/README.md` & `rgwadmin-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/docs/Makefile` & `rgwadmin-2.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/docs/make.bat` & `rgwadmin-2.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/docs/source/conf.py` & `rgwadmin-2.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/docs/source/rgwadmin/user-guide.rst` & `rgwadmin-2.4.3/docs/source/rgwadmin/user-guide.rst`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/rgwadmin/exceptions.py` & `rgwadmin-2.4.3/rgwadmin/exceptions.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/rgwadmin/rgw.py` & `rgwadmin-2.4.3/rgwadmin/rgw.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,33 +404,33 @@
             parameters += '&access-key=%s' % access_key
             parameters += '&secret-key=%s' % secret_key
         if key_type is not None and key_type.lower() in ['s3', 'swift']:
             parameters += '&key-type=%s' % key_type
         if access is not None:
             parameters += '&access=%s' % access
         parameters += '&generate-secret=%s' % generate_secret
-        return self.request('put', '/%s/user?subuser&format=%s&%s' %
+        return self.request('put', '/%s/user?format=%s&%s' %
                             (self._admin, self._response, parameters))
 
     def modify_subuser(self, uid, subuser, secret=None, key_type='swift',
                        access=None, generate_secret=False):
         parameters = 'uid=%s&subuser=%s' % (uid, subuser)
         if secret is not None:
             parameters += '&secret=%s' % secret
         parameters += '&key-type=%s' % key_type
         if access is not None:
             parameters += '&access=%s' % access
         parameters += '&generate-secret=%s' % generate_secret
-        return self.request('post', '/%s/user?subuser&format=%s&%s' %
+        return self.request('post', '/%s/user?format=%s&%s' %
                             (self._admin, self._response, parameters))
 
     def remove_subuser(self, uid, subuser, purge_keys=True):
         parameters = 'uid=%s&subuser=%s&purge-keys=%s' % (uid, subuser,
                                                           purge_keys)
-        return self.request('delete', '/%s/user?subuser&format=%s&%s' %
+        return self.request('delete', '/%s/user?format=%s&%s' %
                             (self._admin, self._response, parameters))
 
     def create_key(self, uid, subuser=None, key_type='s3', access_key=None,
                    secret_key=None, generate_key=True):
         parameters = 'uid=%s' % uid
         if subuser is not None:
             parameters += '&subuser=%s' % subuser
@@ -494,15 +494,15 @@
         if new_bucket_name is not None:
             parameters += '&new-bucket-name=%s' % new_bucket_name
         return self.request('put', '/%s/bucket?format=%s&%s' %
                             (self._admin, self._response, parameters))
 
     def remove_object(self, bucket, object_name):
         parameters = 'bucket=%s&object=%s' % (bucket, object_name)
-        return self.request('delete', '/%s/bucket?object&format=%s&%s' %
+        return self.request('delete', '/%s/bucket?format=%s&%s' %
                             (self._admin, self._response, parameters))
 
     def get_policy(self, bucket, object_name=None):
         parameters = 'bucket=%s' % bucket
         if object_name is not None:
             parameters += '&object=%s' % object_name
         return self.request('get', '/%s/bucket?policy&format=%s&%s' %
```

### Comparing `rgwadmin-2.4.2/rgwadmin/user.py` & `rgwadmin-2.4.3/rgwadmin/user.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/rgwadmin/utils.py` & `rgwadmin-2.4.3/rgwadmin/utils.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/rgwadmin.egg-info/PKG-INFO` & `rgwadmin-2.4.3/rgwadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgwadmin
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python Rados Gateway Admin API
 Home-page: https://github.com/UMIACS/rgwadmin
 Author: Derek Yarnell
 Author-email: derek@umiacs.umd.edu
 Maintainer: UMIACS Staff
 Maintainer-email: github@umiacs.umd.edu
 License: LGPL v2.1
```

### Comparing `rgwadmin-2.4.2/rgwadmin.egg-info/SOURCES.txt` & `rgwadmin-2.4.3/rgwadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/setup.py` & `rgwadmin-2.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/test/test_metadata.py` & `rgwadmin-2.4.3/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/test/test_rgw.py` & `rgwadmin-2.4.3/test/test_rgw.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.2/test/test_user.py` & `rgwadmin-2.4.3/test/test_user.py`

 * *Files identical despite different names*

