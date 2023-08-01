# Comparing `tmp/nonebot_plugin_buff-0.2.0.tar.gz` & `tmp/nonebot_plugin_buff-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_buff-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_buff-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_buff-0.2.0.tar` & `nonebot_plugin_buff-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      697 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/README.md
--rw-r--r--   0        0        0     6540 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/nonebot_plugin_buff/__init__.py
--rw-r--r--   0        0        0      114 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/nonebot_plugin_buff/config.py
--rw-r--r--   0        0        0      451 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      697 2023-08-01 09:10:18.878672 nonebot_plugin_buff-0.2.1/README.md
+-rw-r--r--   0        0        0     5648 2023-08-01 09:10:18.882672 nonebot_plugin_buff-0.2.1/nonebot_plugin_buff/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-01 09:10:18.882672 nonebot_plugin_buff-0.2.1/nonebot_plugin_buff/config.py
+-rw-r--r--   0        0        0      431 2023-08-01 09:10:18.882672 nonebot_plugin_buff-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_buff-0.2.0/README.md` & `nonebot_plugin_buff-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_buff-0.2.0/nonebot_plugin_buff/__init__.py` & `nonebot_plugin_buff-0.2.1/nonebot_plugin_buff/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 
 
 # 后端爬虫所需要的插件
 import httpx
 import re
 import os
-import asyncio
 from bs4 import BeautifulSoup
 
 # 创建本地文件夹，用于存放数据
 save_path = "./search_data"
 if not os.path.exists(save_path):
     os.mkdir(save_path)
 else:
@@ -115,42 +114,22 @@
     
     if not num_list and not obname_list:
         await search.finish('数据库中暂时未收录该饰品')
     else:
         await search.send(asking_txt)
 
 # 正则表达式获取最后一个括号内的内容，就是obtype
-from datetime import timedelta
 
 @search.got("num_index", prompt="请输入序号")
 async def got_num(state: T_State, num_index: str = ArgPlainText()):
     num_input = f"{num_index}"  # 用户输入的序号
     obindex = state['num_list'][int(num_input)]
     obname_full = state['name_list'][int(num_input)]
     pattern = r"\((.*?)\)[^()]*$"
     match = re.search(pattern, obname_full)
     if match:
         obname_type = match.group(1)
     else:
         pass
 
-    async def main():
-        miniprice = await get_miniprice(num=obindex, obtype=obname_type)
-        await search.finish('%s\n现价: ￥ %s\nBuff代码: %s' % (obname_full, miniprice, obindex))
-
-    loop = asyncio.get_event_loop()
-    loop.create_task(main())
-    
-    try:
-        bot = get_bot()
-        if search.is_private_chat():
-
-            await bot.wait(timedelta(minutes=1))  # 设置等待时间为1分钟
-            await search.finish("输入时间超过一分钟，请重新发起查询。")
-        else:
-            await bot.wait(timedelta(minutes=1))  # 设置等待时间为1分钟
-            await search.finish(f"@{search.sender.nickname} 输入时间超过一分钟，请重新发起查询。")
-    except asyncio.TimeoutError:
-        if search.is_private_chat():
-            await search.finish("输入时间超过一分钟，请重新发起查询。")
-        else:
-            await search.finish(f"@{search.sender.nickname} 输入时间超过一分钟，请重新发起查询。")
+    miniprice = await get_miniprice(num=obindex, obtype=obname_type)
+    await search.finish('%s\n现价: ￥ %s\nBuff代码: %s' % (obname_full, miniprice, obindex))
```

### Comparing `nonebot_plugin_buff-0.2.0/PKG-INFO` & `nonebot_plugin_buff-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-buff
-Version: 0.2.0
+Version: 0.2.1
 Summary: 实时爬取BUFF饰品价格
 License: MIT
 Author: Sydrr0
 Author-email: 2562312527@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot2 (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 欢迎使用 nonebot_plugin_buff
 ![image](https://usercontent.githubfast.com/avatars/u/129657153?v=4)
```

