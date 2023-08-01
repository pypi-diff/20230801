# Comparing `tmp/dsw-database-3.25.0.tar.gz` & `tmp/dsw-database-3.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-database-3.25.0.tar", last modified: Tue Jul  4 07:29:26 2023, max compression
+gzip compressed data, was "dsw-database-3.26.0.tar", last modified: Tue Aug  1 07:25:57 2023, max compression
```

## Comparing `dsw-database-3.25.0.tar` & `dsw-database-3.26.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.203403 dsw-database-3.25.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-04 07:29:20.000000 dsw-database-3.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 07:29:26.203403 dsw-database-3.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-04 07:29:20.000000 dsw-database-3.25.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.199403 dsw-database-3.25.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.203403 dsw-database-3.25.0/dsw/database/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 07:29:20.000000 dsw-database-3.25.0/dsw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 07:29:25.000000 dsw-database-3.25.0/dsw/database/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20894 2023-07-04 07:29:20.000000 dsw-database-3.25.0/dsw/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-04 07:29:20.000000 dsw-database-3.25.0/dsw/database/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.203403 dsw-database-3.25.0/dsw_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-04 07:29:20.000000 dsw-database-3.25.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:26.203403 dsw-database-3.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:20.000000 dsw-database-3.25.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:25:57.950982 dsw-database-3.26.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-08-01 07:25:52.000000 dsw-database-3.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-01 07:25:57.950982 dsw-database-3.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-01 07:25:52.000000 dsw-database-3.26.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:25:57.946982 dsw-database-3.26.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:25:57.946982 dsw-database-3.26.0/dsw/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 07:25:52.000000 dsw-database-3.26.0/dsw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 07:25:57.000000 dsw-database-3.26.0/dsw/database/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-08-01 07:25:52.000000 dsw-database-3.26.0/dsw/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-08-01 07:25:52.000000 dsw-database-3.26.0/dsw/database/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:25:57.950982 dsw-database-3.26.0/dsw_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-01 07:25:57.000000 dsw-database-3.26.0/dsw_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-01 07:25:57.000000 dsw-database-3.26.0/dsw_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:25:57.000000 dsw-database-3.26.0/dsw_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:25:57.000000 dsw-database-3.26.0/dsw_database.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 07:25:57.000000 dsw-database-3.26.0/dsw_database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 07:25:57.000000 dsw-database-3.26.0/dsw_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-01 07:25:52.000000 dsw-database-3.26.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 07:25:57.950982 dsw-database-3.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 07:25:52.000000 dsw-database-3.26.0/setup.py
```

### Comparing `dsw-database-3.25.0/LICENSE` & `dsw-database-3.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-database-3.25.0/PKG-INFO` & `dsw-database-3.26.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.25.0
+Version: 3.26.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
```

### Comparing `dsw-database-3.25.0/README.md` & `dsw-database-3.26.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-database-3.25.0/dsw/database/database.py` & `dsw-database-3.26.0/dsw/database/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,16 @@
                                'file_name = %s, content_type = %s, worker_log = %s, ' \
                                'file_size = %s WHERE uuid = %s;'
     SELECT_TEMPLATE = 'SELECT * FROM document_template WHERE id = %s AND app_uuid = %s LIMIT 1;'
     SELECT_TEMPLATE_FILES = 'SELECT * FROM document_template_file ' \
                             'WHERE document_template_id = %s AND app_uuid = %s;'
     SELECT_TEMPLATE_ASSETS = 'SELECT * FROM document_template_asset ' \
                              'WHERE document_template_id = %s AND app_uuid = %s;'
+    CHECK_TABLE_EXISTS = 'SELECT EXISTS(SELECT * FROM information_schema.tables' \
+                         '                       WHERE table_name = %(table_name)s)'
     SELECT_MAIL_CONFIG = 'SELECT icm.* ' \
                          'FROM app_config ac JOIN instance_config_mail icm ' \
                          'ON ac.mail_config_uuid = icm.uuid ' \
                          'WHERE ac.uuid = %(app_uuid)s;'
     UPDATE_COMPONENT_INFO = 'INSERT INTO component (name, version, built_at, created_at, updated_at) ' \
                             'VALUES (%(name)s, %(version)s, %(built_at)s, %(created_at)s, %(updated_at)s)' \
                             'ON CONFLICT (name) DO ' \
@@ -92,14 +94,32 @@
     @tenacity.retry(
         reraise=True,
         wait=tenacity.wait_exponential(multiplier=RETRY_QUERY_MULTIPLIER),
         stop=tenacity.stop_after_attempt(RETRY_QUERY_TRIES),
         before=tenacity.before_log(LOG, logging.DEBUG),
         after=tenacity.after_log(LOG, logging.DEBUG),
     )
+    def _check_table_exists(self, table_name: str) -> bool:
+        with self.conn_query.new_cursor() as cursor:
+            try:
+                cursor.execute(
+                    query=self.CHECK_TABLE_EXISTS,
+                    params={'table_name': table_name},
+                )
+                return cursor.fetchone()[0]
+            except Exception:
+                return False
+
+    @tenacity.retry(
+        reraise=True,
+        wait=tenacity.wait_exponential(multiplier=RETRY_QUERY_MULTIPLIER),
+        stop=tenacity.stop_after_attempt(RETRY_QUERY_TRIES),
+        before=tenacity.before_log(LOG, logging.DEBUG),
+        after=tenacity.after_log(LOG, logging.DEBUG),
+    )
     def fetch_document(self, document_uuid: str, app_uuid: str) -> Optional[DBDocument]:
         with self.conn_query.new_cursor(use_dict=True) as cursor:
             cursor.execute(
                 query=self.SELECT_DOCUMENT,
                 params=(document_uuid, app_uuid),
             )
             result = cursor.fetchall()
@@ -352,37 +372,41 @@
         wait=tenacity.wait_exponential(multiplier=RETRY_QUERY_MULTIPLIER),
         stop=tenacity.stop_after_attempt(RETRY_QUERY_TRIES),
         before=tenacity.before_log(LOG, logging.DEBUG),
         after=tenacity.after_log(LOG, logging.DEBUG),
     )
     def get_mail_config(self, app_uuid: str) -> Optional[DBInstanceConfigMail]:
         with self.conn_query.new_cursor(use_dict=True) as cursor:
+            if not self._check_table_exists(table_name='instance_config_mail'):
+                return None
             try:
                 cursor.execute(
                     query=self.SELECT_MAIL_CONFIG,
                     params={'app_uuid': app_uuid},
                 )
                 result = cursor.fetchone()
                 if result is None:
                     return None
                 return DBInstanceConfigMail.from_dict_row(data=result)
             except Exception as e:
-                LOG.warning(f'Could not retrieve instance_mail_config for app'
+                LOG.warning(f'Could not retrieve instance_config_mail for app'
                             f' "{app_uuid}": {str(e)}')
                 return None
 
     @tenacity.retry(
         reraise=True,
         wait=tenacity.wait_exponential(multiplier=RETRY_QUERY_MULTIPLIER),
         stop=tenacity.stop_after_attempt(RETRY_QUERY_TRIES),
         before=tenacity.before_log(LOG, logging.DEBUG),
         after=tenacity.after_log(LOG, logging.DEBUG),
     )
     def update_component_info(self, name: str, version: str, built_at: datetime.datetime):
         with self.conn_query.new_cursor(use_dict=True) as cursor:
+            if not self._check_table_exists(table_name='component'):
+                return None
             ts_now = datetime.datetime.utcnow()
             try:
                 cursor.execute(
                     query=self.UPDATE_COMPONENT_INFO,
                     params={
                         'name': name,
                         'version': version,
```

### Comparing `dsw-database-3.25.0/dsw/database/model.py` & `dsw-database-3.26.0/dsw/database/model.py`

 * *Files identical despite different names*

### Comparing `dsw-database-3.25.0/dsw_database.egg-info/PKG-INFO` & `dsw-database-3.26.0/dsw_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.25.0
+Version: 3.26.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
```

### Comparing `dsw-database-3.25.0/pyproject.toml` & `dsw-database-3.26.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-database'
-version = "3.25.0"
+version = "3.26.0"
 description = 'Library for managing DSW database'
 readme = 'README.md'
 keywords = ['dsw', 'database']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -22,15 +22,15 @@
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     'psycopg[binary]',
     'tenacity',
     # DSW
-    "dsw-config==3.25.0",
+    "dsw-config==3.26.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

