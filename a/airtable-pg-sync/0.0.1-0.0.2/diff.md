# Comparing `tmp/airtable_pg_sync-0.0.1.tar.gz` & `tmp/airtable_pg_sync-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtable_pg_sync-0.0.1.tar", last modified: Tue Aug  1 00:56:04 2023, max compression
+gzip compressed data, was "airtable_pg_sync-0.0.2.tar", last modified: Tue Aug  1 01:17:11 2023, max compression
```

## Comparing `airtable_pg_sync-0.0.1.tar` & `airtable_pg_sync-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.557350 airtable_pg_sync-0.0.1/
--rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.1/LICENSE
--rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.1/MANIFEST.in
--rw-r--r--   0 benurwin   (501) staff       (20)     4774 2023-08-01 00:56:04.557227 airtable_pg_sync-0.0.1/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     3089 2023-08-01 00:43:11.000000 airtable_pg_sync-0.0.1/README.md
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.552224 airtable_pg_sync-0.0.1/airtable_pg_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2721 2023-08-01 00:39:26.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/cli.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.553530 airtable_pg_sync-0.0.1/airtable_pg_sync/core/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     4322 2023-08-01 00:08:07.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/change_handler.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.554312 airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     4159 2023-08-01 00:08:58.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/airtable.py
--rw-r--r--   0 benurwin   (501) staff       (20)     8578 2023-08-01 00:08:40.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/postgres.py
--rw-r--r--   0 benurwin   (501) staff       (20)     7169 2023-08-01 00:09:07.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/response_parser.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1661 2023-08-01 00:06:21.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/env.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.555322 airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      708 2023-08-01 00:06:57.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/bridges.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1858 2023-08-01 00:09:12.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/changes.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/concepts.py
--rw-r--r--   0 benurwin   (501) staff       (20)      822 2023-07-30 17:51:12.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/env_types.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.556590 airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      502 2023-08-01 00:07:15.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/initial_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     3515 2023-08-01 00:10:06.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/row_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2325 2023-08-01 00:07:51.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/schema_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2620 2023-08-01 00:09:47.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/table_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1031 2023-08-01 00:10:16.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/view_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/logging.conf
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.557049 airtable_pg_sync-0.0.1/airtable_pg_sync/perpetual_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/perpetual_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1139 2023-08-01 00:10:35.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1851 2023-08-01 00:10:44.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/perpetual_sync/webhook_listener.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1296 2023-08-01 00:05:42.000000 airtable_pg_sync-0.0.1/airtable_pg_sync/sync.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 00:56:04.553082 airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/
--rw-r--r--   0 benurwin   (501) staff       (20)     4774 2023-08-01 00:56:04.000000 airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-01 00:56:04.000000 airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/SOURCES.txt
--rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-01 00:56:04.000000 airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/dependency_links.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-01 00:56:04.000000 airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/entry_points.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-01 00:56:04.000000 airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/requires.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-01 00:56:04.000000 airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/top_level.txt
--rw-r--r--   0 benurwin   (501) staff       (20)      859 2023-08-01 00:39:05.000000 airtable_pg_sync-0.0.1/pyproject.toml
--rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-01 00:56:04.557388 airtable_pg_sync-0.0.1/setup.cfg
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.995915 airtable_pg_sync-0.0.2/
+-rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.2/LICENSE
+-rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.2/MANIFEST.in
+-rw-r--r--   0 benurwin   (501) staff       (20)     4774 2023-08-01 01:17:11.995799 airtable_pg_sync-0.0.2/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     3089 2023-08-01 00:43:11.000000 airtable_pg_sync-0.0.2/README.md
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.990644 airtable_pg_sync-0.0.2/airtable_pg_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2706 2023-08-01 01:15:52.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/cli.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.992004 airtable_pg_sync-0.0.2/airtable_pg_sync/core/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     4322 2023-08-01 00:08:07.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/change_handler.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.992940 airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     4159 2023-08-01 00:08:58.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/airtable.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     8578 2023-08-01 00:08:40.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/postgres.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     7169 2023-08-01 00:09:07.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/response_parser.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1661 2023-08-01 00:06:21.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/env.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.994030 airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      708 2023-08-01 00:06:57.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/bridges.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1858 2023-08-01 00:09:12.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/changes.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/concepts.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      822 2023-07-30 17:51:12.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/env_types.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.995230 airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      502 2023-08-01 00:07:15.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/initial_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     3515 2023-08-01 00:10:06.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/row_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2325 2023-08-01 00:07:51.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/schema_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2620 2023-08-01 00:09:47.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/table_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1031 2023-08-01 00:10:16.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/view_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/logging.conf
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.995623 airtable_pg_sync-0.0.2/airtable_pg_sync/perpetual_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/perpetual_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1139 2023-08-01 00:10:35.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1851 2023-08-01 00:10:44.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/perpetual_sync/webhook_listener.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1296 2023-08-01 00:05:42.000000 airtable_pg_sync-0.0.2/airtable_pg_sync/sync.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:17:11.991455 airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/
+-rw-r--r--   0 benurwin   (501) staff       (20)     4774 2023-08-01 01:17:11.000000 airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-01 01:17:11.000000 airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-01 01:17:11.000000 airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-01 01:17:11.000000 airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/entry_points.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-01 01:17:11.000000 airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/requires.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-01 01:17:11.000000 airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/top_level.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)      859 2023-08-01 01:17:02.000000 airtable_pg_sync-0.0.2/pyproject.toml
+-rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-01 01:17:11.995950 airtable_pg_sync-0.0.2/setup.cfg
```

### Comparing `airtable_pg_sync-0.0.1/LICENSE` & `airtable_pg_sync-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/PKG-INFO` & `airtable_pg_sync-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtable_pg_sync
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sync an Airtable base to a Postgres schema in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `airtable_pg_sync-0.0.1/README.md` & `airtable_pg_sync-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/cli.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                           f'{cmd[2]}',
                           f'\n  [italic]{cmd[1].__doc__.strip()} \n' if cmd[1].__doc__ else "\n"
                           )
         formatter.write(sio.getvalue())
 
 
 def setup_logging():
-    logging.config.fileConfig('airtable_pg_sync/logging.conf', disable_existing_loggers=False)
+    logging.config.fileConfig('./logging.conf', disable_existing_loggers=False)
     root_logger = logging.getLogger()
     root_logger.setLevel("INFO")
     root_logger.info(f'Logger created')
 
 
 @click.option('--config', required=True, type=str)
 def one_time_sync(config: str):
```

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/change_handler.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/change_handler.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/airtable.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/airtable.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/postgres.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/postgres.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/clients/response_parser.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/clients/response_parser.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/env.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/env.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/bridges.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/bridges.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/changes.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/changes.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/concepts.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/concepts.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/core/types/env_types.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/core/types/env_types.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/row_syncer.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/row_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/schema_syncer.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/schema_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/table_syncer.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/table_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/initial_sync/view_syncer.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/initial_sync/view_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/perpetual_sync/perpetual_syncer.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/perpetual_sync/perpetual_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/perpetual_sync/webhook_listener.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/perpetual_sync/webhook_listener.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync/sync.py` & `airtable_pg_sync-0.0.2/airtable_pg_sync/sync.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/PKG-INFO` & `airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtable-pg-sync
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sync an Airtable base to a Postgres schema in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `airtable_pg_sync-0.0.1/airtable_pg_sync.egg-info/SOURCES.txt` & `airtable_pg_sync-0.0.2/airtable_pg_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.1/pyproject.toml` & `airtable_pg_sync-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtable_pg_sync"
-version = "0.0.1"
+version = "0.0.2"
 description = "Sync an Airtable base to a Postgres schema in real time"
 readme = "README.md"
 authors = [{ name = "Benjamin Urwin", email = "benurwin@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

