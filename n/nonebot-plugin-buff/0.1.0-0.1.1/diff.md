# Comparing `tmp/nonebot_plugin_buff-0.1.0.tar.gz` & `tmp/nonebot_plugin_buff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_buff-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_buff-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_buff-0.1.0.tar` & `nonebot_plugin_buff-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      699 2023-07-31 11:41:41.621623 nonebot_plugin_buff-0.1.0/README.md
--rw-r--r--   0        0        0     5768 2023-07-31 11:41:41.621623 nonebot_plugin_buff-0.1.0/nonebot_plugin_buff/__init__.py
--rw-r--r--   0        0        0      114 2023-07-31 11:41:41.621623 nonebot_plugin_buff-0.1.0/nonebot_plugin_buff/config.py
--rw-r--r--   0        0        0   500057 2023-07-31 11:41:41.621623 nonebot_plugin_buff-0.1.0/nonebot_plugin_buff/data.txt
--rw-r--r--   0        0        0      436 2023-07-31 11:41:41.621623 nonebot_plugin_buff-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      699 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/README.md
+-rw-r--r--   0        0        0     5805 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/config.py
+-rw-r--r--   0        0        0   500057 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/data.txt
+-rw-r--r--   0        0        0      436 2023-08-01 03:10:13.027639 nonebot_plugin_buff-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_buff-0.1.0/README.md` & `nonebot_plugin_buff-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_buff-0.1.0/nonebot_plugin_buff/__init__.py` & `nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 from nonebot.plugin import PluginMetadata
-
 from .config import Config
-
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-buff",
     description="一款模拟buff查找饰品价格的机器人",
     usage="输入 查询/搜索/查 xxx 按照机器人的提示，将会获取到目前buff市场上最低的饰品价格",
-
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
-
     homepage="https://github.com/Sydrr0/nonebot-plugin-buff",
     # 发布必填。
-
     config=Config,
     # 插件配置项类，如无需配置可不填写。
-
     supported_adapters={"~onebot.v11"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 
 # 插件初始化
@@ -33,15 +27,15 @@
 from nonebot.plugin import on_command
 from nonebot.params import ArgPlainText # 提取消息内的字符串的方法
 from nonebot.adapters import Message
 from nonebot.params import CommandArg 
 from nonebot.typing import T_State   # 继承上一个函数的方法
 
 # 后端爬虫所需要的插件
-import requests
+import httpx
 import re
 import os
 from bs4 import BeautifulSoup
 
 # 创建本地文件夹，用于存放数据
 save_path = "./search_data"
 if not os.path.exists(save_path):
@@ -65,35 +59,35 @@
                 # 提取逗号后面的内容，并转换为 str
                 ob_name = str(line[comma_index + 1:].strip())
                 ob_name_list.append(ob_name)
     # 这里得到了两个列表，第一个是buff序号列表，第二个是商品名称列表
     return num_list,ob_name_list
 
 def sending_txt(name_index):   # 传入两个列表，第一个是符合的商品编码。第二个是名称
-    name_resulr_list = []    # 得到一个用以下 for 循环的结果，需要逐行输出
+    name_result_list = []    # 得到一个用以下 for 循环的结果，需要逐行输出
     for index in range(0,len(name_index)):
         # 把每一行的内容加入到name_resulr_list里面
-        name_resulr_list.append('%i: %s'% (index, name_index[index]))          
+        name_result_list.append('%i: %s'% (index, name_index[index]))          
     # 用换行符把列表里面每一个元素 join 成一个对象
-    result = '\n'.join(str(item) for item in name_resulr_list)
+    result = '\n'.join(str(item) for item in name_result_list)
     # 去除最后一行的换行符
     result = result.rstrip('\n')
     return result
 
-def get_miniprice(num,obtype): # num是获取到的商品index, ob_type是指崭新出厂之类的
+async def get_miniprice(num,obtype): # num是获取到的商品index, ob_type是指崭新出厂之类的
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! ob_type 还未表达，需使用正则表达式提取 !!!!!
     base_url ='https://buff.163.com/goods/'
     extra_url = str(num)
     url = base_url + extra_url
-    response = requests.get(url)
-    page_url = response.text
-    data_getten = BeautifulSoup(page_url, "lxml")
-    mini_price_html = str(data_getten.find_all("div", class_="scope-btns"))
+    async with httpx.AsyncClient() as client: # 异步 httpx 为了防止事件卡死
+        response = await client.get(url)
+        page_url = response.text
+        data_getten = BeautifulSoup(page_url, "lxml")
+        mini_price_html = str(data_getten.find_all("div", class_="scope-btns"))
 
-    # ob_type = r"\((.*?)\)[^()]*$" 是获取obtype的re表达式
     pattern = r'{ob_type}.*?data\-price\="([^"]+)"'.format(ob_type = obtype) 
     # 上面的正则表达式表示 ob_type 后面的第一个 data-price='' 中的值
     match = re.search(pattern, mini_price_html)
     if match:
         return match.group(1) # 查找第一个符合的值
     else:
         return None
```

### Comparing `nonebot_plugin_buff-0.1.0/nonebot_plugin_buff/data.txt` & `nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/data.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_buff-0.1.0/PKG-INFO` & `nonebot_plugin_buff-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-buff
-Version: 0.1.0
+Version: 0.1.1
 Summary: 实时爬取BUFF饰品价格
 License: MIT
 Author: Sydrr0
 Author-email: 2562312527@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

