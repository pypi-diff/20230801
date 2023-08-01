# Comparing `tmp/tradehelper-1.43.tar.gz` & `tmp/tradehelper-1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradehelper-1.43.tar", last modified: Tue Aug  1 13:23:15 2023, max compression
+gzip compressed data, was "tradehelper-1.44.tar", last modified: Tue Aug  1 13:27:47 2023, max compression
```

## Comparing `tradehelper-1.43.tar` & `tradehelper-1.44.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-08-01 13:23:15.649679 tradehelper-1.43/
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      196 2023-08-01 13:23:15.645678 tradehelper-1.43/PKG-INFO
--rw-rw-r--   0 aarav     (1000) aarav     (1000)       38 2023-08-01 13:23:15.649679 tradehelper-1.43/setup.cfg
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      366 2023-08-01 13:22:49.000000 tradehelper-1.43/setup.py
-drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-08-01 13:23:15.645678 tradehelper-1.43/tradehelper/
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      149 2022-06-02 06:39:05.000000 tradehelper-1.43/tradehelper/__init__.py
--rw-rw-r--   0 aarav     (1000) aarav     (1000)    19321 2023-07-28 02:04:28.000000 tradehelper-1.43/tradehelper/tradehelp.py
-drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-08-01 13:23:15.645678 tradehelper-1.43/tradehelper.egg-info/
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      196 2023-08-01 13:23:15.000000 tradehelper-1.43/tradehelper.egg-info/PKG-INFO
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      231 2023-08-01 13:23:15.000000 tradehelper-1.43/tradehelper.egg-info/SOURCES.txt
--rw-rw-r--   0 aarav     (1000) aarav     (1000)        1 2023-08-01 13:23:15.000000 tradehelper-1.43/tradehelper.egg-info/dependency_links.txt
--rw-rw-r--   0 aarav     (1000) aarav     (1000)       31 2023-08-01 13:23:15.000000 tradehelper-1.43/tradehelper.egg-info/requires.txt
--rw-rw-r--   0 aarav     (1000) aarav     (1000)       12 2023-08-01 13:23:15.000000 tradehelper-1.43/tradehelper.egg-info/top_level.txt
+drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-08-01 13:27:47.521001 tradehelper-1.44/
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      196 2023-08-01 13:27:47.521001 tradehelper-1.44/PKG-INFO
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)       38 2023-08-01 13:27:47.521001 tradehelper-1.44/setup.cfg
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      366 2023-08-01 13:27:26.000000 tradehelper-1.44/setup.py
+drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-08-01 13:27:47.521001 tradehelper-1.44/tradehelper/
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      149 2022-06-02 06:39:05.000000 tradehelper-1.44/tradehelper/__init__.py
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)    19319 2023-08-01 13:27:16.000000 tradehelper-1.44/tradehelper/tradehelp.py
+drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-08-01 13:27:47.521001 tradehelper-1.44/tradehelper.egg-info/
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      196 2023-08-01 13:27:47.000000 tradehelper-1.44/tradehelper.egg-info/PKG-INFO
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      231 2023-08-01 13:27:47.000000 tradehelper-1.44/tradehelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)        1 2023-08-01 13:27:47.000000 tradehelper-1.44/tradehelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)       31 2023-08-01 13:27:47.000000 tradehelper-1.44/tradehelper.egg-info/requires.txt
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)       12 2023-08-01 13:27:47.000000 tradehelper-1.44/tradehelper.egg-info/top_level.txt
```

### Comparing `tradehelper-1.43/tradehelper/tradehelp.py` & `tradehelper-1.44/tradehelper/tradehelp.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                 else:
                     data = {
                             'strategy_name': args["strategy_name"],
                             'type': execution_type,
                             'trading_day' : self.trading_day,
                             'args': args
                     }
-                # print(data)
+                print(data)
                 response = requests.post(
                     self.base_url+"execution", headers=self.headers, data=data)
                 response_json = (response.json())
                 # print(response_json)
                 return int(response_json['daily_execution_id'])
         except Exception as e:
             print(e)
```

