# Comparing `tmp/pypomes_db-0.1.9.tar.gz` & `tmp/pypomes_db-0.2.0.tar.gz`

## Comparing `pypomes_db-0.1.9.tar` & `pypomes_db-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    15349 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    15547 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/PKG-INFO
```

### Comparing `pypomes_db-0.1.9/src/pypomes_db/db_pomes.py` & `pypomes_db-0.2.0/src/pypomes_db/db_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 DB_DRIVER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER")
 DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME")
 DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST")
 DB_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_DB_PORT")
 DB_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_DB_PWD")
 DB_USER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_USER")
 
-__CONNECTION_KWARGS: Final[str] = f"DRIVER={{{DB_DRIVER}}};SERVER={DB_HOST},{DB_PORT};" \
-                                  f"DATABASE={DB_NAME};UID={DB_USER};PWD={DB_PWD};TrustServerCertificate=yes;"
+__CONNECTION_KWARGS: Final[str] = (
+    f"DRIVER={{{DB_DRIVER}}};SERVER={DB_HOST},{DB_PORT};"
+    f"DATABASE={DB_NAME};UID={DB_USER};PWD={DB_PWD};TrustServerCertificate=yes;"
+)
 
 
 def db_connect(errors: list[str]) -> Connection:
     """
-    Obtains and returns a connection to the database, or *None* if the connection cannot be obtained.
+    Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     :param errors: incidental error messages
     :return: the connection to the database
     """
     # inicializa a variável de retorno
     result: Connection | None = None
 
@@ -31,37 +33,42 @@
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_exists(errors: list[str], table: str, where_attrs: list[str], where_vals: tuple) -> bool:
     """
-    Determines whether the table *table* in the database contains at least one tuple where *where_attrs* equals
-    *where_values*, respectively. If more than one, the attributes are concatenated by the *AND* logical connector.
-    Returns *None* if there was an error in querying the database.
+    Determine whether the table *table* in the database contains at least one tuple.
+
+    For this determination, the where *where_attrs* are made equal to the
+    *where_values* in the query, respectively.
+    If more than one, the attributes are concatenated by the *AND* logical connector.
+    Return *None* if there was an error in querying the database.
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :return: True if at least one tuple was found
     """
-    sel_stmt: str = f"SELECT * FROM {table}"  # noqa
+    # noinspection PyDataSource
+    sel_stmt: str = "SELECT * FROM " + table
     if len(where_attrs) > 0:
         sel_stmt += " WHERE " + "".join(f"{attr} = ? AND " for attr in where_attrs)[0:-5]
     rec: tuple = db_select_one(errors, sel_stmt, where_vals)
     result: bool = None if len(errors) > 0 else rec is not None
 
     return result
 
 
 def db_select_one(errors: list[str], sel_stmt: str, where_vals: tuple,
                   require_nonempty: bool = False, require_singleton: bool = False) -> tuple:
     """
-    Searches the database and returns the first tuple that satisfies the *sel_stmt* search command.
+    Search the database and return the first tuple that satisfies the *sel_stmt* search command.
+
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. In case of error, or if the search is empty, *None* is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
@@ -104,15 +111,16 @@
 
     return result
 
 
 def db_select_all(errors: list[str], sel_stmt: str,  where_vals: tuple,
                   require_nonempty: bool = False, require_count: int = None) -> list[tuple]:
     """
-    Searches the database and returns all tuples that satisfy the *sel_stmt* search command.
+    Search the database and return all tuples that satisfy the *sel_stmt* search command.
+
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
@@ -154,57 +162,59 @@
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_insert(errors: list[str], insert_stmt: str, insert_vals: tuple) -> int:
     """
-    Inserts a tuple, with values defined in *insert_vals*, into the database.
+    Insert a tuple, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
     return __db_modify(errors, insert_stmt, insert_vals)
 
 
 def db_update(errors: list[str], update_stmt: str,
               update_vals: tuple, where_vals: tuple) -> int:
     """
-    Updates one or more tuples in the database, as defined by the command
-    *update_stmt*. The values for this update are in *update_vals*.
+    Update one or more tuples in the database, as defined by the command *update_stmt*.
+
+    The values for this update are in *update_vals*.
     The values for selecting the tuples to be updated are in *where_vals*.
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :return: the number of updated tuples, or None if an error occurred
     """
     values: tuple = update_vals + where_vals
     return __db_modify(errors, update_stmt, values)
 
 
 def db_delete(errors: list[str], delete_stmt: str, where_vals: tuple) -> int:
     """
-    Deletes one or more tuples in the database, as defined by the *delete_stmt* command.
+    Delete one or more tuples in the database, as defined by the *delete_stmt* command.
+
     The values for selecting the tuples to be deleted are in *where_vals*.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :return: the number of deleted tuples, or None if an error occurred
     """
     return __db_modify(errors, delete_stmt, where_vals)
 
 
 def db_bulk_insert(errors: list[str], insert_stmt: str, insert_vals: list[tuple]) -> int:
     """
-    Inserts the tuples, with values defined in *insert_vals*, into the database.
+    Insert the tuples, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
@@ -244,47 +254,50 @@
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
                 cursor.execute(stmt, proc_vals)
 
                 # has 'require_nonempty' been defined, and the search is empty ?
                 if require_nonempty and cursor.rowcount == 0:
                     # yes, report the error
                     errors.append(f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
-                                  f"for executing stored procedure '{proc_name}', with values '{proc_vals}'")
+                                  f"for stored procedure '{proc_name}', with values '{proc_vals}'")
 
                 # has 'require_count' been defined, and a different number of tuples was returned ?
                 elif isinstance(require_count, int) and require_count != cursor.rowcount:
                     # yes, report the error
                     errors.append(f"{cursor.rowcount} tuples returned, "
                                   f"but {require_count} expected, in '{DB_NAME}' at '{DB_HOST}', "
-                                  f"for executing stored procedure '{proc_name}', with values '{proc_vals}'")
+                                  f"for stored procedure '{proc_name}', with values '{proc_vals}'")
                 else:
                     # obtain the returned tuples
                     rows: list[Row] = cursor.fetchall()
                     for row in rows:
                         result.append(tuple(row))
+            conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def __db_modify(errors: list[str], modify_stmt: str, bind_vals: tuple) -> int:
     """
-    Modifies the database, inserting, updating or deleting tuples, according to the
-    *modify_stmt* command definitions. The values for this modification, followed by the
-    values for selecting tuples are in *bind_vals*.
+    Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
+
+    The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
 
     :param errors: incidental error messages
     :param modify_stmt: INSERT, UPDATE, or DELETE command
     :param bind_vals: values for database modification, and for tuples selection
     :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
     """
     # initialize the return variable
@@ -303,40 +316,41 @@
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def __db_msg_clean(msg: str) -> str:
     """
-    Clean the given *msg* string, by replacing double quotes with single quotes,
+    Clean the given *msg* string.
+
+    The cleaning is carriedc out by replacing double quotes with single quotes,
     and newlines and tabs with whitespace, and by removing backslashes.
 
     :param msg: the string to be cleaned
     :return: the cleaned string
     """
     return msg.replace('"', "'") \
               .replace("\n", " ") \
               .replace("\t", " ") \
               .replace("\\", "")
 
 
 def __db_except_msg(exception: Exception) -> str:
     """
-    Formats and returns the error message corresponding to the exception raised
-    while accessing the database.
+    Format and return the error message corresponding to the exception raised while accessing the database.
 
     :param exception: the exception raised
     :return:the formatted error message
     """
     return f"Error accessing {DB_NAME} at {DB_HOST}: {__db_msg_clean(f'{exception}')}"
 
 
 def __db_build_query_msg(sel_stmt: str, where_vals: tuple) -> str:
     """
-    Formats and returns the message indicative of an empty search.
+    Format and return the message indicative of an empty search.
 
     :param sel_stmt: the search command
     :param where_vals: values associated with the search criteria
     :return: message indicative of empty search
     """
     result: str = __db_msg_clean(sel_stmt)
```

### Comparing `pypomes_db-0.1.9/LICENSE` & `pypomes_db-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.9/pyproject.toml` & `pypomes_db-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "pip>=23.1.2",
+    "pip>=23.2.1",
     "psycopg2-binary>=2.9.6",
     "pyodbc>=4.0.39",
-    "pypomes_core>=0.1.4",
+    "pypomes_core>=0.2.1",
     "setuptools>=68.0.0",
-    "wheel>=0.40.0"
+    "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

