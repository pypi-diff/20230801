# Comparing `tmp/test-server-0.0.8.tar.gz` & `tmp/test-server-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/test-server-0.0.8.tar", last modified: Thu Feb 19 07:35:13 2015, max compression
+gzip compressed data, was "dist/test-server-0.0.9.tar", last modified: Thu Feb 19 14:31:58 2015, max compression
```

## Comparing `test-server-0.0.8.tar` & `test-server-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 07:35:13.000000 test-server-0.0.8/
--rw-r--r--   0 lorien    (1000) lorien    (1000)     1582 2015-02-18 19:19:20.000000 test-server-0.0.8/README.rst
-drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 07:35:13.000000 test-server-0.0.8/script/
--rw-r--r--   0 lorien    (1000) lorien    (1000)      876 2015-02-17 09:38:25.000000 test-server-0.0.8/script/test.py
--rw-r--r--   0 lorien    (1000) lorien    (1000)        0 2015-02-17 08:25:04.000000 test-server-0.0.8/script/__init__.py
-drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 07:35:13.000000 test-server-0.0.8/test_server.egg-info/
--rw-r--r--   0 lorien    (1000) lorien    (1000)      305 2015-02-19 07:35:13.000000 test-server-0.0.8/test_server.egg-info/SOURCES.txt
--rw-r--r--   0 lorien    (1000) lorien    (1000)       12 2015-02-19 07:35:13.000000 test-server-0.0.8/test_server.egg-info/requires.txt
--rw-r--r--   0 lorien    (1000) lorien    (1000)       24 2015-02-19 07:35:13.000000 test-server-0.0.8/test_server.egg-info/top_level.txt
--rw-r--r--   0 lorien    (1000) lorien    (1000)        1 2015-02-19 07:35:13.000000 test-server-0.0.8/test_server.egg-info/dependency_links.txt
--rw-r--r--   0 lorien    (1000) lorien    (1000)     2760 2015-02-19 07:35:13.000000 test-server-0.0.8/test_server.egg-info/PKG-INFO
--rw-r--r--   0 lorien    (1000) lorien    (1000)      917 2015-02-19 07:35:05.000000 test-server-0.0.8/setup.py
-drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 07:35:13.000000 test-server-0.0.8/test/
--rw-r--r--   0 lorien    (1000) lorien    (1000)     6915 2015-02-19 07:34:00.000000 test-server-0.0.8/test/server.py
--rw-r--r--   0 lorien    (1000) lorien    (1000)        0 2015-02-17 08:25:04.000000 test-server-0.0.8/test/__init__.py
--rw-r--r--   0 lorien    (1000) lorien    (1000)       59 2015-02-19 07:35:13.000000 test-server-0.0.8/setup.cfg
-drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 07:35:13.000000 test-server-0.0.8/test_server/
--rw-r--r--   0 lorien    (1000) lorien    (1000)     6925 2015-02-19 07:31:41.000000 test-server-0.0.8/test_server/server.py
--rw-r--r--   0 lorien    (1000) lorien    (1000)       60 2015-02-19 07:35:05.000000 test-server-0.0.8/test_server/__init__.py
--rw-r--r--   0 lorien    (1000) lorien    (1000)     2760 2015-02-19 07:35:13.000000 test-server-0.0.8/PKG-INFO
+drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 14:31:58.000000 test-server-0.0.9/
+-rw-r--r--   0 lorien    (1000) lorien    (1000)     1582 2015-02-18 19:19:20.000000 test-server-0.0.9/README.rst
+drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 14:31:58.000000 test-server-0.0.9/script/
+-rw-r--r--   0 lorien    (1000) lorien    (1000)      876 2015-02-17 09:38:25.000000 test-server-0.0.9/script/test.py
+-rw-r--r--   0 lorien    (1000) lorien    (1000)        0 2015-02-17 08:25:04.000000 test-server-0.0.9/script/__init__.py
+drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 14:31:58.000000 test-server-0.0.9/test_server.egg-info/
+-rw-r--r--   0 lorien    (1000) lorien    (1000)      326 2015-02-19 14:31:57.000000 test-server-0.0.9/test_server.egg-info/SOURCES.txt
+-rw-r--r--   0 lorien    (1000) lorien    (1000)       12 2015-02-19 14:31:57.000000 test-server-0.0.9/test_server.egg-info/requires.txt
+-rw-r--r--   0 lorien    (1000) lorien    (1000)       24 2015-02-19 14:31:57.000000 test-server-0.0.9/test_server.egg-info/top_level.txt
+-rw-r--r--   0 lorien    (1000) lorien    (1000)        1 2015-02-19 14:31:57.000000 test-server-0.0.9/test_server.egg-info/dependency_links.txt
+-rw-r--r--   0 lorien    (1000) lorien    (1000)     2760 2015-02-19 14:31:57.000000 test-server-0.0.9/test_server.egg-info/PKG-INFO
+-rw-r--r--   0 lorien    (1000) lorien    (1000)      917 2015-02-19 14:31:38.000000 test-server-0.0.9/setup.py
+drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 14:31:58.000000 test-server-0.0.9/test/
+-rw-r--r--   0 lorien    (1000) lorien    (1000)     6980 2015-02-19 14:30:11.000000 test-server-0.0.9/test/server.py
+-rw-r--r--   0 lorien    (1000) lorien    (1000)        0 2015-02-17 08:25:04.000000 test-server-0.0.9/test/__init__.py
+-rw-r--r--   0 lorien    (1000) lorien    (1000)       59 2015-02-19 14:31:58.000000 test-server-0.0.9/setup.cfg
+drwxr-xr-x   0 lorien    (1000) lorien    (1000)        0 2015-02-19 14:31:58.000000 test-server-0.0.9/test_server/
+-rw-r--r--   0 lorien    (1000) lorien    (1000)      159 2015-02-19 13:17:09.000000 test-server-0.0.9/test_server/error.py
+-rw-r--r--   0 lorien    (1000) lorien    (1000)     7922 2015-02-19 14:29:52.000000 test-server-0.0.9/test_server/server.py
+-rw-r--r--   0 lorien    (1000) lorien    (1000)       60 2015-02-19 14:31:38.000000 test-server-0.0.9/test_server/__init__.py
+-rw-r--r--   0 lorien    (1000) lorien    (1000)     2760 2015-02-19 14:31:58.000000 test-server-0.0.9/PKG-INFO
```

### Comparing `test-server-0.0.8/README.rst` & `test-server-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `test-server-0.0.8/script/test.py` & `test-server-0.0.9/script/test.py`

 * *Files identical despite different names*

### Comparing `test-server-0.0.8/test_server.egg-info/PKG-INFO` & `test-server-0.0.9/test_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: test-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: Server to test HTTP clients
 Home-page: UNKNOWN
 Author: Gregory Petukhov
 Author-email: lorien@lorien.name
 License: MIT
 Description: ===========
         Test-server
```

### Comparing `test-server-0.0.8/setup.py` & `test-server-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import os.path
 
 ROOT = os.path.dirname(os.path.realpath(__file__))
 
 setup(
     name = 'test-server',
-    version = '0.0.8',
+    version = '0.0.9',
     description = 'Server to test HTTP clients',
     long_description = open(os.path.join(ROOT, 'README.rst')).read(),
     author = 'Gregory Petukhov',
     author_email = 'lorien@lorien.name',
     install_requires = ['tornado', 'six'],
     packages = ['test_server', 'script', 'test'],
     license = "MIT",
```

### Comparing `test-server-0.0.8/test/server.py` & `test-server-0.0.9/test/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from unittest import TestCase
-try:
-    from urllib import urlopen
-except ImportError:
-    from urllib.request import urlopen
+from six.moves.urllib.request import urlopen
+from six.moves.urllib.error import HTTPError
 import time
-import six
 
 from test_server import TestServer
 
 
 class ServerTestCase(TestCase):
     @classmethod
     def setUpClass(cls):
@@ -36,35 +33,50 @@
         self.assertEqual(self.server.request['args']['bar'], '1')
 
     def test_post(self):
         self.server.response['post.data'] = b'foo'
         data = urlopen(self.server.get_url(), b'THE POST').read()
         self.assertEqual(data, self.server.response['post.data'])
 
-    def test_callback_wtf(self):
-        class ContentGenerator():
+    def test_data_iterator(self):
+        class ContentGenerator(object):
             def __init__(self):
                 self.count = 0
 
-            def __call__(self):
+            def __iter__(self):
+                return self
+
+            def next(self):
                 self.count += 1
                 return 'foo'
 
+            __next__ = next
+
         gen = ContentGenerator()
         self.server.response['get.data'] = gen
         urlopen(self.server.get_url()).read()
         self.assertEqual(gen.count, 1)
         urlopen(self.server.get_url()).read()
         self.assertEqual(gen.count, 2)
         # Now create POST request which should no be
         # processed with ContentGenerator which is bind to GET
         # requests
         urlopen(self.server.get_url(), b'some post').read()
         self.assertEqual(gen.count, 2)
 
+    def test_data_generator(self):
+        def gen():
+            yield b'one'
+            yield b'two'
+
+        self.server.response['get.data'] = gen()
+        self.assertEquals(b'one', urlopen(self.server.get_url()).read())
+        self.assertEquals(b'two', urlopen(self.server.get_url()).read())
+        self.assertRaises(HTTPError, urlopen, self.server.get_url())
+
     def test_response_once_get(self):
         self.server.response['data'] = b'base'
         self.assertEquals(b'base', urlopen(self.server.get_url()).read())
 
         self.server.response_once['data'] = b'tmp'
         self.assertEquals(b'tmp', urlopen(self.server.get_url()).read())
 
@@ -126,20 +138,15 @@
         self.assertEqual(info.read(), b'Hello')
 
     def test_response_once_code(self):
         info = urlopen(self.server.get_url())
         self.assertEqual(info.getcode(), 200)
 
         self.server.response_once['code'] = 403
-        if six.PY2:
-            info = urlopen(self.server.get_url())
-            self.assertEqual(info.getcode(), 403)
-        else:
-            from urllib.error import HTTPError
-            self.assertRaises(HTTPError, urlopen, self.server.get_url())
+        self.assertRaises(HTTPError, urlopen, self.server.get_url())
 
         info = urlopen(self.server.get_url())
         self.assertEqual(info.getcode(), 200)
 
     def test_response_once_cookies(self):
         self.server.response['cookies'] = [('foo', 'bar')]
         info = urlopen(self.server.get_url())
@@ -150,19 +157,14 @@
         self.assertFalse('foo=bar' in info.headers['Set-Cookie'])
         self.assertTrue('baz=gaz' in info.headers['Set-Cookie'])
 
         info = urlopen(self.server.get_url())
         self.assertTrue('foo=bar' in info.headers['Set-Cookie'])
         self.assertFalse('baz=gaz' in info.headers['Set-Cookie'])
 
-    def test_response_content_callable(self):
-        self.server.response['data'] = lambda: b'Hello'
-        info = urlopen(self.server.get_url())
-        self.assertEqual(info.read(), b'Hello')
-
     def test_timeout_iterator(self):
         delays = (0.5, 0.3, 0.1)
         self.server.timeout_iterator = iter(delays)
 
         for delay in delays:
             start = time.time()
             urlopen(self.server.get_url())
```

### Comparing `test-server-0.0.8/test_server/server.py` & `test-server-0.0.9/test_server/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from tornado.ioloop import IOLoop
 import tornado.web
 import time
 import collections
 import tornado.gen
 from tornado.httpserver import HTTPServer
 from six.moves.urllib.parse import urljoin
+import six
 
-__all__ = ('TestServer',)
-
+from test_server.error import TestServerRuntimeError
 
-class TestServerRuntimeError(Exception):
-    pass
+__all__ = ('TestServer',)
 
 
 class TestServer(object):
     request = {}
     response = {}
     response_once = {'headers': []}
     sleep = {}
@@ -100,45 +99,66 @@
                 charset = SERVER.request['charset']
                 SERVER.request['data'] = self.request.body
 
                 callback = SERVER.get_param('callback', method)
                 if callback:
                     callback(self)
                 else:
-                    headers_sent = set()
+                    response = {
+                        'code': None,
+                        'headers': [],
+                        'data': None,
+                    }
+
+                    response['code'] = SERVER.get_param('code', method)
 
-                    self.set_status(SERVER.get_param('code', method))
                     for key, val in SERVER.get_param('cookies', method):
                         # Set-Cookie: name=newvalue; expires=date;
                         # path=/; domain=.example.org.
-                        self.add_header('Set-Cookie', '%s=%s' % (key, val))
+                        response['headers'].append(
+                            ('Set-Cookie', '%s=%s' % (key, val)))
 
                     for key, value in SERVER.get_param('headers', method):
-                        self.set_header(key, value)
-                        headers_sent.add(key)
+                        response['headers'].append((key, value))
 
-                    self.set_header('Listen-Port',
-                                    str(self.application.listen_port))
+                    response['headers'].append(
+                        ('Listen-Port', str(self.application.listen_port)))
 
-                    if 'Content-Type' not in headers_sent:
+                    header_keys = [x[0] for x in response['headers']]
+                    if 'Content-Type' not in header_keys:
                         charset = 'utf-8'
-                        self.set_header('Content-Type',
-                                        'text/html; charset=%s' % charset)
-                        headers_sent.add('Content-Type')
+                        response['headers'].append(
+                            ('Content-Type',
+                             'text/html; charset=%s' % charset))
 
                     data = SERVER.get_param('data', method)
-                    if isinstance(data, collections.Callable):
-                        self.write(data())
+                    if isinstance(data, six.string_types):
+                        response['data'] = data
+                    elif isinstance(data, six.binary_type):
+                        response['data'] = data
+                    elif isinstance(data, collections.Iterable):
+                        try:
+                            response['data'] = next(data)
+                        except StopIteration:
+                            response['code'] = 405
+                            response['data'] = b''
                     else:
-                        self.write(data)
+                        raise TestServerRuntimeError('Data parameter should '
+                                                     'be string or iterable '
+                                                     'object')
 
                     if SERVER.timeout_iterator:
                         yield tornado.gen.Task(IOLoop.instance().add_timeout,
                                                time.time() +
                                                next(SERVER.timeout_iterator))
+
+                    self.set_status(response['code'])
+                    for key, val in response['headers']:
+                        self.add_header(key, val)
+                    self.write(response['data'])
                     self.finish()
 
             get = method_handler
             post = method_handler
             put = method_handler
             patch = method_handler
             delete = method_handler
```

### Comparing `test-server-0.0.8/PKG-INFO` & `test-server-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: test-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: Server to test HTTP clients
 Home-page: UNKNOWN
 Author: Gregory Petukhov
 Author-email: lorien@lorien.name
 License: MIT
 Description: ===========
         Test-server
```

