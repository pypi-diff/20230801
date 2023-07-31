# Comparing `tmp/pyxk-0.6.7.tar.gz` & `tmp/pyxk-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.7.tar", last modified: Mon Jul 31 13:33:00 2023, max compression
+gzip compressed data, was "pyxk-0.6.8.tar", last modified: Mon Jul 31 23:17:40 2023, max compression
```

## Comparing `pyxk-0.6.7.tar` & `pyxk-0.6.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:33:00.309178 pyxk-0.6.7/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.7/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:33:00.309178 pyxk-0.6.7/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.7/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:33:00.309178 pyxk-0.6.7/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.7/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:33:00.309178 pyxk-0.6.7/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.7/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    22508 2023-07-31 13:16:20.000000 pyxk-0.6.7/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.7/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:33:00.309178 pyxk-0.6.7/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.7/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.7/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:33:00.309178 pyxk-0.6.7/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.7/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8840 2023-07-31 12:53:28.000000 pyxk-0.6.7/pyxk/m3u8/_initial.py
--rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.7/pyxk/m3u8/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.7/pyxk/m3u8/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    10217 2023-07-31 13:31:37.000000 pyxk-0.6.7/pyxk/m3u8/m3u8parse.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:33:00.309178 pyxk-0.6.7/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.7/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.7/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.7/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.7/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.7/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:33:00.309178 pyxk-0.6.7/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:33:00.000000 pyxk-0.6.7/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      558 2023-07-31 13:33:00.000000 pyxk-0.6.7/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-31 13:33:00.000000 pyxk-0.6.7/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-07-31 13:33:00.000000 pyxk-0.6.7/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       62 2023-07-31 13:33:00.000000 pyxk-0.6.7/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-07-31 13:33:00.000000 pyxk-0.6.7/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-31 13:33:00.309178 pyxk-0.6.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      898 2023-07-31 13:32:40.000000 pyxk-0.6.7/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.8/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 23:17:40.394998 pyxk-0.6.8/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.8/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.384998 pyxk-0.6.8/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.8/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.8/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    23004 2023-07-31 23:06:20.000000 pyxk-0.6.8/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.8/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.8/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.8/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.8/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8840 2023-07-31 13:41:16.000000 pyxk-0.6.8/pyxk/m3u8/_initial.py
+-rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.8/pyxk/m3u8/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.8/pyxk/m3u8/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    10217 2023-07-31 13:31:37.000000 pyxk-0.6.8/pyxk/m3u8/m3u8parse.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.8/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.8/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.8/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.8/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.8/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      558 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       62 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-31 23:17:40.394998 pyxk-0.6.8/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      898 2023-07-31 22:46:51.000000 pyxk-0.6.8/setup.py
```

### Comparing `pyxk-0.6.7/LICENSE` & `pyxk-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/PKG-INFO` & `pyxk-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.7
+Version: 0.6.8
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.7/README.md` & `pyxk-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/aclient/client.py` & `pyxk-0.6.8/pyxk/aclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
     Download.run()
     """
 
     limit: int = 100
     timeout: Timeout = None
     verify: bool = True
-    warning: bool = False
+    warning: bool = True
     headers: Union[dict, CIMDict] = CIMultiDict(default_headers())
     semaphore: Union[int, asyncio.Semaphore] = 32
     user_agent: Optional[str] = None
     req_kwargs: dict = {}
     start_urls: Union[List[str], List[Tuple[str, dict]]] = []
     async_sleep: Union[int, float] = 0
     max_retries: int = 15
     aiohttp_kwargs: dict = {}
     status_retry_list: List[int] = []
     status_error_list: List[int] = []
-    until_request_succeed: Union[bool, List[int]] = True
+    until_request_succeed: Union[bool, List[int]] = False
     ATTRS = {
         'timeout': 10,
         'semaphore': 16,
         'user_agent': get_user_agent(),
     }
 
     def __init__(self, *, base_url: URL = None, **kwargs):
@@ -178,20 +178,40 @@
         await self.stop()
         # 关闭 aiohttp session
         if self.session:
             await self.session.close()
         # 关闭 aiohttp session 之后调用
         await self.close()
 
-    async def start_request(self):
-        """start_urls 默认运行方法"""
+    async def start_request(
+        self,
+        callback: Optional[Callable] = None,
+        set_base_url: bool = True,
+        **kwargs
+    ):
+        """start_urls 默认运行方法
+
+        :param callback: 回调函数
+        :param set_base_url: 设置base url
+        :param kwargs: 请求可选关键字参数
+        """
         if not self.start_urls or not isinstance(self.start_urls, (list, tuple)):
-            raise NotImplementedError(f'Invalid start_urls, got {self.start_urls!r}')
+            raise NotImplementedError(
+                f'Invalid start_urls, got {self.start_urls!r}'
+            )
 
-        return await self.gather(self.start_urls, self.parse, set_base_url=True, **dict(self.req_kwargs))
+        kw = copy.deepcopy(dict(self.req_kwargs))
+        kw.update(kwargs)
+
+        return await self.gather(
+            self.start_urls,
+            callback if callable(callback) else self.parse,
+            set_base_url=set_base_url,
+            **kw
+        )
 
     async def request(
         self,
         url: URL,
         callback: Optional[Callable] = None,
         *,
         method: str = "GET",
@@ -202,38 +222,21 @@
 
         :return:
         :param url: URL
         :param callback: 响应response 回调函数(函数是异步的)
         :param method: 请求方法(default: GET)
         :param cb_kwargs: 传递给回调函数的关键字参数
         :param kwargs: 异步请求 request参数
-            params
-            data
-            json
-            cookies
-            headers
-            skip_auto_headers
-            auth
-            allow_redirects
-            max_redirects
-            compress
-            chunked
-            expect100
-            raise_for_status
-            read_until_eof
-            proxy
-            proxy_auth
-            timeout
-            verify_ssl
-            fingerprint
-            ssl_context
-            ssl
-            proxy_headers
-            trace_request_ctx
-            read_bufsize
+            params, data, json, cookies, headers,
+            skip_auto_headers, auth, allow_redirects,
+            max_redirects, compress, chunked, expect100,
+            raise_for_status, read_until_eof, proxy, proxy_auth,
+            timeout, verify_ssl, fingerprint,
+            ssl_context, ssl, proxy_headers,
+            trace_request_ctx, read_bufsize
         :return: Response, Any
         """
         status_retry_list, status_error_list = self.status_retry_list.copy(), self.status_error_list.copy()
         url, response, result, exc_from_request = self.build_url(url), None, None, None
         warning = {
             'status_retry_list': True,
             'status_error_list': True,
@@ -249,14 +252,18 @@
                     response = result = await self.session.request(method=method, url=url, **kwargs)
 
                     # 直到请求成功
                     if self.until_request_succeed:
                         if response.status in self.until_request_succeed:
                             status_retry_list, status_error_list = [], []
                         else:
+                            # 状态码错误
+                            if response.status in status_error_list:
+                                raise aiohttp_exceptions.ClientError(f'<Response[{response.status}] {url}>')
+
                             # 提示信息
                             await self._warning('until_request_succeed', url, warning, response)
                             continue
 
                     # 状态码错误
                     if response.status in status_error_list:
                         raise aiohttp_exceptions.ClientError(f'<Response[{response.status}] {url}>')
@@ -397,18 +404,19 @@
 
             # 更新数据
             urls[index] = url
             cb_kwargs.update(cb_kwargs_list[index])
             cb_kwargs_list[index] = cb_kwargs
 
         # 设置base_url
-        if set_base_url and isinstance(set_base_url, str):
-            self.base_url = set_base_url
-        elif set_base_url and not self.base_url:
-            self.base_url = urllib.urljoin(urls[0], '.')
+        if set_base_url:
+            if isinstance(set_base_url, str):
+                self.base_url = set_base_url
+            elif not self.base_url:
+                self.base_url = urllib.urljoin(urls[0], '.')
 
         # 提交异步任务
         tasks = [
             self.request(
                 url=url,
                 callback=callback,
                 method=method,
```

### Comparing `pyxk-0.6.7/pyxk/aclient/typedef.py` & `pyxk-0.6.8/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/aes/cryptor.py` & `pyxk-0.6.8/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/m3u8/_initial.py` & `pyxk-0.6.8/pyxk/m3u8/_initial.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/m3u8/downloader.py` & `pyxk-0.6.8/pyxk/m3u8/downloader.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/m3u8/entry_point.py` & `pyxk-0.6.8/pyxk/m3u8/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/m3u8/m3u8parse.py` & `pyxk-0.6.8/pyxk/m3u8/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/requests/api.py` & `pyxk-0.6.8/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/requests/entry_point.py` & `pyxk-0.6.8/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/requests/sessions.py` & `pyxk-0.6.8/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk/utils.py` & `pyxk-0.6.8/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/pyxk.egg-info/PKG-INFO` & `pyxk-0.6.8/pyxk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.7
+Version: 0.6.8
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.7/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.8/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.7/setup.py` & `pyxk-0.6.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as read_file_obj:
     long_description = read_file_obj.read()
 
 setuptools.setup(
     name='pyxk',
-    version='0.6.7',
+    version='0.6.8',
     author='kai139',
     install_requires=[
         'requests', 'pycryptodome', 'rich', 'm3u8', 'aiohttp', 'aiofiles', 'click', 'parsel'
     ],
     entry_points={
         'console_scripts': [
             'm3u8 = pyxk.m3u8.entry_point:main',
```

