# Comparing `tmp/gdocsync-0.0.6.tar.gz` & `tmp/gdocsync-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdocsync-0.0.6.tar", last modified: Thu Jul 13 04:55:08 2023, max compression
+gzip compressed data, was "gdocsync-0.0.7.tar", last modified: Tue Aug  1 00:47:56 2023, max compression
```

## Comparing `gdocsync-0.0.6.tar` & `gdocsync-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.387510 gdocsync-0.0.6/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.6/LICENSE
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:55:08.387569 gdocsync-0.0.6/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.6/README.rst
--rw-r--r--   0 peterdemin   (503) staff       (20)    21043 2023-07-13 03:49:48.000000 gdocsync-0.0.6/pyproject.toml
--rw-r--r--   0 peterdemin   (503) staff       (20)      757 2023-07-13 04:55:08.387844 gdocsync-0.0.6/setup.cfg
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.384156 gdocsync-0.0.6/src/
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.386654 gdocsync-0.0.6/src/gdocsync/
--rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.6/src/gdocsync/__init__.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      393 2023-07-13 04:36:15.000000 gdocsync-0.0.6/src/gdocsync/cli.py
--rw-r--r--   0 peterdemin   (503) staff       (20)       68 2023-07-13 04:33:19.000000 gdocsync-0.0.6/src/gdocsync/constants.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     3262 2023-07-13 04:43:14.000000 gdocsync-0.0.6/src/gdocsync/docs_importer.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     3124 2023-07-13 02:23:07.000000 gdocsync-0.0.6/src/gdocsync/google_drive_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1365 2023-07-13 04:53:59.000000 gdocsync-0.0.6/src/gdocsync/html_cleaner.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1366 2023-07-13 02:31:07.000000 gdocsync-0.0.6/src/gdocsync/johnny_decimal.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      760 2023-07-13 04:39:53.000000 gdocsync-0.0.6/src/gdocsync/pandoc_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.6/src/gdocsync/regexes.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      824 2023-07-13 04:33:19.000000 gdocsync-0.0.6/src/gdocsync/shelve_cache.py
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.387400 gdocsync-0.0.6/src/gdocsync.egg-info/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      541 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/SOURCES.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/dependency_links.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/entry_points.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       78 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/requires.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/top_level.txt
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-08-01 00:47:56.905157 gdocsync-0.0.7/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.7/LICENSE
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1077 2023-08-01 00:47:56.905230 gdocsync-0.0.7/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      632 2023-07-13 21:01:49.000000 gdocsync-0.0.7/README.rst
+-rw-r--r--   0 peterdemin   (503) staff       (20)    21172 2023-07-13 20:57:49.000000 gdocsync-0.0.7/pyproject.toml
+-rw-r--r--   0 peterdemin   (503) staff       (20)      757 2023-08-01 00:47:56.905520 gdocsync-0.0.7/setup.cfg
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-08-01 00:47:56.901275 gdocsync-0.0.7/src/
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-08-01 00:47:56.904278 gdocsync-0.0.7/src/gdocsync/
+-rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.7/src/gdocsync/__init__.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      393 2023-07-13 04:36:15.000000 gdocsync-0.0.7/src/gdocsync/cli.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)       68 2023-07-13 04:33:19.000000 gdocsync-0.0.7/src/gdocsync/constants.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3262 2023-07-13 04:43:14.000000 gdocsync-0.0.7/src/gdocsync/docs_importer.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3368 2023-08-01 00:47:25.000000 gdocsync-0.0.7/src/gdocsync/google_drive_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1480 2023-07-13 20:57:49.000000 gdocsync-0.0.7/src/gdocsync/html_cleaner.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1477 2023-07-13 20:57:49.000000 gdocsync-0.0.7/src/gdocsync/johnny_decimal.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      762 2023-07-13 20:57:49.000000 gdocsync-0.0.7/src/gdocsync/pandoc_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.7/src/gdocsync/regexes.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      824 2023-07-13 04:33:19.000000 gdocsync-0.0.7/src/gdocsync/shelve_cache.py
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-08-01 00:47:56.905056 gdocsync-0.0.7/src/gdocsync.egg-info/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1077 2023-08-01 00:47:56.000000 gdocsync-0.0.7/src/gdocsync.egg-info/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      541 2023-08-01 00:47:56.000000 gdocsync-0.0.7/src/gdocsync.egg-info/SOURCES.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-08-01 00:47:56.000000 gdocsync-0.0.7/src/gdocsync.egg-info/dependency_links.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-08-01 00:47:56.000000 gdocsync-0.0.7/src/gdocsync.egg-info/entry_points.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       78 2023-08-01 00:47:56.000000 gdocsync-0.0.7/src/gdocsync.egg-info/requires.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-08-01 00:47:56.000000 gdocsync-0.0.7/src/gdocsync.egg-info/top_level.txt
```

### Comparing `gdocsync-0.0.6/LICENSE` & `gdocsync-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.6/pyproject.toml` & `gdocsync-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 use_parentheses = true
 line_length = 100
 
 [tool.flake8]
 max-line-length = 100
 max-complexity = 10
 
+[tool.mypy]
+packages = ["gdocsync"]
+
+[[tool.mypy.overrides]]
+module = "google_auth_oauthlib.flow"
+ignore_missing_imports = true
+
 [tool.pylint.main]
 # Analyse import fallback blocks. This can be used to support both Python 2 and 3
 # compatible code, which means that the block might have code that exists only in
 # one or another interpreter, leading to false positives when analysed.
 # analyse-fallback-blocks =
 
 # Always return a 0 (non-error) status code, even if lint errors are found. This
```

### Comparing `gdocsync-0.0.6/setup.cfg` & `gdocsync-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdocsync
-version = 0.0.6
+version = 0.0.7
 author = Peter Demin
 author_email = peterdemin@gmail.com
 description = 
 long_description = file:README.rst
 url = https://github.com/peterdemin/gdocsync
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `gdocsync-0.0.6/src/gdocsync/docs_importer.py` & `gdocsync-0.0.7/src/gdocsync/docs_importer.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.6/src/gdocsync/google_drive_client.py` & `gdocsync-0.0.7/src/gdocsync/google_drive_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os.path
 from dataclasses import dataclass
 from typing import List
 
+from google.auth.exceptions import RefreshError
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 from .shelve_cache import ShelveCache
 
@@ -35,18 +36,24 @@
         # time.
         with self._cache.session() as cache:
             if token := cache.get("token"):
                 creds = Credentials.from_authorized_user_info(token, SCOPES)
             else:
                 creds = None
             # If there are no (valid) credentials available, let the user log in.
+            fresh = False
             if not creds or not creds.valid:
                 if creds and creds.expired and creds.refresh_token:
-                    creds.refresh(Request())
-                else:
+                    try:
+                        creds.refresh(Request())
+                    except RefreshError:
+                        pass
+                    else:
+                        fresh = True
+                if not fresh:
                     flow = InstalledAppFlow.from_client_secrets_file(self._CREDENTIALS_PATH, SCOPES)
                     creds = flow.run_local_server(port=0)
                 # Save the credentials for the next run
                 cache["token"] = json.loads(creds.to_json())
             return creds
```

### Comparing `gdocsync-0.0.6/src/gdocsync/html_cleaner.py` & `gdocsync-0.0.7/src/gdocsync/html_cleaner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from typing import Iterable
+from typing import Iterable, cast, List
 from urllib.parse import parse_qs, urlparse
 
 from lxml import etree
+from lxml.etree import _Element as ElementType
 
 
 class HTMLCleaner:
     GOOGLE_TRACKING = "https://www.google.com/url"
     BOLD_SELECTORS = [
         '//span[@class="c1"]',
         '//span[contains(@style,"font-weight:700")]',
     ]
 
     def __call__(self, html_contents: str) -> str:
-        htmlparser = etree.HTMLParser()
-        tree = etree.fromstring(html_contents, htmlparser)
+        tree = etree.fromstring(html_contents, cast(etree.XMLParser, etree.HTMLParser()))
         etree.strip_elements(tree, "style")
         self._fix_spans(tree)
         self._fix_links(tree)
         return etree.tostring(tree, pretty_print=True).decode("utf-8")
 
-    def _fix_spans(self, tree: etree.ElementTree) -> None:
+    def _fix_spans(self, tree: ElementType) -> None:
         for bold_span in self._iter_bold_spans(tree):
             bold_span.tag = "b"
-            bold_span.text = bold_span.text.strip()
+            if bold_span.text:
+                bold_span.text = bold_span.text.strip()
         etree.strip_tags(tree, "span")
 
-    def _iter_bold_spans(self, tree: etree.ElementTree) -> Iterable[etree.Element]:
+    def _iter_bold_spans(self, tree: ElementType) -> Iterable[ElementType]:
         for selector in self.BOLD_SELECTORS:
-            yield from tree.xpath(selector)
+            yield from cast(List[ElementType], tree.xpath(selector))
 
-    def _fix_links(self, tree: etree.ElementTree) -> None:
-        for link in tree.xpath("//a"):
+    def _fix_links(self, tree: ElementType) -> None:
+        for link in cast(List[ElementType], tree.xpath("//a")):
             url = link.get("href")
             if not url or not url.startswith(self.GOOGLE_TRACKING):
                 continue
             if real_url := parse_qs(urlparse(url).query).get("q", [""])[0]:
                 link.set("href", real_url)
```

### Comparing `gdocsync-0.0.6/src/gdocsync/johnny_decimal.py` & `gdocsync-0.0.7/src/gdocsync/johnny_decimal.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     category: str
     index: str
     name: str
 
     @classmethod
     def parse(cls, name: str) -> "JohnnyDecimal":
         match_obj = RE_JOHNNY_DECIMAL.match(name)
+        if match_obj is None:
+            raise ValueError(f'{name} does not follow Johnny Decimal notation.')
         groups = match_obj.groups()
         return cls(
             category=groups[0],
             index=groups[1],
             name=groups[2],
         )
```

### Comparing `gdocsync-0.0.6/src/gdocsync/pandoc_client.py` & `gdocsync-0.0.7/src/gdocsync/pandoc_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import subprocess
 import tempfile
 
 
 class PandocClient:
-    def convert_to_rst(self, source_bytes: bytes, target_path: str, extension: str = "odt") -> str:
+    def convert_to_rst(self, source_bytes: bytes, target_path: str, extension: str = "odt") -> None:
         target_dir = os.path.dirname(target_path)
         with tempfile.TemporaryDirectory() as temp_dir:
             source_name = os.path.join(temp_dir, f"source.{extension}")
             with open(source_name, "wb") as f_in:
                 f_in.write(source_bytes)
             os.system(f"pandoc {source_name} -o {target_path} --extract-media {target_dir}")
 
-    def html_to_rst(self, source_path: str, target_path: str) -> str:
+    def html_to_rst(self, source_path: str, target_path: str) -> None:
         subprocess.check_call(
             ("pandoc", source_path, "-o", os.path.basename(target_path)),
             cwd=os.path.dirname(target_path),
         )
```

### Comparing `gdocsync-0.0.6/src/gdocsync/shelve_cache.py` & `gdocsync-0.0.7/src/gdocsync/shelve_cache.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.6/src/gdocsync.egg-info/SOURCES.txt` & `gdocsync-0.0.7/src/gdocsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

