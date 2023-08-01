# Comparing `tmp/nonebot_plugin_bind-0.1.1.tar.gz` & `tmp/nonebot_plugin_bind-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bind-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_bind-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_bind-0.1.1.tar` & `nonebot_plugin_bind-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4098 2023-08-01 02:53:25.352916 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/__init__.py
--rw-r--r--   0        0        0      351 2023-08-01 02:53:25.344910 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/types.py
--rw-r--r--   0        0        0     7027 2023-08-01 03:05:37.685301 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/user_sql.py
--rw-r--r--   0        0        0     1489 2023-08-01 02:53:25.348915 nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/utils.py
--rw-r--r--   0        0        0      461 2023-08-01 03:37:58.822103 nonebot_plugin_bind-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2494 2023-08-01 03:37:47.563579 nonebot_plugin_bind-0.1.1/README.md
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4098 2023-08-01 02:53:25.352916 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/__init__.py
+-rw-r--r--   0        0        0      351 2023-08-01 02:53:25.344910 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/types.py
+-rw-r--r--   0        0        0     7027 2023-08-01 03:05:37.685301 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/user_sql.py
+-rw-r--r--   0        0        0     1489 2023-08-01 02:53:25.348915 nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/utils.py
+-rw-r--r--   0        0        0      522 2023-08-01 03:40:01.857921 nonebot_plugin_bind-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2526 2023-08-01 03:41:13.902443 nonebot_plugin_bind-0.1.2/README.md
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/__init__.py` & `nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/user_sql.py` & `nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/user_sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.1/nonebot_plugin_bind/utils.py` & `nonebot_plugin_bind-0.1.2/nonebot_plugin_bind/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bind-0.1.1/README.md` & `nonebot_plugin_bind-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 | 命令                  | 限制    | 含义       |
 |---------------------|-------|----------|
 | 'bind' 或 '绑定'       | 群聊或私聊 | 发起绑定事件   |
 | 'bindinfo' 或 '绑定信息' | 仅私聊   | 查看账户绑定信息 |
 
 具体使用请看下图流程示例  
-(如果是在群聊中发起的绑定,不会显示下面的绑定信息,只会显示其他内容)
-![使用qq发送bind命令](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/1.png)  
-![使用discord发送bind命令和token](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/2.png)  
-![使用qq发送密钥确认绑定](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/3.png)  
+(如果是在群聊中发起的绑定,不会显示下面的绑定信息,只会显示其他内容)  
+![使用qq发送bind命令](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/1.png)  
+![使用discord发送bind命令和token](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/2.png)  
+![使用qq发送密钥确认绑定](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/3.png)  
 
 ## 开发者说明
 使用依赖注入获取用户信息的示例
 
 ```python
 from typing import Annotated
```

### Comparing `nonebot_plugin_bind-0.1.1/PKG-INFO` & `nonebot_plugin_bind-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bind
-Version: 0.1.1
+Version: 0.1.2
 Summary: nonebot多平台账户信息绑定
+Home-page: https://github.com/canxin121/nonebot_plugin_bind
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -42,18 +43,18 @@
 
 | 命令                  | 限制    | 含义       |
 |---------------------|-------|----------|
 | 'bind' 或 '绑定'       | 群聊或私聊 | 发起绑定事件   |
 | 'bindinfo' 或 '绑定信息' | 仅私聊   | 查看账户绑定信息 |
 
 具体使用请看下图流程示例  
-(如果是在群聊中发起的绑定,不会显示下面的绑定信息,只会显示其他内容)
-![使用qq发送bind命令](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/1.png)  
-![使用discord发送bind命令和token](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/2.png)  
-![使用qq发送密钥确认绑定](https://github.com/canxin121/nonebot_plugin_bind/blob/main/src/3.png)  
+(如果是在群聊中发起的绑定,不会显示下面的绑定信息,只会显示其他内容)  
+![使用qq发送bind命令](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/1.png)  
+![使用discord发送bind命令和token](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/2.png)  
+![使用qq发送密钥确认绑定](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/3.png)  
 
 ## 开发者说明
 使用依赖注入获取用户信息的示例
 
 ```python
 from typing import Annotated
```

