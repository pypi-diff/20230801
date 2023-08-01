# Comparing `tmp/nonebot_plugin_bind-0.1.3.tar.gz` & `tmp/nonebot_plugin_bind-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bind-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_bind-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_bind-0.1.3.tar` & `nonebot_plugin_bind-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4586 2023-08-01 03:55:55.753846 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/__init__.py
--rw-r--r--   0        0        0      351 2023-08-01 02:53:25.344910 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/types.py
--rw-r--r--   0        0        0     7027 2023-08-01 03:05:37.685301 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/user_sql.py
--rw-r--r--   0        0        0     1489 2023-08-01 02:53:25.348915 nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/utils.py
--rw-r--r--   0        0        0      522 2023-08-01 04:08:48.387719 nonebot_plugin_bind-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2627 2023-08-01 04:07:03.126006 nonebot_plugin_bind-0.1.3/README.md
--rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5928 2023-08-01 10:13:17.266547 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 09:12:10.853222 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/_types.py
+-rw-r--r--   0        0        0     5414 2023-08-01 09:26:34.170289 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/user_sql.py
+-rw-r--r--   0        0        0     1078 2023-08-01 07:01:38.000000 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/utils.py
+-rw-r--r--   0        0        0      522 2023-08-01 09:34:12.103709 nonebot_plugin_bind-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3018 2023-08-01 10:20:30.698992 nonebot_plugin_bind-0.1.4/README.md
+-rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_bind-0.1.3/nonebot_plugin_bind/__init__.py` & `nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from nonebot import get_driver
 from nonebot import on_command
 from nonebot.adapters import Event, Bot
 from nonebot.matcher import Matcher
 from nonebot.params import ArgStr, T_State, CommandArg, RawCommand
 from nonebot.plugin import PluginMetadata
 
-from .types import Bind
-from .user_sql import edit_user, del_user, User
-from .utils import get_params, get_user, GetUser, _is_private_
+from ._types import Bind
+from .user_sql import User, merge_user, del_platform_user
+from .utils import GetUser, _is_private_
 
 __plugin_meta__ = PluginMetadata(
     name="跨平台账户绑定",
     description="nonebot多适配器通用的跨平台账户绑定插件",
-    usage="1.使用'bind'或'绑定'命令发起绑定事件\n2.使用'bindinfo'或'绑定信息'查看绑定信息",
+    usage="1.使用'bind'或'绑定'命令可以将其他通用账户绑定至当前通用账户\n2.使用'bindinfo'或'绑定信息'查看通用账户的平台账户绑定信息\n3.使用'rebind'或者'取消绑定'可以取消本平台账户和通用账户的绑定,并形成一个新的通用账户",
     type="library",
     homepage="https://github.com/canxin121/nonebot_plugin_bind",
     supported_adapters={"~onebot.v11", "~telegram", "~kaiheila", "~feishu", "~villa"},
 )
 
 SECONDS = str(get_driver().config.session_expire_timeout.seconds)
 
@@ -38,69 +38,94 @@
 
 @_bind_.handle()
 async def _bind__(bot: Bot,
                   event: Event,
                   matcher: Matcher,
                   state: T_State,
                   cmd: Annotated[str, RawCommand()],
-                  _token=CommandArg(), ):
+                  user: Annotated[User, GetUser()],
+                  _token=CommandArg(),
+                  ):
     global Binds
     if str(_token):
-        token = str(_token).replace(" ", "").replace("\n", "")
-        if len(token) == 6:
-            if token in Binds.keys():
-                Binds[token].params = get_params(bot, event)
-                user = await get_user(bot, event)
+        _token = str(_token).replace(" ", "").replace("\n", "")
+        if len(_token) == 6:
+            if _token in Binds.keys():
                 msg = ""
-                if user is not None:
-                    Binds[token].orgin_user = user
-                    if _is_private_(event, bot):
-                        msg += f"当前账户的绑定信息如下:\n{str(user)}"
-                msg += f"\n注意事项:\n1.绑定是将本平台账户绑定至刚才发送'{str(cmd)}'命令的平台的账户\n2.绑定后本平台账户所绑定的其他账户和信息都将丢失,替换至刚才发送'{str(cmd)}'命令的平台的账户的绑定信息\n\n使用方式:\b\n如果确认绑定,请用刚才发送'{str(cmd)}'命令的平台的账户在{SECONDS}秒内直接发送以下密钥:\n {Binds[token]._key}"
+                Binds[_token].origin_user = user
+                if _is_private_(event, bot):
+                    msg += f"当前通用账户的绑定的平台账户如下:\n{str(user)}"
+                msg += f"\n注意事项:\n1.此命令是将本通用账户的绑定信息迁移到刚才发送'{str(cmd)}'命令通用账户\n2.本命令会丢失以当前通用账户身份存储的所有数据,且不可逆,所以请小心使用\n\n使用方式:\b\n如果确认绑定,请用刚才发送'{str(cmd)}'命令的平台的账户在{SECONDS}秒内直接发送以下密钥:\n{Binds[_token]._key}"
                 await matcher.finish(msg)
             else:
                 await matcher.finish("密钥错误或已过期")
         else:
             await matcher.finish("密钥格式错误 或 请勿在初次发送bind命令时追加信息")
-    user = await get_user(bot, event)
-    _token = str(secrets.token_hex(3))
-    scheduler = AsyncIOScheduler()
-    scheduler.add_job(del_Bind, 'date', run_date=datetime.now() + timedelta(seconds=120), args=[_token])
-    scheduler.start()
-    bind = Bind(user)
-    state['_token'] = _token
-    Binds[_token] = bind
-    if _is_private_(event, bot):
-        msg = f"当前账户的绑定信息如下:\n{str(user)}"
     else:
-        msg = ""
-    msg += f'\n注意事项:\n1.绑定是将其他平台账户绑定至当前平台账户身份\n2.绑定后其他平台的账户所绑定的其他账户和信息都将丢失,替换为当前平台用户绑定信息\n\n使用方式:\b\n请用需要绑定的另一个平台的账号在{SECONDS}秒内发送以下内容:\n{str(cmd)} {_token}\n\n发送"取消"或"算了"可以终止绑定'
-    await matcher.send(msg)
+        _token = str(secrets.token_hex(3))
+        scheduler = AsyncIOScheduler()
+        scheduler.add_job(del_Bind, 'date', run_date=datetime.now() + timedelta(seconds=int(SECONDS)), args=[_token])
+        scheduler.start()
+        bind = Bind()
+        bind.to_user = user
+        state['_token'] = _token
+        Binds[_token] = bind
+        if _is_private_(event, bot):
+            msg = f"当前通用账户的绑定的平台账户如下:\n{str(user)}"
+        else:
+            msg = ""
+        msg += f'\n注意事项:\n1.一个通用账户可以绑定多个平台账户\n2.此命令是将另一个通用账户的绑定信息合并到当前通用账户\n3.本命令会丢失以另一个通用账户身份存储的所有数据,且不可逆,所以请小心使用\n\n使用方式:\b\n请用需要绑定的另一个平台的账号在{SECONDS}秒内发送以下内容:\n{str(cmd)} {_token}\n\n发送"取消"或"算了"可以终止绑定'
+        await matcher.send(msg)
 
 
 @_bind_.got("key")
 async def bind___(
         state: T_State,
         matcher: Matcher,
         args: str = ArgStr("key")):
     _token = state['_token']
     key = str(args).replace(" ", "").replace("\n", "")
     if key == Binds[_token]._key:
-        if Binds[_token].orgin_user is not None:
-            await del_user(Binds[_token].orgin_user)
-        await edit_user(Binds[_token].user, **Binds[_token].params)
-        del Binds[_token]
-        await matcher.finish("成功绑定至本平台账户")
+        try:
+            await merge_user(Binds[_token].to_user, Binds[_token].origin_user)
+        except Exception as e:
+            raise e
+        finally:
+            del Binds[_token]
+        await matcher.finish("成功绑定至本通用账户")
     elif key in ["取消", "算了", "结束"]:
         del_Bind(_token)
         await matcher.finish("取消绑定")
 
 
 _bind_info_ = on_command("bindinfo", aliases={"绑定信息"})
 
 
 @_bind_info_.handle()
 async def __(event: Event, bot: Bot, matcher: Matcher, user: Annotated[User, GetUser()]):
     if _is_private_(event, bot):
-        await matcher.finish(f"当前账户的绑定信息如下:\n{str(user)}")
+        await matcher.finish(f"当前通用账户的绑定的平台账户如下:\n{str(user)}")
     else:
         await matcher.finish("账户绑定信息只能在私聊中查看")
+
+
+_re_bind_ = on_command("rebind", aliases={"取消绑定"})
+
+
+@_re_bind_.handle()
+async def _re_bind___(event: Event, bot: Bot, state: T_State, matcher: Matcher, user: Annotated[User, GetUser()]):
+    state['user'] = user
+    msg = ""
+    if _is_private_(event, bot):
+        msg += f"当前账户的绑定信息如下:\n{str(user)}\n\n"
+    msg += "注意事项:\n1.取消绑定仅是将本平台账户独立开来,并形成新的通用账户,而不会影响剩余绑定在一起的平台账户\n2.取消绑定是可逆的,只需要再次绑定即可\n\n确定要将本平台账户独立开来吗?\n输入'确定' 或 'ok'来确认执行,其他任意语句取消操作"
+    await matcher.send(msg)
+
+
+@_re_bind_.got("arg")
+async def _re_bind_confirm(event: Event, bot: Bot, state: T_State, matcher: Matcher, arg: str = ArgStr("arg")):
+    user = state['user']
+    if str(arg) in ['确定', 'ok']:
+        await del_platform_user(user, platform=bot.adapter.get_name(), account=event.get_user_id())
+        await matcher.finish("成功取消绑定")
+    else:
+        await matcher.finish("取消操作")
```

### Comparing `nonebot_plugin_bind-0.1.3/pyproject.toml` & `nonebot_plugin_bind-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-bind"
-version = "0.1.3"
+version = "0.1.4"
 description = "nonebot多平台账户信息绑定"
 authors = ["canxin <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_bind" }]
 homepage = 'https://github.com/canxin121/nonebot_plugin_bind'
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_bind-0.1.3/README.md` & `nonebot_plugin_bind-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -25,41 +25,42 @@
 - kook(开黑啦)
 - villa(大别野)
 - 飞书
 # 使用说明
 
 ## 用户使用说明
 
-| 命令                  | 限制    | 含义       |
-|---------------------|-------|----------|
-| 'bind' 或 '绑定'       | 群聊或私聊 | 发起绑定事件   |
-| 'bindinfo' 或 '绑定信息' | 仅私聊   | 查看账户绑定信息 |
+| 命令                  | 限制    | 含义                          |
+|---------------------|-------|-----------------------------|
+| 'bind' 或 '绑定'       | 群聊或私聊 | 将其他通用账户绑定至当前通用账户            |
+| 'bindinfo' 或 '绑定信息' | 仅私聊   | 查看当前通用账户的平台账户绑定信息           |
+| 'rebind' 或 '取消绑定'   | 仅私聊   | 取消本平台账户和通用账户的绑定,并形成一个新的通用账户 |
 
 具体使用请看下图流程示例  
 (如果是在群聊中发起的绑定,不会显示下面的绑定信息,只会显示其他内容)  
 ![使用qq发送bind命令](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/1.png)  
 ![使用discord发送bind命令和token](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/2.png)  
 ![使用qq发送密钥确认绑定](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/3.png)  
+![取消绑定](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/4.png)  
 
 ## 开发者说明
-使用依赖注入获取用户信息的示例
+使用依赖注入获取用户信息的示例  
+注入后获得的user是一个通用账户的class,其属性id是可以用来区分不同通用账户的唯一值,另一个属性platform_users储存通用账户绑定的所有的平台账户的信息  
 
 ```python
 from typing import Annotated
 
 from nonebot import require
 require('nonebot_plugin_bind')
 
 from nonebot_plugin_bind import GetUser
 
 _bind_info_ = on_command("bindinfo", aliases={"绑定信息"})
 
 
 @_bind_info_.handle()
-async def __(event: Event, bot: Bot, matcher: Matcher, user: Annotated[User, GetUser()]):
-    # 这里获取到的user可以访问属性来获取用户的具体账户信息,其中user.id是每个跨平台用户的唯一索引,也可以使用str()方法来转化成字符串
+async def _bind_info____(event: Event, bot: Bot, matcher: Matcher, user: Annotated[User, GetUser()]):
     if _is_private_(event, bot):
-        await matcher.finish(f"当前账户的绑定信息如下:\n{str(user)}")
+        await matcher.finish(f"当前通用账户的绑定的平台账户如下:\n{str(user)}")
     else:
         await matcher.finish("账户绑定信息只能在私聊中查看")
-
 ```
```

### Comparing `nonebot_plugin_bind-0.1.3/PKG-INFO` & `nonebot_plugin_bind-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bind
-Version: 0.1.3
+Version: 0.1.4
 Summary: nonebot多平台账户信息绑定
 Home-page: https://github.com/canxin121/nonebot_plugin_bind
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -44,42 +44,43 @@
 - kook(开黑啦)
 - villa(大别野)
 - 飞书
 # 使用说明
 
 ## 用户使用说明
 
-| 命令                  | 限制    | 含义       |
-|---------------------|-------|----------|
-| 'bind' 或 '绑定'       | 群聊或私聊 | 发起绑定事件   |
-| 'bindinfo' 或 '绑定信息' | 仅私聊   | 查看账户绑定信息 |
+| 命令                  | 限制    | 含义                          |
+|---------------------|-------|-----------------------------|
+| 'bind' 或 '绑定'       | 群聊或私聊 | 将其他通用账户绑定至当前通用账户            |
+| 'bindinfo' 或 '绑定信息' | 仅私聊   | 查看当前通用账户的平台账户绑定信息           |
+| 'rebind' 或 '取消绑定'   | 仅私聊   | 取消本平台账户和通用账户的绑定,并形成一个新的通用账户 |
 
 具体使用请看下图流程示例  
 (如果是在群聊中发起的绑定,不会显示下面的绑定信息,只会显示其他内容)  
 ![使用qq发送bind命令](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/1.png)  
 ![使用discord发送bind命令和token](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/2.png)  
 ![使用qq发送密钥确认绑定](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/3.png)  
+![取消绑定](https://raw.githubusercontent.com/canxin121/nonebot_plugin_bind/main/src/4.png)  
 
 ## 开发者说明
-使用依赖注入获取用户信息的示例
+使用依赖注入获取用户信息的示例  
+注入后获得的user是一个通用账户的class,其属性id是可以用来区分不同通用账户的唯一值,另一个属性platform_users储存通用账户绑定的所有的平台账户的信息  
 
 ```python
 from typing import Annotated
 
 from nonebot import require
 require('nonebot_plugin_bind')
 
 from nonebot_plugin_bind import GetUser
 
 _bind_info_ = on_command("bindinfo", aliases={"绑定信息"})
 
 
 @_bind_info_.handle()
-async def __(event: Event, bot: Bot, matcher: Matcher, user: Annotated[User, GetUser()]):
-    # 这里获取到的user可以访问属性来获取用户的具体账户信息,其中user.id是每个跨平台用户的唯一索引,也可以使用str()方法来转化成字符串
+async def _bind_info____(event: Event, bot: Bot, matcher: Matcher, user: Annotated[User, GetUser()]):
     if _is_private_(event, bot):
-        await matcher.finish(f"当前账户的绑定信息如下:\n{str(user)}")
+        await matcher.finish(f"当前通用账户的绑定的平台账户如下:\n{str(user)}")
     else:
         await matcher.finish("账户绑定信息只能在私聊中查看")
-
 ```
```

