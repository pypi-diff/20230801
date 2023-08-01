# Comparing `tmp/nonebot_plugin_bind-0.1.2.tar.gz` & `tmp/nonebot_plugin_bind-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bind-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_bind-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_bind-0.1.2.tar` & `nonebot_plugin_bind-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4098 2023-08-01 02:53:25.352916 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/__init__.py
--rw-r--r--   0        0        0      351 2023-08-01 02:53:25.344910 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/types.py
--rw-r--r--   0        0        0     7027 2023-08-01 03:05:37.685301 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/user_sql.py
--rw-r--r--   0        0        0     1489 2023-08-01 02:53:25.348915 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/utils.py
--rw-r--r--   0        0        0      522 2023-08-01 03:40:01.857921 nonebot_plugin_bind-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2526 2023-08-01 03:41:13.902443 nonebot_plugin_bind-0.1.2/README.md
--rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4586 2023-08-01 03:55:55.753846 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/__init__.py
+-rw-r--r--   0        0        0      351 2023-08-01 02:53:25.344910 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/types.py
+-rw-r--r--   0        0        0     7027 2023-08-01 03:05:37.685301 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/user_sql.py
+-rw-r--r--   0        0        0     1489 2023-08-01 02:53:25.348915 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/utils.py
+-rw-r--r--   0        0        0      522 2023-08-01 04:08:48.387719 nonebot_plugin_bind-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2627 2023-08-01 04:07:03.126006 nonebot_plugin_bind-0.1.3/README.md
+-rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/__init__.py` & `nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,19 +4,29 @@
 
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from nonebot import get_driver
 from nonebot import on_command
 from nonebot.adapters import Event, Bot
 from nonebot.matcher import Matcher
 from nonebot.params import ArgStr, T_State, CommandArg, RawCommand
+from nonebot.plugin import PluginMetadata
 
 from .types import Bind
 from .user_sql import edit_user, del_user, User
 from .utils import get_params, get_user, GetUser, _is_private_
 
+__plugin_meta__ = PluginMetadata(
+    name="跨平台账户绑定",
+    description="nonebot多适配器通用的跨平台账户绑定插件",
+    usage="1.使用'bind'或'绑定'命令发起绑定事件\n2.使用'bindinfo'或'绑定信息'查看绑定信息",
+    type="library",
+    homepage="https://github.com/canxin121/nonebot_plugin_bind",
+    supported_adapters={"~onebot.v11", "~telegram", "~kaiheila", "~feishu", "~villa"},
+)
+
 SECONDS = str(get_driver().config.session_expire_timeout.seconds)
 
 Binds: dict = {}
 
 
 def del_Bind(_token):
     if _token in Binds.keys():
```

### Comparing `nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/user_sql.py` & `nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/user_sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/utils.py` & `nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.2/pyproject.toml` & `nonebot_plugin_bind-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-bind"
-version = "0.1.2"
+version = "0.1.3"
 description = "nonebot多平台账户信息绑定"
 authors = ["canxin <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_bind" }]
 homepage = 'https://github.com/canxin121/nonebot_plugin_bind'
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_bind-0.1.2/README.md` & `nonebot_plugin_bind-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,21 @@
     <br />
     <a href="https://github.com/canxin121/nonebot_plugin_bind/releases/">
     <a href="https://img.shields.io/github/last-commit/canxin121/nonebot_plugin_bind">
     </a>
 </p>
 <div align="left">
 
+# 适配支持
+- onebotv11
+- telegram
+- discord
+- kook(开黑啦)
+- villa(大别野)
+- 飞书
 # 使用说明
 
 ## 用户使用说明
 
 | 命令                  | 限制    | 含义       |
 |---------------------|-------|----------|
 | 'bind' 或 '绑定'       | 群聊或私聊 | 发起绑定事件   |
```

### Comparing `nonebot_plugin_bind-0.1.2/PKG-INFO` & `nonebot_plugin_bind-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bind
-Version: 0.1.2
+Version: 0.1.3
 Summary: nonebot多平台账户信息绑定
 Home-page: https://github.com/canxin121/nonebot_plugin_bind
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -33,14 +33,21 @@
     <br />
     <a href="https://github.com/canxin121/nonebot_plugin_bind/releases/">
     <a href="https://img.shields.io/github/last-commit/canxin121/nonebot_plugin_bind">
     </a>
 </p>
 <div align="left">
 
+# 适配支持
+- onebotv11
+- telegram
+- discord
+- kook(开黑啦)
+- villa(大别野)
+- 飞书
 # 使用说明
 
 ## 用户使用说明
 
 | 命令                  | 限制    | 含义       |
 |---------------------|-------|----------|
 | 'bind' 或 '绑定'       | 群聊或私聊 | 发起绑定事件   |
```

