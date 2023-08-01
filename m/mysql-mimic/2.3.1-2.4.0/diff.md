# Comparing `tmp/mysql-mimic-2.3.1.tar.gz` & `tmp/mysql-mimic-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.3.1.tar", last modified: Fri Jul 28 20:45:53 2023, max compression
+gzip compressed data, was "mysql-mimic-2.4.0.tar", last modified: Tue Aug  1 19:35:54 2023, max compression
```

## Comparing `mysql-mimic-2.3.1.tar` & `mysql-mimic-2.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    19029 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    29117 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:35:54.948172 mysql-mimic-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-08-01 19:35:54.948172 mysql-mimic-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:35:54.944172 mysql-mimic-2.4.0/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22740 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19029 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:35:54.944172 mysql-mimic-2.4.0/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-08-01 19:35:54.000000 mysql-mimic-2.4.0/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-01 19:35:54.000000 mysql-mimic-2.4.0/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:35:54.000000 mysql-mimic-2.4.0/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-01 19:35:54.000000 mysql-mimic-2.4.0/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 19:35:54.000000 mysql-mimic-2.4.0/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:35:54.948172 mysql-mimic-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:35:54.948172 mysql-mimic-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 19:35:22.000000 mysql-mimic-2.4.0/tests/test_version.py
```

### Comparing `mysql-mimic-2.3.1/LICENSE` & `mysql-mimic-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/PKG-INFO` & `mysql-mimic-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.3.1
+Version: 2.4.0
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.3.1/README.md` & `mysql-mimic-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/auth.py` & `mysql-mimic-2.4.0/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/charset.py` & `mysql-mimic-2.4.0/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/connection.py` & `mysql-mimic-2.4.0/mysql_mimic/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from ssl import SSLContext
-from typing import Optional, Dict, Any, Iterator
+from typing import Optional, Dict, Any, Iterator, AsyncIterator
 
 from mysql_mimic.auth import (
     AuthInfo,
     Forbidden,
     Success,
     AuthPlugin,
     AuthState,
@@ -22,15 +22,15 @@
 from mysql_mimic.prepared import PreparedStatement, REGEX_PARAM
 from mysql_mimic.results import ensure_result_set, ResultSet
 from mysql_mimic import types, packets, context
 from mysql_mimic.schema import com_field_list_to_show_statement
 from mysql_mimic.session import BaseSession
 from mysql_mimic.stream import MysqlStream, ConnectionClosed
 from mysql_mimic.types import Capabilities
-from mysql_mimic.utils import seq
+from mysql_mimic.utils import seq, aiterate
 
 logger = logging.getLogger(__name__)
 
 
 class Connection:
     _MAX_PREPARED_STMT_ID = 2**32
 
@@ -348,22 +348,24 @@
         await self.stream.write(self.ok())
 
     async def handle_field_list(self, data: bytes) -> None:
         com_field_list = parse_com_field_list(self.client_charset, data)
         sql = com_field_list_to_show_statement(com_field_list)
         result = await self.query(sql=sql, query_attrs={})
         columns = b"".join(
-            make_column_definition_41(
-                server_charset=self.server_charset,
-                table=com_field_list.table,
-                name=row[0],
-                is_com_field_list=True,
-                default=row[4],
-            )
-            for row in result.rows
+            [
+                make_column_definition_41(
+                    server_charset=self.server_charset,
+                    table=com_field_list.table,
+                    name=row[0],
+                    is_com_field_list=True,
+                    default=row[4],
+                )
+                async for row in aiterate(result.rows)
+            ]
         )
         await self.stream.write(columns)
         await self.stream.write(self.ok_or_eof())
 
     async def handle_query(self, data: bytes) -> None:
         """
         https://dev.mysql.com/doc/internals/en/com-query.html
@@ -379,15 +381,15 @@
 
         result_set = await self.query(com_query.sql, com_query.query_attrs)
 
         if not result_set:
             await self.stream.write(self.ok())
             return
 
-        for packet in self.text_resultset(result_set):
+        async for packet in self.text_resultset(result_set):
             await self.stream.write(packet)
 
     async def handle_stmt_prepare(self, data: bytes) -> None:
         """
         https://dev.mysql.com/doc/internals/en/com-stmt-prepare.html
 
         COM_STMT_PREPARE creates a prepared statement from the passed query string.
@@ -453,43 +455,47 @@
                     server_charset=self.server_charset,
                     name=column.name,
                     column_type=column.type,
                     character_set=column.character_set,
                 )
             )
 
-        rows = (
-            packets.make_binary_resultrow(r, result_set.columns)
-            for r in result_set.rows
-        )
+        async def gen_rows() -> AsyncIterator[bytes]:
+            async for r in aiterate(result_set.rows):
+                yield packets.make_binary_resultrow(r, result_set.columns)
+
+        rows = gen_rows()
 
         if com_stmt_execute.use_cursor:
             com_stmt_execute.stmt.cursor = rows
             await self.stream.write(
                 self.ok_or_eof(flags=types.ServerStatus.SERVER_STATUS_CURSOR_EXISTS)
             )
         else:
             if not self.deprecate_eof():
                 await self.stream.write(self.eof())
-            for row in rows:
+            async for row in rows:
                 await self.stream.write(row)
             await self.stream.write(self.ok_or_eof())
 
     async def handle_stmt_fetch(self, data: bytes) -> None:
         """
         https://dev.mysql.com/doc/internals/en/com-stmt-fetch.html
 
         COM_STMT_FETCH fetches rows from an existing resultset after a COM_STMT_EXECUTE.
         """
         com_stmt_fetch = packets.parse_handle_stmt_fetch(data)
 
         stmt = self.get_stmt(com_stmt_fetch.stmt_id)
         assert stmt.cursor is not None
         count = 0
-        for _, packet in zip(range(com_stmt_fetch.num_rows), stmt.cursor):
+
+        async for packet in stmt.cursor:
+            if count >= com_stmt_fetch.num_rows:
+                break
             await self.stream.write(packet)
             count += 1
 
         done = count < com_stmt_fetch.num_rows
 
         await self.stream.write(
             self.ok_or_eof(
@@ -526,15 +532,15 @@
         if stmt_id in self.prepared_stmts:
             return self.prepared_stmts[stmt_id]
         raise MysqlError(f"Unknown statement: {stmt_id}", ErrorCode.UNKNOWN_PROCEDURE)
 
     async def query(self, sql: str, query_attrs: Dict[str, str]) -> ResultSet:
         logger.debug("Received query: %s", sql)
 
-        result_set = ensure_result_set(
+        result_set = await ensure_result_set(
             await self.session.handle_query(sql, query_attrs)
         )
         return result_set
 
     def ok(self, **kwargs: Any) -> bytes:
         return packets.make_ok(
             capabilities=self.capabilities,
@@ -570,15 +576,15 @@
         return packets.make_error(
             capabilities=self.capabilities, server_charset=self.server_charset, **kwargs
         )
 
     def deprecate_eof(self) -> bool:
         return Capabilities.CLIENT_DEPRECATE_EOF in self.capabilities
 
-    def text_resultset(self, result_set: ResultSet) -> Iterator[bytes]:
+    async def text_resultset(self, result_set: ResultSet) -> AsyncIterator[bytes]:
         yield packets.make_column_count(
             capabilities=self.capabilities, column_count=len(result_set.columns)
         )
 
         for column in result_set.columns:
             yield packets.make_column_definition_41(
                 server_charset=self.server_charset,
@@ -588,15 +594,15 @@
             )
 
         if not self.deprecate_eof():
             yield self.eof()
 
         affected_rows = 0
 
-        for row in result_set.rows:
+        async for row in aiterate(result_set.rows):
             affected_rows += 1
             yield packets.make_text_resultset_row(row, result_set.columns)
 
         yield self.ok_or_eof(affected_rows=affected_rows)
 
     def com_stmt_prepare_response(
         self, statement: PreparedStatement
```

### Comparing `mysql-mimic-2.3.1/mysql_mimic/constants.py` & `mysql-mimic-2.4.0/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/errors.py` & `mysql-mimic-2.4.0/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/intercept.py` & `mysql-mimic-2.4.0/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/packets.py` & `mysql-mimic-2.4.0/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/results.py` & `mysql-mimic-2.4.0/mysql_mimic/results.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from __future__ import annotations
 
 import io
 import struct
 from dataclasses import dataclass
 from datetime import datetime, date, timedelta
-from typing import Iterable, Sequence, Optional, Callable, Any, Union, Tuple, Dict
+from typing import (
+    Iterable,
+    Sequence,
+    Optional,
+    Callable,
+    Any,
+    Union,
+    Tuple,
+    Dict,
+    AsyncIterable,
+    cast,
+)
 
 from mysql_mimic.errors import MysqlError
 from mysql_mimic.types import ColumnType, str_len, uint_1, uint_2, uint_4
 from mysql_mimic.charset import CharacterSet
-
+from mysql_mimic.utils import aiterate
 
 Encoder = Callable[[Any, "ResultColumn"], bytes]
 
 
 class ResultColumn:
     """
     Column data for a result set
@@ -50,73 +61,111 @@
 
     def __repr__(self) -> str:
         return f"ResultColumn({self.name} {self.type.name})"
 
 
 @dataclass
 class ResultSet:
-    rows: Iterable[Sequence]
+    rows: Iterable[Sequence] | AsyncIterable[Sequence]
     columns: Sequence[ResultColumn]
 
     def __bool__(self) -> bool:
         return bool(self.columns)
 
 
 AllowedColumn = Union[ResultColumn, str]
 AllowedResult = Union[
-    ResultSet, Tuple[Sequence[Sequence[Any]], Sequence[AllowedColumn]], None
+    ResultSet,
+    Tuple[Sequence[Sequence[Any]], Sequence[AllowedColumn]],
+    Tuple[AsyncIterable[Sequence[Any]], Sequence[AllowedColumn]],
+    None,
 ]
 
 
-def ensure_result_set(result: AllowedResult) -> ResultSet:
+async def ensure_result_set(result: AllowedResult) -> ResultSet:
     if result is None:
         return ResultSet([], [])
     if isinstance(result, ResultSet):
         return result
     if isinstance(result, tuple):
         if len(result) != 2:
             raise MysqlError(
                 f"Result tuple should be of size 2. Received: {len(result)}"
             )
         rows = result[0]
         columns = result[1]
 
+        return await _ensure_result_cols(rows, columns)
+
+    raise MysqlError(f"Unexpected result set type: {type(result)}")
+
+
+async def _ensure_result_cols(
+    rows: Sequence[Sequence[Any]] | AsyncIterable[Sequence[Any]],
+    columns: Sequence[AllowedColumn],
+) -> ResultSet:
+    # Which columns need to be inferred?
+    remaining = {
+        col: i for i, col in enumerate(columns) if not isinstance(col, ResultColumn)
+    }
+
+    if not remaining:
         return ResultSet(
             rows=rows,
-            columns=[_ensure_result_col(col, i, rows) for i, col in enumerate(columns)],
+            columns=cast(Sequence[ResultColumn], columns),
         )
 
-    raise MysqlError(f"Unexpected result set type: {type(result)}")
+    # Copy the columns
+    columns = list(columns)
+
+    arows = aiterate(rows)
 
+    # Keep track of rows we've consumed from the iterator so we can add them back
+    peeks = []
 
-def _ensure_result_col(
-    column: AllowedColumn, idx: int, rows: Sequence[Sequence[Any]]
-) -> ResultColumn:
-    if isinstance(column, ResultColumn):
-        return column
-
-    if isinstance(column, str):
-        value = _find_first_non_null_value(idx, rows)
-        type_ = infer_type(value)
-        return ResultColumn(
-            name=column,
-            type=type_,
+    # Find the first non-null value for each column
+    while remaining:
+        try:
+            peek = await arows.__anext__()
+        except StopAsyncIteration:
+            break
+
+        peeks.append(peek)
+
+        inferred = []
+        for name, i in remaining.items():
+            value = peek[i]
+            if value is not None:
+                type_ = infer_type(value)
+                columns[i] = ResultColumn(
+                    name=str(name),
+                    type=type_,
+                )
+                inferred.append(name)
+
+        for name in inferred:
+            remaining.pop(name)
+
+    # If we failed to find a non-null value, set the type to NULL
+    for name, i in remaining.items():
+        columns[i] = ResultColumn(
+            name=str(name),
+            type=ColumnType.NULL,
         )
 
-    raise MysqlError(f"Unexpected result column value: {column}")
+    # Add the consumed rows back in to the iterator
+    async def gen_rows() -> AsyncIterable[Sequence[Any]]:
+        for row in peeks:
+            yield row
 
+        async for row in arows:
+            yield row
 
-def _find_first_non_null_value(
-    idx: int, rows: Sequence[Sequence[Any]]
-) -> Optional[Any]:
-    for row in rows:
-        value = row[idx]
-        if value is not None:
-            return value
-    return None
+    assert all(isinstance(col, ResultColumn) for col in columns)
+    return ResultSet(rows=gen_rows(), columns=cast(Sequence[ResultColumn], columns))
 
 
 def _binary_encode_tiny(col: ResultColumn, val: Any) -> bytes:
     return uint_1(int(bool(val)))
 
 
 def _binary_encode_str(col: ResultColumn, val: Any) -> bytes:
```

### Comparing `mysql-mimic-2.3.1/mysql_mimic/schema.py` & `mysql-mimic-2.4.0/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/server.py` & `mysql-mimic-2.4.0/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/session.py` & `mysql-mimic-2.4.0/mysql_mimic/session.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/stream.py` & `mysql-mimic-2.4.0/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/types.py` & `mysql-mimic-2.4.0/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic/variables.py` & `mysql-mimic-2.4.0/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.4.0/mysql_mimic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.3.1
+Version: 2.4.0
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.3.1/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.4.0/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/setup.py` & `mysql-mimic-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/tests/test_auth.py` & `mysql-mimic-2.4.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/tests/test_query.py` & `mysql-mimic-2.4.0/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import io
 from contextlib import closing
 from datetime import date, datetime, timedelta
 from typing import Any, Callable, Awaitable, Sequence, Dict, List, Tuple, Type
 
 import pytest
 import pytest_asyncio
@@ -831,7 +832,30 @@
     query_fixture: QueryFixture,
     sql: str,
     msg: str,
 ) -> None:
     with pytest.raises(Exception) as ctx:
         await query_fixture(sql)
     assert msg in str(ctx.value)
+
+
+@pytest.mark.asyncio
+async def test_async_iterator(
+    session: MockSession,
+    server: MysqlServer,
+    query_fixture: QueryFixture,
+) -> None:
+    async def generate_rows() -> Any:
+        yield 1, None, None
+        await asyncio.sleep(0)
+        yield None, "2", None
+        await asyncio.sleep(0)
+        yield None, None, None
+
+    session.return_value = (generate_rows(), ["a", "b", "c"])
+
+    result = await query_fixture("SELECT * FROM x")
+    assert [
+        {"a": 1, "b": None, "c": None},
+        {"a": None, "b": "2", "c": None},
+        {"a": None, "b": None, "c": None},
+    ] == result
```

### Comparing `mysql-mimic-2.3.1/tests/test_ssl.py` & `mysql-mimic-2.4.0/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/tests/test_stream.py` & `mysql-mimic-2.4.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/tests/test_types.py` & `mysql-mimic-2.4.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.1/tests/test_variables.py` & `mysql-mimic-2.4.0/tests/test_variables.py`

 * *Files identical despite different names*

