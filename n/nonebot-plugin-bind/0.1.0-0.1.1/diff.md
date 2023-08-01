# Comparing `tmp/nonebot_plugin_bind-0.1.0.tar.gz` & `tmp/nonebot_plugin_bind-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bind-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_bind-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_bind-0.1.0.tar` & `nonebot_plugin_bind-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4098 2023-08-01 02:53:25.352916 nonebot_plugin_bind-0.1.0/nonebot_plugin_bind/__init__.py
--rw-r--r--   0        0        0      351 2023-08-01 02:53:25.344910 nonebot_plugin_bind-0.1.0/nonebot_plugin_bind/types.py
--rw-r--r--   0        0        0     7027 2023-08-01 03:05:37.685301 nonebot_plugin_bind-0.1.0/nonebot_plugin_bind/user_sql.py
--rw-r--r--   0        0        0     1489 2023-08-01 02:53:25.348915 nonebot_plugin_bind-0.1.0/nonebot_plugin_bind/utils.py
--rw-r--r--   0        0        0      461 2023-08-01 03:04:29.038076 nonebot_plugin_bind-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2873 2023-08-01 03:26:22.460679 nonebot_plugin_bind-0.1.0/README.md
--rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4098 2023-08-01 02:53:25.352916 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/__init__.py
+-rw-r--r--   0        0        0      351 2023-08-01 02:53:25.344910 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/types.py
+-rw-r--r--   0        0        0     7027 2023-08-01 03:05:37.685301 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/user_sql.py
+-rw-r--r--   0        0        0     1489 2023-08-01 02:53:25.348915 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/utils.py
+-rw-r--r--   0        0        0      461 2023-08-01 03:37:58.822103 nonebot_plugin_bind-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2494 2023-08-01 03:37:47.563579 nonebot_plugin_bind-0.1.1/README.md
+-rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_bind-0.1.0/nonebot_plugin_bind/__init__.py` & `nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.0/nonebot_plugin_bind/user_sql.py` & `nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/user_sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.0/nonebot_plugin_bind/utils.py` & `nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.0/README.md` & `nonebot_plugin_bind-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,64 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-bind
+Version: 0.1.1
+Summary: nonebot多平台账户信息绑定
+Author: canxin
+Author-email: 1969730106@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: APScheduler (>=3.10.1,<4.0.0)
+Requires-Dist: SQLAlchemy (>=2.0.19,<3.0.0)
+Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
+Requires-Dist: nonebot2 (>=2.0.1,<3.0.0)
+Description-Content-Type: text/markdown
+
 <div align="center">
   <a href="https://github.com/canxin121">
     <img src="https://socialify.git.ci/canxin121/nonebot_plugin_bind/image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto" width="700" height="350">
   </a>
-  <h1>nonebot_plugin_bind仓库</h1>
-  <p><em>nonebot_plugin_bind</em></p>
+  <h1>nonebot_plugin_bind</h1>
 </div>
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/nonebot-plugin-bind">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-bind" alt="pypi">
     </a>
     <img src="https://img.shields.io/pypi/pyversions/nonebot-plugin-bind" alt="python">
     <img src="https://img.shields.io/pypi/dm/nonebot-plugin-bind" alt="pypi">
     <br />
-    <a href="https://onebot.dev/">
-    <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_plugin_bind/releases/">
-    <img src="https://img.shields.io/github/last-commit/canxin121/nonebot_plugin_bind" alt="github">
+    <a href="https://img.shields.io/github/last-commit/canxin121/nonebot_plugin_bind">
     </a>
 </p>
 <div align="left">
 
 # 使用说明
 
 ## 用户使用说明
 
 | 命令                  | 限制    | 含义       |
 |---------------------|-------|----------|
 | 'bind' 或 '绑定'       | 群聊或私聊 | 发起绑定事件   |
 | 'bindinfo' 或 '绑定信息' | 仅私聊   | 查看账户绑定信息 |
 
 具体使用请看下图流程示例  
-![使用qq发送bind命令]('src/1.png')  
-![使用discord发送bind命令和token]('src/2.png')  
-![使用qq发送密钥确认绑定]('src/3.png')  
+(如果是在群聊中发起的绑定,不会显示下面的绑定信息,只会显示其他内容)
+![使用qq发送bind命令](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/1.png)  
+![使用discord发送bind命令和token](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/2.png)  
+![使用qq发送密钥确认绑定](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/3.png)  
 
 ## 开发者说明
 使用依赖注入获取用户信息的示例
 
-```
+```python
 from typing import Annotated
 
 from nonebot import require
 require('nonebot_plugin_bind')
 
 from nonebot_plugin_bind import GetUser
 
@@ -53,8 +69,9 @@
 async def __(event: Event, bot: Bot, matcher: Matcher, user: Annotated[User, GetUser()]):
     # 这里获取到的user可以访问属性来获取用户的具体账户信息,其中user.id是每个跨平台用户的唯一索引,也可以使用str()方法来转化成字符串
     if _is_private_(event, bot):
         await matcher.finish(f"当前账户的绑定信息如下:\n{str(user)}")
     else:
         await matcher.finish("账户绑定信息只能在私聊中查看")
 
-```
+```
+
```

