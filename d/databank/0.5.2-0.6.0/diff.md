# Comparing `tmp/databank-0.5.2.tar.gz` & `tmp/databank-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databank-0.5.2.tar", max compression
+gzip compressed data, was "databank-0.6.0.tar", max compression
```

## Comparing `databank-0.5.2.tar` & `databank-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-20 07:06:09.012225 databank-0.5.2/LICENSE
--rw-r--r--   0        0        0     3490 2023-07-20 07:06:09.012225 databank-0.5.2/README.md
--rw-r--r--   0        0        0       78 2023-07-20 07:06:09.012225 databank-0.5.2/databank/__init__.py
--rw-r--r--   0        0        0     7487 2023-07-20 07:06:09.012225 databank-0.5.2/databank/core.py
--rw-r--r--   0        0        0     3497 2023-07-20 07:06:09.012225 databank-0.5.2/databank/query.py
--rw-r--r--   0        0        0     2180 2023-07-20 07:06:09.012225 databank-0.5.2/databank/utils.py
--rw-r--r--   0        0        0      513 2023-07-20 07:06:09.016225 databank-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 databank-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-01 09:34:46.751353 databank-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4788 2023-08-01 09:34:46.751353 databank-0.6.0/README.md
+-rw-r--r--   0        0        0       78 2023-08-01 09:34:46.751353 databank-0.6.0/databank/__init__.py
+-rw-r--r--   0        0        0     9480 2023-08-01 09:34:46.751353 databank-0.6.0/databank/core.py
+-rw-r--r--   0        0        0     3497 2023-08-01 09:34:46.751353 databank-0.6.0/databank/query.py
+-rw-r--r--   0        0        0     2180 2023-08-01 09:34:46.751353 databank-0.6.0/databank/utils.py
+-rw-r--r--   0        0        0      513 2023-08-01 09:34:46.751353 databank-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5269 1970-01-01 00:00:00.000000 databank-0.6.0/PKG-INFO
```

### Comparing `databank-0.5.2/LICENSE` & `databank-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databank-0.5.2/README.md` & `databank-0.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -82,26 +82,40 @@
 
 ```python
 >>> from databank.utils import serialize_params
 >>> serialize_params({"member": "Ringo", "song": ["Don't Pass Me By", "Octopus's Garden"]})
 {'member': 'Ringo', 'song': '["Don\'t Pass Me By", "Octopus\'s Garden"]'}
 ```
 
+### Executing Queries in the Background
+
+For both `execute()` and `execute_many()` you can pass an `in_background` keyword argument (which is by default `False`). If set to `True`, the query will be executed in the background in another thread and the method will return immediately the `Thread` object (i.e. non-blocking). You can call `join()` on that object to wait for the query to finish or just do nothing and go on:
+
+```python
+>>> db.execute("INSERT INTO beatles (id, member) VALUES (:id, :member);", {"id": 4, "member": "Klaus"}, in_background=True)
+<Thread(Thread-1 (_execute), started 140067398776512)>
+```
+
+Beware that if you are using `in_background=True`, you have to make sure that the connection pool size is large enough to handle the number of concurrent queries and that your program is running long enough if you are not explicitly waiting for the thread to finish. Also note that this might lead to a range of other issues like locking, reduced performance or even deadlocks. You also might want to set an explicit timeout for queries by passing e.g. `{"options": "-c statement_timeout=60000"}` for PostgreSQL when initializing the `Database` object to kill all queries taking longer than 60 seconds.
+
+
 ## Query Collection
 
 You can also organize SQL queries in an SQL file and load them into a `QueryCollection`:
 
 ```sql
 /* @name insert_data */
 INSERT INTO beatles (id, member) VALUES (:id, :member);
 
 /* @name select_all_data */
 SELECT * FROM beatles;
 ```
 
+> This idea is borrowed from [PgTyped](https://pgtyped.dev/docs/sql-file)
+
 A query _must_ have a header comment with the name of the query. If a query name is not unique, the last query with the same name will be used. You can parse that file and load the queries into a `QueryCollection`:
 
 ```python
 >>> from databank import QueryCollection
 >>> queries = QueryCollection.from_file("queries.sql")
 ```
```

### Comparing `databank-0.5.2/databank/core.py` & `databank-0.6.0/databank/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from threading import Thread
 from typing import Iterable, Mapping
 
 from sqlalchemy import create_engine, text
 from sqlalchemy.engine import Engine, ResultProxy
 from sqlalchemy.engine.row import RowProxy
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.sql.elements import TextClause
@@ -15,15 +16,46 @@
         ----------
         url : str
             URL of the database to connect to.
         """
         self.engine: Engine = create_engine(url, **kwargs)
         self.session: scoped_session = scoped_session(sessionmaker(bind=self.engine))
 
-    def execute(self, query: str, params: Mapping = {}):
+    def execute(
+        self,
+        query: str,
+        params: Mapping = {},
+        *,
+        in_background: bool = False,
+    ) -> Thread | None:
+        """Execute and commit the given SQL query, optionally bind the params first.
+
+        Parameters
+        ----------
+        query : str
+            SQL query to execute.
+        params : Mapping
+            Parameters to bind to the query.
+        in_background : bool
+            If True, execute the query in the background, by default False.
+
+        Returns
+        -------
+        Thread | None
+            If `in_background` is True, returns the `Thread` object, otherwise nothing.
+        """
+        if in_background:
+            # run query in background thread and return thread object
+            thread = Thread(target=self._execute, args=(query, params))
+            thread.start()
+            return thread
+        else:
+            self._execute(query, params)
+
+    def _execute(self, query: str, params: Mapping = {}):
         """Execute and commit the given SQL query, optionally bind the params first.
 
         Parameters
         ----------
         query : str
             SQL query to execute.
         params : Mapping
@@ -41,15 +73,46 @@
             self.session.rollback()
             self.session.remove()
             raise
         else:
             self.session.commit()
             self.session.remove()
 
-    def execute_many(self, query: str, params: Iterable[Mapping] = []):
+    def execute_many(
+        self,
+        query: str,
+        params: Iterable[Mapping] = [],
+        *,
+        in_background: bool = False,
+    ) -> Thread | None:
+        """Execute and commit multiple SQL queries, optionally bind the iterable of params first.
+
+        Parameters
+        ----------
+        query : str
+            SQL query to execute.
+        params : Iterable[Mapping]
+            Iterable of params to bind to the query.
+        in_background : bool
+            If True, execute the query in the background, by default False.
+
+        Returns
+        -------
+        Thread | None
+            If `in_background` is True, returns the `Thread` object, otherwise nothing.
+        """
+        if in_background:
+            # run query in background thread and return thread object
+            thread = Thread(target=self._execute_many, args=(query, params))
+            thread.start()
+            return thread
+        else:
+            self._execute_many(query, params)
+
+    def _execute_many(self, query: str, params: Iterable[Mapping] = []):
         """Execute and commit multiple SQL queries, optionally bind the iterable of params first.
 
         Parameters
         ----------
         query : str
             SQL query to execute.
         params : Iterable[Mapping]
@@ -185,16 +248,21 @@
             raise
         else:
             self.session.commit()
             self.session.remove()
 
         return row._asdict() if row else {}
 
-    def execute_fetch_many(self, query: str, params: Iterable[Mapping] = [], n: int = 1) -> list[dict]:
-        """Execute multiple SQL queries, optionally bind params, fetch first `n` results of last query.
+    def execute_fetch_many(
+        self,
+        query: str,
+        params: Iterable[Mapping] = [],
+        n: int = 1,
+    ) -> list[dict]:
+        """Execute SQL queries, optionally bind params, fetch first `n` results of last query.
 
         Parameters
         ----------
         query : str
             SQL query to execute.
         params : Iterable[Mapping]
             Iterable of params to bind to the query.
```

### Comparing `databank-0.5.2/databank/query.py` & `databank-0.6.0/databank/query.py`

 * *Files identical despite different names*

### Comparing `databank-0.5.2/databank/utils.py` & `databank-0.6.0/databank/utils.py`

 * *Files identical despite different names*

### Comparing `databank-0.5.2/pyproject.toml` & `databank-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databank"
-version = "0.5.2"
+version = "0.6.0"
 description = "Databank is an easy-to-use Python library for making raw SQL queries in a multi-threaded environment."
 readme = "README.md"
 authors = ["snapADDY GmbH <info@snapaddy.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sqlalchemy = "^2.0.4"
```

### Comparing `databank-0.5.2/PKG-INFO` & `databank-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databank
-Version: 0.5.2
+Version: 0.6.0
 Summary: Databank is an easy-to-use Python library for making raw SQL queries in a multi-threaded environment.
 Author: snapADDY GmbH
 Author-email: info@snapaddy.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -95,26 +95,40 @@
 
 ```python
 >>> from databank.utils import serialize_params
 >>> serialize_params({"member": "Ringo", "song": ["Don't Pass Me By", "Octopus's Garden"]})
 {'member': 'Ringo', 'song': '["Don\'t Pass Me By", "Octopus\'s Garden"]'}
 ```
 
+### Executing Queries in the Background
+
+For both `execute()` and `execute_many()` you can pass an `in_background` keyword argument (which is by default `False`). If set to `True`, the query will be executed in the background in another thread and the method will return immediately the `Thread` object (i.e. non-blocking). You can call `join()` on that object to wait for the query to finish or just do nothing and go on:
+
+```python
+>>> db.execute("INSERT INTO beatles (id, member) VALUES (:id, :member);", {"id": 4, "member": "Klaus"}, in_background=True)
+<Thread(Thread-1 (_execute), started 140067398776512)>
+```
+
+Beware that if you are using `in_background=True`, you have to make sure that the connection pool size is large enough to handle the number of concurrent queries and that your program is running long enough if you are not explicitly waiting for the thread to finish. Also note that this might lead to a range of other issues like locking, reduced performance or even deadlocks. You also might want to set an explicit timeout for queries by passing e.g. `{"options": "-c statement_timeout=60000"}` for PostgreSQL when initializing the `Database` object to kill all queries taking longer than 60 seconds.
+
+
 ## Query Collection
 
 You can also organize SQL queries in an SQL file and load them into a `QueryCollection`:
 
 ```sql
 /* @name insert_data */
 INSERT INTO beatles (id, member) VALUES (:id, :member);
 
 /* @name select_all_data */
 SELECT * FROM beatles;
 ```
 
+> This idea is borrowed from [PgTyped](https://pgtyped.dev/docs/sql-file)
+
 A query _must_ have a header comment with the name of the query. If a query name is not unique, the last query with the same name will be used. You can parse that file and load the queries into a `QueryCollection`:
 
 ```python
 >>> from databank import QueryCollection
 >>> queries = QueryCollection.from_file("queries.sql")
 ```
```

