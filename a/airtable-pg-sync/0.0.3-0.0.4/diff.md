# Comparing `tmp/airtable_pg_sync-0.0.3.tar.gz` & `tmp/airtable_pg_sync-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtable_pg_sync-0.0.3.tar", last modified: Tue Aug  1 01:29:05 2023, max compression
+gzip compressed data, was "airtable_pg_sync-0.0.4.tar", last modified: Tue Aug  1 09:43:18 2023, max compression
```

## Comparing `airtable_pg_sync-0.0.3.tar` & `airtable_pg_sync-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.828820 airtable_pg_sync-0.0.3/
--rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.3/LICENSE
--rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.3/MANIFEST.in
--rw-r--r--   0 benurwin   (501) staff       (20)     4774 2023-08-01 01:29:05.828688 airtable_pg_sync-0.0.3/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     3089 2023-08-01 00:43:11.000000 airtable_pg_sync-0.0.3/README.md
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.823356 airtable_pg_sync-0.0.3/airtable_pg_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2770 2023-08-01 01:27:51.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/cli.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.824752 airtable_pg_sync-0.0.3/airtable_pg_sync/core/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     4322 2023-08-01 00:08:07.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/change_handler.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.825685 airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     4159 2023-08-01 00:08:58.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/airtable.py
--rw-r--r--   0 benurwin   (501) staff       (20)     8578 2023-08-01 00:08:40.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/postgres.py
--rw-r--r--   0 benurwin   (501) staff       (20)     7169 2023-08-01 00:09:07.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/response_parser.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1661 2023-08-01 00:06:21.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/env.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.826844 airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      708 2023-08-01 00:06:57.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/bridges.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1858 2023-08-01 00:09:12.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/changes.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/concepts.py
--rw-r--r--   0 benurwin   (501) staff       (20)      822 2023-07-30 17:51:12.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/env_types.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.827996 airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      502 2023-08-01 00:07:15.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/initial_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     3515 2023-08-01 00:10:06.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/row_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2325 2023-08-01 00:07:51.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/schema_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2620 2023-08-01 00:09:47.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/table_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1031 2023-08-01 00:10:16.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/view_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/logging.conf
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.828369 airtable_pg_sync-0.0.3/airtable_pg_sync/perpetual_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/perpetual_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1139 2023-08-01 00:10:35.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1851 2023-08-01 00:10:44.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/perpetual_sync/webhook_listener.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1296 2023-08-01 00:05:42.000000 airtable_pg_sync-0.0.3/airtable_pg_sync/sync.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 01:29:05.824170 airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/
--rw-r--r--   0 benurwin   (501) staff       (20)     4774 2023-08-01 01:29:05.000000 airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-01 01:29:05.000000 airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/SOURCES.txt
--rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-01 01:29:05.000000 airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/dependency_links.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-01 01:29:05.000000 airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/entry_points.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-01 01:29:05.000000 airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/requires.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-01 01:29:05.000000 airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/top_level.txt
--rw-r--r--   0 benurwin   (501) staff       (20)      859 2023-08-01 01:28:48.000000 airtable_pg_sync-0.0.3/pyproject.toml
--rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-01 01:29:05.828852 airtable_pg_sync-0.0.3/setup.cfg
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.670292 airtable_pg_sync-0.0.4/
+-rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.4/LICENSE
+-rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.4/MANIFEST.in
+-rw-r--r--   0 benurwin   (501) staff       (20)     5647 2023-08-01 09:43:18.670137 airtable_pg_sync-0.0.4/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     3962 2023-08-01 09:33:58.000000 airtable_pg_sync-0.0.4/README.md
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.664416 airtable_pg_sync-0.0.4/airtable_pg_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2770 2023-08-01 01:27:51.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/cli.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.665874 airtable_pg_sync-0.0.4/airtable_pg_sync/core/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     4322 2023-08-01 00:08:07.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/change_handler.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.666815 airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     4159 2023-08-01 00:08:58.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/airtable.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     8578 2023-08-01 00:08:40.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/postgres.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     7169 2023-08-01 00:09:07.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/response_parser.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1661 2023-08-01 00:06:21.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/env.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.667974 airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      708 2023-08-01 00:06:57.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/bridges.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1858 2023-08-01 00:09:12.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/changes.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/concepts.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      822 2023-07-30 17:51:12.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/env_types.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.669462 airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      502 2023-08-01 00:07:15.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/initial_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     3515 2023-08-01 00:10:06.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/row_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2325 2023-08-01 00:07:51.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/schema_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2620 2023-08-01 00:09:47.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/table_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1031 2023-08-01 00:10:16.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/view_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/logging.conf
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.669909 airtable_pg_sync-0.0.4/airtable_pg_sync/perpetual_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/perpetual_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1139 2023-08-01 00:10:35.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1851 2023-08-01 00:10:44.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/perpetual_sync/webhook_listener.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1296 2023-08-01 00:05:42.000000 airtable_pg_sync-0.0.4/airtable_pg_sync/sync.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-01 09:43:18.665371 airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/
+-rw-r--r--   0 benurwin   (501) staff       (20)     5647 2023-08-01 09:43:18.000000 airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-01 09:43:18.000000 airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-01 09:43:18.000000 airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-01 09:43:18.000000 airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/entry_points.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-01 09:43:18.000000 airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/requires.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-01 09:43:18.000000 airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/top_level.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)      859 2023-08-01 09:43:08.000000 airtable_pg_sync-0.0.4/pyproject.toml
+-rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-01 09:43:18.670325 airtable_pg_sync-0.0.4/setup.cfg
```

### Comparing `airtable_pg_sync-0.0.3/LICENSE` & `airtable_pg_sync-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/PKG-INFO` & `airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: airtable_pg_sync
-Version: 0.0.3
+Name: airtable-pg-sync
+Version: 0.0.4
 Summary: Sync an Airtable base to a Postgres schema in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -30,14 +30,22 @@
 - **One-off-sync**: This mode will replicate the Airtable base in the specified Postgres schema
   and then exit. This is useful for creating snapshots of the base for analysis or for storage as a backup.
 - **Perpetual sync**: This mode will replicate the Airtable base in the specified Postgres schema
   and then continue to watch for changes in the base. When a change is detected, the
   change will be applied to the Postgres schema. This is useful for creating a
   replica of the base that can be used for analysis in real time.
 
+
+This library will produce a Postgres table and view for each of the tables in the specified Airtable base.
+The table will take the Airtable table id for its name and the field ids for its column names. The view will have the 
+same name as the Airtable table and the column names will be the same as the Airtable column names.
+For most analysis use cases it makes sense to use the view as it is more readable, but for applications requiring 
+robustness with respect to column name changes the table should be used.
+
+
 ## Installation
 
 To install the library, run the following command:
 
 ```bash
 pip install airtable-postgres-sync
 ```
@@ -100,14 +108,22 @@
 
 ```python
 from airtable_pg_sync import Sync
 
 Sync(config_path="/path/to/config.yml", perpetual=True / False).run()
 ```
 
+
+## Testing and Deployment
+
+When testing this library for your use case the [ngrok](https://ngrok.com/) service is very useful. It allows you to listen 
+for requests sent over the internet to your PC (ie the webhook POST requests).
+
+For deployment it is recommended that you run the library in an AWS EC2 type service. A t2.micro instance should suffice.
+
 ## Bugs, Feature Requests, and Contributions
 
 If you find a bug or have a feature request, please open an issue
 on [GitHub](https://github.com/benurwin/airtable_pg_sync/issues).
 Any contributions are welcome and appreciated. If you would like to
 contribute, please open a pull request on [GitHub](https://github.com/benurwin/airtable_pg_sync/pulls).
```

### Comparing `airtable_pg_sync-0.0.3/README.md` & `airtable_pg_sync-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 - **One-off-sync**: This mode will replicate the Airtable base in the specified Postgres schema
   and then exit. This is useful for creating snapshots of the base for analysis or for storage as a backup.
 - **Perpetual sync**: This mode will replicate the Airtable base in the specified Postgres schema
   and then continue to watch for changes in the base. When a change is detected, the
   change will be applied to the Postgres schema. This is useful for creating a
   replica of the base that can be used for analysis in real time.
 
+
+This library will produce a Postgres table and view for each of the tables in the specified Airtable base.
+The table will take the Airtable table id for its name and the field ids for its column names. The view will have the 
+same name as the Airtable table and the column names will be the same as the Airtable column names.
+For most analysis use cases it makes sense to use the view as it is more readable, but for applications requiring 
+robustness with respect to column name changes the table should be used.
+
+
 ## Installation
 
 To install the library, run the following command:
 
 ```bash
 pip install airtable-postgres-sync
 ```
@@ -76,14 +84,22 @@
 
 ```python
 from airtable_pg_sync import Sync
 
 Sync(config_path="/path/to/config.yml", perpetual=True / False).run()
 ```
 
+
+## Testing and Deployment
+
+When testing this library for your use case the [ngrok](https://ngrok.com/) service is very useful. It allows you to listen 
+for requests sent over the internet to your PC (ie the webhook POST requests).
+
+For deployment it is recommended that you run the library in an AWS EC2 type service. A t2.micro instance should suffice.
+
 ## Bugs, Feature Requests, and Contributions
 
 If you find a bug or have a feature request, please open an issue
 on [GitHub](https://github.com/benurwin/airtable_pg_sync/issues).
 Any contributions are welcome and appreciated. If you would like to
 contribute, please open a pull request on [GitHub](https://github.com/benurwin/airtable_pg_sync/pulls).
```

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/cli.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/cli.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/change_handler.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/change_handler.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/airtable.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/airtable.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/postgres.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/postgres.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/clients/response_parser.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/clients/response_parser.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/env.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/env.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/bridges.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/bridges.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/changes.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/changes.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/concepts.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/concepts.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/core/types/env_types.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/core/types/env_types.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/row_syncer.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/row_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/schema_syncer.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/schema_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/table_syncer.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/table_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/initial_sync/view_syncer.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/initial_sync/view_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/perpetual_sync/perpetual_syncer.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/perpetual_sync/perpetual_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/perpetual_sync/webhook_listener.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/perpetual_sync/webhook_listener.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync/sync.py` & `airtable_pg_sync-0.0.4/airtable_pg_sync/sync.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/PKG-INFO` & `airtable_pg_sync-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: airtable-pg-sync
-Version: 0.0.3
+Name: airtable_pg_sync
+Version: 0.0.4
 Summary: Sync an Airtable base to a Postgres schema in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -30,14 +30,22 @@
 - **One-off-sync**: This mode will replicate the Airtable base in the specified Postgres schema
   and then exit. This is useful for creating snapshots of the base for analysis or for storage as a backup.
 - **Perpetual sync**: This mode will replicate the Airtable base in the specified Postgres schema
   and then continue to watch for changes in the base. When a change is detected, the
   change will be applied to the Postgres schema. This is useful for creating a
   replica of the base that can be used for analysis in real time.
 
+
+This library will produce a Postgres table and view for each of the tables in the specified Airtable base.
+The table will take the Airtable table id for its name and the field ids for its column names. The view will have the 
+same name as the Airtable table and the column names will be the same as the Airtable column names.
+For most analysis use cases it makes sense to use the view as it is more readable, but for applications requiring 
+robustness with respect to column name changes the table should be used.
+
+
 ## Installation
 
 To install the library, run the following command:
 
 ```bash
 pip install airtable-postgres-sync
 ```
@@ -100,14 +108,22 @@
 
 ```python
 from airtable_pg_sync import Sync
 
 Sync(config_path="/path/to/config.yml", perpetual=True / False).run()
 ```
 
+
+## Testing and Deployment
+
+When testing this library for your use case the [ngrok](https://ngrok.com/) service is very useful. It allows you to listen 
+for requests sent over the internet to your PC (ie the webhook POST requests).
+
+For deployment it is recommended that you run the library in an AWS EC2 type service. A t2.micro instance should suffice.
+
 ## Bugs, Feature Requests, and Contributions
 
 If you find a bug or have a feature request, please open an issue
 on [GitHub](https://github.com/benurwin/airtable_pg_sync/issues).
 Any contributions are welcome and appreciated. If you would like to
 contribute, please open a pull request on [GitHub](https://github.com/benurwin/airtable_pg_sync/pulls).
```

### Comparing `airtable_pg_sync-0.0.3/airtable_pg_sync.egg-info/SOURCES.txt` & `airtable_pg_sync-0.0.4/airtable_pg_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.3/pyproject.toml` & `airtable_pg_sync-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtable_pg_sync"
-version = "0.0.3"
+version = "0.0.4"
 description = "Sync an Airtable base to a Postgres schema in real time"
 readme = "README.md"
 authors = [{ name = "Benjamin Urwin", email = "benurwin@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

