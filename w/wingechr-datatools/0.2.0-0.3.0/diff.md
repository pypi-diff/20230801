# Comparing `tmp/wingechr-datatools-0.2.0.tar.gz` & `tmp/wingechr-datatools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wingechr-datatools-0.2.0.tar", last modified: Sat Jul 29 11:54:51 2023, max compression
+gzip compressed data, was "wingechr-datatools-0.3.0.tar", last modified: Tue Aug  1 14:14:47 2023, max compression
```

## Comparing `wingechr-datatools-0.2.0.tar` & `wingechr-datatools-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.883850 wingechr-datatools-0.2.0/
--rw-rw-rw-   0        0        0      115 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/.bumpversion.cfg
-drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.680285 wingechr-datatools-0.2.0/.github/
-drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.742725 wingechr-datatools-0.2.0/.github/workflows/
--rw-rw-rw-   0        0        0      898 2023-07-24 13:10:24.000000 wingechr-datatools-0.2.0/.github/workflows/test.yml
--rw-rw-rw-   0        0        0      116 2023-07-26 15:28:45.000000 wingechr-datatools-0.2.0/.gitignore
--rw-rw-rw-   0        0        0     1215 2023-07-24 13:10:24.000000 wingechr-datatools-0.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      489 2023-07-29 11:54:51.882869 wingechr-datatools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.852726 wingechr-datatools-0.2.0/datatools/
--rw-rw-rw-   0        0        0      220 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/__init__.py
--rw-rw-rw-   0        0        0     3510 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/__main__.py
--rw-rw-rw-   0        0        0     2292 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/cache.py
--rw-rw-rw-   0        0        0      680 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/exceptions.py
--rw-rw-rw-   0        0        0     3823 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/load.py
--rw-rw-rw-   0        0        0    10530 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/storage.py
--rw-rw-rw-   0        0        0    10349 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/utils.py
--rw-rw-rw-   0        0        0      136 2023-07-24 13:10:24.000000 wingechr-datatools-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:54:51.883850 wingechr-datatools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.865496 wingechr-datatools-0.2.0/tests/
--rw-rw-rw-   0        0        0      289 2023-07-27 09:42:54.000000 wingechr-datatools-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     5006 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tests/test_01_utils.py
--rw-rw-rw-   0        0        0     6435 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tests/test_02_storage.py
--rw-rw-rw-   0        0        0      862 2023-07-26 15:28:45.000000 wingechr-datatools-0.2.0/tests/test_04_cache.py
--rw-rw-rw-   0        0        0      921 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tests/test_05_sql.py
--rw-rw-rw-   0        0        0      117 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tox.ini
-drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.880850 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/
--rw-rw-rw-   0        0        0      489 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 14:14:47.486397 wingechr-datatools-0.3.0/
+-rw-rw-rw-   0        0        0      115 2023-08-01 13:55:10.000000 wingechr-datatools-0.3.0/.bumpversion.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 14:14:47.266156 wingechr-datatools-0.3.0/.github/
+drwxrwxrwx   0        0        0        0 2023-08-01 14:14:47.314445 wingechr-datatools-0.3.0/.github/workflows/
+-rw-rw-rw-   0        0        0      897 2023-07-30 10:05:04.000000 wingechr-datatools-0.3.0/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0      116 2023-07-26 15:28:45.000000 wingechr-datatools-0.3.0/.gitignore
+-rw-rw-rw-   0        0        0     1215 2023-07-24 13:10:24.000000 wingechr-datatools-0.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      489 2023-08-01 14:14:47.484755 wingechr-datatools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-08-01 13:57:49.000000 wingechr-datatools-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 14:14:47.342073 wingechr-datatools-0.3.0/datatools/
+-rw-rw-rw-   0        0        0      395 2023-08-01 13:55:10.000000 wingechr-datatools-0.3.0/datatools/__init__.py
+-rw-rw-rw-   0        0        0     4188 2023-07-31 07:09:38.000000 wingechr-datatools-0.3.0/datatools/__main__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-29 12:45:26.000000 wingechr-datatools-0.3.0/datatools/cache.py
+-rw-rw-rw-   0        0        0      680 2023-07-29 11:54:21.000000 wingechr-datatools-0.3.0/datatools/exceptions.py
+-rw-rw-rw-   0        0        0     4223 2023-07-30 15:54:29.000000 wingechr-datatools-0.3.0/datatools/load.py
+-rw-rw-rw-   0        0        0    11818 2023-08-01 13:52:35.000000 wingechr-datatools-0.3.0/datatools/storage.py
+-rw-rw-rw-   0        0        0    12218 2023-07-31 07:39:20.000000 wingechr-datatools-0.3.0/datatools/utils.py
+-rw-rw-rw-   0        0        0      136 2023-07-24 13:10:24.000000 wingechr-datatools-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 14:14:47.486897 wingechr-datatools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2023-08-01 13:55:10.000000 wingechr-datatools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:14:47.414062 wingechr-datatools-0.3.0/tests/
+-rw-rw-rw-   0        0        0      423 2023-07-30 10:05:04.000000 wingechr-datatools-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     6191 2023-07-30 10:05:04.000000 wingechr-datatools-0.3.0/tests/test_01_utils.py
+-rw-rw-rw-   0        0        0     6558 2023-07-30 10:46:06.000000 wingechr-datatools-0.3.0/tests/test_02_storage.py
+-rw-rw-rw-   0        0        0      862 2023-07-26 15:28:45.000000 wingechr-datatools-0.3.0/tests/test_04_cache.py
+-rw-rw-rw-   0        0        0      921 2023-07-29 11:54:21.000000 wingechr-datatools-0.3.0/tests/test_05_sql.py
+-rw-rw-rw-   0        0        0      117 2023-07-29 11:54:21.000000 wingechr-datatools-0.3.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-08-01 14:14:47.481113 wingechr-datatools-0.3.0/wingechr_datatools.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-08-01 14:14:46.000000 wingechr-datatools-0.3.0/wingechr_datatools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-08-01 14:14:47.000000 wingechr-datatools-0.3.0/wingechr_datatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 14:14:46.000000 wingechr-datatools-0.3.0/wingechr_datatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-08-01 14:14:46.000000 wingechr-datatools-0.3.0/wingechr_datatools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2023-08-01 14:14:46.000000 wingechr-datatools-0.3.0/wingechr_datatools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 14:14:46.000000 wingechr-datatools-0.3.0/wingechr_datatools.egg-info/top_level.txt
```

### Comparing `wingechr-datatools-0.2.0/.github/workflows/test.yml` & `wingechr-datatools-0.3.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: test
 
 on:
   push:
     branches:
-      - main
+      - dev
 
 jobs:
   test:
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest] # macos-latest
     runs-on: ${{ matrix.os }}
```

### Comparing `wingechr-datatools-0.2.0/.pre-commit-config.yaml` & `wingechr-datatools-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wingechr-datatools-0.2.0/datatools/__main__.py` & `wingechr-datatools-0.3.0/datatools/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 
 import json
 import logging
 import sys
 
 import click
 
-from . import Storage, __version__
+from . import GLOBAL_LOCATION, LOCAL_LOCATION, Storage, __version__
 from .exceptions import DataDoesNotExists, DatatoolsException
-from .load import write_uri
-from .utils import parse_cli_metadata
+from .load import open_uri, write_uri
+from .utils import as_uri, json_serialize, parse_cli_metadata
 
 
 @click.group()
 @click.pass_context
 @click.version_option(__version__)
 @click.option(
     "--loglevel",
     "-l",
     type=click.Choice(["debug", "info", "warning", "error"], case_sensitive=False),
     default="info",
     show_default=True,
 )
 @click.option("--location", "-d")
-def main(ctx, loglevel, location):
+@click.option("--global-location", "-g", is_flag=True)
+def main(ctx, loglevel, location, global_location):
     """Script entry point."""
     # setup default logging
     loglevel = getattr(logging, loglevel.upper())
     format = "[%(asctime)s %(levelname)7s] %(message)s"
     datefmt = "%Y-%m-%d %H:%M:%S"
     logging.basicConfig(level=loglevel, format=format, datefmt=datefmt)
     # setup color logging
@@ -37,14 +38,20 @@
         coloredlogs.DEFAULT_LOG_FORMAT = format
         coloredlogs.DEFAULT_DATE_FORMAT = datefmt
         coloredlogs.DEFAULT_FIELD_STYLES = {"asctime": {"color": None}}
         coloredlogs.install(level=loglevel)
     except ModuleNotFoundError:
         pass
 
+    if location and global_location:
+        raise DatatoolsException("location and global-location are mutually exclusive")
+    if global_location:
+        location = GLOBAL_LOCATION
+    if not location:
+        location = LOCAL_LOCATION
     ctx.obj = Storage(location=location)
 
 
 @main.command("data-get")
 @click.pass_obj
 @click.argument("data_path")
 @click.argument("file_path")
@@ -70,28 +77,35 @@
 @main.command("data-put")
 @click.pass_obj
 @click.option("--exist-ok", "-e", is_flag=True)
 @click.argument("source")
 @click.argument("data_path", required=False)
 def data_put(storage: Storage, source, data_path: str = None, exist_ok=False):
     if source in ("", "-"):
-        source = sys.stdin.buffer
-    norm_data_path = storage.data_put(
-        data=source, data_path=data_path, exist_ok=exist_ok
-    )
+        data = sys.stdin.buffer
+        metadata = {}
+    else:
+        uri = as_uri(source=source)
+        data, metadata = open_uri(uri)
+        if data_path is None:
+            data_path = uri
+    logging.debug(data)
+    norm_data_path = storage.data_put(data=data, data_path=data_path, exist_ok=exist_ok)
+    if metadata:
+        storage.metadata_put(data_path=norm_data_path, metadata=metadata)
     print(norm_data_path)
 
 
 @main.command("metadata-get")
 @click.pass_obj
 @click.argument("data_path")
 @click.argument("metadata_path", required=False)
 def metadata_get(storage: Storage, data_path, metadata_path):
     results = storage.metadata_get(data_path=data_path, metadata_path=metadata_path)
-    print(json.dumps(results, indent=2, ensure_ascii=True))
+    print(json.dumps(results, indent=2, ensure_ascii=True, default=json_serialize))
 
 
 @main.command("metadata-put")
 @click.pass_obj
 @click.argument("data_path")
 @click.argument("metadata_key_vals", nargs=-1, required=True)
 def metadata_put(storage: Storage, data_path, metadata_key_vals):
```

### Comparing `wingechr-datatools-0.2.0/datatools/cache.py` & `wingechr-datatools-0.3.0/datatools/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import functools
 import hashlib
 import json
 import logging
 import pickle
 
+from datatools.utils import json_serialize
+
 DEFAULT_FROM_BYTES = pickle.loads
 DEFAULT_TO_BYTES = pickle.dumps
 
 
 DEFAULT_MEDIA_TYPE = "application/x-pickle"
 
 
 def get_hash(object):
-    bytes = json.dumps(object, sort_keys=True, ensure_ascii=False).encode()
+    bytes = json.dumps(
+        object, sort_keys=True, ensure_ascii=False, default=json_serialize
+    ).encode()
     job_id = hashlib.md5(bytes).hexdigest()
     return job_id
 
 
 def get_job_description(fun, args, kwargs):
     return {
         "function": fun.__name__,
```

### Comparing `wingechr-datatools-0.2.0/datatools/exceptions.py` & `wingechr-datatools-0.3.0/datatools/exceptions.py`

 * *Files identical despite different names*

### Comparing `wingechr-datatools-0.2.0/datatools/load.py` & `wingechr-datatools-0.3.0/datatools/load.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 import logging
 import os
 import re
 from io import BufferedReader, BytesIO
 from pathlib import Path
 from typing import Tuple
-from urllib.parse import parse_qs, urlencode, urlsplit
+from urllib.parse import parse_qs, unquote, urlencode, urlsplit
 
 import requests
 import sqlalchemy as sa
 
 from .cache import DEFAULT_MEDIA_TYPE, DEFAULT_TO_BYTES
 from .utils import (
     filepath_abs_to_uri,
+    get_sql_table_schema,
     normalize_sql_query,
     parse_content_type,
     remove_auth_from_uri_or_path,
     uri_to_filepath_abs,
 )
 
 PARAM_SQL_QUERY = "q"
 
 
-def get_table_schema(cursor):
-    fields = [
-        {"name": name, "data_type": data_type, "is_nullable": is_nullable}
-        for (
-            name,
-            data_type,
-            _display_size,
-            _internal_size,
-            _precision,
-            _scale,
-            is_nullable,
-        ) in cursor.description
-    ]
-    return {"fields": fields}
-
-
 def open_uri(uri: str) -> Tuple[BufferedReader, dict]:
     metadata = {}
 
     metadata["source.path"] = remove_auth_from_uri_or_path(uri)
 
     url_parts = urlsplit(uri)
 
     # protocol routing
     if url_parts.scheme == "file":
         file_path = uri_to_filepath_abs(uri)
         data = open(file_path, "rb")
 
     elif url_parts.scheme in ["http", "https"]:
-        res = requests.get(uri, stream=True)
+        # because we want to encode auth headers
+        # in the uri, we place it in the netloc
+        # part before the @host (instead of the basic auth)
+        # if it's basic auth, the pattern is `user:pass`
+        # if it's a header, it's header=value
+        match_header = re.match("^([^=@]+)=([^=@]+)@(.+)$", url_parts.netloc)
+        headers = {}
+        if match_header:
+            h_name, h_val, netloc = match_header.groups()
+            h_name = unquote(h_name)
+            h_val = unquote(h_val)
+            url_parts = url_parts._replace(netloc=netloc)
+            headers[h_name] = h_val
+            logging.debug("Stripping auth header from uri")
+
+        res = requests.get(uri, stream=True, headers=headers)
+
         res.raise_for_status()
         content_type = res.headers.get("Content-Type")
         if content_type:
             _meta = parse_content_type(content_type)
             metadata.update(_meta)
             logging.info(_meta)
 
         data = res.raw
 
     elif "sql" in url_parts.scheme:
         # pop sql query
         query_dict = parse_qs(url_parts.query)
         sql_query = query_dict.pop(PARAM_SQL_QUERY)[0]
+        sql_query = unquote(sql_query)
         sql_query = normalize_sql_query(sql_query)
+
         metadata["source.query"] = sql_query
         # doseq: if False: encode arrays differently
         query_str = urlencode(query_dict, doseq=True)
         url_parts = url_parts._replace(query=query_str)
 
         if not url_parts.netloc:
             # usually, netloc is empty, and so geturl() drops the "//"" at the beginning
@@ -79,15 +82,15 @@
         connection_string = url_parts.geturl()
         logging.debug(f"Connect: {connection_string}")
         eng = sa.create_engine(connection_string)
         with eng.connect() as con:
             with con:
                 logging.debug(f"Exceute: {sql_query}")
                 res = con.execute(sa.text(sql_query))
-                data_schema = get_table_schema(res.cursor)
+                data_schema = get_sql_table_schema(res.cursor)
                 logging.debug(f"Schema: {data_schema}")
 
                 # data = pd.DataFrame(res.fetchall())
                 data = [rec._asdict() for rec in res.fetchall()]
 
                 logging.debug(f"Rows: {len(data)}")
         # make sure everything is closed
```

### Comparing `wingechr-datatools-0.2.0/datatools/storage.py` & `wingechr-datatools-0.3.0/datatools/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,37 +13,38 @@
 
 from .cache import cache
 from .exceptions import DataDoesNotExists, DataExists, IntegrityError, InvalidPath
 from .load import open_uri
 from .utils import (
     as_byte_iterator,
     as_uri,
+    get_default_storage_location,
     get_now_str,
     get_user_w_host,
     json_serialize,
     make_file_readonly,
     make_file_writable,
     normalize_path,
 )
 
 # remote
-# PARAM_METADATA_PATH = "p"
-# PARAM_DATA_PATH = "path"
-# PARAM_VALUE = "value"
 ROOT_METADATA_PATH = "$"  # root
-# DEFAULT_PORT = 8000
 HASHED_DATA_PATH_PREFIX = "hash/"
 ALLOWED_HASH_METHODS = ["md5", "sha256"]
 
 DEFAULT_HASH_METHOD = ALLOWED_HASH_METHODS[0]
 
+GLOBAL_LOCATION = get_default_storage_location()
+LOCAL_LOCATION = "__data__"
+
 
 class Storage:
-    def __init__(self, location):
-        self.location = location
+    def __init__(self, location=None):
+        location = location or LOCAL_LOCATION
+        self.location = os.path.abspath(location)
         logging.debug(f"Location: {self.location}")
 
     def __enter__(self):
         # does not do anything currently
         return self
 
     def __exit__(self, *args):
@@ -138,18 +139,23 @@
 
         logging.debug(f"WRITING {metadata_filepath}")
         with open(metadata_filepath, "wb") as file:
             file.write(metadata_bytes)
 
     def data_put(
         self,
-        data: Union[BufferedReader, bytes, Iterable],
+        data: Union[BufferedReader, bytes, Iterable, str],
         data_path: str = None,
         exist_ok=None,
     ) -> str:
+        if isinstance(data, str):
+            return self._data_put_uri(
+                source=data, data_path=data_path, exist_ok=bool(exist_ok)
+            )
+
         # if not datapath: map to default hash endpoint
         if not data_path:
             norm_data_path = self._get_norm_data_path(
                 f"{HASHED_DATA_PATH_PREFIX}{DEFAULT_HASH_METHOD}"
             )
             if exist_ok is False:
                 logging.warning("without a data path, exist_ok = False will be ignored")
@@ -186,19 +192,24 @@
         size = 0
         hasher = getattr(hashlib, hash_method)()
         data = as_byte_iterator(data)
 
         with NamedTemporaryFile(
             mode="wb", dir=data_dir, delete=False, prefix=filename + "+"
         ) as file:
-            logging.debug(f"WRITING {file.name}")
-            for chunk in data:
-                size += len(chunk)
-                hasher.update(chunk)
-                file.write(chunk)
+            try:
+                logging.debug(f"WRITING {file.name}")
+                for chunk in data:
+                    size += len(chunk)
+                    hasher.update(chunk)
+                    file.write(chunk)
+            except Exception:
+                file.close()
+                os.remove(file.name)
+                raise
 
         hashsum = hasher.hexdigest()
 
         if filepath_is_hash:
             data_filepath = os.path.join(data_dir, hashsum)
             # replace placeholder
             n_placeholder = len("__HASHFILE__")
@@ -224,33 +235,58 @@
             "source.datetime": get_now_str(),
             "source.name": norm_data_path,
         }
         self.metadata_put(data_path=norm_data_path, metadata=metadata)
 
         return norm_data_path
 
+    def _data_put_uri(self, source: str, data_path=None, exist_ok=False) -> str:
+        uri = as_uri(source=source)
+        data_path = data_path or uri
+        norm_data_path = self.data_exists(data_path=data_path)
+        if norm_data_path:
+            if exist_ok:
+                return norm_data_path
+            else:
+                raise FileExistsError(uri)
+        data, metadata = open_uri(uri)
+        norm_data_path = self.data_put(data=data, data_path=data_path, exist_ok=False)
+        if metadata:
+            self.metadata_put(data_path=norm_data_path, metadata=metadata)
+        return norm_data_path
+
     def data_open(self, data_path: str, auto_load_uri: bool = False) -> BufferedReader:
         if auto_load_uri and not self.data_exists(data_path=data_path):
-            uri = as_uri(source=data_path)
-            data, metadata = open_uri(uri)
-            norm_data_path = self.data_put(data=data, data_path=uri, exist_ok=False)
-            if metadata:
-                self.metadata_put(data_path=data_path, metadata=metadata)
+            norm_data_path = self._data_put_uri(
+                source=data_path, data_path=None, exist_ok=False
+            )
         else:
             norm_data_path = self.data_exists(data_path=data_path)
 
         if not norm_data_path:
             raise DataDoesNotExists(data_path)
 
         data_filepath = self._get_data_filepath(norm_data_path=norm_data_path)
         logging.debug(f"READING {data_filepath}")
         data = open(data_filepath, "rb")
 
         return data
 
+    def get_filepath(self, data_path: str) -> str:
+        norm_data_path = self.data_exists(data_path=data_path)
+
+        if not norm_data_path:
+            raise DataDoesNotExists(data_path)
+
+        data_filepath = self._get_data_filepath(norm_data_path=norm_data_path)
+        # just to be sure
+        make_file_readonly(data_filepath)
+
+        return data_filepath
+
     def data_exists(self, data_path) -> str:
         norm_data_path = self._get_norm_data_path(data_path)
         data_filepath = self._get_data_filepath(norm_data_path=norm_data_path)
         if os.path.exists(data_filepath):
             return norm_data_path
 
     def data_delete(self, data_path: str) -> None:
```

### Comparing `wingechr-datatools-0.2.0/datatools/utils.py` & `wingechr-datatools-0.3.0/datatools/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import atexit
+import csv
 import datetime
+import inspect
 import json
 import logging
 import os
 import re
 import socket
 import sys
 import time
 from contextlib import ExitStack
-from io import BufferedReader, BytesIO
+from io import BufferedReader, DEFAULT_BUFFER_SIZE as _DEFAULT_BUFFER_SIZE
 from pathlib import Path
 from typing import Iterable, Union
 from urllib.parse import unquote, unquote_plus, urlsplit
 
 import appdirs
+import chardet
+import numpy as np
+import pandas as pd
 import requests
 import sqlparse
 import tzlocal
 import unidecode
 
 from .exceptions import InvalidPath
 
@@ -27,15 +32,15 @@
 FILEMOD_WRITE = 0o222
 ANONYMOUS_USER = "Anonymous"
 LOCALHOST = "localhost"
 
 
 # default is 1024 * 8
 # wsgi often uses 1024 * 16
-DEFAULT_BUFFER_SIZE = 8 * 1024
+DEFAULT_BUFFER_SIZE = _DEFAULT_BUFFER_SIZE
 
 # global exit stack
 exit_stack = ExitStack()
 # register at error
 sys.excepthook = exit_stack.__exit__
 # also register on regular exit
 atexit.register(exit_stack.__exit__, None, None, None)
@@ -139,14 +144,39 @@
         raise InvalidPath(_path)
     if path != _path:
         logging.debug(f"Translating {_path} => {path}")
 
     return path
 
 
+def normalize_name(name: str) -> str:
+    """should be all lowercase ascii
+    * uri: remove query
+
+    """
+    _name = name  # cop
+    name = unquote_plus(name)
+    name = name.lower()
+    for cin, cout in [
+        ("ä", "ae"),
+        ("ö", "oe"),
+        ("ü", "ue"),
+        ("ß", "ss"),
+    ]:
+        name = name.replace(cin, cout)
+    name = unidecode.unidecode(name)
+    name = re.sub(r"[^a-z0-9]+", "_", name)
+    name = name.strip("_")
+
+    if not name:
+        raise InvalidPath(_name)
+
+    return name
+
+
 def get_default_storage_location() -> str:
     """get the users data storage path"""
     return os.path.join(
         appdirs.user_data_dir(
             appname="datatools", appauthor=None, version=None, roaming=False
         ),
         "data",
@@ -202,14 +232,18 @@
 
 
 def platform_is_windows() -> bool:
     # os.name: 'posix', 'nt', 'java'
     return os.name == "nt"
 
 
+def platform_is_unix() -> bool:
+    return not platform_is_windows()
+
+
 def make_file_readonly(file_path: str) -> None:
     """Note: in WIndows, this also prevents delete
     but not in Linux
     """
     current_permissions = os.stat(file_path).st_mode
     readonly_permissions = current_permissions & ~FILEMOD_WRITE
     os.chmod(file_path, readonly_permissions)
@@ -350,32 +384,71 @@
 def json_serialize(x):
     if isinstance(x, datetime.datetime):
         return x.strftime(DATETIMETZ_FMT)
     elif isinstance(x, datetime.date):
         return x.strftime(DATE_FMT)
     elif isinstance(x, datetime.time):
         return x.strftime(TIME_FMT)
-    elif isinstance(x, type):
+    elif isinstance(x, np.bool_):
+        return bool(x)
+    elif inspect.isclass(x):
         # classname
         return x.__name__
     else:
-        raise NotImplementedError(type(x))
-
-
-def iter_chunks(input):
-    if isinstance(input, bytes):
-        input = BytesIO(input)
+        raise NotImplementedError(f"{x.__class__}: {x}")
 
 
 def as_byte_iterator(data: Union[bytes, Iterable, BufferedReader]) -> Iterable[bytes]:
     if isinstance(data, bytes):
         yield data
     elif isinstance(data, BufferedReader):
         while True:
-            chunk = input.read(DEFAULT_BUFFER_SIZE)
+            chunk = data.read(DEFAULT_BUFFER_SIZE)
+            logging.debug(f"read {len(chunk)} bytes")
             if not chunk:
                 break
             yield chunk
     elif isinstance(data, Iterable):
         yield from data
     else:
         raise NotImplementedError(type(data))
+
+
+def detect_encoding(sample_data: bytes):
+    result = chardet.detect(sample_data)
+    if result["confidence"] < 1:
+        logging.warning(f"Chardet encoding detection < 100%: {result}")
+    return result["encoding"]
+
+
+def detect_csv_dialect(sample_data: str):
+    dialect = csv.Sniffer().sniff(sample_data)
+    return dialect
+
+
+def get_sql_table_schema(cursor):
+    fields = [
+        {"name": name, "data_type": data_type, "is_nullable": is_nullable}
+        for (
+            name,
+            data_type,
+            _display_size,
+            _internal_size,
+            _precision,
+            _scale,
+            is_nullable,
+        ) in cursor.description
+    ]
+    return {"fields": fields}
+
+
+def get_df_table_schema(df: pd.DataFrame):
+    fields = []
+    for cname in df.columns:
+        fields.append(
+            {
+                "name": cname,
+                "data_type": df[cname].dtype.name,
+                "is_nullable": (df[cname].isna() | df[cname].isnull()).any(),
+            }
+        )
+    return {"fields": fields}
```

### Comparing `wingechr-datatools-0.2.0/setup.py` & `wingechr-datatools-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,20 +12,21 @@
             "requests",
             "tzlocal",
             "unidecode",
             "sqlalchemy>=2.0",
             "sqlparse",
             "pyodbc",
             "pandas",
+            "chardet",
         ],
         name="wingechr-datatools",
         description=None,
         long_description=None,
         long_description_content_type="text/markdown",
-        version="0.2.0",
+        version="0.3.0",
         author="Christian Winger",
         author_email="c@wingechr.de",
         url="https://github.com/wingechr/datatools",
         platforms=["any"],
         license="Public Domain",
         project_urls={"Bug Tracker": "https://github.com/wingechr/datatools"},
         classifiers=[
```

### Comparing `wingechr-datatools-0.2.0/tests/test_01_utils.py` & `wingechr-datatools-0.3.0/tests/test_01_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 import os
 import re
 import unittest
 from io import BytesIO
 from pathlib import PurePosixPath, PureWindowsPath
 from tempfile import TemporaryDirectory
 
+import numpy as np
+import pandas as pd
+
 from datatools.utils import (
     as_byte_iterator,
     filepath_abs_to_uri,
+    get_df_table_schema,
     get_hostname,
     get_now_str,
     get_user_w_host,
+    json_serialize,
     make_file_readonly,
     make_file_writable,
     normalize_path,
     normalize_sql_query,
     parse_cli_metadata,
     platform_is_windows,
     uri_to_filepath_abs,
@@ -34,14 +39,15 @@
             ("https://a/b/", "http/a/b"),
             ("https://a:8000/b", "http/a/b"),
             ("https://a/b/?a=1#x", "http/a/b/x"),
             ("https://a/b?a=1#.x", "http/a/b.x"),
             ("http://a.com#x", "http/a.comx"),
             ("http://a.com#/x", "http/a.com/x"),
             ("http://user:pass@a.com", "http/a.com"),
+            ("http://header=token@a.com", "http/a.com"),
             ("Lower  Case with SPACE ! ", "lower_case_with_space"),
             (
                 "François fährt Straßenbahn zum Café Málaga",
                 "francois_faehrt_strassenbahn_zum_cafe_malaga",
             ),
             (
                 "https://www.domain-name.de/path%202021.pdf",
@@ -146,7 +152,36 @@
         self.assertEqual(b"".join(data_l), data)
 
         # check self
         data1 = as_byte_iterator([data[:5], data[5:]])
         data_l = list(as_byte_iterator(data1))
         self.assertEqual(len(data_l), 2)
         self.assertEqual(b"".join(data_l), data)
+
+    def test_json_serialize(self):
+        res = json_serialize(object)
+        self.assertEqual(res, "object")
+
+    def test_get_df_table_schema(self):
+        df = pd.DataFrame(
+            {
+                "i": [0, 0, 80, 10, 20],
+                "c": ["x", "x", "x", None, "x"],
+                "b": [True, False, True, True, False],
+                "f": [np.inf, np.nan, 10.1, -12.231, 1e4],
+            }
+        )
+        schema = get_df_table_schema(df)
+        self.assertTrue(
+            objects_euqal(
+                schema,
+                {
+                    "fields": [
+                        {"name": "i", "data_type": "int64", "is_nullable": False},
+                        {"name": "c", "data_type": "object", "is_nullable": True},
+                        {"name": "b", "data_type": "bool", "is_nullable": False},
+                        {"name": "f", "data_type": "float64", "is_nullable": True},
+                    ]
+                },
+            ),
+            schema,
+        )
```

### Comparing `wingechr-datatools-0.2.0/tests/test_02_storage.py` & `wingechr-datatools-0.3.0/tests/test_02_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 import os
 import subprocess as sp
 import sys
 
 # import secrets
 import unittest
 from tempfile import TemporaryDirectory
-from urllib.parse import urlsplit
 
 from datatools.cache import DEFAULT_FROM_BYTES
 from datatools.exceptions import DataDoesNotExists, DataExists, InvalidPath
 from datatools.storage import HASHED_DATA_PATH_PREFIX, Storage
-from datatools.utils import (  # exit_stack,
+from datatools.utils import (
     DEFAULT_BUFFER_SIZE,
-    as_uri,
     get_free_port,
     make_file_writable,
     normalize_path,
+    platform_is_unix,
     wait_for_server,
 )
 
 from . import objects_euqal
 
 
 class MyTemporaryDirectory(TemporaryDirectory):
@@ -57,15 +56,17 @@
             [
                 sys.executable,
                 "-m",
                 "http.server",
                 str(port),
                 "--directory",
                 self.static_dir,
-            ]
+            ],
+            stdout=sp.DEVNULL,  # do not show server startup message
+            stderr=sp.DEVNULL,  # do not show server request logging
         )
         wait_for_server(self.static_url)
 
     def tearDown(self) -> None:
         self.http_proc.terminate()  # or kill
         self.http_proc.wait()
 
@@ -162,20 +163,22 @@
         with self.storage.data_open(data_path=uri, auto_load_uri=True) as file:
             data = file.read()
         data = DEFAULT_FROM_BYTES(data)
         self.assertEqual(data[0]["value"], 1)
 
         # save test file
         db_filepath = self.static_dir + "/test.db"
-        with open(db_filepath, "wb") as file:
-            pass
+        # file should be created by sqlalchemy
 
-        # platform independent: no baskslash, abspath, always starts with /
-        db_path = urlsplit(as_uri(db_filepath)).path
-        uri = f"sqlite://{db_path}?q=select 1 as value#/query1"
+        # only for sqlite:
+        # in need an additional slash in linux for abs path
+        if platform_is_unix:
+            db_filepath = "/" + db_filepath
+
+        uri = f"sqlite://{db_filepath}?q=select 1 as value#/query1"
         with self.storage.data_open(data_path=uri, auto_load_uri=True) as file:
             data = file.read()
         data = DEFAULT_FROM_BYTES(data)
         self.assertEqual(data[0]["value"], 1)
 
         uri = f"{self.static_url}/test.db"
         with self.storage.data_open(data_path=uri, auto_load_uri=True) as file:
```

### Comparing `wingechr-datatools-0.2.0/tests/test_04_cache.py` & `wingechr-datatools-0.3.0/tests/test_04_cache.py`

 * *Files identical despite different names*

### Comparing `wingechr-datatools-0.2.0/tests/test_05_sql.py` & `wingechr-datatools-0.3.0/tests/test_05_sql.py`

 * *Files identical despite different names*

### Comparing `wingechr-datatools-0.2.0/wingechr_datatools.egg-info/SOURCES.txt` & `wingechr-datatools-0.3.0/wingechr_datatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

