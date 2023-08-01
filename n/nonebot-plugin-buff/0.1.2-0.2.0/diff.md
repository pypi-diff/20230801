# Comparing `tmp/nonebot_plugin_buff-0.1.2.tar.gz` & `tmp/nonebot_plugin_buff-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_buff-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_buff-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_buff-0.1.2.tar` & `nonebot_plugin_buff-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      699 2023-08-01 03:49:06.772918 nonebot_plugin_buff-0.1.2/README.md
--rw-r--r--   0        0        0     5805 2023-08-01 03:49:06.772918 nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/__init__.py
--rw-r--r--   0        0        0      114 2023-08-01 03:49:06.772918 nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/config.py
--rw-r--r--   0        0        0   500057 2023-08-01 03:49:06.776919 nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/data.txt
--rw-r--r--   0        0        0      433 2023-08-01 03:49:06.776919 nonebot_plugin_buff-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      697 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/README.md
+-rw-r--r--   0        0        0     6540 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/nonebot_plugin_buff/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/nonebot_plugin_buff/config.py
+-rw-r--r--   0        0        0      451 2023-08-01 07:41:32.645659 nonebot_plugin_buff-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_buff-0.1.2/README.md` & `nonebot_plugin_buff-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 
  1. 先安装**nonebot_plugin_buff**
  2. 启用此插件，具体请看**nonebot**官网文档
  3. 在入口文件下面的**search_data**目录下添加最新的**data.txt**
  4. 发送 **查询/查 xxx** ，然后跟随bot指令即可查询价格
 
  ## 附件
-data.txt下载地址：[Release最新版本下载地址](https://github.com/Sydrr0/nonebot-plugin-buff/releases/tag/data.txt)
+data.txt下载地址：[Release最新版本下载地址](https://github.com/Sydrr0/nonebot-plugin-buff/releases/tag/v0.2.0)
 
 联系QQ：**2562312527**
```

### Comparing `nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/__init__.py` & `nonebot_plugin_buff-0.2.0/nonebot_plugin_buff/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,19 +25,23 @@
 # nonebot2 的函数导入
 from nonebot.matcher import Matcher
 from nonebot.plugin import on_command
 from nonebot.params import ArgPlainText # 提取消息内的字符串的方法
 from nonebot.adapters import Message
 from nonebot.params import CommandArg 
 from nonebot.typing import T_State   # 继承上一个函数的方法
+from nonebot import get_bot
+
+
 
 # 后端爬虫所需要的插件
 import httpx
 import re
 import os
+import asyncio
 from bs4 import BeautifulSoup
 
 # 创建本地文件夹，用于存放数据
 save_path = "./search_data"
 if not os.path.exists(save_path):
     os.mkdir(save_path)
 else:
@@ -90,42 +94,63 @@
     if match:
         return match.group(1) # 查找第一个符合的值
     else:
         return None
 
 
 
+
 @search.handle()  # 这是为了接收 查询xxx 中的xxx
 async def handle_function(matcher: Matcher, args: Message = CommandArg()):
     if args.extract_plain_text():
         matcher.set_arg("name", args)  # 获取的xxx
     
-@search.got("name", prompt="请输入饰品名称")   # 用got函数继承xxx
+@search.got("name", prompt="请输入饰品名称")
 async def got_name(state: T_State, name: str = ArgPlainText()):
-    name_input = (f"{name}") # 用户使用 查询xxx 这里的 name_input 即为xxx type:str
-    num_list = find_numbers(name_input)[0]   # 获取序号的列表
-    obname_list = find_numbers(name_input)[1]   # 获取物品名称的列表
-    asking_txt = sending_txt(name_index= obname_list)
-    state['num_list'] = num_list   # 保存list到下一个函数内使用
+    name_input = f"{name}"  # 用户输入的饰品名称
+    num_list = find_numbers(name_input)[0]  # 获取序号的列表
+    obname_list = find_numbers(name_input)[1]  # 获取物品名称的列表
+    asking_txt = sending_txt(name_index=obname_list)
+    state['num_list'] = num_list  # 保存list到下一个函数内使用
     state['name_list'] = obname_list
-    await search.send(asking_txt)
+    
+    if not num_list and not obname_list:
+        await search.finish('数据库中暂时未收录该饰品')
+    else:
+        await search.send(asking_txt)
 
+# 正则表达式获取最后一个括号内的内容，就是obtype
+from datetime import timedelta
 
 @search.got("num_index", prompt="请输入序号")
-async def got_num(state: T_State ,num_index: str = ArgPlainText()):
-    num_input = (f"{num_index}") # 用户使用序号 这里的 num_input 即为index type:str 
+async def got_num(state: T_State, num_index: str = ArgPlainText()):
+    num_input = f"{num_index}"  # 用户输入的序号
     obindex = state['num_list'][int(num_input)]
     obname_full = state['name_list'][int(num_input)]
-    # 正则表达式获取最后一个括号内的内容，就是obtype
     pattern = r"\((.*?)\)[^()]*$"
     match = re.search(pattern, obname_full)
     if match:
         obname_type = match.group(1)
     else:
         pass
-    # 使用 get_miniprice() 获取此时的最低价格, 并结束此次事件
-    miniprice = get_miniprice(num= obindex, obtype= obname_type)
-    await search.finish('%s\n'
-                        '现价: ￥ %s'
-                        'Buff代码: %s'% (obname_full,
-                                        miniprice,
-                                        obindex))
+
+    async def main():
+        miniprice = await get_miniprice(num=obindex, obtype=obname_type)
+        await search.finish('%s\n现价: ￥ %s\nBuff代码: %s' % (obname_full, miniprice, obindex))
+
+    loop = asyncio.get_event_loop()
+    loop.create_task(main())
+    
+    try:
+        bot = get_bot()
+        if search.is_private_chat():
+
+            await bot.wait(timedelta(minutes=1))  # 设置等待时间为1分钟
+            await search.finish("输入时间超过一分钟，请重新发起查询。")
+        else:
+            await bot.wait(timedelta(minutes=1))  # 设置等待时间为1分钟
+            await search.finish(f"@{search.sender.nickname} 输入时间超过一分钟，请重新发起查询。")
+    except asyncio.TimeoutError:
+        if search.is_private_chat():
+            await search.finish("输入时间超过一分钟，请重新发起查询。")
+        else:
+            await search.finish(f"@{search.sender.nickname} 输入时间超过一分钟，请重新发起查询。")
```

### Comparing `nonebot_plugin_buff-0.1.2/PKG-INFO` & `nonebot_plugin_buff-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-buff
-Version: 0.1.2
+Version: 0.2.0
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
+Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot2 (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 欢迎使用 nonebot_plugin_buff
 ![image](https://usercontent.githubfast.com/avatars/u/129657153?v=4)
@@ -25,11 +26,11 @@
 
  1. 先安装**nonebot_plugin_buff**
  2. 启用此插件，具体请看**nonebot**官网文档
  3. 在入口文件下面的**search_data**目录下添加最新的**data.txt**
  4. 发送 **查询/查 xxx** ，然后跟随bot指令即可查询价格
 
  ## 附件
-data.txt下载地址：[Release最新版本下载地址](https://github.com/Sydrr0/nonebot-plugin-buff/releases/tag/data.txt)
+data.txt下载地址：[Release最新版本下载地址](https://github.com/Sydrr0/nonebot-plugin-buff/releases/tag/v0.2.0)
 
 联系QQ：**2562312527**
```

