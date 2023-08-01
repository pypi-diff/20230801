# Comparing `tmp/tidy_tweet-1.0.0a4.tar.gz` & `tmp/tidy_tweet-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-1.0.0a4.tar", last modified: Mon Jul 24 05:04:22 2023, max compression
+gzip compressed data, was "tidy_tweet-1.0.0a5.tar", last modified: Tue Aug  1 07:12:34 2023, max compression
```

## Comparing `tidy_tweet-1.0.0a4.tar` & `tidy_tweet-1.0.0a5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.839943 tidy_tweet-1.0.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.843943 tidy_tweet-1.0.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.843943 tidy_tweet-1.0.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/docs/data_model.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/docs/data_model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/docs/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/generate_schema_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.839943 tidy_tweet-1.0.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.843943 tidy_tweet-1.0.0a4/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17895 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/test_overall.py
```

### Comparing `tidy_tweet-1.0.0a4/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0a5/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/.github/workflows/tests.yml` & `tidy_tweet-1.0.0a5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/LICENSE` & `tidy_tweet-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/PKG-INFO` & `tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tidy_tweet
-Version: 1.0.0a4
+Name: tidy-tweet
+Version: 1.0.0a5
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a4/README.md` & `tidy_tweet-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/contributing.md` & `tidy_tweet-1.0.0a5/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/docs/data_model.drawio` & `tidy_tweet-1.0.0a5/docs/data_model.drawio`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/docs/data_model.svg` & `tidy_tweet-1.0.0a5/docs/data_model.svg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/docs/schema.md` & `tidy_tweet-1.0.0a5/docs/schema.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/generate_schema_diagram.py` & `tidy_tweet-1.0.0a5/generate_schema_diagram.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/setup.cfg` & `tidy_tweet-1.0.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0a5/src/tidy_tweet/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0a5/src/tidy_tweet/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,53 +51,60 @@
         return msg
 
     def __str__(self):
         return "LibraryVersionMismatchWarning: " + self.message()
 
 
 def initialise_sqlite(
-    db_name: Union[str, PathLike], allow_existing_database: bool = False
+    db_name: Union[str, PathLike],
+    allow_existing_database: bool = False,
+    strict_mode: bool = True,
 ):
     """
     Creates and initialises an empty sqlite database for loading tweet data into.
 
     The database schema can be seen in the resulting sqlite .db file, or as a list
     of create table statements in `tidy_tweet.database_schema`
 
     :param db_name: File path to create a new database at. This is expected to not
     already exist.
     :param allow_existing_database: Only set this to True if you want to add the
     tidy_tweet tables to an existing database, such as one where you have other data
     pre-existing. This function expects the tidy_tweet tables to not already exist in
     the database. This behaviour, while possible, is not currently supported by
     tidy_tweet.
+    :param strict_mode: By default, tables are created in SQLite strict mode to help
+    catch parsing errors. For compatibility with some tools, you may need to disable
+    this.
     """
     db_name = Path(db_name)
 
     if not allow_existing_database:
         assert not db_name.exists()
 
+    create_table_statements = mapping.get_create_table_statements(strict_mode)
+
     with sqlite3.connect(db_name) as db:
         cursor = db.cursor()
-        for tbl_stmt in mapping.create_table_statements:
+        for tbl_stmt in create_table_statements:
             cursor.execute(tbl_stmt)
 
         # Initialise the schema related metadata first, otherwise if an
         # insert fails we end up with a schema version of null.
         # cursor.executemany(
         #     mapping.sql_by_table["_metadata"]["insert"],
         #     mapping.map_tidy_tweet_metadata()["_metadata"],
         # )
 
         if not allow_existing_database:
             # ".tables" only works in the sqlite shell!
             cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
             created_tables = cursor.fetchall()
             logger.debug("Created database tables: " + str(created_tables))
-            assert len(created_tables) == len(mapping.create_table_statements)
+            assert len(created_tables) == len(create_table_statements)
             cursor.execute("create table schema_version (schema_version text)")
             cursor.execute(
                 "insert into schema_version values (:version)",
                 {"version": mapping.SCHEMA_VERSION},
             )
 
         # Create views
```

### Comparing `tidy_tweet-1.0.0a4/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0a5/src/tidy_tweet/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,10 +117,11 @@
     def __init__(self, file_name: str, page_number: int, *args):
         self.file_name = file_name
         self.page_number = page_number
 
         super().__init__(*args)
 
     def __str__(self):
-        return "tidy_tweet encountered an error while parsing page " \
-               f"{self.page_number} of file {self.file_name}"
-
+        return (
+            "tidy_tweet encountered an error while parsing page "
+            f"{self.page_number} of file {self.file_name}"
+        )
```

### Comparing `tidy_tweet-1.0.0a4/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0a5/src/tidy_tweet/tweet_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,10 +619,13 @@
 # We have both create and assert statements for all tables
 for table_sql in sql_by_table.values():
     assert {"create", "insert"} <= table_sql.keys()
 
 
 # --- Convenience lists ---
 
-create_table_statements = [
-    clean_sql_statement(tbl["create"] + " strict") for tbl in sql_by_table.values()
-]
+
+def get_create_table_statements(strict_mode=True):
+    strict = " strict" if strict_mode else ""
+    return [
+        clean_sql_statement(tbl["create"] + strict) for tbl in sql_by_table.values()
+    ]
```

### Comparing `tidy_tweet-1.0.0a4/src/tidy_tweet/utilities.py` & `tidy_tweet-1.0.0a5/src/tidy_tweet/utilities.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tidy-tweet
-Version: 1.0.0a4
+Name: tidy_tweet
+Version: 1.0.0a5
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0a5/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/tests/test_cli.py` & `tidy_tweet-1.0.0a5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a4/tests/test_overall.py` & `tidy_tweet-1.0.0a5/tests/test_overall.py`

 * *Files identical despite different names*

