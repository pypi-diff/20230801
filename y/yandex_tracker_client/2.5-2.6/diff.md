# Comparing `tmp/yandex_tracker_client-2.5.tar.gz` & `tmp/yandex_tracker_client-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yandex_tracker_client-2.5.tar", last modified: Tue Jul 11 11:47:08 2023, max compression
+gzip compressed data, was "dist/yandex_tracker_client-2.6.tar", last modified: Tue Aug  1 20:35:08 2023, max compression
```

## Comparing `yandex_tracker_client-2.5.tar` & `yandex_tracker_client-2.6.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client/
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       80 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/__init__.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     2394 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/client.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)    37008 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/collections.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7744 2023-07-11 09:41:20.000000 yandex_tracker_client-2.5/yandex_tracker_client/connection.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     3337 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/exceptions.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7480 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/objects.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       93 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/settings.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1096 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/uriutils.py
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/PKG-INFO
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      535 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/SOURCES.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)        1 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/dependency_links.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       52 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/requires.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       22 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/top_level.txt
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)      180 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/AUTHORS
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1607 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/LICENSE
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     8808 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/README.rst
--rwxrwxr-x   0 smosker  (346405873) LD\Domain Users (593637566)     1520 2023-07-11 11:28:09.000000 yandex_tracker_client-2.5/setup.py
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/PKG-INFO
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       38 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/setup.cfg
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client/
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       80 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/__init__.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     2394 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/client.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)    37008 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/collections.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     8175 2023-08-01 05:36:59.000000 yandex_tracker_client-2.6/yandex_tracker_client/connection.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     3337 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/exceptions.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7480 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/objects.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       93 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/settings.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1096 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/uriutils.py
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/PKG-INFO
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      519 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/SOURCES.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)        1 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/dependency_links.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       52 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/requires.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       22 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/top_level.txt
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     9249 2023-08-01 05:36:59.000000 yandex_tracker_client-2.6/README.rst
+-rwxrwxr-x   0 smosker  (346405873) LD\Domain Users (593637566)     1520 2023-08-01 20:35:02.000000 yandex_tracker_client-2.6/setup.py
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/PKG-INFO
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       38 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/setup.cfg
```

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client/client.py` & `yandex_tracker_client-2.6/yandex_tracker_client/client.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client/collections.py` & `yandex_tracker_client-2.6/yandex_tracker_client/collections.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client/connection.py` & `yandex_tracker_client-2.6/yandex_tracker_client/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,24 @@
     method.func_name = name.lower()
     return method
 
 
 class Connection(object):
 
     def __init__(self,
-                 token,
+                 token=None,
                  org_id=None,
                  base_url="https://api.tracker.yandex.net",
                  timeout=10,
                  retries=10,
                  headers=None,
                  api_version=VERSION_V2,
                  verify=True,
                  cloud_org_id=None,
+                 iam_token=None,
                  ):
 
         self.session = requests.Session()
         self.session.verify = verify
 
         if headers is not None:
             self.session.headers.update(headers)
@@ -54,14 +55,22 @@
         self.session.headers['Content-Type'] = 'application/json'
 
         if cloud_org_id:
             if cloud_org_id and org_id:
                 raise exceptions.TrackerClientError("Use either org_id or cloud_org_id to specify organization")
             self.session.headers['X-Cloud-Org-Id'] = cloud_org_id
 
+        if token and iam_token:
+            raise exceptions.TrackerClientError("Use OAuth or IAM token for authorization")
+
+        if iam_token:
+            if not cloud_org_id:
+                raise exceptions.TrackerClientError("IAM token works only with cloud organizations. Use cloud_org_id to specify org id.")
+            self.session.headers['Authorization'] = 'Bearer ' + iam_token
+
         # Check validity headers for requests >= 2.11
         for header in self.session.headers.items():
             check_header_validity(header)
 
         self.base_url = base_url
         self.api_version = api_version
         self.timeout = timeout
```

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client/exceptions.py` & `yandex_tracker_client-2.6/yandex_tracker_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client/objects.py` & `yandex_tracker_client-2.6/yandex_tracker_client/objects.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client/uriutils.py` & `yandex_tracker_client-2.6/yandex_tracker_client/uriutils.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client.egg-info/PKG-INFO` & `yandex_tracker_client-2.6/yandex_tracker_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yandex-tracker-client
-Version: 2.5
+Version: 2.6
 Summary: Client for Yandex.Tracker
 Home-page: https://github.com/yandex/yandex_tracker_client
 Author: Yandex Team
 Author-email: smosker@yandex-team.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python yandex.tracker api-client
```

### Comparing `yandex_tracker_client-2.5/yandex_tracker_client.egg-info/SOURCES.txt` & `yandex_tracker_client-2.6/yandex_tracker_client.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-AUTHORS
-LICENSE
 README.rst
 setup.py
 yandex_tracker_client/__init__.py
 yandex_tracker_client/client.py
 yandex_tracker_client/collections.py
 yandex_tracker_client/connection.py
 yandex_tracker_client/exceptions.py
```

### Comparing `yandex_tracker_client-2.5/README.rst` & `yandex_tracker_client-2.6/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 yandex_tracker_client
 =====================
 
-**yandex_tracker_client** provides python interface to `Yandex.Tracker
+**yandex_tracker_client** provides python interface to `Yandex Tracker
 v2 API <https://tech.yandex.com/connect/tracker/>`_.
 
 Installation
 ------------
 
 **yandex_tracker_client** could be installed by pip:
 
 .. code:: bash
 
    pip install yandex_tracker_client
 
 Configuring
 -----------
 
-The Yandex.Tracker API uses the OAuth 2.0 protocol for application
+The Yandex Tracker API uses the OAuth 2.0 protocol for application
 authorization. Applications use the OAuth 2.0 protocol to access Yandex
 services on behalf of a user.
 You can get your token `here <https://tech.yandex.com/connect/tracker/api/concepts/access-docpage/>`_.
+You can also use IAM tokens for Yandex Cloud organizations. Read `here <https://cloud.yandex.com/en/docs/iam/concepts/authorization/iam-token>`_ about IAM tokens.
 
 Usage
 -----
 
 To use client you need to initialize client first:
 
 .. code:: python
 
    from yandex_tracker_client import TrackerClient
 
    client = TrackerClient(token=<token>, org_id=<org_id>)
 
+For Yandex Cloud organizations you need to use cloud_org_id instead of org_id parameter. Use iam_token parameter for temporary IAM tokens.
+
+.. code:: python
+   from yandex_tracker_client import TrackerClient
+   client = TrackerClient(iam_token=<token>, cloud_org_id=<org_id>)
+
+
 **Getting issue:**
 
 .. code:: python
 
    issue = client.issues['MYQUEUE-42']
    print issue.deadline, issue.updatedAt
 
@@ -62,15 +70,15 @@
    )
 
 **Updating issue:**
 
 .. code:: python
 
    issue = client.issues['MYQUEUE-42']
-   issue.update(summary='East or west, Yandex.Tracker is the best', priority='minor')
+   issue.update(summary='East or west, Yandex Tracker is the best', priority='minor')
 
 **Searching for issues:**
 
 .. code:: python
 
    issues = client.issues.find('Queue: MYQUEUE Assignee: me()') #You can copy this query from ui tracker interface
    print [issue.key for issue in issues]
@@ -288,18 +296,18 @@
 
    from yandex_tracker_client import TrackerClient
 
    client = TrackerClient(token=<token>, org_id=<org_id>)
 
    def sent_employee_to_vacation(assignee, replace_with):
        """
-       :param assignee: login in Yandex.Tracker
+       :param assignee: login in Yandex Tracker
        :type assignee: ``str``
 
-       :param replace_with: login in Yandex.Tracker
+       :param replace_with: login in Yandex Tracker
        :type replace_with: ``str``
 
        :return: is operation was successful
        :rtype: ``bool``
        """
        issues_to_transfer = client.issues.find(filter={'queue': 'MYQUEUE', 'assignee': assignee})
        bulk_change = client.bulkchange.update(issues_to_transfer, assignee=replace_with)
```

### Comparing `yandex_tracker_client-2.5/setup.py` & `yandex_tracker_client-2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='yandex_tracker_client',
-    version='2.5',
+    version='2.6',
     description='Client for Yandex.Tracker',
     author='Yandex Team',
     author_email='smosker@yandex-team.ru',
     url='https://github.com/yandex/yandex_tracker_client',
     long_description='',
     packages=['yandex_tracker_client'],
     classifiers=['Development Status :: 5 - Production/Stable',
```

### Comparing `yandex_tracker_client-2.5/PKG-INFO` & `yandex_tracker_client-2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yandex_tracker_client
-Version: 2.5
+Version: 2.6
 Summary: Client for Yandex.Tracker
 Home-page: https://github.com/yandex/yandex_tracker_client
 Author: Yandex Team
 Author-email: smosker@yandex-team.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python yandex.tracker api-client
```

