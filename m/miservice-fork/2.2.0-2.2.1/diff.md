# Comparing `tmp/miservice_fork-2.2.0.tar.gz` & `tmp/miservice_fork-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miservice_fork-2.2.0.tar", last modified: Tue Aug  1 05:01:55 2023, max compression
+gzip compressed data, was "miservice_fork-2.2.1.tar", last modified: Tue Aug  1 13:48:57 2023, max compression
```

## Comparing `miservice_fork-2.2.0.tar` & `miservice_fork-2.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 05:01:55.532311 miservice_fork-2.2.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      463 2023-08-01 05:01:55.532105 miservice_fork-2.2.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     3562 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/README.md
--rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.2.0/micli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 05:01:55.530070 miservice_fork-2.2.0/miservice/
--rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.2.0/miservice/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/miservice/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     3146 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/miservice/cli.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/miservice/miaccount.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/miservice/miiocommand.py
--rwxr-xr-x   0 hyi        (502) staff       (20)    10548 2023-03-12 07:10:00.000000 miservice_fork-2.2.0/miservice/miioservice.py
--rw-r--r--   0 hyi        (502) staff       (20)     3530 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/miservice/minaservice.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 05:01:55.531824 miservice_fork-2.2.0/miservice_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      463 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      424 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       46 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)        8 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       10 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-08-01 05:01:55.532367 miservice_fork-2.2.0/setup.cfg
--rwxr-xr-x   0 hyi        (502) staff       (20)      900 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 13:48:57.724675 miservice_fork-2.2.1/
+-rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.2.1/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      463 2023-08-01 13:48:57.724379 miservice_fork-2.2.1/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     3562 2023-08-01 05:01:39.000000 miservice_fork-2.2.1/README.md
+-rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.2.1/micli.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 13:48:57.721346 miservice_fork-2.2.1/miservice/
+-rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.2.1/miservice/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.2.1/miservice/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3268 2023-08-01 13:47:52.000000 miservice_fork-2.2.1/miservice/cli.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-08-01 05:01:39.000000 miservice_fork-2.2.1/miservice/miaccount.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2023-03-11 14:21:43.000000 miservice_fork-2.2.1/miservice/miiocommand.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)    10548 2023-03-12 07:10:00.000000 miservice_fork-2.2.1/miservice/miioservice.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3530 2023-03-11 14:21:43.000000 miservice_fork-2.2.1/miservice/minaservice.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 13:48:57.724033 miservice_fork-2.2.1/miservice_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      463 2023-08-01 13:48:57.000000 miservice_fork-2.2.1/miservice_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      424 2023-08-01 13:48:57.000000 miservice_fork-2.2.1/miservice_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-08-01 13:48:57.000000 miservice_fork-2.2.1/miservice_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       46 2023-08-01 13:48:57.000000 miservice_fork-2.2.1/miservice_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        8 2023-08-01 13:48:57.000000 miservice_fork-2.2.1/miservice_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       10 2023-08-01 13:48:57.000000 miservice_fork-2.2.1/miservice_fork.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-08-01 13:48:57.724748 miservice_fork-2.2.1/setup.cfg
+-rwxr-xr-x   0 hyi        (502) staff       (20)      900 2023-08-01 13:48:50.000000 miservice_fork-2.2.1/setup.py
```

### Comparing `miservice_fork-2.2.0/LICENSE` & `miservice_fork-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.2.0/README.md` & `miservice_fork-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.2.0/miservice/cli.py` & `miservice_fork-2.2.1/miservice/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,20 +42,22 @@
                 session,
                 env.get("MI_USER"),
                 env.get("MI_PASS"),
                 os.path.join(str(Path.home()), ".mi.token"),
             )
             result = ""
             mina_service = MiNAService(account)
-            result = await mina_service.device_list()
-            device_id = find_device_id(result, env.get("MI_DID", ""))
             if args.startswith("mina"):
                 if len(args) > 4:
                     await mina_service.send_message(result, -1, args[4:])
             elif args.split(" ")[0].strip() in ["play", "pause"]:
+                result = await mina_service.device_list()
+                if not env.get("MI_DID"):
+                    raise Exception("Please export MI_DID in your env")
+                device_id = find_device_id(result, env.get("MI_DID", ""))
                 args_list = args.split(" ")
                 if len(args_list) == 1:
                     if args_list[0] == "pause":
                         await mina_service.player_pause(device_id)
                     else:
                         print("Please provice play url")
                     return
```

### Comparing `miservice_fork-2.2.0/miservice/miaccount.py` & `miservice_fork-2.2.1/miservice/miaccount.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.2.0/miservice/miiocommand.py` & `miservice_fork-2.2.1/miservice/miiocommand.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.2.0/miservice/miioservice.py` & `miservice_fork-2.2.1/miservice/miioservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.2.0/miservice/minaservice.py` & `miservice_fork-2.2.1/miservice/minaservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.2.0/setup.py` & `miservice_fork-2.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup
 
 setup(
     name="miservice_fork",
     description="XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService",
-    version="2.2.0",
+    version="2.2.1",
     license="MIT",
     author="Yonsm, yihong0618",
     author_email="Yonsm@qq.com, zouzou0208@gmail.com",
     url="https://github.com/yihong0618/MiService",
     packages=["miservice"],
     scripts=["micli.py"],
     python_requires=">=3.7",
```

