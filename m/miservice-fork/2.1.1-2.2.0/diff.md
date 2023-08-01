# Comparing `tmp/miservice_fork-2.1.1.tar.gz` & `tmp/miservice_fork-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miservice_fork-2.1.1.tar", last modified: Sun Mar 12 13:35:18 2023, max compression
+gzip compressed data, was "miservice_fork-2.2.0.tar", last modified: Tue Aug  1 05:01:55 2023, max compression
```

## Comparing `miservice_fork-2.1.1.tar` & `miservice_fork-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-03-12 13:35:18.850306 miservice_fork-2.1.1/
--rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.1.1/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      463 2023-03-12 13:35:18.849938 miservice_fork-2.1.1/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     3467 2023-03-12 07:08:18.000000 miservice_fork-2.1.1/README.md
--rwxr-xr-x   0 hyi        (502) staff       (20)       73 2023-03-11 14:21:43.000000 miservice_fork-2.1.1/micli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-03-12 13:35:18.837892 miservice_fork-2.1.1/miservice/
--rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.1.1/miservice/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.1.1/miservice/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     2263 2023-03-12 13:34:13.000000 miservice_fork-2.1.1/miservice/cli.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5649 2023-03-11 14:57:58.000000 miservice_fork-2.1.1/miservice/miaccount.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2023-03-11 14:21:43.000000 miservice_fork-2.1.1/miservice/miiocommand.py
--rwxr-xr-x   0 hyi        (502) staff       (20)    10548 2023-03-12 07:10:00.000000 miservice_fork-2.1.1/miservice/miioservice.py
--rw-r--r--   0 hyi        (502) staff       (20)     3530 2023-03-11 14:21:43.000000 miservice_fork-2.1.1/miservice/minaservice.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-03-12 13:35:18.845069 miservice_fork-2.1.1/miservice_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      463 2023-03-12 13:35:18.000000 miservice_fork-2.1.1/miservice_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      424 2023-03-12 13:35:18.000000 miservice_fork-2.1.1/miservice_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2023-03-12 13:35:18.000000 miservice_fork-2.1.1/miservice_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       46 2023-03-12 13:35:18.000000 miservice_fork-2.1.1/miservice_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)        8 2023-03-12 13:35:18.000000 miservice_fork-2.1.1/miservice_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       10 2023-03-12 13:35:18.000000 miservice_fork-2.1.1/miservice_fork.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-03-12 13:35:18.850380 miservice_fork-2.1.1/setup.cfg
--rwxr-xr-x   0 hyi        (502) staff       (20)      900 2023-03-12 13:34:20.000000 miservice_fork-2.1.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 05:01:55.532311 miservice_fork-2.2.0/
+-rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      463 2023-08-01 05:01:55.532105 miservice_fork-2.2.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     3562 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/README.md
+-rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.2.0/micli.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 05:01:55.530070 miservice_fork-2.2.0/miservice/
+-rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.2.0/miservice/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/miservice/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3146 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/miservice/cli.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/miservice/miaccount.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/miservice/miiocommand.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)    10548 2023-03-12 07:10:00.000000 miservice_fork-2.2.0/miservice/miioservice.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3530 2023-03-11 14:21:43.000000 miservice_fork-2.2.0/miservice/minaservice.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-01 05:01:55.531824 miservice_fork-2.2.0/miservice_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      463 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      424 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       46 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        8 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       10 2023-08-01 05:01:55.000000 miservice_fork-2.2.0/miservice_fork.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-08-01 05:01:55.532367 miservice_fork-2.2.0/setup.cfg
+-rwxr-xr-x   0 hyi        (502) staff       (20)      900 2023-08-01 05:01:39.000000 miservice_fork-2.2.0/setup.py
```

### Comparing `miservice_fork-2.1.1/LICENSE` & `miservice_fork-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.1.1/README.md` & `miservice_fork-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # MiService
 XiaoMi Cloud Service for mi.com
 This is a fork from https://github.com/Yonsm/MiService made some change for xiaogpt
 
 ## Install
 ```
+pip3 install -U miservice_fork
+or 
 pip3 install .
 ```
 
 ## Library
 ```
 MiService：XiaoMi Cloud Service
   |
@@ -84,15 +86,15 @@
 export MI_DID=<Device ID|Name>
 ```
 
 ### 4. 查询设备的接口文档
 
 查询设备的 MIoT 接口能力描述：
 ```
-micli.py spec xiaomi.wifispeaker.lx04
+micli spec xiaomi.wifispeaker.lx04
 ```
 其中分为属性获取、属性设置、动作调用三种描述。
 
 ### 5. 查询音量属性
 
 ```
 micli.py 2-1
@@ -120,10 +122,17 @@
 ```
 
 其中 `#1` 表示设备语音回应，如果要执行默默关灯（不要音箱回应），可以如下：
 ```
 micli.py 5-4 关灯 #0
 ```
 
-### 8. 其它应用
+## 8. 播放音乐
+
+```
+micli play ${mp3_url} 
+micli stop
+```
+
+### 9. 其它应用
 
 在扩展插件中使用，比如，参考 [ZhiMsg 小爱同学 TTS 播报/执行插件](https://github.com/Yonsm/ZhiMsg)
```

### Comparing `miservice_fork-2.1.1/miservice/cli.py` & `miservice_fork-2.2.0/miservice/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,32 +17,55 @@
 
 def usage():
     print("MiService %s - XiaoMi Cloud Service\n")
     print("Usage: The following variables must be set:")
     print("           export MI_USER=<Username>")
     print("           export MI_PASS=<Password>")
     print("           export MI_DID=<Device ID|Name>\n")
-    print(miio_command_help(prefix=sys.argv[0] + " "))
+    print(miio_command_help(prefix="micli" + " "))
+
+
+def find_device_id(hardware_data, mi_did):
+    for h in hardware_data:
+        if h.get("miotDID", "") == str(mi_did):
+            return h.get("deviceID")
+        else:
+            continue
+    else:
+        raise Exception(f"we have no mi_did: please use `micli mina` to check")
 
 
 async def main(args):
     try:
         async with ClientSession() as session:
             env = os.environ
             account = MiAccount(
                 session,
                 env.get("MI_USER"),
                 env.get("MI_PASS"),
                 os.path.join(str(Path.home()), ".mi.token"),
             )
+            result = ""
+            mina_service = MiNAService(account)
+            result = await mina_service.device_list()
+            device_id = find_device_id(result, env.get("MI_DID", ""))
             if args.startswith("mina"):
-                service = MiNAService(account)
-                result = await service.device_list()
                 if len(args) > 4:
-                    await service.send_message(result, -1, args[4:])
+                    await mina_service.send_message(result, -1, args[4:])
+            elif args.split(" ")[0].strip() in ["play", "pause"]:
+                args_list = args.split(" ")
+                if len(args_list) == 1:
+                    if args_list[0] == "pause":
+                        await mina_service.player_pause(device_id)
+                    else:
+                        print("Please provice play url")
+                    return
+                # make device_id
+                await mina_service.play_by_url(device_id, args_list[1])
+                return
             else:
                 service = MiIOService(account)
                 result = await miio_command(
                     service, env.get("MI_DID"), args, sys.argv[0] + " "
                 )
             if not isinstance(result, str):
                 result = json.dumps(result, indent=2, ensure_ascii=False)
```

### Comparing `miservice_fork-2.1.1/miservice/miaccount.py` & `miservice_fork-2.2.0/miservice/miaccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         url = "https://account.xiaomi.com/pass/" + uri
         async with self.session.request(
             "GET" if data is None else "POST",
             url,
             data=data,
             cookies=cookies,
             headers=headers,
-            ssl = False,
+            ssl=False,
         ) as r:
             raw = await r.read()
         resp = json.loads(raw[11:])
         _LOGGER.debug("%s: %s", uri, resp)
         return resp
 
     async def _securityTokenService(self, location, nonce, ssecurity):
```

### Comparing `miservice_fork-2.1.1/miservice/miiocommand.py` & `miservice_fork-2.2.0/miservice/miiocommand.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.1.1/miservice/miioservice.py` & `miservice_fork-2.2.0/miservice/miioservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.1.1/miservice/minaservice.py` & `miservice_fork-2.2.0/miservice/minaservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.1.1/setup.py` & `miservice_fork-2.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup
 
 setup(
     name="miservice_fork",
     description="XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService",
-    version="2.1.1",
+    version="2.2.0",
     license="MIT",
     author="Yonsm, yihong0618",
     author_email="Yonsm@qq.com, zouzou0208@gmail.com",
     url="https://github.com/yihong0618/MiService",
     packages=["miservice"],
     scripts=["micli.py"],
     python_requires=">=3.7",
```

