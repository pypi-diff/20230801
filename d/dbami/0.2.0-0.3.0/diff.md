# Comparing `tmp/dbami-0.2.0.tar.gz` & `tmp/dbami-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbami-0.2.0.tar", last modified: Thu Jun 22 20:30:24 2023, max compression
+gzip compressed data, was "dbami-0.3.0.tar", last modified: Tue Aug  1 18:29:46 2023, max compression
```

## Comparing `dbami-0.2.0.tar` & `dbami-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.898576 dbami-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-22 20:30:14.000000 dbami-0.2.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.890576 dbami-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.894576 dbami-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:30:14.000000 dbami-0.2.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-22 20:30:14.000000 dbami-0.2.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-22 20:30:14.000000 dbami-0.2.0/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-22 20:30:14.000000 dbami-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-22 20:30:14.000000 dbami-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-22 20:30:14.000000 dbami-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-22 20:30:14.000000 dbami-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 20:30:14.000000 dbami-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 20:30:24.898576 dbami-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 20:30:14.000000 dbami-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 20:30:14.000000 dbami-0.2.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-22 20:30:14.000000 dbami-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-22 20:30:14.000000 dbami-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:30:24.898576 dbami-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.890576 dbami-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.894576 dbami-0.2.0/src/dbami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/pg_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-22 20:30:14.000000 dbami-0.2.0/src/dbami/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.898576 dbami-0.2.0/src/dbami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 20:30:24.000000 dbami-0.2.0/src/dbami.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:30:24.898576 dbami-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_find_next_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_pg_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-22 20:30:14.000000 dbami-0.2.0/tests/test_sqlfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:46.652710 dbami-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 18:29:36.000000 dbami-0.3.0/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:46.648710 dbami-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:46.648710 dbami-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-01 18:29:36.000000 dbami-0.3.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-01 18:29:36.000000 dbami-0.3.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-01 18:29:36.000000 dbami-0.3.0/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-01 18:29:36.000000 dbami-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-01 18:29:36.000000 dbami-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 18:29:36.000000 dbami-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-01 18:29:36.000000 dbami-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-01 18:29:36.000000 dbami-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 18:29:46.652710 dbami-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 18:29:36.000000 dbami-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 18:29:36.000000 dbami-0.3.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-01 18:29:36.000000 dbami-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-01 18:29:36.000000 dbami-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:29:46.652710 dbami-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:46.648710 dbami-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:46.648710 dbami-0.3.0/src/dbami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/pg_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 18:29:36.000000 dbami-0.3.0/src/dbami/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:46.652710 dbami-0.3.0/src/dbami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 18:29:46.000000 dbami-0.3.0/src/dbami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-01 18:29:46.000000 dbami-0.3.0/src/dbami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:29:46.000000 dbami-0.3.0/src/dbami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 18:29:46.000000 dbami-0.3.0/src/dbami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-01 18:29:46.000000 dbami-0.3.0/src/dbami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 18:29:46.000000 dbami-0.3.0/src/dbami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:46.652710 dbami-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/test_find_next_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/test_pg_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 18:29:36.000000 dbami-0.3.0/tests/test_sqlfile.py
```

### Comparing `dbami-0.2.0/.github/workflows/python-publish.yaml` & `dbami-0.3.0/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/.github/workflows/python-test.yml` & `dbami-0.3.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/.github/workflows/snyk-scan.yml` & `dbami-0.3.0/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/.gitignore` & `dbami-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/.pre-commit-config.yaml` & `dbami-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/CHANGELOG.md` & `dbami-0.3.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.3.0] - 2023-08-01
+
+### Changed
+
+- Connection reuse support extracted into `get_db_connection`, now all
+  invocations of `get_db_connection` automatically support connection reuse.
+  ([#11])
+
 ## [v0.2.0] - 2023-06-22
 
 ### Added
 
 - `list-fixtures` command ([#10])
 - `load-fixture` command ([#10])
 - `DB.execute_sql()` method for running arbitrary SQL against a database ([#10])
@@ -21,12 +29,14 @@
 - Schema version when applying `schema.sql` comes from max migration version,
   removing the need to track the version table and update it in that file. ([#10])
 
 ## [v0.1.0] - 2023-05-25
 
 Initial release
 
-[unreleased]: https://github.com/element84/dbami/compare/v0.2.0...main
+[unreleased]: https://github.com/element84/dbami/compare/v0.3.0...main
+[v0.3.0]: https://github.com/element84/dbami/compare/v0.2.0...v0.3.0
 [v0.2.0]: https://github.com/element84/dbami/compare/v0.1.0...v0.2.0
 [v0.1.0]: https://github.com/element84/dbami/tree/v0.1.0
 
 [#10]: https://github.com/Element84/dbami/pull/10
+[#11]: https://github.com/Element84/dbami/pull/11
```

### Comparing `dbami-0.2.0/CONTRIBUTING.md` & `dbami-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/LICENSE` & `dbami-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/PKG-INFO` & `dbami-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbami
-Version: 0.2.0
+Version: 0.3.0
 Summary: Lightweight, Python-based, framework-agnostic async PostgreSQL migration tool
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,migration,async
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dbami-0.2.0/README.md` & `dbami-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/pyproject.toml` & `dbami-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/src/dbami/cli.py` & `dbami-0.3.0/src/dbami/cli.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/src/dbami/db.py` & `dbami-0.3.0/src/dbami/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import logging
 import sys
-from contextlib import AsyncExitStack, asynccontextmanager
+from contextlib import asynccontextmanager
 from pathlib import Path
 from typing import AsyncGenerator, Literal, Optional, TextIO, Union
 
 import asyncpg
 from buildpg import V, render
 
 from dbami import exceptions
@@ -275,31 +275,31 @@
         self.fixtures[name] = SqlFile(f)
 
     @staticmethod
     @asynccontextmanager
     async def get_db_connection(**kwargs):
         conn = None
         try:
-            conn = await asyncpg.connect(**kwargs)
-            yield conn
+            if kwargs.get("conn"):
+                yield kwargs["conn"]
+            else:
+                conn = await asyncpg.connect(**kwargs)
+                yield conn
         finally:
             if conn:
                 await conn.close()
 
     @classmethod
     async def execute_sql(cls, sql: str, *query_params, **kwargs) -> None:
         if not sql:
             # asyncpg chokes on an empty string,
             # so we bail out early on any non-truthy sql
             return
 
-        async with AsyncExitStack() as stack:
-            conn: asyncpg.Connection = kwargs.get(
-                "conn",
-            ) or await stack.enter_async_context(cls.get_db_connection(**kwargs))
+        async with cls.get_db_connection(**kwargs) as conn:
             await conn.execute(sql, *query_params)
 
     @classmethod
     async def create_database(cls, db_name: str, **kwargs) -> None:
         kwargs["database"] = ""
         await cls.execute_sql(f'CREATE DATABASE "{db_name}";', **kwargs)
 
@@ -312,19 +312,15 @@
     async def run_sqlfile(cls, sqlfile: SqlFile, **kwargs) -> None:
         await cls.execute_sql(sqlfile.path.read_text(), **kwargs)
 
     async def get_current_version(
         self,
         **kwargs,
     ) -> Optional[int]:
-        async with AsyncExitStack() as stack:
-            conn: asyncpg.Connection = kwargs.get(
-                "conn"
-            ) or await stack.enter_async_context(self.get_db_connection(**kwargs))
-
+        async with self.get_db_connection(**kwargs) as conn:
             query, _ = render(
                 """
                 SELECT
                     version
                 FROM :version_table
                 WHERE
                     applied_at = (SELECT max(applied_at) from :version_table)
@@ -347,25 +343,21 @@
         next_migration = find_next_migration(schema_version, self.migrations)
 
         while next_migration:
             yield next_migration
             next_migration = next_migration.child
 
     async def load_schema(self, **kwargs) -> None:
-        async with AsyncExitStack() as stack:
-            conn: asyncpg.Connection = kwargs.pop(
-                "conn",
-                None,
-            ) or await stack.enter_async_context(self.get_db_connection(**kwargs))
-            await stack.enter_async_context(conn.transaction())
-            await self.run_sqlfile(self.schema, conn=conn, **kwargs)
-            await self._update_schema_version(
-                max(self.migrations.keys()),
-                conn,
-            )
+        async with self.get_db_connection(**kwargs) as conn:
+            async with conn.transaction():
+                await self.run_sqlfile(self.schema, conn=conn)
+                await self._update_schema_version(
+                    max(self.migrations.keys()),
+                    conn,
+                )
 
     async def load_fixture(self, fixture_name: str, **kwargs):
         try:
             fixture = self.fixtures[fixture_name]
         except KeyError:
             raise FileNotFoundError(f"Unknown fixture: '{fixture_name}'")
```

### Comparing `dbami-0.2.0/src/dbami/pg_dump.py` & `dbami-0.3.0/src/dbami/pg_dump.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/src/dbami.egg-info/PKG-INFO` & `dbami-0.3.0/src/dbami.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbami
-Version: 0.2.0
+Version: 0.3.0
 Summary: Lightweight, Python-based, framework-agnostic async PostgreSQL migration tool
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,migration,async
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dbami-0.2.0/src/dbami.egg-info/SOURCES.txt` & `dbami-0.3.0/src/dbami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/tests/conftest.py` & `dbami-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/tests/test_cli.py` & `dbami-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/tests/test_db.py` & `dbami-0.3.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/tests/test_find_next_migration.py` & `dbami-0.3.0/tests/test_find_next_migration.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/tests/test_migration.py` & `dbami-0.3.0/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/tests/test_pg_dump.py` & `dbami-0.3.0/tests/test_pg_dump.py`

 * *Files identical despite different names*

### Comparing `dbami-0.2.0/tests/test_sqlfile.py` & `dbami-0.3.0/tests/test_sqlfile.py`

 * *Files identical despite different names*

