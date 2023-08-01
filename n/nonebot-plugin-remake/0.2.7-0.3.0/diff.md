# Comparing `tmp/nonebot_plugin_remake-0.2.7.tar.gz` & `tmp/nonebot_plugin_remake-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_remake-0.2.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_remake-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_remake-0.2.7.tar` & `nonebot_plugin_remake-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,27 @@
--rw-r--r--   0        0        0     1063 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/LICENSE
--rw-r--r--   0        0        0     1164 2022-06-21 14:58:14.380000 nonebot_plugin_remake-0.2.7/README.md
--rw-r--r--   0        0        0     5590 2022-10-03 06:58:13.080000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/__init__.py
--rw-r--r--   0        0        0      679 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/age.py
--rw-r--r--   0        0        0     3138 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/event.py
--rw-r--r--   0        0        0     1794 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/life.py
--rw-r--r--   0        0        0     5405 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/property.py
--rw-r--r--   0        0        0  1967564 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/resources/age.json
--rw-r--r--   0        0        0   365677 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/resources/events.json
--rw-r--r--   0        0        0    29583 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/resources/talents.json
--rw-r--r--   0        0        0     3258 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/talent.py
--rw-r--r--   0        0        0      960 2022-06-20 15:38:57.520000 nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/utils.py
--rw-r--r--   0        0        0      610 2022-10-03 06:58:22.190000 nonebot_plugin_remake-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2009 2022-10-03 06:59:10.593313 nonebot_plugin_remake-0.2.7/setup.py
--rw-r--r--   0        0        0     1917 2022-10-03 06:59:10.593558 nonebot_plugin_remake-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1164 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/README.md
+-rw-r--r--   0        0        0     7728 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/__init__.py
+-rw-r--r--   0        0        0      679 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/age.py
+-rw-r--r--   0        0        0      127 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/config.py
+-rw-r--r--   0        0        0    11874 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/drawer.py
+-rw-r--r--   0        0        0     3138 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/event.py
+-rw-r--r--   0        0        0     2596 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/life.py
+-rw-r--r--   0        0        0     6700 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/property.py
+-rw-r--r--   0        0        0  1967733 2023-08-01 18:43:54.676067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/age.json
+-rw-r--r--   0        0        0   377196 2023-08-01 18:43:54.676067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/events.json
+-rw-r--r--   0        0        0    29584 2023-08-01 18:43:54.676067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/talents.json
+-rw-r--r--   0        0        0  1895036 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/fonts/方正像素12.ttf
+-rw-r--r--   0        0        0     9336 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/bg_summary.png
+-rw-r--r--   0        0        0     6810 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/bg_talent.png
+-rw-r--r--   0        0        0     4590 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_chr.png
+-rw-r--r--   0        0        0     1586 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_int.png
+-rw-r--r--   0        0        0      904 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_mny.png
+-rw-r--r--   0        0        0     3319 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_spr.png
+-rw-r--r--   0        0        0     2873 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_str.png
+-rw-r--r--   0        0        0      195 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/title_left.png
+-rw-r--r--   0        0        0      208 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/title_right.png
+-rw-r--r--   0        0        0    86169 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/titlebar.png
+-rw-r--r--   0        0        0     3258 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/talent.py
+-rw-r--r--   0        0        0      960 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/utils.py
+-rw-r--r--   0        0        0      664 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 nonebot_plugin_remake-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_remake-0.2.7/LICENSE` & `nonebot_plugin_remake-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.2.7/README.md` & `nonebot_plugin_remake-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/__init__.py` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,89 @@
-import re
-import random
 import itertools
+import random
+import re
 import traceback
-from typing import List, Tuple, Optional
+from io import BytesIO
+from typing import List, Optional, Tuple
 
-from nonebot import on_command
+from nonebot import get_driver, on_command, require
+from nonebot.adapters import Bot, Event
+from nonebot.log import logger
+from nonebot.params import ArgPlainText
+from nonebot.plugin import PluginMetadata
 from nonebot.rule import to_me
 from nonebot.typing import T_State
-from nonebot.plugin import PluginMetadata
-from nonebot.params import ArgPlainText
-from nonebot.adapters.onebot.v11 import (
-    Bot,
-    MessageEvent,
-    GroupMessageEvent,
-)
-from nonebot.log import logger
+from nonebot.utils import run_sync
+
+require("nonebot_plugin_saa")
 
-from .life import Life
+from nonebot_plugin_saa import Image, MessageFactory
+from nonebot_plugin_saa import __plugin_meta__ as saa_plugin_meta
+
+from .config import Config
+from .drawer import draw_life, save_jpg
+from .life import Life, PerAgeProperty, PerAgeResult
+from .property import Summary
 from .talent import Talent
 
 __plugin_meta__ = PluginMetadata(
     name="人生重开",
     description="人生重开模拟器",
     usage="@我 remake/liferestart/人生重开",
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-remake",
+    config=Config,
+    supported_adapters=saa_plugin_meta.supported_adapters,
     extra={
         "unique_name": "remake",
         "example": "@小Q remake",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.2.7",
+        "version": "0.3.0",
     },
 )
 
+remake_config = Config.parse_obj(get_driver().config.dict())
+
+onebot_v11_loaded = False
+if remake_config.remake_send_forword_msg:
+    try:
+        from nonebot.adapters.onebot.v11 import Bot as V11Bot
+        from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
+        from nonebot.adapters.onebot.v11 import MessageEvent as V11MEvent
+
+        def is_onebot_v11(bot: Bot):
+            return isinstance(bot, V11Bot)
+
+        async def send_forward_msg(
+            bot: V11Bot,
+            event: V11MEvent,
+            name: str,
+            uin: str,
+            msgs: List[str],
+        ):
+            def to_json(msg):
+                return {
+                    "type": "node",
+                    "data": {"name": name, "uin": uin, "content": msg},
+                }
+
+            messages = [to_json(msg) for msg in msgs]
+            if isinstance(event, V11GMEvent):
+                await bot.call_api(
+                    "send_group_forward_msg", group_id=event.group_id, messages=messages
+                )
+            else:
+                await bot.call_api(
+                    "send_private_forward_msg", user_id=event.user_id, messages=messages
+                )
+
+        onebot_v11_loaded = True
+    except ImportError:
+        logger.warning("无法加载 OneBot V11 适配器，发送转发消息设置失效")
+
 
 remake = on_command(
     "remake",
     aliases={"liferestart", "人生重开", "人生重来"},
     block=True,
     rule=to_me(),
     priority=12,
@@ -52,15 +101,15 @@
     des = "\n".join([f"{i}.{t}" for i, t in enumerate(talents)])
     await remake.send(f"{msg}\n\n{des}")
 
 
 @remake.got("nums")
 async def _(state: T_State, reply: str = ArgPlainText("nums")):
     def conflict_talents(talents: List[Talent]) -> Optional[Tuple[Talent, Talent]]:
-        for (t1, t2) in itertools.combinations(talents, 2):
+        for t1, t2 in itertools.combinations(talents, 2):
             if t1.exclusive_with(t2):
                 return t1, t2
         return None
 
     life_: Life = state["life"]
     talents: List[Talent] = state["talents"]
 
@@ -97,15 +146,15 @@
     )
     await remake.send(msg)
 
 
 @remake.got("prop")
 async def _(
     bot: Bot,
-    event: MessageEvent,
+    event: Event,
     state: T_State,
     reply: str = ArgPlainText("prop"),
 ):
     life_: Life = state["life"]
     talents: List[Talent] = state["talents_selected"]
     total_prop = life_.total_property()
 
@@ -130,46 +179,57 @@
         await remake.finish("人生重开已取消")
 
     prop = {"CHR": nums[0], "INT": nums[1], "STR": nums[2], "MNY": nums[3]}
     life_.apply_property(prop)
 
     await remake.send("你的人生正在重开...")
 
-    msgs = [
-        "已选择以下天赋：\n" + "\n".join([str(t) for t in talents]),
-        "已设置如下属性：\n" + f"颜值{nums[0]} 智力{nums[1]} 体质{nums[2]} 家境{nums[3]}",
-    ]
+    init_prop = life_.get_property()
+    results = [result for result in life_.run()]
+    summary = life_.gen_summary()
+
     try:
-        life_msgs = []
-        for s in life_.run():
-            life_msgs.append("\n".join(s))
-        n = 5
-        life_msgs = [
-            "\n\n".join(life_msgs[i : i + n]) for i in range(0, len(life_msgs), n)
-        ]
-        msgs.extend(life_msgs)
-        msgs.append(life_.gen_summary())
-        await send_forward_msg(bot, event, "人生重开模拟器", bot.self_id, msgs)
+        if (
+            remake_config.remake_send_forword_msg
+            and onebot_v11_loaded
+            and is_onebot_v11(bot)
+        ):
+            assert isinstance(bot, V11Bot)
+            assert isinstance(event, V11MEvent)
+            msgs = get_life_msgs(talents, init_prop, results, summary)
+            await send_forward_msg(bot, event, "人生重开模拟器", bot.self_id, msgs)
+            return
+
+        img = await get_life_img(talents, init_prop, results, summary)
+        await MessageFactory(Image(img)).send()
     except:
         logger.warning(traceback.format_exc())
         await remake.finish("你的人生重开失败（")
 
 
-async def send_forward_msg(
-    bot: Bot,
-    event: MessageEvent,
-    name: str,
-    uin: str,
-    msgs: List[str],
-):
-    def to_json(msg):
-        return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
+@run_sync
+def get_life_img(
+    talents: List[Talent],
+    init_prop: PerAgeProperty,
+    results: List[PerAgeResult],
+    summary: Summary,
+) -> BytesIO:
+    return save_jpg(draw_life(talents, init_prop, results, summary))
 
-    messages = [to_json(msg) for msg in msgs]
-    if isinstance(event, GroupMessageEvent):
-        await bot.call_api(
-            "send_group_forward_msg", group_id=event.group_id, messages=messages
-        )
-    else:
-        await bot.call_api(
-            "send_private_forward_msg", user_id=event.user_id, messages=messages
-        )
+
+def get_life_msgs(
+    talents: List[Talent],
+    init_prop: PerAgeProperty,
+    results: List[PerAgeResult],
+    summary: Summary,
+):
+    msgs = [
+        "已选择以下天赋：\n" + "\n".join([str(t) for t in talents]),
+        "已设置如下属性：\n"
+        + f"颜值{init_prop.CHR} 智力{init_prop.INT} 体质{init_prop.STR} 家境{init_prop.MNY}",
+    ]
+    life_msgs = [str(result) for result in results]
+    n = 5
+    life_msgs = ["\n\n".join(life_msgs[i : i + n]) for i in range(0, len(life_msgs), n)]
+    msgs.extend(life_msgs)
+    msgs.append(str(summary))
+    return msgs
```

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/age.py` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/age.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from pathlib import Path
-from typing import List, Dict
+from typing import Dict, List
 
-from .property import Property
 from .event import WeightedEvent
+from .property import Property
 
 
 class AgeManager:
     def __init__(self, prop: Property):
         self.prop = prop
         self.ages: Dict[int, List[WeightedEvent]] = {}
```

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/event.py` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/resources/age.json` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/age.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999990745430696%*

 * *Differences: {"'53'": "{'event': {insert: [(198, '21326'), (199, '21327')]}}",*

 * * "'54'": "{'event': {insert: [(198, '21326'), (199, '21327')]}}",*

 * * "'55'": "{'event': {insert: [(198, '21326'), (199, '21327')]}}",*

 * * "'56'": "{'event': {insert: [(189, '21326'), (190, '21327')]}}"}*

```diff
@@ -62579,14 +62579,16 @@
             "11447*0.05",
             "11448*0.05",
             "11449*0.05",
             "11450*0.05",
             "20567*0.01",
             "11497*0.05",
             "11498*0.05",
+            "21326",
+            "21327",
             "40065*1000000000000000000",
             "40066*100000000000000000",
             "40067*100000000000000000",
             "40068*100000000000000000",
             "40069*100000000000000000",
             "40070*10000000000000000",
             "40071*10000000000000000",
@@ -62800,14 +62802,16 @@
             "11447*0.05",
             "11448*0.05",
             "11449*0.05",
             "11450*0.05",
             "11497*0.05",
             "11498*0.05",
             "11499*0.1",
+            "21326",
+            "21327",
             "40065*1000000000000000000",
             "40066*100000000000000000",
             "40067*100000000000000000",
             "40068*100000000000000000",
             "40069*100000000000000000",
             "40070*10000000000000000",
             "40071*10000000000000000",
@@ -63021,14 +63025,16 @@
             "11472*0.1",
             "11473*0.1",
             "11474*0.1",
             "11497*0.05",
             "11498*0.05",
             "11499*0.1",
             "10426*0.1",
+            "21326",
+            "21327",
             "40065*1000000000000000000",
             "40066*100000000000000000",
             "40067*100000000000000000",
             "40068*100000000000000000",
             "40069*100000000000000000",
             "40070*10000000000000000",
             "40071*10000000000000000",
@@ -63233,14 +63239,16 @@
             "11493*0.05",
             "11494*0.05",
             "11495*0.05",
             "11497*0.05",
             "11498*0.05",
             "11499*0.1",
             "10426*0.1",
+            "21326",
+            "21327",
             "40065*1000000000000000000",
             "40066*100000000000000000",
             "40067*100000000000000000",
             "40068*100000000000000000",
             "40069*100000000000000000",
             "40070*10000000000000000",
             "40071*10000000000000000",
```

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/resources/events.json` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/events.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9647781228433452%*

 * *Differences: {"'10004'": "{'grade': 2}",*

 * * "'10006'": "{'grade': 2}",*

 * * "'10007'": "{'exclude': '(MNY<3)|(EVT?[10007,10008,20007,20008])'}",*

 * * "'10008'": "{'exclude': '(MNY<3)|(EVT?[10007,10008,20007,20008])'}",*

 * * "'10011'": "{'grade': 2}",*

 * * "'10018'": "{'grade': 1}",*

 * * "'10019'": "{'grade': 1}",*

 * * "'10027'": "{'grade': 1}",*

 * * "'10035'": "{'exclude': '(EVT?[10035,20035])|(TLT?[1011])'}",*

 * * "'10036'": "{'exclude': 'EVT?[10011,10024,10016,10017,10036,10037,10038,20037,20038]'}",*

 * * "'10048'": "{'exclude': 'EVT?[10048,20048]'}",*

 * * "' […]*

```diff
@@ -30,14 +30,15 @@
         "exclude": "STR>6",
         "id": 10003,
         "postEvent": "\u5bb6\u91cc\u82b1\u4e86\u4e0d\u5c11\u94b1\u3002"
     },
     "10004": {
         "NoRandom": 1,
         "event": "\u53ef\u80fd\u662f\u7389\u4f69\u4fdd\u4f51\uff0c\u4f60\u6d3b\u4e86\u4e0b\u6765\u3002",
+        "grade": 2,
         "id": 10004
     },
     "10005": {
         "branch": [
             "TLT?[1002]:10006",
             "STR<3&MNY<3:10000"
         ],
@@ -45,39 +46,40 @@
         "exclude": "INT>7",
         "id": 10005,
         "postEvent": "\u53d7\u4e86\u8f7b\u4f24\u3002"
     },
     "10006": {
         "NoRandom": 1,
         "event": "\u7ea2\u809a\u515c\u6302\u5728\u4e86\u684c\u89d2\u4e0a\uff0c\u4f60\u6ca1\u6709\u53d7\u4f24\u3002",
+        "grade": 2,
         "id": 10006
     },
     "10007": {
         "branch": [
             "INT>5:20008",
             "CHR>5:20007"
         ],
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u5f00\u59cb\u770b\u52a8\u6f2b\u3002",
-        "exclude": "(MNY<3)|(EVT?[10007,10008])",
+        "exclude": "(MNY<3)|(EVT?[10007,10008,20007,20008])",
         "id": 10007,
         "include": "TLT?[1005]"
     },
     "10008": {
         "branch": [
             "INT>5:20008",
             "CHR>5:20007"
         ],
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u5f00\u59cb\u770b\u52a8\u6f2b\u3002",
-        "exclude": "(MNY<3)|(EVT?[10007,10008])",
+        "exclude": "(MNY<3)|(EVT?[10007,10008,20007,20008])",
         "id": 10008
     },
     "10009": {
         "event": "\u4f60\u4ece\u5c0f\u751f\u6d3b\u5728\u519c\u6751",
         "exclude": "TLT?[1010,1013,1014]",
         "id": 10009,
         "include": "(MNY<8)|(TLT?[1012])"
@@ -87,14 +89,15 @@
         "exclude": "TLT?[1012,1014]",
         "id": 10010,
         "include": "(MNY>1)|(TLT?[1010,1013])"
     },
     "10011": {
         "event": "\u4f60\u51fa\u751f\u5728\u7f8e\u5229\u575a\uff0c\u62e5\u6709\u7f8e\u56fd\u56fd\u7c4d",
         "exclude": "TLT?[1010,1012]",
+        "grade": 2,
         "id": 10011,
         "include": "(MNY>8)|(TLT?[1014])"
     },
     "10012": {
         "branch": [
             "MNY<2:10013"
         ],
@@ -166,25 +169,27 @@
     "10018": {
         "effect": {
             "MNY": 2,
             "SPR": 1
         },
         "event": "\u4f60\u7684\u7236\u4eb2\u5728\u79cd\u5730\u65f6\u610f\u5916\u53d1\u73b0\u4e00\u7bb1\u91d1\u6761\u3002",
         "exclude": "EVT?[10018,10017]",
+        "grade": 1,
         "id": 10018,
         "include": "EVT?[10009]",
         "postEvent": "\u5bb6\u5883\u6709\u6240\u597d\u8f6c\u3002"
     },
     "10019": {
         "effect": {
             "SPR": 1,
             "STR": 1
         },
         "event": "\u4f60\u7684\u7236\u6bcd\u5bf9\u4f60\u89c6\u82e5\u73cd\u5b9d\uff0c\u5475\u62a4\u5907\u81f3\u3002",
         "exclude": "EVT?[10015,10016,10017,10019]",
+        "grade": 1,
         "id": 10019
     },
     "10020": {
         "effect": {
             "INT": -1
         },
         "event": "\u4f60\u5929\u8d44\u806a\u9896\uff0c\u4f46\u5bb6\u4eba\u5e76\u4e0d\u61c2\u5982\u4f55\u57f9\u517b\u3002",
@@ -251,14 +256,15 @@
     "10027": {
         "effect": {
             "MNY": 2,
             "SPR": 1
         },
         "event": "\u4f60\u7684\u6bcd\u4eb2\u6551\u4e86\u4e2a\u4eba\uff0c\u5f97\u5230\u4e86\u5f88\u591a\u611f\u8c22\u91d1\u3002",
         "exclude": "EVT?[10027,10016]",
+        "grade": 1,
         "id": 10027,
         "include": "EVT?[10009]",
         "postEvent": "\u5bb6\u5883\u6709\u6240\u597d\u8f6c\u3002"
     },
     "10028": {
         "branch": [
             "CHR>7:20029",
@@ -341,28 +347,28 @@
         "branch": [
             "CHR>7:20035"
         ],
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u7684\u5927\u59d0\u51fa\u5ac1\uff0c\u6536\u4e86\u5f88\u591a\u5f69\u793c\u3002",
-        "exclude": "(EVT?[10035])|(TLT?[1011])",
+        "exclude": "(EVT?[10035,20035])|(TLT?[1011])",
         "id": 10035,
         "include": "EVT?[10009]"
     },
     "10036": {
         "branch": [
             "INT>8:20037",
             "INT>5:20038"
         ],
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u559c\u6b22\u7528\u7236\u6bcd\u7684\u624b\u673a\u73a9\u738b\u8005\u8363\u8000\u3002",
-        "exclude": "EVT?[10011,10024,10016,10017,10036,10037,10038]",
+        "exclude": "EVT?[10011,10024,10016,10017,10036,10037,10038,20037,20038]",
         "id": 10036,
         "include": "MNY>2"
     },
     "10037": {
         "effect": {
             "SPR": 1
         },
@@ -466,15 +472,15 @@
         "include": "EVT?[10009]"
     },
     "10048": {
         "branch": [
             "(EVT?[10009])&(CHR<3):20048"
         ],
         "event": "\u4f60\u7684\u7ed8\u753b\u5929\u8d4b\u597d\u50cf\u4e0d\u9519\u3002",
-        "exclude": "EVT?[10048]",
+        "exclude": "EVT?[10048,20048]",
         "id": 10048
     },
     "10049": {
         "branch": [
             "(EVT?[10009])&(CHR<3):20049"
         ],
         "event": "\u4f60\u7684\u97f3\u4e50\u5929\u8d4b\u597d\u50cf\u4e0d\u9519\u3002",
@@ -522,22 +528,24 @@
     },
     "10055": {
         "NoRandom": 1,
         "branch": [
             "INT>9:10056"
         ],
         "event": "\u4f60\u5bf9\u81ea\u7136\u89c4\u5f8b\u6709\u6240\u89c2\u5bdf\u3002",
+        "grade": 1,
         "id": 10055
     },
     "10056": {
         "NoRandom": 1,
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u5bf9\u690d\u7269\u548c\u517b\u751f\u6709\u6240\u9886\u609f\u3002",
+        "grade": 2,
         "id": 10056
     },
     "10057": {
         "event": "\u4f60\u5f00\u59cb\u4e0b\u5730\u5e72\u519c\u6d3b\u3002",
         "exclude": "EVT?[10057,10025]",
         "id": 10057,
         "include": "EVT?[10009]"
@@ -693,14 +701,15 @@
     "10074": {
         "NoRandom": 1,
         "effect": {
             "MNY": 2,
             "SPR": 2
         },
         "event": "\u4f60\u60f3\u65b9\u8bbe\u6cd5\u6253\u5f00\u4e86\u9501\u3002",
+        "grade": 1,
         "id": 10074,
         "postEvent": "\u91cc\u9762\u6709\u5927\u91cf\u73e0\u5b9d\u3002"
     },
     "10075": {
         "branch": [
             "INT<3:20075"
         ],
@@ -708,38 +717,43 @@
         "exclude": "EVT?[10075]",
         "id": 10075,
         "include": "STR>8"
     },
     "10076": {
         "event": "\u4f60\u53d1\u73b0\u52a8\u7269\u597d\u50cf\u90fd\u4e0d\u600e\u4e48\u5bb3\u6015\u4f60\u3002",
         "exclude": "EVT?[10076,10052]",
+        "grade": 1,
         "id": 10076,
         "include": "(CHR>9)&(EVT?[10009])"
     },
     "10077": {
         "event": "\u4f60\u53d1\u73b0\u4f60\u548c\u5176\u4ed6\u4eba\u7684\u60f3\u6cd5\u597d\u50cf\u90fd\u4e0d\u4e00\u6837\u3002",
         "exclude": "EVT?[10077,10090]",
+        "grade": 1,
         "id": 10077,
         "include": "INT>9"
     },
     "10078": {
         "event": "\u4f60\u4eec\u5bb6\u6210\u4e3a\u6751\u91cc\u6700\u5bcc\u7684\u5bb6\u5ead\u3002",
         "exclude": "EVT?[10078,10025]",
+        "grade": 1,
         "id": 10078,
         "include": "(MNY>7)&(EVT?[10009])"
     },
     "10079": {
         "event": "\u4f60\u7684\u9ad8\u989c\u503c\u5df2\u7ecf\u5728\u5468\u8fb9\u5bb6\u55bb\u6237\u6653\u3002",
         "exclude": "EVT?[10079]",
+        "grade": 1,
         "id": 10079,
         "include": "(CHR>7)&(EVT?[10009])"
     },
     "10080": {
         "event": "\u6709\u4eba\u5c06\u4f60\u53d1\u5728\u4e86\u7f51\u4e0a\uff0c\u4f60\u5c0f\u6709\u540d\u6c14\u3002",
         "exclude": "EVT?[10080]",
+        "grade": 2,
         "id": 10080,
         "include": "(CHR>8)&(EVT?[10079])",
         "postEvent": "\u5f88\u591a\u4eba\u6765\u4f60\u5bb6\u62cd\u77ed\u89c6\u9891\u3002"
     },
     "10081": {
         "branch": [
             "STR>5&MNY<5:10082"
@@ -809,14 +823,15 @@
     },
     "10087": {
         "effect": {
             "MNY": 2
         },
         "event": "\u4f60\u5df2\u7ecf\u8d22\u52a1\u81ea\u7531\uff0c\u4e0d\u518d\u51fa\u5356\u8eab\u4f53\u3002",
         "exclude": "EVT?[10087]",
+        "grade": 1,
         "id": 10087,
         "include": "EVT?[10084,20056]"
     },
     "10088": {
         "effect": {
             "SPR": 2
         },
@@ -827,28 +842,30 @@
     },
     "10089": {
         "effect": {
             "MNY": 1,
             "SPR": 1
         },
         "event": "\u56fd\u5bb6\u6276\u8d2b\uff0c\u4f60\u5bb6\u83b7\u5f97\u4e86\u5e2e\u52a9\u3002",
+        "grade": 1,
         "id": 10089,
         "include": "(MNY<4)&(EVT?[10009])"
     },
     "10090": {
         "branch": [
             "STR<5:10000"
         ],
         "effect": {
             "INT": -1,
             "SPR": -1,
             "STR": -1
         },
         "event": "\u4f60\u7684\u667a\u529b\u8fc7\u9ad8\uff0c\u88ab\u5916\u661f\u4eba\u6293\u8d70\u505a\u5b9e\u9a8c\u3002",
         "exclude": "EVT?[10090]",
+        "grade": 1,
         "id": 10090,
         "include": "INT>9",
         "postEvent": "\u53c8\u653e\u4e86\u56de\u6765\u3002"
     },
     "10091": {
         "branch": [
             "(INT>9)&(CHR<3):20091",
@@ -969,14 +986,15 @@
         "exclude": "EVT?[10105,10025]",
         "id": 10105,
         "include": "EVT?[10101]"
     },
     "10106": {
         "event": "\u4f60\u671f\u672b\u8003\u8bd5\u8003\u4e86100\u5206\u3002",
         "exclude": "EVT?[10106]",
+        "grade": 1,
         "id": 10106,
         "include": "(INT>7)&(EVT?[10101])"
     },
     "10107": {
         "effect": {
             "SPR": -1
         },
@@ -1000,19 +1018,21 @@
         "exclude": "EVT?[10109,10113,10114]",
         "id": 10109,
         "include": "(CHR>7)&(EVT?[10101])"
     },
     "10110": {
         "event": "\u4f60\u51fa\u751f\u4e86\uff0c\u662f\u6781\u4e3a\u7f55\u89c1\u7684\u65e0\u6027\u4eba\u3002",
         "exclude": "TLT?[1003,1004,1024,1113]",
+        "grade": 2,
         "id": 10110
     },
     "10111": {
         "event": "\u4f60\u51fa\u751f\u4e86\uff0c\u662f\u6781\u4e3a\u7f55\u89c1\u7684\u53cc\u6027\u4eba\u3002",
         "exclude": "TLT?[1003,1004,1025]",
+        "grade": 2,
         "id": 10111
     },
     "10112": {
         "effect": {
             "SPR": -2
         },
         "event": "\u540c\u5b66\u603b\u662f\u6b3a\u8d1f\u4f60\u3002",
@@ -1061,14 +1081,15 @@
     },
     "10117": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u5f53\u4e0a\u4e86\u73ed\u957f\u3002",
         "exclude": "EVT?[10117]",
+        "grade": 1,
         "id": 10117,
         "include": "(CHR>3)&(INT>6)&(EVT?[10101])"
     },
     "10118": {
         "event": "\u4f60\u5f53\u4e0a\u4e86\u9886\u64cd\u5458\u3002",
         "exclude": "EVT?[10118]",
         "id": 10118,
@@ -1179,22 +1200,24 @@
         "include": "(INT>4)&(EVT?[10101])"
     },
     "10132": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u83b7\u8bc4\u4e09\u597d\u5b66\u751f\u3002",
+        "grade": 1,
         "id": 10132,
         "include": "(STR>5)&(INT>5)&(EVT?[10101])"
     },
     "10133": {
         "effect": {
             "SPR": 2
         },
         "event": "\u4f60\u83b7\u8bc4\u4e09\u597d\u6807\u5175\u3002",
+        "grade": 1,
         "id": 10133,
         "include": "(STR>7)&(INT>7)&(EVT?[10101])"
     },
     "10134": {
         "event": "\u6709\u540c\u5b66\u5728\u73ed\u4e0a\u70ab\u8000\u65b0\u73a9\u5177\uff0c\u88ab\u8001\u5e08\u6ca1\u6536\u4e86\u3002",
         "exclude": "EVT?[10134]",
         "id": 10134,
@@ -1374,25 +1397,27 @@
     },
     "10158": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u4e70\u5f69\u7968\u4e2d\u4e86\u4e2a\u5c0f\u5956\u3002",
         "exclude": "EVT?[10158]",
+        "grade": 1,
         "id": 10158,
         "include": "EVT?[10157]",
         "postEvent": "\u867d\u7136\u94b1\u4e0d\u591a\u4f46\u5f88\u5feb\u4e50\u3002"
     },
     "10159": {
         "effect": {
             "MNY": 2,
             "SPR": 2
         },
         "event": "\u4f60\u4e70\u5f69\u7968\u4e2d\u4e86\u4e2a\u5927\u5956\u3002",
         "exclude": "EVT?[10159]",
+        "grade": 2,
         "id": 10159,
         "include": "EVT?[10157]"
     },
     "10160": {
         "event": "\u4f60\u7559\u4e86\u4e00\u7ea7\u3002",
         "exclude": "EVT?[10160,10025,10156,10155]",
         "id": 10160,
@@ -1603,21 +1628,23 @@
     },
     "10190": {
         "effect": {
             "SPR": 1
         },
         "event": "\u6e38\u620f\u6c34\u5e73\u5f88\u9ad8\uff0c\u8fdc\u8fd1\u7f51\u5427\u95fb\u540d\u3002",
         "exclude": "EVT?[10190]",
+        "grade": 1,
         "id": 10190,
         "include": "(STR>2)&(INT>7)&(EVT?[10188,10194])",
         "postEvent": "\u7f51\u5427\u8001\u677f\u5141\u8bb8\u4f60\u514d\u8d39\u4e0a\u7f51\u3002"
     },
     "10191": {
         "event": "\u88ab\u516c\u53f8\u53d1\u6398\uff0c\u8fdb\u5165\u7535\u7ade\u57f9\u8bad\u961f\u3002",
         "exclude": "EVT?[10191]",
+        "grade": 1,
         "id": 10191,
         "include": "EVT?[10190,10942]",
         "postEvent": "\u524d\u5f80\u5927\u57ce\u5e02\u3002"
     },
     "10192": {
         "branch": [
             "TLT?[1039]:10193",
@@ -1637,14 +1664,15 @@
         "NoRandom": 1,
         "effect": {
             "MNY": 2,
             "SPR": 2,
             "STR": -2
         },
         "event": "\u8fde\u7eed\u593a\u5f97\u5927\u5956\u3002",
+        "grade": 2,
         "id": 10193
     },
     "10194": {
         "event": "\u5f00\u59cb\u53bb\u7f51\u5427\uff0c\u6c89\u8ff7\u6e38\u620f\u3002",
         "exclude": "EVT?[10194,10188]",
         "id": 10194,
         "include": "(TLT?[1039])&(EVT?[10009])"
@@ -1683,45 +1711,49 @@
         "exclude": "(INT<3)|(EVT?[10198,10200,10199,10025,10156,10155])",
         "id": 10199,
         "include": "EVT?[10101]"
     },
     "10200": {
         "event": "\u4e2d\u8003\u8003\u7684\u5f88\u597d\uff0c\u4e0a\u4e86\u57ce\u91cc\u7684\u597d\u9ad8\u4e2d\u3002",
         "exclude": "(INT<6)|(EVT?[10198,10200,10199,10025,10156,10155])",
+        "grade": 1,
         "id": 10200,
         "include": "(MNY>2)&(INT>5)&(EVT?[10101])"
     },
     "10201": {
         "event": "\u6253\u7bee\u7403\u3001\u8e22\u8db3\u7403\u53d7\u4f24\u3002",
         "exclude": "(STR>9)|(EVT?[10201,10002])",
         "id": 10201,
         "include": "(STR>4)&(MNY>2)&(EVT?[10101])"
     },
     "10202": {
         "event": "\u88ab\u89c6\u5bdf\u7684\u4f53\u6821\u6559\u7ec3\u53d1\u6398\u3002\u53bb\u4f53\u6821\u8bad\u7ec3\u3002",
         "exclude": "EVT?[10202]",
+        "grade": 1,
         "id": 10202,
         "include": "(STR>6)&(EVT?[10184])"
     },
     "10203": {
         "branch": [
             "SPR>8:10204"
         ],
         "event": "\u8fdb\u5165\u7701\u961f\u3002",
         "exclude": "EVT?[10203,10204]",
+        "grade": 1,
         "id": 10203,
         "include": "EVT?[10202,10939]",
         "postEvent": "\u523b\u82e6\u8bad\u7ec3\u3002"
     },
     "10204": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u8868\u73b0\u7a81\u51fa\uff0c\u8fdb\u5165\u56fd\u5bb6\u961f\u3002",
+        "grade": 2,
         "id": 10204
     },
     "10205": {
         "branch": [
             "SPR>8:10204"
         ],
         "effect": {
@@ -1743,35 +1775,38 @@
             "SPR>9:10208"
         ],
         "effect": {
             "MNY": 1,
             "SPR": 1
         },
         "event": "\u53c2\u52a0\u5965\u8fd0\u4f1a\u3002",
+        "grade": 2,
         "id": 10207,
         "include": "EVT?[10204]",
         "postEvent": "\u593a\u5f97\u5956\u724c\u3002"
     },
     "10208": {
         "NoRandom": 1,
         "branch": [
             "SPR>10:10209"
         ],
         "effect": {
             "SPR": 1
         },
         "event": "\u593a\u5f97\u91d1\u724c\u3002",
+        "grade": 3,
         "id": 10208
     },
     "10209": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u5e76\u6253\u7834\u4e16\u754c\u7eaa\u5f55\u3002",
+        "grade": 3,
         "id": 10209
     },
     "10210": {
         "event": "\u9000\u5f79\u3002",
         "exclude": "EVT?[10210]",
         "id": 10210,
         "include": "EVT?[10203]",
@@ -1812,14 +1847,15 @@
     },
     "10215": {
         "branch": [
             "TLT?[1108]:20215"
         ],
         "event": "\u9047\u4e0a\u8857\u4e0a\u7684\u9ed1\u793e\u4f1a\u5bf9\u62fc\uff0c\u5f88\u9707\u64bc\u3002",
         "exclude": "EVT?[10215,10185]",
+        "grade": 1,
         "id": 10215,
         "include": "EVT?[10009]"
     },
     "10216": {
         "event": "\u5750\u516c\u4ea4\u8f66\u88ab\u52ab\u8f66\u6536\u4fdd\u62a4\u8d39\u3002",
         "exclude": "EVT?[10216,10185]",
         "id": 10216,
@@ -2029,14 +2065,15 @@
     },
     "10239": {
         "effect": {
             "SPR": 1
         },
         "event": "\u9ad8\u8003\uff0c\u4f60\u8003\u4e0a\u4e86\u5927\u57ce\u5e02\u7684\u91cd\u70b9\u672c\u79d1\u3002",
         "exclude": "EVT?[10239,10238,10237,10468]",
+        "grade": 1,
         "id": 10239,
         "include": "(INT>7)&(EVT?[10199,10200])"
     },
     "10240": {
         "event": "\u4f60\u53c2\u52a0\u4e86\u793e\u4f1a\u5b9e\u8df5\u3002",
         "exclude": "EVT?[10240]",
         "id": 10240,
@@ -2179,14 +2216,15 @@
         "exclude": "EVT?[10198,10199,10200,10025,10156,10155,10258]",
         "id": 10258,
         "include": "(STR>5)&(EVT?[10009,10940])"
     },
     "10259": {
         "event": "\u4f60\u6b63\u5f0f\u5165\u4f0d\u3002",
         "exclude": "EVT?[10259,10468]",
+        "grade": 1,
         "id": 10259,
         "include": "EVT?[10258]"
     },
     "10260": {
         "event": "\u5e73\u6de1\u4f46\u4e0d\u5e73\u51e1\u7684\u519b\u65c5\u751f\u6daf\u3002",
         "id": 10260,
         "include": "EVT?[10259]"
@@ -2230,14 +2268,15 @@
     },
     "10265": {
         "NoRandom": 1,
         "effect": {
             "MNY": 2
         },
         "event": "\u5f53\u4e0a\u4e86\u6751\u59d4\u4e66\u8bb0\u3002",
+        "grade": 1,
         "id": 10265
     },
     "10266": {
         "event": "\u4f60\u548c\u9694\u58c1\u6751\u8001\u6751\u59d4\u4e66\u8bb0\u5bb6\u7684\u5b69\u5b50\u7ed3\u5a5a\u4e86\u3002",
         "exclude": "(EVT?[10266])|(TLT?[1027])",
         "id": 10266,
         "include": "EVT?[10265]"
@@ -2512,95 +2551,105 @@
     },
     "10297": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u5357\u65b9\u65c5\u6e38\u3002",
         "exclude": "EVT?[10297]",
+        "grade": 1,
         "id": 10297,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10298": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u5317\u65b9\u65c5\u6e38\u3002",
         "exclude": "EVT?[10298]",
+        "grade": 1,
         "id": 10298,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10299": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u897f\u85cf\u65c5\u6e38\u3002",
         "exclude": "EVT?[10299]",
+        "grade": 1,
         "id": 10299,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10300": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u65b0\u7586\u65c5\u6e38\u3002",
         "exclude": "EVT?[10300]",
+        "grade": 1,
         "id": 10300,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10301": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u722c\u9ec4\u5c71\u3002",
         "exclude": "EVT?[10301]",
+        "grade": 1,
         "id": 10301,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10302": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u722c\u6cf0\u5c71\u3002",
         "exclude": "EVT?[10302]",
+        "grade": 1,
         "id": 10302,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10303": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u676d\u5dde\u770b\u897f\u6e56\u3002",
         "exclude": "EVT?[10303]",
+        "grade": 1,
         "id": 10303,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10304": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u8499\u53e4\u770b\u8349\u539f\u3002",
         "exclude": "EVT?[10304]",
+        "grade": 1,
         "id": 10304,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10305": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u5317\u4eac\u65c5\u6e38\u3002",
         "exclude": "EVT?[10305]",
+        "grade": 1,
         "id": 10305,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10306": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53bb\u4e0a\u6d77\u65c5\u6e38\u3002",
         "exclude": "EVT?[10306]",
+        "grade": 1,
         "id": 10306,
         "include": "(TLT?[1041,1027])&(EVT?[10009])"
     },
     "10307": {
         "event": "\u4f60\u7a81\u7136\u53d1\u73b0\uff0c\u4ece\u4f60\u7ed3\u5a5a\u90a3\u5929\u8d77\uff0c\u4f60\u7684\u4eba\u751f\u5c31\u7ed3\u675f\u4e86\u3002",
         "exclude": "EVT?[10307]",
         "id": 10307,
@@ -2715,14 +2764,15 @@
             "CHR": 3,
             "INT": 3,
             "SPR": 2,
             "STR": 3
         },
         "event": "\u4f60\u4ece\u76d2\u5b50\u4e2d\u83b7\u5f97\u4e86\u7ec3\u6c14\u6cd5\u95e8\uff0c\u7a81\u7834\u5230\u51dd\u6c14\u4e00\u5c42\u3002",
         "exclude": "EVT?[10323]",
+        "grade": 3,
         "id": 10323,
         "include": "TLT?[1048]",
         "postEvent": "\u5bff\u5143\u63d0\u5347\u5230200\u5e74\u3002"
     },
     "10324": {
         "effect": {
             "STR": 1
@@ -2735,104 +2785,115 @@
     },
     "10325": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u4e8c\u5c42\u3002",
         "exclude": "EVT?[10325]",
+        "grade": 1,
         "id": 10325,
         "include": "(EVT?[10323])&(STR>10)&(TLT?[1048])"
     },
     "10326": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u4e09\u5c42\u3002",
         "exclude": "EVT?[10326]",
+        "grade": 1,
         "id": 10326,
         "include": "(EVT?[10325])&(STR>12)&(TLT?[1048])"
     },
     "10327": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u56db\u5c42\u3002",
         "exclude": "EVT?[10327]",
+        "grade": 1,
         "id": 10327,
         "include": "(EVT?[10326])&(STR>15)&(TLT?[1048])"
     },
     "10328": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u4e94\u5c42\u3002",
         "exclude": "EVT?[10328]",
+        "grade": 1,
         "id": 10328,
         "include": "(EVT?[10327])&(STR>20)&(TLT?[1048])"
     },
     "10329": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u516d\u5c42\u3002",
         "exclude": "EVT?[10329]",
+        "grade": 1,
         "id": 10329,
         "include": "(EVT?[10328])&(STR>25)&(TLT?[1048])"
     },
     "10330": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u4e03\u5c42\u3002",
         "exclude": "EVT?[10330]",
+        "grade": 1,
         "id": 10330,
         "include": "(EVT?[10329])&(STR>30)&(TLT?[1048])"
     },
     "10331": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u516b\u5c42\u3002",
         "exclude": "EVT?[10331]",
+        "grade": 1,
         "id": 10331,
         "include": "(EVT?[10330])&(STR>38)&(TLT?[1048])"
     },
     "10332": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51dd\u6c14\u4e5d\u5c42\u3002",
         "exclude": "EVT?[10332]",
+        "grade": 1,
         "id": 10332,
         "include": "(EVT?[10331])&(STR>50)&(TLT?[1048])"
     },
     "10333": {
         "effect": {
             "INT": 1,
             "STR": 10
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u4e00\u5c42\u3002",
         "exclude": "EVT?[10333]",
+        "grade": 2,
         "id": 10333,
         "include": "(EVT?[10332])&(STR>100)&(TLT?[1048])",
         "postEvent": "\u5bff\u5143\u63d0\u5347\u5230300\u5e74\u3002"
     },
     "10334": {
         "effect": {
             "STR": 10
         },
         "event": "\u4f60\u6361\u5230\u5f02\u679c\uff0c\u4f53\u8d28\u5927\u5e45\u63d0\u5347\u3002",
+        "grade": 1,
         "id": 10334,
         "include": "TLT?[1048]"
     },
     "10335": {
         "effect": {
             "STR": 20
         },
         "event": "\u4f60\u53d1\u73b0\u7075\u6c14\u6d53\u90c1\u4e4b\u5904\uff0c\u4f53\u8d28\u5927\u5e45\u63d0\u5347\u3002",
+        "grade": 1,
         "id": 10335,
         "include": "TLT?[1048]"
     },
     "10336": {
         "effect": {
             "STR": 2
         },
@@ -2844,87 +2905,96 @@
     },
     "10337": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u4e8c\u5c42\u3002",
         "exclude": "EVT?[10337]",
+        "grade": 1,
         "id": 10337,
         "include": "(EVT?[10333])&(STR>120)&(TLT?[1048])"
     },
     "10338": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u4e09\u5c42\u3002",
         "exclude": "EVT?[10338]",
+        "grade": 1,
         "id": 10338,
         "include": "(EVT?[10337])&(STR>140)&(TLT?[1048])"
     },
     "10339": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u56db\u5c42\u3002",
         "exclude": "EVT?[10339]",
+        "grade": 1,
         "id": 10339,
         "include": "(EVT?[10338])&(STR>160)&(TLT?[1048])"
     },
     "10340": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u4e94\u5c42\u3002",
         "exclude": "EVT?[10340]",
+        "grade": 1,
         "id": 10340,
         "include": "(EVT?[10339])&(STR>190)&(TLT?[1048])"
     },
     "10341": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u516d\u5c42\u3002",
         "exclude": "EVT?[10341]",
+        "grade": 1,
         "id": 10341,
         "include": "(EVT?[10340])&(STR>220)&(TLT?[1048])"
     },
     "10342": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u4e03\u5c42\u3002",
         "exclude": "EVT?[10342]",
+        "grade": 1,
         "id": 10342,
         "include": "(EVT?[10341])&(STR>250)&(TLT?[1048])"
     },
     "10343": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u516b\u5c42\u3002",
         "exclude": "EVT?[10343]",
+        "grade": 1,
         "id": 10343,
         "include": "(EVT?[10342])&(STR>280)&(TLT?[1048])"
     },
     "10344": {
         "effect": {
             "STR": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u4e5d\u5c42\u3002",
         "exclude": "EVT?[10344]",
+        "grade": 1,
         "id": 10344,
         "include": "(EVT?[10343])&(STR>320)&(TLT?[1048])"
     },
     "10345": {
         "effect": {
             "INT": 2,
             "STR": 20
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u4e00\u5c42\u3002",
         "exclude": "EVT?[10345,10361]",
+        "grade": 2,
         "id": 10345,
         "include": "(EVT?[10344])&(STR>400)&(TLT?[1048])",
         "postEvent": "\u5bff\u5143\u63d0\u5347\u5230400\u5e74\u3002"
     },
     "10346": {
         "branch": [
             "STR>0:10000"
@@ -2952,32 +3022,35 @@
     "10348": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u4e8c\u5c42\u3002",
         "exclude": "EVT?[10348]",
+        "grade": 1,
         "id": 10348,
         "include": "(EVT?[10345,10361])&(STR>450)&(INT>10)&(TLT?[1048])"
     },
     "10349": {
         "effect": {
             "STR": 100
         },
         "event": "\u56fe\u4f60\u7f8e\u8272\uff0c\u4e00\u4e2a\u5883\u754c\u6781\u9ad8\u7684\u4eba\u5f3a\u884c\u548c\u4f60\u53cc\u4fee\u3002",
         "exclude": "EVT?[10349]",
+        "grade": 1,
         "id": 10349,
         "include": "(EVT?[10333])&(CHR>10)&(TLT?[1048])",
         "postEvent": "\u4f53\u8d28\u5927\u5e45\u63d0\u5347\u3002"
     },
     "10350": {
         "effect": {
             "STR": 50
         },
         "event": "\u4f60\u53d1\u73b0\u4e00\u79cd\u52a0\u5feb\u4fee\u884c\u901f\u5ea6\u7684\u65b9\u6cd5\u3002",
+        "grade": 1,
         "id": 10350,
         "include": "(EVT?[10333])&(INT>10)&(TLT?[1048])",
         "postEvent": "\u4f53\u8d28\u5927\u5e45\u63d0\u5347\u3002"
     },
     "10351": {
         "effect": {
             "STR": 5
@@ -2989,74 +3062,81 @@
     "10352": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u4e09\u5c42\u3002",
         "exclude": "EVT?[10352]",
+        "grade": 1,
         "id": 10352,
         "include": "(EVT?[10348])&(STR>500)&(INT>15)&(TLT?[1048])"
     },
     "10353": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u56db\u5c42\u3002",
         "exclude": "EVT?[10353]",
+        "grade": 1,
         "id": 10353,
         "include": "(EVT?[10352])&(STR>550)&(INT>20)&(TLT?[1048])"
     },
     "10354": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u4e94\u5c42\u3002",
         "exclude": "EVT?[10354]",
+        "grade": 1,
         "id": 10354,
         "include": "(EVT?[10353])&(STR>600)&(INT>30)&(TLT?[1048])"
     },
     "10355": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u516d\u5c42\u3002",
         "exclude": "EVT?[10355]",
+        "grade": 1,
         "id": 10355,
         "include": "(EVT?[10354])&(STR>650)&(INT>40)&(TLT?[1048])"
     },
     "10356": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u4e03\u5c42\u3002",
         "exclude": "EVT?[10356]",
+        "grade": 1,
         "id": 10356,
         "include": "(EVT?[10355])&(STR>700)&(INT>50)&(TLT?[1048])"
     },
     "10357": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u516b\u5c42\u3002",
         "exclude": "EVT?[10357]",
+        "grade": 1,
         "id": 10357,
         "include": "(EVT?[10356])&(STR>750)&(INT>65)&(TLT?[1048])"
     },
     "10358": {
         "effect": {
             "INT": 1,
             "STR": 3
         },
         "event": "\u4f60\u7a81\u7834\u5230\u91d1\u4e39\u4e5d\u5c42\u3002",
         "exclude": "EVT?[10358]",
+        "grade": 1,
         "id": 10358,
         "include": "(EVT?[10357])&(STR>850)&(INT>80)&(TLT?[1048])"
     },
     "10359": {
         "branch": [
             "STR>1000:10360",
             "STR<1000:10000"
@@ -3070,25 +3150,27 @@
         "NoRandom": 1,
         "effect": {
             "INT": 50,
             "SPR": 2,
             "STR": 500
         },
         "event": "\u4f60\u5c06\u5176\u8d8a\u7ea7\u53cd\u6740\u3002",
+        "grade": 2,
         "id": 10360,
         "postEvent": "\u5f97\u5230\u5927\u91cf\u5b9d\u7269\u3002\u5c5e\u6027\u63d0\u5347\u3002"
     },
     "10361": {
         "effect": {
             "INT": 50,
             "SPR": 1,
             "STR": 500
         },
         "event": "\u4f60\u670d\u7528\u4e86\u7956\u4f20\u836f\u4e38\uff0c\u7a81\u7834\u5230\u4e86\u91d1\u4e39\u4e00\u5c42\u3002",
         "exclude": "EVT?[10361,10345]",
+        "grade": 3,
         "id": 10361,
         "include": "(EVT?[10344])&(TLT?[1048])&(TLT?[1065])",
         "postEvent": "\u5e76\u4e14\u4f60\u6709\u4e24\u679a\u91d1\u4e39\u3002\u5bff\u5143\u63d0\u5347\u5230500\u5e74\u3002"
     },
     "10362": {
         "effect": {
             "INT": 1,
@@ -3103,14 +3185,15 @@
     "10363": {
         "effect": {
             "INT": 10,
             "STR": 100
         },
         "event": "\u4f60\u52a0\u5165\u4e86\u4e00\u4e2a\u9690\u4e16\u5b97\u6d3e\u6210\u4e3a\u957f\u8001\u3002",
         "exclude": "EVT?[10363]",
+        "grade": 1,
         "id": 10363,
         "include": "(EVT?[10345,10361])&(STR>450)&(INT>10)&(TLT?[1048])",
         "postEvent": "\u5f97\u5230\u5927\u91cf\u4fee\u70bc\u8d44\u6e90\u3002"
     },
     "10364": {
         "effect": {
             "STR": 10
@@ -3121,26 +3204,30 @@
     },
     "10365": {
         "effect": {
             "INT": 30
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u4e00\u5c42\u3002",
         "exclude": "EVT?[10365]",
+        "grade": 2,
         "id": 10365,
         "include": "(EVT?[10358])&(STR>1000)&(INT>100)&(TLT?[1048])",
         "postEvent": "\u5bff\u5143\u63d0\u5347\u5230500\u5e74\u3002"
     },
     "10366": {
-        "effect": {
-            "INT": 10,
-            "STR": 100
-        },
-        "event": "\u4f60\u65a9\u6740\u4e86\u5927\u91cf\u7b51\u57fa\u4fee\u58eb\uff0c\u83b7\u5f97\u4e0d\u5c11\u8d44\u6e90\u3002",
+        "branch": [
+            "INT>50:20366",
+            "MNY>4:20365",
+            "TLT?[1048]:20364"
+        ],
+        "event": "\u4f60\u53c2\u52a0\u4e86\u4e00\u573a\u62cd\u5356\u4f1a\u3002",
+        "exclude": "EVT?[10366]",
+        "grade": 1,
         "id": 10366,
-        "include": "(EVT?[10345,10361])&(STR>450)&(INT>10)&(TLT?[1048])"
+        "include": "(STR>100)&(TLT?[1048])"
     },
     "10367": {
         "effect": {
             "INT": 2,
             "STR": 1
         },
         "event": "\u609f\u9053\u3002",
@@ -3160,97 +3247,107 @@
     },
     "10369": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u4e8c\u5c42\u3002",
         "exclude": "EVT?[10369]",
+        "grade": 1,
         "id": 10369,
         "include": "(EVT?[10365])&(INT>150)"
     },
     "10370": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u4e09\u5c42\u3002",
         "exclude": "EVT?[10370]",
+        "grade": 1,
         "id": 10370,
         "include": "(EVT?[10369])&(INT>180)"
     },
     "10371": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u56db\u5c42\u3002",
         "exclude": "EVT?[10371]",
+        "grade": 1,
         "id": 10371,
         "include": "(EVT?[10370])&(INT>210)"
     },
     "10372": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u4e94\u5c42\u3002",
         "exclude": "EVT?[10372]",
+        "grade": 1,
         "id": 10372,
         "include": "(EVT?[10371])&(INT>240)"
     },
     "10373": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u516d\u5c42\u3002",
         "exclude": "EVT?[10373]",
+        "grade": 1,
         "id": 10373,
         "include": "(EVT?[10372])&(INT>280)"
     },
     "10374": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u4e03\u5c42\u3002",
         "exclude": "EVT?[10374]",
+        "grade": 1,
         "id": 10374,
         "include": "(EVT?[10373])&(INT>320)"
     },
     "10375": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u516b\u5c42\u3002",
         "exclude": "EVT?[10375]",
+        "grade": 1,
         "id": 10375,
         "include": "(EVT?[10374])&(INT>360)"
     },
     "10376": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7a81\u7834\u5230\u5143\u5a74\u4e5d\u5c42\u3002",
         "exclude": "EVT?[10376]",
+        "grade": 1,
         "id": 10376,
         "include": "(EVT?[10375])&(INT>400)"
     },
     "10377": {
         "effect": {
             "INT": 10,
             "STR": 10
         },
         "event": "\u4f60\u7a81\u7834\u5230\u6e21\u52ab\u671f\u3002",
         "exclude": "EVT?[10377]",
+        "grade": 2,
         "id": 10377,
         "include": "(EVT?[10375])&(INT>500)"
     },
     "10378": {
         "effect": {
             "INT": 1,
             "STR": 10
         },
         "event": "\u51c6\u5907\u6e21\u52ab\u3002",
         "exclude": "EVT?[10378]",
+        "grade": 2,
         "id": 10378,
         "include": "(EVT?[10377])&(INT>500)"
     },
     "10379": {
         "branch": [
             "STR>0:10000"
         ],
@@ -3264,307 +3361,337 @@
     "10380": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u6c34\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[10380]",
+        "grade": 2,
         "id": 10380,
         "include": "(EVT?[10365])&(INT>100)"
     },
     "10381": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u706b\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[10381]",
+        "grade": 2,
         "id": 10381,
         "include": "(EVT?[10365])&(INT>100)"
     },
     "10382": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u91d1\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[10382]",
+        "grade": 2,
         "id": 10382,
         "include": "(EVT?[10365])&(INT>100)"
     },
     "10383": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u6728\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[10383]",
+        "grade": 2,
         "id": 10383,
         "include": "(EVT?[10365])&(INT>100)"
     },
     "10384": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u571f\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[10384]",
+        "grade": 2,
         "id": 10384,
         "include": "(EVT?[10365])&(INT>100)"
     },
     "10385": {
         "effect": {
             "INT": 20
         },
         "event": "\u4f60\u8fdb\u5165\u987f\u609f\u72b6\u6001\u3002",
+        "grade": 1,
         "id": 10385,
         "include": "(EVT?[10365])&(INT>100)"
     },
     "10386": {
         "effect": {
             "INT": 50,
             "STR": 50
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u7a7a\u95f4\u5927\u9053\u3002",
         "exclude": "EVT?[10386]",
+        "grade": 3,
         "id": 10386,
         "include": "(EVT?[10365])&(INT>300)"
     },
     "10387": {
         "effect": {
             "INT": 50,
             "STR": 50
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u65f6\u95f4\u5927\u9053\u3002",
         "exclude": "EVT?[10387]",
+        "grade": 3,
         "id": 10387,
         "include": "(EVT?[10365])&(INT>300)"
     },
     "10388": {
         "effect": {
             "INT": 100,
             "STR": 100
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u6df7\u6c8c\u5927\u9053\u3002",
         "exclude": "EVT?[10388]",
+        "grade": 3,
         "id": 10388,
         "include": "(EVT?[10365])&(INT>300)"
     },
     "10389": {
         "effect": {
             "INT": 75,
             "STR": 75
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u751f\u547d\u5927\u9053\u3002",
         "exclude": "EVT?[10389]",
+        "grade": 3,
         "id": 10389,
         "include": "(EVT?[10365])&(INT>300)"
     },
     "10390": {
         "effect": {
             "INT": 75,
             "STR": 75
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u6bc1\u706d\u5927\u9053\u3002",
         "exclude": "EVT?[10390]",
+        "grade": 3,
         "id": 10390,
         "include": "(EVT?[10365])&(INT>300)"
     },
     "10391": {
         "branch": [
             "EVT?[10377]:10392"
         ],
         "event": "\u5f00\u59cb\u6e21\u52ab\u3002\u4e5d\u91cd\u96f7\u52ab\u5f00\u59cb\u3002",
+        "grade": 3,
         "id": 10391,
         "include": "EVT?[10377]"
     },
     "10392": {
         "NoRandom": 1,
         "branch": [
             "STR>1100:10393",
             "(STR<1101)&(TLT?[1134]):20409",
             "STR<1101:10000"
         ],
         "event": "\u7b2c\u4e00\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10392
     },
     "10393": {
         "NoRandom": 1,
         "branch": [
             "STR>1200:10394",
             "(STR<1201)&(TLT?[1134]):20409",
             "STR<1201:10000"
         ],
         "event": "\u7b2c\u4e8c\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10393
     },
     "10394": {
         "NoRandom": 1,
         "branch": [
             "STR>1300:10395",
             "(STR<1301)&(TLT?[1134]):20409",
             "STR<1301:10000"
         ],
         "event": "\u7b2c\u4e09\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10394
     },
     "10395": {
         "NoRandom": 1,
         "branch": [
             "STR>1400:10396",
             "(STR<1401)&(TLT?[1134]):20409",
             "STR<1401:10000"
         ],
         "event": "\u7b2c\u56db\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10395
     },
     "10396": {
         "NoRandom": 1,
         "branch": [
             "STR>1500:10397",
             "(STR<1501)&(TLT?[1134]):20409",
             "STR<1501:10000"
         ],
         "event": "\u7b2c\u4e94\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10396
     },
     "10397": {
         "NoRandom": 1,
         "branch": [
             "STR>1600:10398",
             "(STR<1601)&(TLT?[1134]):20409",
             "STR<1601:10000"
         ],
         "event": "\u7b2c\u516d\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10397
     },
     "10398": {
         "NoRandom": 1,
         "branch": [
             "STR>1700:10399",
             "(STR<1701)&(TLT?[1134]):20409",
             "STR<1701:10000"
         ],
         "event": "\u7b2c\u4e03\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10398
     },
     "10399": {
         "NoRandom": 1,
         "branch": [
             "STR>1800:10400",
             "(STR<1801)&(TLT?[1134]):20409",
             "STR<1801:10000"
         ],
         "event": "\u7b2c\u516b\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10399
     },
     "10400": {
         "NoRandom": 1,
         "branch": [
             "(STR>2000)|(EVT?[20381]):10401",
             "(STR<2001)&(TLT?[1134]):20409",
             "STR<2001:10000"
         ],
         "event": "\u7b2c\u4e5d\u91cd\u96f7\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10400
     },
     "10401": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10377]:10402"
         ],
         "event": "\u96f7\u52ab\u5ea6\u8fc7\uff0c\u5143\u795e\u52ab\u5f00\u59cb\u3002",
+        "grade": 3,
         "id": 10401
     },
     "10402": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10382,20367]:10403",
             "(EVT?[10377])&(TLT?[1134]):20409",
             "EVT?[10377]:10000"
         ],
         "event": "\u91d1\u4e4b\u5143\u795e\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10402
     },
     "10403": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10383,20367]:10404",
             "(EVT?[10377])&(TLT?[1134]):20409",
             "EVT?[10377]:10000"
         ],
         "event": "\u6728\u4e4b\u5143\u795e\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10403
     },
     "10404": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10380,20367]:10405",
             "(EVT?[10377])&(TLT?[1134]):20409",
             "EVT?[10377]:10000"
         ],
         "event": "\u6c34\u4e4b\u5143\u795e\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10404
     },
     "10405": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10381,20367]:10406",
             "(EVT?[10377])&(TLT?[1134]):20409",
             "EVT?[10377]:10000"
         ],
         "event": "\u706b\u4e4b\u5143\u795e\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10405
     },
     "10406": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10384,20367]:10407",
             "(EVT?[10377])&(TLT?[1134]):20409",
             "EVT?[10377]:10000"
         ],
         "event": "\u571f\u4e4b\u5143\u795e\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10406
     },
     "10407": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10386,10387,10388,10389,10390,20367]:10408",
             "(EVT?[10377])&(TLT?[1134]):20409",
             "EVT?[10377]:10000"
         ],
         "event": "\u672c\u6e90\u5143\u795e\u52ab\u843d\u4e0b\u3002",
+        "grade": 3,
         "id": 10407
     },
     "10408": {
         "NoRandom": 1,
         "branch": [
             "SPR>10:10409",
             "(EVT?[10377])&(TLT?[1134]):20409",
             "EVT?[10377]:10000"
         ],
         "event": "\u5fc3\u9b54\u52ab\u964d\u4e34\u3002",
+        "grade": 3,
         "id": 10408
     },
     "10409": {
         "NoRandom": 1,
         "effect": {
             "LIF": -1
         },
         "event": "\u6e21\u52ab\u6210\u529f\uff01\u4f60\u98de\u5347\u5230\u4ed9\u754c\u4e86\u3002",
+        "grade": 3,
         "id": 10409,
         "postEvent": "\u4f60\u4f5c\u4e3a\u201c\u4eba\u201d\u7684\u4eba\u751f\u7ed3\u675f\u4e86\u3002"
     },
     "10410": {
         "branch": [
             "STR>5:20410",
             "INT<6:20411"
         ],
         "event": "\u4f60\u6210\u4e3a\u4e86\u52a8\u6f2b\u9ad8\u624b\uff0c\u7ecf\u5e38\u5728\u7f51\u4e0a\u9a82\u6218\u3002",
-        "exclude": "(EVT?[10410,10002])|(TLT?[1014])",
+        "exclude": "(EVT?[10410,10002,20410,20411])|(TLT?[1014])",
         "id": 10410,
         "include": "EVT?[10189]"
     },
     "10411": {
         "branch": [
             "STR>6:20412",
             "INT<4:20413"
@@ -3586,63 +3713,54 @@
         ],
         "event": "\u67d0\u5916\u7c4d\u77e5\u540d\u660e\u661f\u56e0\u5f3a\u5978\u7f6a\u88ab\u6293\u3002",
         "exclude": "EVT?[10413,20413]",
         "id": 10413,
         "include": "EVT?[10009]"
     },
     "10414": {
-        "event": "\u9644\u8fd1\u5f00\u59cb\u6d41\u884c\u80ba\u708e\uff0c\u4f60\u5728\u5bb6\u4e2d\u4e0d\u6562\u51fa\u95e8\u3002",
+        "event": "\u4f60\u8fde\u5237\u4e8620\u6761\u77ed\u89c6\u9891\uff0c\u53d1\u73b0\u6240\u6709\u4eba\u7528\u7684\u90fd\u662f\u540c\u6b3e\u97f3\u4e50\u3002",
         "exclude": "EVT?[10414]",
         "id": 10414,
         "include": "EVT?[10009]"
     },
     "10415": {
-        "branch": [
-            "(EVT?[10237,10238,10239])&(INT<8):20415"
-        ],
         "event": "\u9ad8\u8003\u6539\u9769\uff0c\u82f1\u8bed\u88ab\u53d6\u6d88\u4e86\u3002",
         "exclude": "EVT?[10415]",
         "id": 10415,
         "include": "EVT?[10009]"
     },
     "10416": {
-        "event": "\u9ad8\u8003\u6539\u9769\uff0c\u65b0\u589e\u4e86\u4e2d\u7279\u793e\u4f5c\u4e3a\u5fc5\u8003\u79d1\u76ee\u3002",
+        "event": "\u653f\u6cbb\u6210\u4e3a\u5e7c\u513f\u56ed\u5fc5\u4fee\u8bfe\u3002",
         "exclude": "EVT?[10416]",
         "id": 10416,
         "include": "EVT?[10009,10010]"
     },
     "10417": {
         "branch": [
             "STR>9:20417"
         ],
         "event": "\u4f53\u80b2\u603b\u5c40\u65b0\u89c4\u5b9a\uff0c\u4f53\u6d4b\u6210\u7ee9\u5fc5\u987b100\u7c73\u8dd1\u8fdb10\u79d2\u624d\u53ca\u683c\u3002",
-        "exclude": "EVT?[10417]",
+        "exclude": "EVT?[10417,20417]",
         "id": 10417,
         "include": "EVT?[10009]"
     },
     "10418": {
-        "branch": [
-            "INT<2:20418"
-        ],
-        "event": "\u5854\u5229\u73ed\u7ec4\u7ec7\u5360\u9886\u534e\u76db\u987f\u3002",
+        "event": "\u5730\u72f1\u7b11\u8bdd\u5427\u88ab\u767e\u5ea6\u5b98\u65b9\u6c38\u4e45\u5173\u95ed\u3002",
         "exclude": "EVT?[10418]",
         "id": 10418,
         "include": "EVT?[10009]"
     },
     "10419": {
-        "branch": [
-            "INT<2:20419"
-        ],
-        "event": "\u672c\u00b7\u62c9\u767b\u590d\u51fa\uff0c\u53d1\u89c6\u9891\u79f0\u5f53\u5e74\u662f\u5047\u6b7b\u3002",
+        "event": "\u6211\u56fd\u4eba\u53e3\u589e\u957f\u4ece\u9ad8\u901f\u53d1\u5c55\u8f6c\u53d8\u4e3a\u9ad8\u8d28\u91cf\u53d1\u5c55\uff0c\u7a33\u4e2d\u6709\u8fdb\u3002",
         "exclude": "EVT?[10419]",
         "id": 10419,
         "include": "EVT?[10009]"
     },
     "10420": {
-        "event": "\u5e0c\u7279\u52d2\u7684\u9057\u9aa8\u88ab\u53d1\u73b0\u3002",
+        "event": "\u56fd\u5bb6\u51fa\u53f0\u76f8\u5173\u89c4\u5b9a\uff0c\u7535\u5b50\u6e38\u620f\u7684\u6253\u6597\u573a\u666f\u4e0d\u80fd\u51fa\u73b0\u4efb\u4f55\u989c\u8272\u7684\u6db2\u4f53\u3002",
         "exclude": "EVT?[10420]",
         "id": 10420,
         "include": "EVT?[10009]"
     },
     "10421": {
         "branch": [
             "(INT<4)&(MNY>8):20421"
@@ -3653,24 +3771,24 @@
         "include": "EVT?[10009]"
     },
     "10422": {
         "branch": [
             "INT>8:20422"
         ],
         "event": "\u636e\u8bf4\u6709\u4eba\u5728\u6df1\u5c71\u91cc\u53d1\u73b0\u4e86\u53e4\u88c5\u7684\u5c45\u6c11\u3002\u5b98\u65b9\u901a\u62a5\u662f\u5728\u62cd\u7535\u89c6\u5267\u3002",
-        "exclude": "EVT?[10422]",
+        "exclude": "EVT?[10422,20422]",
         "id": 10422,
         "include": "EVT?[10009,10010]"
     },
     "10423": {
         "branch": [
             "(CHR>8)|(MNY>8):20423"
         ],
         "event": "\u9694\u58c1\u57ce\u5e02\u53d1\u751f\u7279\u5927\u4ea4\u901a\u4e8b\u6545\uff0c\u6570\u5341\u4eba\u4f24\u4ea1\u3002",
-        "exclude": "EVT?[10423]",
+        "exclude": "EVT?[10423,20423]",
         "id": 10423,
         "include": "EVT?[10009,10010]"
     },
     "10424": {
         "branch": [
             "SPR>9:20425"
         ],
@@ -3689,15 +3807,16 @@
         "include": "EVT?[10009,11470]"
     },
     "10426": {
         "branch": [
             "(CHR>8)&(MNY>8):20426"
         ],
         "event": "\u4e2d\u56fd\u5927\u9646\u6536\u590d\u53f0\u6e7e\u3002",
-        "exclude": "EVT?[10426]",
+        "exclude": "EVT?[10426,20426]",
+        "grade": 1,
         "id": 10426,
         "include": "EVT?[10009]"
     },
     "10427": {
         "event": "\u6e05\u534e\u5317\u5927\u5408\u5e76\u4e3a\u6e05\u5317\u5927\u5b66\u3002",
         "exclude": "EVT?[10427]",
         "id": 10427,
@@ -3716,32 +3835,26 @@
         "include": "EVT?[10009]"
     },
     "10430": {
         "branch": [
             "INT>9:20431"
         ],
         "event": "VR\u6280\u672f\u7a81\u7834\uff0c\u7528\u6237\u53ef\u4ee5\u610f\u8bc6\u8fdb\u5165\u865a\u62df\u7a7a\u95f4\u3002\u76ee\u524d\u8be5\u6280\u672f\u8fd8\u672a\u8fdb\u5165\u6c11\u7528\u3002",
-        "exclude": "EVT?[10430]",
+        "exclude": "EVT?[10430,20431]",
         "id": 10430,
         "include": "EVT?[10009]"
     },
     "10431": {
-        "branch": [
-            "MNY>6:20432"
-        ],
-        "event": "\u6e38\u54c8\u7c73\u53d1\u5e03\u6b21\u65f6\u4ee3\u624b\u6e38\u5927\u4f5c\u300a\u795e\u539f\u300b\u3002",
+        "event": "\u6709\u53f2\u4ee5\u6765\u6700\u5927\u80a1\u707e\u51fa\u73b0\u3002",
         "exclude": "EVT?[10431]",
         "id": 10431,
         "include": "EVT?[10009]"
     },
     "10432": {
-        "branch": [
-            "SPR>7:20433"
-        ],
-        "event": "\u817e\u8baf\u6536\u8d2d\u7f51\u6613\u3002",
+        "event": "\u5143\u5b87\u5b99\u65f6\u4ee3\u6765\u4e34\uff0c\u7f51\u6613CEO\u81ea\u79f0\u5143\u59cb\u5929\u5c0a\uff0c\u54d4\u54e9\u54d4\u54e9CEO\u81ea\u79f0\u5143\u5e1d\uff0c\u7c73\u54c8\u6e38CEO\u81ea\u79f0\u5143\u6279\u3002",
         "exclude": "EVT?[10432]",
         "id": 10432,
         "include": "EVT?[10009]"
     },
     "10433": {
         "event": "\u62fc\u591a\u591a\u6536\u8d2d\u963f\u91cc\u5df4\u5df4\u3002",
         "exclude": "EVT?[10433]",
@@ -3761,48 +3874,48 @@
         "include": "EVT?[10009]"
     },
     "10436": {
         "branch": [
             "EVT![10268,10269,10272]:20436"
         ],
         "event": "\u4e2d\u56fd\u5f00\u653e\u5341\u516b\u80ce\u751f\u80b2\u3002",
-        "exclude": "EVT?[10436]",
+        "exclude": "EVT?[10436,20436]",
         "id": 10436,
         "include": "EVT?[10009]"
     },
     "10437": {
         "branch": [
             "STR>2:20437"
         ],
         "event": "\u5168\u7403\u65b0\u51a0\u786e\u8bca\u75c5\u4f8b\u9996\u6b21\u6e05\u96f6\u3002",
-        "exclude": "EVT?[10437]",
+        "exclude": "EVT?[10437,20437]",
         "id": 10437,
         "include": "EVT?[10009]"
     },
     "10438": {
-        "event": "\u66f9\u53bf\u6210\u529f\u7533\u529e2066\u5e74\u5965\u8fd0\u4f1a\u3002",
+        "event": "\u67d0\u5e02\u5047\u610f\u8bbe\u7acb\u9ec4\u8d4c\u6bd2\u573a\u6240\uff0c\u8b66\u65b9\u5b88\u5728\u73b0\u573a\u5c06\u8fdd\u6cd5\u4eba\u5458\u5168\u90e8\u6293\u83b7\uff0c\u5e02\u6c11\u7eb7\u7eb7\u7fd8\u8d77\u4e86\u5927\u62c7\u6307\u3002",
         "exclude": "EVT?[10438]",
         "id": 10438,
         "include": "EVT?[10009]"
     },
     "10439": {
         "event": "\u65e5\u672c\u6b66\u529b\u653b\u5360\u73cd\u73e0\u6e2f\u3002",
-        "exclude": "EVT?[10439,11476]",
+        "exclude": "EVT?[10439]",
         "id": 10439,
         "include": "EVT?[10009]"
     },
     "10440": {
         "event": "\u671d\u9c9c\u8ba1\u5212\u5411\u7f8e\u56fd\u548c\u97e9\u56fd\u6295\u4e0b\u4e24\u9897\u539f\u5b50\u5f39\u3002",
         "exclude": "EVT?[10440]",
         "id": 10440,
         "include": "EVT?[10009]",
         "postEvent": "\u8ba1\u5212\u8d25\u9732\u3002"
     },
     "10441": {
-        "event": "\u829c\u6e56\u673a\u573a\u4e16\u754c\u6392\u540d\u5347\u81f3\u7b2c\u4e00\u3002",
+        "event": "\u5927\u91cf\u7f51\u7ea2\u5728\u81ea\u5df1\u7684\u7f51\u540d\u524d\u52a0\u4e0a\u4e86\u5f53\u5730\u5730\u540d\u3002\u540c\u5e74\u591a\u540d\u7f51\u7ea2\u88ab\u62db\u5b89\u6210\u4e3a\u5f53\u5730\u5e72\u90e8\u3002",
         "exclude": "EVT?[10441]",
         "id": 10441,
         "include": "EVT?[10009]"
     },
     "10442": {
         "event": "\u868c\u57e0\u623f\u4ef7\u4e00\u5e74\u5185\u7ffb\u500d\uff0c\u56fd\u5bb6\u51fa\u624b\u8c03\u63a7\u3002",
         "exclude": "EVT?[10442]",
@@ -3810,24 +3923,24 @@
         "include": "EVT?[10009]"
     },
     "10443": {
         "branch": [
             "(MNY<4)&(SPR<4):20443"
         ],
         "event": "\u6211\u56fd\u4e24\u6781\u5206\u5316\u8fc5\u901f\u51cf\u5c0f\uff0c\u4eba\u6c11\u5e78\u798f\u6307\u6570\u8fdb\u4e00\u6b65\u63d0\u9ad8\u3002",
-        "exclude": "EVT?[10443]",
+        "exclude": "EVT?[10443,20443]",
         "id": 10443,
         "include": "EVT?[10009,10010]"
     },
     "10444": {
         "branch": [
             "MNY<3:20444"
         ],
         "event": "\u4e2d\u56fdGDP\u8d85\u8fc7\u7f8e\u56fd\u3002",
-        "exclude": "EVT?[10444]",
+        "exclude": "EVT?[10444,20444]",
         "id": 10444,
         "include": "EVT?[10009,10010]"
     },
     "10445": {
         "event": "\u6c5f\u82cf\u7701\u7701\u4f1a\u6539\u4e3a\u82cf\u5dde\u3002",
         "exclude": "EVT?[10445]",
         "id": 10445,
@@ -3846,15 +3959,15 @@
         "include": "EVT?[10009]"
     },
     "10448": {
         "branch": [
             "MNY<4:20448"
         ],
         "event": "\u56fd\u5bb6\u516c\u5e03\u4e2d\u4ea7\u9636\u7ea7\u6807\u51c6\uff1a\u5bb6\u5ead\u5e74\u6536\u5165100\u4e07\u3002",
-        "exclude": "EVT?[10448,11297]",
+        "exclude": "EVT?[10448,11297,20448]",
         "id": 10448,
         "include": "EVT?[10009,10010]"
     },
     "10449": {
         "event": "\u6d77\u5e95\u706b\u5c71\u7206\u53d1\uff0c\u9a6c\u91cc\u4e9a\u7eb3\u6d77\u6c9f\u88ab\u586b\u5e73\u3002",
         "exclude": "EVT?[10449]",
         "id": 10449,
@@ -3867,15 +3980,15 @@
         "include": "EVT?[10009]"
     },
     "10451": {
         "branch": [
             "(MNY<4)&(TLT![1010]):20452"
         ],
         "event": "\u5317\u4eac\u4e00\u672c\u5f55\u53d6\u7387\u9996\u6b21\u8d85\u8fc799%\u3002",
-        "exclude": "EVT?[10451]",
+        "exclude": "EVT?[10451,20452]",
         "id": 10451,
         "include": "EVT?[10009,10010]"
     },
     "10452": {
         "branch": [
             "(SPR>6)&(INT>2):20453"
         ],
@@ -3922,24 +4035,25 @@
     },
     "10458": {
         "branch": [
             "(INT>10)&(TLT?[1135]):20462",
             "INT>10:20461"
         ],
         "event": "\u6709\u4e2a\u4e5e\u4e10\u5411\u4f60\u63a8\u9500\u201c\u4ed9\u6cd5\u201d\u79d8\u7c4d\u3002",
-        "exclude": "EVT?[10458]",
+        "exclude": "EVT?[10458,20462,20461]",
+        "grade": 1,
         "id": 10458,
         "postEvent": "\u4f60\u6ca1\u6709\u642d\u7406\u4ed6\u3002"
     },
     "10459": {
         "branch": [
             "INT<4:20459"
         ],
         "event": "\u6700\u65b0\u7814\u7a76\u663e\u793a\uff0c\u4eba\u7c7b\u7684\u5bff\u547d\u6781\u9650\u662f500\u5c81\u3002",
-        "exclude": "EVT?[10459]",
+        "exclude": "EVT?[10459,20459]",
         "id": 10459,
         "include": "EVT?[10009,10010]"
     },
     "10460": {
         "branch": [
             "SPR>6:20460"
         ],
@@ -3979,23 +4093,25 @@
     },
     "10466": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u5728\u8d2d\u7269\u65f6\u4e2d\u4e86\u4e2a\u4e8c\u7b49\u5956\uff1a\u4e00\u4e2a\u7535\u51b0\u7bb1\u3002",
         "exclude": "EVT?[10464,10465,10466,10467]",
+        "grade": 1,
         "id": 10466,
         "include": "EVT?[10009]"
     },
     "10467": {
         "effect": {
             "SPR": 2
         },
         "event": "\u4f60\u5728\u8d2d\u7269\u65f6\u4e2d\u4e86\u4e2a\u4e00\u7b49\u5956\uff1a\u4e09\u4e9a\u4e03\u65e5\u6e38\u3002",
         "exclude": "EVT?[10464,10465,10466,10467]",
+        "grade": 2,
         "id": 10467,
         "include": "EVT?[10009]",
         "postEvent": "\u4f60\u5feb\u4e50\u5730\u6e38\u73a9\u4e86\u4e00\u4e2a\u51ac\u5929\u3002"
     },
     "10468": {
         "event": "\u4f60\u8fdb\u5165\u6d41\u6c34\u7ebf\u5de5\u5382\u5de5\u4f5c\u3002",
         "exclude": "EVT?[10475,10476,10477,10226,10468]",
@@ -4159,14 +4275,15 @@
     },
     "10494": {
         "branch": [
             "STR<0:10000"
         ],
         "event": "\u4f53\u8d28\u8fc7\u4f4e\uff0c\u80ce\u6b7b\u8179\u4e2d\u3002",
         "exclude": "TLT?[1071]",
+        "grade": 1,
         "id": 10494,
         "include": "STR<0"
     },
     "10495": {
         "effect": {
             "INT": 1,
             "SPR": 1,
@@ -4218,14 +4335,15 @@
         "exclude": "EVT?[10501]",
         "id": 10501,
         "include": "EVT?[10011]"
     },
     "10502": {
         "event": "\u5bb6\u91cc\u5f88\u6709\u94b1\uff0c\u7236\u6bcd\u6240\u6709\u4e1c\u897f\u90fd\u4e3a\u4f60\u51c6\u5907\u6700\u597d\u7684\u3002",
         "exclude": "EVT?[10502]",
+        "grade": 1,
         "id": 10502,
         "include": "(MNY>7)&(EVT?[10011])"
     },
     "10503": {
         "event": "\u5bb6\u91cc\u5f88\u7a77\uff0c\u4f46\u7236\u6bcd\u5c3d\u529b\u4e3a\u4f60\u51c6\u5907\u66f4\u597d\u7684\u751f\u6d3b\u3002",
         "exclude": "EVT?[10503]",
         "id": 10503,
@@ -4260,32 +4378,36 @@
         "exclude": "EVT?[10508]",
         "id": 10508,
         "include": "EVT?[10011]"
     },
     "10509": {
         "event": "\u4f60\u7684\u7236\u6bcd\u8bf7\u4e86\u5bb6\u6559\u6765\u6559\u4f60\u6e38\u6cf3\u3002",
         "exclude": "EVT?[10509]",
+        "grade": 1,
         "id": 10509,
         "include": "EVT?[10504]"
     },
     "10510": {
         "event": "\u4f60\u7684\u7236\u6bcd\u8bf7\u4e86\u5bb6\u6559\u6765\u6559\u4f60\u5f39\u94a2\u7434\u3002",
         "exclude": "EVT?[10510]",
+        "grade": 1,
         "id": 10510,
         "include": "EVT?[10504]"
     },
     "10511": {
         "event": "\u4f60\u7684\u7236\u6bcd\u8bf7\u4e86\u5bb6\u6559\u6765\u6559\u4f60\u6cd5\u8bed\u3002",
         "exclude": "EVT?[10511,10512]",
+        "grade": 1,
         "id": 10511,
         "include": "EVT?[10504]"
     },
     "10512": {
         "event": "\u4f60\u7684\u7236\u6bcd\u8bf7\u4e86\u5bb6\u6559\u6765\u6559\u4f60\u897f\u73ed\u7259\u8bed\u3002",
         "exclude": "EVT?[10511,10512]",
+        "grade": 1,
         "id": 10512,
         "include": "EVT?[10504]"
     },
     "10513": {
         "effect": {
             "SPR": -1
         },
@@ -4348,14 +4470,15 @@
     },
     "10521": {
         "effect": {
             "SPR": 1
         },
         "event": "\u6709\u597d\u51e0\u4e2a\u5c0f\u670b\u53cb\u5411\u4f60\u8868\u767d\u3002",
         "exclude": "EVT?[10521]",
+        "grade": 1,
         "id": 10521,
         "include": "(CHR>6)&(EVT?[10011])"
     },
     "10522": {
         "effect": {
             "SPR": -1
         },
@@ -4468,23 +4591,25 @@
     },
     "10536": {
         "effect": {
             "MNY": 1
         },
         "event": "\u7236\u6bcd\u7684\u4e8b\u4e1a\u975e\u5e38\u6210\u529f\uff0c\u5bb6\u5883\u53d8\u5f97\u66f4\u597d\u4e86\u3002",
         "exclude": "EVT?[10536]",
+        "grade": 1,
         "id": 10536,
         "include": "EVT?[10504]"
     },
     "10537": {
         "effect": {
             "MNY": 1
         },
         "event": "\u7236\u6bcd\u7684\u4e8b\u4e1a\u53d6\u5f97\u4e86\u4e00\u5b9a\u6210\u529f\uff0c\u5bb6\u5883\u6709\u6240\u597d\u8f6c\u3002",
         "exclude": "EVT?[10537]",
+        "grade": 1,
         "id": 10537,
         "include": "EVT?[10505]"
     },
     "10538": {
         "event": "\u8001\u5e08\u6559\u4f60\u4eec\u64cd\u4f5c\u7535\u8111\uff0c\u4f46\u4f60\u65e9\u5c31\u4f1a\u4e86\u3002",
         "exclude": "EVT?[10538]",
         "id": 10538,
@@ -4504,14 +4629,15 @@
         "exclude": "EVT?[10540]",
         "id": 10540,
         "include": "EVT?[10011]"
     },
     "10541": {
         "event": "\u4f60\u4e0a\u4e86\u4e00\u4e2a\u8457\u540d\u7684\u8d35\u65cf\u4e2d\u5b66\u3002",
         "exclude": "EVT?[10541]",
+        "grade": 2,
         "id": 10541,
         "include": "(MNY>7)&(EVT?[10011])"
     },
     "10542": {
         "event": "\u4f60\u4e0a\u4e86\u4e00\u4e2a\u666e\u901a\u7684\u4e2d\u5b66\u3002",
         "exclude": "EVT?[10542]",
         "id": 10542,
@@ -4522,56 +4648,62 @@
         "exclude": "EVT?[10543]",
         "id": 10543,
         "include": "EVT?[10541]"
     },
     "10544": {
         "event": "\u8bfe\u4e1a\u5f88\u8f7b\u677e\uff0c\u51e0\u4e4e\u6ca1\u6709\u4f5c\u4e1a\uff0c\u6bcf\u5929\u4e0b\u5348\u653e\u5b66\u5c31\u6709\u5404\u79cd\u6d3b\u52a8\u3002",
         "exclude": "EVT?[10544]",
+        "grade": 1,
         "id": 10544,
         "include": "EVT?[10542]"
     },
     "10545": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u5f88\u559c\u6b22\u653e\u5b66\u6216\u5468\u672b\u5728\u5b66\u6821\u73a9\u6ed1\u96ea\u548c\u66f2\u68cd\u7403\u3002",
         "exclude": "EVT?[10545]",
+        "grade": 1,
         "id": 10545,
         "include": "(STR>2)&(EVT?[10541])"
     },
     "10546": {
         "effect": {
             "STR": 1
         },
         "event": "\u4f60\u5728\u5b66\u6821\u5b66\u4f1a\u4e86\u9a91\u9a6c\u548c\u9ad8\u5c14\u592b\u3002",
         "exclude": "EVT?[10546]",
+        "grade": 1,
         "id": 10546,
         "include": "(INT>2)&(STR>2)&(EVT?[10541])"
     },
     "10547": {
         "event": "\u4f60\u4e2d\u5348\u7ecf\u5e38\u5728\u56fe\u4e66\u9986\u548c\u53e6\u5916\u4e24\u4e2a\u534e\u88d4\u540c\u5b66\u4e00\u8d77\u5b66\u4e60\u3002",
         "exclude": "EVT?[10547]",
         "id": 10547,
         "include": "EVT?[10541]"
     },
     "10548": {
         "event": "\u4f60\u7684\u540c\u73ed\u540c\u5b66\u4e2d\u6709\u8457\u540d\u660e\u661f\u7684\u5973\u513f\u3001\u8457\u540d\u94f6\u884c\u5bb6\u7684\u5c0f\u513f\u5b50\u3002",
         "exclude": "EVT?[10548,10549,10550]",
+        "grade": 2,
         "id": 10548,
         "include": "EVT?[10541]"
     },
     "10549": {
         "event": "\u4f60\u7684\u540c\u73ed\u540c\u5b66\u4e2d\u6709\u8457\u540d\u7403\u661f\u7684\u513f\u5b50\u3002",
         "exclude": "EVT?[10548,10549,10550]",
+        "grade": 2,
         "id": 10549,
         "include": "EVT?[10541]"
     },
     "10550": {
         "event": "\u4f60\u7684\u540c\u73ed\u540c\u5b66\u4e2d\u6709\u8457\u540d\u653f\u5ba2\u7684\u5973\u513f\u548c\u67d0\u5c0f\u56fd\u7687\u5ba4\u7684\u738b\u5b50\u3002",
         "exclude": "EVT?[10548,10549,10550]",
+        "grade": 2,
         "id": 10550,
         "include": "EVT?[10541]"
     },
     "10551": {
         "event": "\u867d\u7136\u8bfe\u4f59\u6d3b\u52a8\u5f88\u4e30\u5bcc\uff0c\u4e0d\u8fc7\u540c\u5b66\u4eec\u5b66\u4e60\u90fd\u5f88\u8ba4\u771f\u3002",
         "exclude": "EVT?[10551]",
         "id": 10551,
@@ -4579,14 +4711,15 @@
     },
     "10552": {
         "effect": {
             "SPR": 1
         },
         "event": "\u5b66\u6821\u7ec4\u7ec7\u4e86\u4e00\u573a\u53bb\u6b27\u6d32\u7684\u65c5\u884c\u3002",
         "exclude": "EVT?[10552]",
+        "grade": 1,
         "id": 10552,
         "include": "EVT?[10541]"
     },
     "10553": {
         "event": "\u4f60\u53c2\u6f14\u4e86\u4e00\u573a\u620f\u5267\u6f14\u51fa\u3002",
         "exclude": "EVT?[10553]",
         "id": 10553,
@@ -4634,20 +4767,22 @@
         "exclude": "EVT?[10558]",
         "id": 10558,
         "include": "EVT?[10011]"
     },
     "10559": {
         "event": "\u5f88\u591a\u540c\u5b66\u627e\u4f60\u6c42\u4ea4\u5f80\u3002",
         "exclude": "EVT?[10559]",
+        "grade": 1,
         "id": 10559,
         "include": "EVT?[20558]"
     },
     "10560": {
         "event": "\u4e0d\u5c11\u540c\u5b66\u627e\u4f60\u6c42\u4ea4\u5f80\u3002",
         "exclude": "EVT?[10560]",
+        "grade": 1,
         "id": 10560,
         "include": "(TLT?[1028])&(EVT?[10011])"
     },
     "10561": {
         "effect": {
             "SPR": 1
         },
@@ -4790,68 +4925,77 @@
         "exclude": "EVT?[10577]",
         "id": 10577,
         "include": "EVT?[10505]"
     },
     "10578": {
         "event": "\u4f60\u8ddf\u968f\u7236\u6bcd\u56de\u4e2d\u56fd\u4e86\u3002",
         "exclude": "TLT?[1073]",
+        "grade": 1,
         "id": 10578,
         "include": "(INT<7)&(EVT?[10542])"
     },
     "10579": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u4e16\u754c\u540d\u6821\u3002",
         "exclude": "EVT?[10579,10578]",
+        "grade": 2,
         "id": 10579,
         "include": "EVT?[10011]"
     },
     "10580": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u54c8\u4f5b\u5927\u5b66\u3002",
         "exclude": "EVT?[10580]",
+        "grade": 2,
         "id": 10580,
         "include": "(INT>8)&(EVT?[10011])"
     },
     "10581": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u8036\u9c81\u5927\u5b66\u3002",
         "exclude": "EVT?[10581]",
+        "grade": 2,
         "id": 10581,
         "include": "(INT>8)&(EVT?[10011])"
     },
     "10582": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u9ebb\u7701\u7406\u5de5\u5927\u5b66\u3002",
         "exclude": "EVT?[10582]",
+        "grade": 2,
         "id": 10582,
         "include": "(INT>8)&(EVT?[10011])"
     },
     "10583": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u52a0\u5dde\u4f2f\u514b\u5229\u3002",
         "exclude": "EVT?[10583]",
+        "grade": 2,
         "id": 10583,
         "include": "(INT>8)&(EVT?[10011])"
     },
     "10584": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u65af\u5766\u798f\u5927\u5b66\u3002",
         "exclude": "EVT?[10584]",
+        "grade": 2,
         "id": 10584,
         "include": "(INT>8)&(EVT?[10011])"
     },
     "10585": {
         "event": "\u4f60\u7684\u4e00\u4e2a\u719f\u6089\u7684\u540c\u5b66\u56e0\u4e3a\u538b\u529b\u592a\u5927\u9000\u5b66\u4e86\u3002",
         "exclude": "EVT?[10585]",
         "id": 10585,
         "include": "EVT?[10579,10580,10581,10582,10583,10584]"
     },
     "10586": {
         "event": "\u4f60\u4ee5\u7559\u5b66\u751f\u8eab\u4efd\u88ab\u6e05\u534e\u5927\u5b66\u5f55\u53d6\u3002",
         "exclude": "(EVT?[10586])|(TLT?[1107])",
+        "grade": 2,
         "id": 10586,
         "include": "EVT?[10578]"
     },
     "10587": {
         "event": "\u4f60\u4ee5\u7559\u5b66\u751f\u8eab\u4efd\u88ab\u5317\u4eac\u5927\u5b66\u5f55\u53d6\u3002",
         "exclude": "EVT?[10587]",
+        "grade": 2,
         "id": 10587,
         "include": "EVT?[10578]"
     },
     "10588": {
         "event": "\u65e0\u4e8b\u53d1\u751f\u3002",
         "id": 10588,
         "include": "TLT?[1103]"
@@ -4978,20 +5122,22 @@
     },
     "10607": {
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u524d\u5f80\u534e\u5c14\u8857\u5de5\u4f5c\uff0c\u5e74\u6536\u5165\u7ea6\u51e0\u5341\u4e07\u5200\u3002",
         "exclude": "EVT?[10607,10608,10609]",
+        "grade": 1,
         "id": 10607,
         "include": "EVT?[10606]"
     },
     "10608": {
         "event": "\u4f60\u524d\u5f80\u7845\u8c37\u521b\u4e1a\u3002",
         "exclude": "EVT?[10607,10608,10609]",
+        "grade": 1,
         "id": 10608,
         "include": "(MNY>8)&(EVT?[10606,10565])"
     },
     "10609": {
         "event": "\u4f60\u5728\u5bfc\u5e08\u7684\u5b9e\u9a8c\u5ba4\u641e\u79d1\u7814\u3002",
         "exclude": "EVT?[10607,10608,10609]",
         "id": 10609,
@@ -5023,62 +5169,69 @@
         "exclude": "(EVT?[10612,11232,10610,10611])|(TLT?[1027])",
         "id": 10612,
         "include": "EVT?[10579,10580,10581,10582,10583,10584]"
     },
     "10613": {
         "event": "\u6709\u5bb6\u91cc\u7684\u8d44\u91d1\u548c\u4eba\u8109\u652f\u6301\uff0c\u4f60\u7684\u521b\u4e1a\u975e\u5e38\u6210\u529f\u3002",
         "exclude": "EVT?[10613]",
+        "grade": 1,
         "id": 10613,
         "include": "EVT?[10608]"
     },
     "10614": {
         "event": "\u4f60\u7ed3\u8bc6\u4e86\u8bb8\u591a\u540c\u5b66\u548c\u7236\u6bcd\u4ecb\u7ecd\u7684\u5546\u4e1a\u4f19\u4f34\u3002",
         "exclude": "EVT?[10614]",
+        "grade": 1,
         "id": 10614,
         "include": "EVT?[10608,10607]"
     },
     "10615": {
         "event": "\u4f60\u975e\u5e38\u52aa\u529b\uff0c\u5728\u793e\u4ea4\u4e4b\u4e2d\u6210\u957f\u5f88\u5feb\u3002",
         "exclude": "EVT?[10615]",
+        "grade": 1,
         "id": 10615,
         "include": "EVT?[10608,10607]"
     },
     "10616": {
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u7684\u516c\u53f8\u8d8a\u505a\u8d8a\u5927\uff0c\u5b8c\u6210\u4e86\u591a\u8f6e\u878d\u8d44\uff0c\u7528\u6237\u6570\u4e5f\u7a81\u7834\u4e86\u5343\u4e07\u3002",
         "exclude": "EVT?[10616]",
+        "grade": 2,
         "id": 10616,
         "include": "EVT?[10608]"
     },
     "10617": {
         "event": "\u4f60\u7684\u516c\u53f8\u4ea7\u54c1\u7528\u6237\u6570\u7834\u767e\u4e07\u3002",
         "exclude": "EVT?[10617]",
+        "grade": 1,
         "id": 10617,
         "include": "EVT?[10608]"
     },
     "10618": {
         "event": "\u4f60\u8bf7\u4e86\u51e0\u4f4d\u4e2d\u5b66\u5927\u5b66\u65f6\u7684\u670b\u53cb\u52a0\u5165\u4f60\u7684\u516c\u53f8\u3002",
         "exclude": "EVT?[10618]",
         "id": 10618,
         "include": "EVT?[10608]"
     },
     "10619": {
         "event": "\u4f60\u7684\u516c\u53f8\u4ea7\u54c1\u7528\u6237\u6570\u7834\u4ebf\u3002",
         "exclude": "EVT?[10619]",
+        "grade": 2,
         "id": 10619,
         "include": "EVT?[10608]"
     },
     "10620": {
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u7684\u516c\u53f8\u4e0a\u5e02\u4e86\u3002",
         "exclude": "EVT?[10620]",
+        "grade": 2,
         "id": 10620,
         "include": "EVT?[10608]"
     },
     "10621": {
         "event": "\u4f60\u7684\u5b69\u5b50\u51fa\u751f\u4e86\u3002",
         "exclude": "(EVT?[10621])|(TLT?[1041,1046])",
         "id": 10621,
@@ -5089,29 +5242,32 @@
         "exclude": "(EVT?[10622])|(TLT?[1027])",
         "id": 10622,
         "include": "EVT?[10608]"
     },
     "10623": {
         "event": "\u4f60\u4e70\u4e86\u51e0\u8f86\u6570\u767e\u4e07\u3001\u4e0a\u5343\u4e07\u7684\u8c6a\u8f66\u3002",
         "exclude": "EVT?[10623]",
+        "grade": 2,
         "id": 10623,
         "include": "EVT?[10608]"
     },
     "10624": {
         "event": "\u4f60\u5728\u51e0\u5ea7\u5927\u57ce\u5e02\u90fd\u8d2d\u5165\u4e86\u8c6a\u5b85\uff0c\u8fd8\u4e70\u4e86\u6d77\u8fb9\u522b\u5885\u3002",
         "exclude": "EVT?[10624]",
+        "grade": 2,
         "id": 10624,
         "include": "EVT?[10608]"
     },
     "10625": {
         "branch": [
             "TLT?[1108]:20625"
         ],
         "event": "\u4f60\u88ab\u798f\u5e03\u65af\u8bc4\u4e3a\u7f8e\u56fd\u6700\u5e74\u8f7b\u7684\u767e\u4ebf\u5bcc\u8c6a\u6392\u540d\u7b2c\u4e00\u3002",
         "exclude": "EVT?[10625]",
+        "grade": 3,
         "id": 10625,
         "include": "EVT?[10608]"
     },
     "10626": {
         "event": "\u4f60\u521b\u7acb\u4e86\u597d\u51e0\u5bb6\u516c\u53f8\u3002",
         "exclude": "EVT?[10626]",
         "id": 10626,
@@ -5164,26 +5320,28 @@
         "exclude": "EVT?[10634]",
         "id": 10634,
         "include": "EVT?[10621]"
     },
     "10635": {
         "event": "\u4f60\u88ab\u8bc4\u4e3a\u672c\u4e16\u4ee3\u5341\u5927\u79d1\u6280\u4eba\u7269\u3002",
         "exclude": "EVT?[10635]",
+        "grade": 3,
         "id": 10635,
         "include": "EVT?[10608]"
     },
     "10636": {
         "event": "\u4f60\u7684\u5de5\u4f5c\u73b0\u5728\u5f88\u8f7b\u677e\uff0c\u5927\u591a\u6570\u65f6\u95f4\u90fd\u5728\u5bb6\u5e26\u5a03\u3002",
         "exclude": "EVT?[10636]",
         "id": 10636,
         "include": "(EVT?[10608])&(EVT?[10621])"
     },
     "10637": {
         "event": "\u4f60\u4eec\u4e00\u5bb6\u642c\u5bb6\u5230\u4e86\u745e\u58eb\u3002",
         "exclude": "EVT?[10637]",
+        "grade": 1,
         "id": 10637,
         "include": "EVT?[10608]"
     },
     "10638": {
         "event": "\u865a\u62df\u73b0\u5b9e\u6280\u672f\u5df2\u7ecf\u975e\u5e38\u6210\u719f\uff0c\u4f60\u73a9\u7684\u5174\u8da3\u4e0d\u5927\u3002",
         "exclude": "EVT?[10638]",
         "id": 10638,
@@ -5194,53 +5352,60 @@
         "exclude": "EVT?[10639]",
         "id": 10639,
         "include": "EVT?[10608]"
     },
     "10640": {
         "event": "\u4f60\u4eec\u4e00\u5bb6\u53bb\u4e86\u6b27\u6d32\u5404\u56fd\u65c5\u6e38\u3002",
         "exclude": "EVT?[10640]",
+        "grade": 1,
         "id": 10640,
         "include": "EVT?[10608]"
     },
     "10641": {
         "event": "\u4f60\u4eec\u4e00\u5bb6\u53bb\u4e86\u6fb3\u5927\u5229\u4e9a\u548c\u65b0\u897f\u5170\u65c5\u6e38\u3002",
         "exclude": "EVT?[10641]",
+        "grade": 1,
         "id": 10641,
         "include": "EVT?[10608]"
     },
     "10642": {
         "event": "\u4f60\u4eec\u4e00\u5bb6\u53bb\u4e86\u4e1c\u5357\u4e9a\u65c5\u6e38\u3002",
         "exclude": "EVT?[10642]",
+        "grade": 1,
         "id": 10642,
         "include": "EVT?[10608]"
     },
     "10643": {
         "event": "\u4f60\u4eec\u4e00\u5bb6\u53bb\u4e86\u57c3\u53ca\u548c\u963f\u8054\u914b\u65c5\u6e38\u3002",
         "exclude": "EVT?[10643]",
+        "grade": 1,
         "id": 10643,
         "include": "EVT?[10608]"
     },
     "10644": {
         "event": "\u4f60\u4eec\u4e00\u5bb6\u53bb\u4e86\u590f\u5a01\u5937\u65c5\u6e38\u3002",
         "exclude": "EVT?[10644]",
+        "grade": 1,
         "id": 10644,
         "include": "EVT?[10608]"
     },
     "10645": {
         "event": "\u4f60\u4eec\u4e00\u5bb6\u53bb\u4e86\u4e2d\u56fd\u65c5\u6e38\u3002",
         "exclude": "EVT?[10645]",
+        "grade": 1,
         "id": 10645,
         "include": "EVT?[10608,10607]"
     },
     "10646": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u6210\u4e3a\u4e86\u4e16\u754c\u9996\u5bcc\u3002",
         "exclude": "EVT?[10646]",
+        "grade": 3,
         "id": 10646,
         "include": "EVT?[10608]"
     },
     "10647": {
         "branch": [
             "TLT?[1108]:20647"
         ],
@@ -5314,14 +5479,15 @@
         "exclude": "TLT?[1048]",
         "id": 10657,
         "include": "EVT?[10011]"
     },
     "10658": {
         "event": "\u4f60\u8d22\u52a1\u81ea\u7531\uff0c\u8d2d\u4e70\u4e86\u540d\u8f66\u548c\u8c6a\u5b85\u3002",
         "exclude": "EVT?[10658]",
+        "grade": 1,
         "id": 10658,
         "include": "EVT?[10607]"
     },
     "10659": {
         "branch": [
             "TLT?[1108]:20659"
         ],
@@ -5360,26 +5526,29 @@
         "exclude": "EVT?[10663]",
         "id": 10663,
         "include": "EVT?[10609]"
     },
     "10664": {
         "event": "\u4f60\u7684\u5b9e\u9a8c\u53d6\u5f97\u4e86\u7a81\u7834\u3002",
         "exclude": "EVT?[10664]",
+        "grade": 1,
         "id": 10664,
         "include": "EVT?[10609]"
     },
     "10665": {
         "event": "\u4f60\u4e00\u5e74\u5185\u53d1\u8868\u4e86\u591a\u7bc7SCI\u3002",
         "exclude": "EVT?[10665]",
+        "grade": 2,
         "id": 10665,
         "include": "EVT?[10609]"
     },
     "10666": {
         "event": "\u4f60\u548c\u8001\u677f\u53d1\u8868\u4e86\u4e00\u7bc7Nature\u3002",
         "exclude": "EVT?[10666]",
+        "grade": 2,
         "id": 10666,
         "include": "EVT?[10609]"
     },
     "10667": {
         "event": "\u4f60\u7559\u6821\u62c5\u4efb\u52a9\u6559\u3002",
         "exclude": "EVT?[10667]",
         "id": 10667,
@@ -5389,128 +5558,145 @@
         "event": "\u4f60\u5904\u4e8e\u505a\u5b9e\u9a8c\u548c\u53d1paper\u7684\u65e0\u5c3d\u5faa\u73af\u4e2d\u3002",
         "id": 10668,
         "include": "EVT?[10609]"
     },
     "10669": {
         "event": "\u4f60\u62c5\u4efb\u526f\u6559\u6388\u3002",
         "exclude": "EVT?[10669]",
+        "grade": 1,
         "id": 10669,
         "include": "EVT?[10609]"
     },
     "10670": {
         "event": "\u4f60\u53d1\u8868\u4e00\u7bc7\u4e00\u4f5cNature\u3002",
         "exclude": "EVT?[10670]",
         "id": 10670,
         "include": "EVT?[10609]"
     },
     "10671": {
         "event": "\u4f60\u88ab\u6bcd\u6821\u8058\u4e3a\u6b63\u6559\u6388\u3002",
         "exclude": "EVT?[10671]",
+        "grade": 2,
         "id": 10671,
         "include": "EVT?[10669]"
     },
     "10672": {
         "event": "\u4f60\u88ab\u4e2d\u56fd\u591a\u6240\u540d\u6821\u8058\u4e3a\u5ba2\u5ea7\u6559\u6388\u3002",
         "exclude": "EVT?[10672]",
+        "grade": 1,
         "id": 10672,
         "include": "EVT?[10609]"
     },
     "10673": {
         "event": "\u4f60\u83b7\u5f97\u591a\u9879\u5927\u5956\u3002",
         "exclude": "EVT?[10673]",
+        "grade": 2,
         "id": 10673,
         "include": "EVT?[10609]"
     },
     "10674": {
         "event": "\u4f60\u5728\u5fae\u89c2\u7c92\u5b50\u9886\u57df\u53d6\u5f97\u91cd\u8981\u7a81\u7834\u3002",
         "exclude": "EVT?[10674,10675,10676]",
+        "grade": 2,
         "id": 10674,
         "include": "EVT?[10609]"
     },
     "10675": {
         "event": "\u4f60\u5728\u9057\u4f20\u9886\u57df\u53d6\u5f97\u91cd\u8981\u7a81\u7834\u3002",
         "exclude": "EVT?[10674,10675,10676]",
+        "grade": 2,
         "id": 10675,
         "include": "EVT?[10609]"
     },
     "10676": {
         "event": "\u4f60\u5728\u6750\u6599\u9886\u57df\u53d6\u5f97\u91cd\u8981\u7a81\u7834\u3002",
         "exclude": "EVT?[10674,10675,10676]",
+        "grade": 2,
         "id": 10676,
         "include": "EVT?[10609]"
     },
     "10677": {
         "event": "\u4f60\u6210\u4e3a\u7f8e\u56fd\u79d1\u5b66\u9662\u9662\u58eb\u3002",
         "exclude": "EVT?[10677]",
+        "grade": 3,
         "id": 10677,
         "include": "EVT?[10609]"
     },
     "10678": {
         "event": "\u4f60\u6210\u4e3a\u4e2d\u56fd\u79d1\u5b66\u9662\u5916\u7c4d\u9662\u58eb\u3002",
         "exclude": "EVT?[10678]",
+        "grade": 3,
         "id": 10678,
         "include": "EVT?[10609]"
     },
     "10679": {
         "effect": {
             "MNY": 1,
             "SPR": 2
         },
         "event": "\u4f60\u83b7\u5f97\u4e86\u8bfa\u8d1d\u5c14\u7269\u7406\u5b66\u5956\u3002",
         "exclude": "EVT?[10679]",
+        "grade": 3,
         "id": 10679,
         "include": "EVT?[10674]"
     },
     "10680": {
         "effect": {
             "MNY": 1,
             "SPR": 2
         },
         "event": "\u4f60\u83b7\u5f97\u4e86\u8bfa\u8d1d\u5c14\u751f\u7406\u5b66\u6216\u533b\u5b66\u5956\u3002",
         "exclude": "EVT?[10680]",
+        "grade": 3,
         "id": 10680,
         "include": "EVT?[10675]"
     },
     "10681": {
         "effect": {
             "MNY": 1,
             "SPR": 2
         },
         "event": "\u4f60\u83b7\u5f97\u4e86\u8bfa\u8d1d\u5c14\u5316\u5b66\u5956\u3002",
         "exclude": "EVT?[10681]",
+        "grade": 3,
         "id": 10681,
         "include": "EVT?[10676]"
     },
     "10682": {
         "event": "\u4f60\u653e\u5f03\u7f8e\u56fd\u56fd\u7c4d\uff0c\u6bc5\u7136\u52a0\u5165\u4e2d\u56fd\u56fd\u7c4d\u524d\u5f80\u4e2d\u56fd\u7684\u5927\u5b66\u3002",
         "exclude": "EVT?[10682]",
+        "grade": 3,
         "id": 10682,
         "include": "EVT?[10609]"
     },
     "10683": {
         "event": "\u4f60\u521b\u5efa\u4e86\u4e00\u4e2a\u4ee5\u4f60\u540d\u5b57\u547d\u540d\u7684\u6148\u5584\u57fa\u91d1\u4f1a\u3002",
         "exclude": "EVT?[10683]",
+        "grade": 1,
         "id": 10683,
         "include": "EVT?[10608]"
     },
     "10684": {
         "event": "\u4f60\u51b3\u5b9a\u5c06\u4f60\u7684\u9057\u4ea7\u90fd\u6350\u8d60\u7ed9\u6bcd\u6821\u3002",
         "exclude": "EVT?[10684,10685,10682]",
+        "grade": 1,
         "id": 10684,
         "include": "EVT?[10609]"
     },
     "10685": {
         "event": "\u4f60\u51b3\u5b9a\u5c06\u4f60\u7684\u9057\u4ea7\u90fd\u6350\u8d60\u7ed9\u4e2d\u56fd\u5927\u5b66\u7528\u4e8e\u5efa\u8bbe\u3002",
         "exclude": "EVT?[10685,10684]",
+        "grade": 1,
         "id": 10685,
         "include": "EVT?[10682]"
     },
     "10686": {
         "event": "\u4f60\u7684\u8bba\u6587\u4ed6\u5f15\u8d85\u8fc7\u5341\u4e07\u3002",
         "exclude": "EVT?[10686]",
+        "grade": 1,
         "id": 10686,
         "include": "EVT?[10609]"
     },
     "10687": {
         "event": "\u4f60\u5728\u4e16\u754c\u5de1\u56de\u8bb2\u5ea7\u3002",
         "id": 10687,
         "include": "EVT?[10609]"
@@ -5532,14 +5718,15 @@
         "exclude": "EVT?[10690]",
         "id": 10690,
         "include": "EVT?[10607,10608]"
     },
     "10691": {
         "event": "\u6709\u4eba\u4ee5\u4f60\u7684\u4eba\u751f\u4e3a\u539f\u672c\u62cd\u6444\u4e86\u7535\u5f71\u3002",
         "exclude": "EVT?[10691]",
+        "grade": 1,
         "id": 10691,
         "include": "EVT?[10608]"
     },
     "10692": {
         "event": "\u4f60\u7684\u81ea\u4f20\u4e00\u76f4\u8d85\u7ea7\u7545\u9500\u3002\u4eba\u4eec\u88ab\u4f60\u7684\u52aa\u529b\u548c\u7cbe\u795e\u6240\u6253\u52a8\u3002",
         "exclude": "EVT?[10692]",
         "id": 10692,
@@ -5620,15 +5807,15 @@
     "10705": {
         "event": "\u4e2d\u56fd\u5ba3\u5e03\u540c\u6027\u604b\u4e3a\u72af\u7f6a\uff0c\u5c06\u81f3\u5c11\u5224\u59043\u5e74\u4ee5\u4e0b\u7684\u6709\u671f\u5f92\u5211\u3002",
         "exclude": "EVT?[10705]",
         "id": 10705,
         "include": "EVT?[10011]"
     },
     "10706": {
-        "event": "\u91d1\u6b63\u6069\u5728\u671d\u9c9c\u79f0\u5e1d\uff0c\u6539\u4e3a\u5e1d\u5236\u3002",
+        "event": "\u4e3a\u51cf\u5c11\u62db\u8058\u65f6\u7684\u6027\u522b\u6b67\u89c6\uff0c\u67d0\u5730\u51fa\u53f0\u65b0\u89c4\u5b9a\uff1a\u5458\u5de5\u4f11\u4ea7\u5047\u65f6\u7684\u5de5\u8d44\u5c06\u5ef6\u8fdf\u5230\u4ea7\u5047\u7ed3\u675f\u540e\u7684\u76f8\u540c\u957f\u5ea6\u65f6\u95f4\u5185\u968f\u5de5\u8d44\u53d1\u653e\u3002",
         "exclude": "EVT?[10706]",
         "id": 10706,
         "include": "EVT?[10011]"
     },
     "10707": {
         "event": "\u4f60\u5b66\u4f1a\u4e86\u6253\u9ebb\u5c06\u3002",
         "exclude": "EVT?[10707]",
@@ -5679,20 +5866,22 @@
         "exclude": "EVT?[10714]",
         "id": 10714,
         "include": "EVT?[10011]"
     },
     "10715": {
         "event": "\u4f60\u53d1\u73b0\u4e86\u5927\u7edf\u4e00\u6a21\u578b\u3002",
         "exclude": "EVT?[10715]",
+        "grade": 3,
         "id": 10715,
         "include": "EVT?[10679]"
     },
     "10716": {
         "event": "\u4f60\u518d\u6b21\u83b7\u5f97\u8bfa\u8d1d\u5c14\u7269\u7406\u5b66\u5956\u3002",
         "exclude": "EVT?[10716]",
+        "grade": 3,
         "id": 10716,
         "include": "EVT?[10715]"
     },
     "10717": {
         "event": "\u4f60\u611f\u89c9\u5b66\u6821\u7684\u73af\u5883\u5404\u65b9\u9762\u90fd\u4e0d\u5982\u7f8e\u56fd\u597d\u3002",
         "exclude": "EVT?[10717]",
         "id": 10717,
@@ -5783,23 +5972,25 @@
     },
     "10731": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u5047\u671f\u53bb\u4e86\u4e0a\u6d77\u548c\u9999\u6e2f\u73a9\u3002",
         "exclude": "EVT?[10731]",
+        "grade": 1,
         "id": 10731,
         "include": "EVT?[10586,10587]"
     },
     "10732": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u5047\u671f\u53bb\u897f\u85cf\u65c5\u6e38\u3002",
         "exclude": "EVT?[10732]",
+        "grade": 1,
         "id": 10732,
         "include": "EVT?[10586,10587]"
     },
     "10733": {
         "event": "\u6709\u77ed\u89c6\u9891\u4e3b\u64ad\u91c7\u8bbf\u4f60\u82f1\u6587\u6c34\u5e73\u5982\u4f55\uff0c\u4f60\u5047\u88c5\u662f\u666e\u901a\u5b66\u751f\u4f5c\u7b54\u3002",
         "exclude": "EVT?[10733]",
         "id": 10733,
@@ -5822,14 +6013,15 @@
         "exclude": "EVT?[10736]",
         "id": 10736,
         "include": "EVT?[10586,10587]"
     },
     "10737": {
         "event": "\u4f60\u8fdb\u5165\u540d\u4f01\u5de5\u4f5c\u3002",
         "exclude": "EVT?[10737]",
+        "grade": 1,
         "id": 10737,
         "include": "EVT?[10586,10587]"
     },
     "10738": {
         "event": "\u4f60\u7684\u5de5\u4f5c\u5e76\u4e0d\u50cf\u5176\u4ed6\u4eba\u76db\u4f20\u7684\u90a3\u79cd996\uff0c\u4e0b\u5348\u4e0b\u73ed\u540e\u4f60\u8fd8\u53bb\u5065\u8eab\u3002",
         "exclude": "EVT?[10738]",
         "id": 10738,
@@ -5837,14 +6029,15 @@
     },
     "10739": {
         "effect": {
             "SPR": 1
         },
         "event": "\u516c\u53f8\u7ec4\u7ec7\u53bb\u9a6c\u5c14\u4ee3\u592b\u65c5\u6e38\u3002",
         "exclude": "EVT?[10739]",
+        "grade": 1,
         "id": 10739,
         "include": "EVT?[10586,10587]"
     },
     "10740": {
         "effect": {
             "SPR": 1
         },
@@ -5891,24 +6084,26 @@
     },
     "10746": {
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u5347\u804c\u4e86\u3002",
         "exclude": "EVT?[10746,10002,10110,10111]",
+        "grade": 1,
         "id": 10746,
         "include": "EVT?[10586,10587]"
     },
     "10747": {
         "effect": {
             "MNY": 1,
             "SPR": 1
         },
         "event": "\u4f60\u53c8\u5347\u804c\u4e86\u3002",
         "exclude": "EVT?[10747,10002,10110,10111]",
+        "grade": 1,
         "id": 10747,
         "include": "EVT?[10746]"
     },
     "10748": {
         "event": "\u4f60\u6709\u6b21\u5728\u5730\u94c1\u4e0a\u88ab\u5077\u4e86\u624b\u673a\uff0c\u62a5\u8b66\u540e\u8b66\u65b9\u9ad8\u5ea6\u91cd\u89c6\uff0c\u7acb\u5373\u51fa\u52a8\uff0c\u5f53\u5929\u5c31\u8ffd\u56de\u4e86\u4f60\u7684\u624b\u673a\u3002",
         "exclude": "EVT?[10748]",
         "id": 10748,
@@ -5919,20 +6114,22 @@
         "exclude": "EVT?[10749]",
         "id": 10749,
         "include": "EVT?[10586,10587]"
     },
     "10750": {
         "event": "\u4f60\u5728\u89c6\u9891APP\u4e0a\u5206\u4eab\u4f60\u7684\u4eba\u751f\uff0c\u6536\u83b7\u5927\u91cf\u7c89\u4e1d\u3002",
         "exclude": "EVT?[10750]",
+        "grade": 1,
         "id": 10750,
         "include": "(CHR>6)&(EVT?[10586,10587])"
     },
     "10751": {
         "event": "\u4f60\u7ecf\u5e38\u901b\u77e5\u4e4e\u5e76\u56de\u7b54\u56fd\u5916\u548c\u5546\u4e1a\u76f8\u5173\u95ee\u9898\uff0c\u8fc5\u901f\u6210\u4e3a\u5927V\u3002",
         "exclude": "EVT?[10751]",
+        "grade": 1,
         "id": 10751,
         "include": "EVT?[10586,10587]"
     },
     "10752": {
         "event": "\u4f60\u9010\u6e10\u610f\u8bc6\u5230\u4f60\u548c\u666e\u901a\u4e2d\u56fd\u4eba\u601d\u7ef4\u65b9\u5f0f\u7684\u4e0d\u540c\u3002",
         "exclude": "EVT?[10752]",
         "id": 10752,
@@ -5943,14 +6140,15 @@
         "exclude": "EVT?[10753,10001]",
         "id": 10753,
         "include": "EVT?[10586,10587]"
     },
     "10754": {
         "event": "\u4f60\u7ec4\u7ec7\u4e00\u4e9b\u7ebf\u4e0b\u6d3b\u52a8\uff0c\u548c\u5f88\u591a\u906d\u9047\u6027\u522b\u6b67\u89c6\u7684\u4eba\u4e00\u8d77\u8ba8\u8bba\u65b9\u6848\u548c\u5206\u4eab\u7ecf\u5386\u3002",
         "exclude": "EVT?[10754]",
+        "grade": 1,
         "id": 10754,
         "include": "EVT?[10753]"
     },
     "10755": {
         "event": "\u4f60\u51fa\u4e86\u4e00\u672c\u63cf\u7ed8\u548c\u5206\u6790\u6027\u522b\u6b67\u89c6\u73b0\u8c61\u7684\u4e66\u3002",
         "exclude": "EVT?[10755]",
         "id": 10755,
@@ -5958,35 +6156,39 @@
     },
     "10756": {
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u7684\u7406\u8d22\u6536\u76ca\u4e0d\u9519\u3002",
         "exclude": "EVT?[10756]",
+        "grade": 1,
         "id": 10756,
         "include": "(MNY>6)&(EVT?[10586,10587])"
     },
     "10757": {
         "event": "\u4f60\u53bb\u9ec4\u5c71\u65c5\u6e38\u3002",
         "exclude": "EVT?[10757]",
+        "grade": 1,
         "id": 10757,
         "include": "EVT?[10586,10587]"
     },
     "10758": {
         "event": "\u4f60\u8bf7\u4e86\u5e74\u5047\u4e00\u53e3\u6c14\u6e38\u73a9\u4e86\u4e94\u5cb3\u3002",
         "exclude": "EVT?[10758]",
+        "grade": 1,
         "id": 10758,
         "include": "EVT?[10586,10587]"
     },
     "10759": {
         "branch": [
             "INT<7:20759"
         ],
         "event": "\u4f60\u53bb\u4e09\u4e9a\u65c5\u6e38\u3002",
         "exclude": "EVT?[10759]",
+        "grade": 1,
         "id": 10759,
         "include": "EVT?[10586,10587]"
     },
     "10760": {
         "event": "\u4f60\u7684\u4e00\u4f4d\u540c\u4e8b\u4ee3\u5b55\u4e86\u7b2c\u4e09\u80ce\u3002",
         "exclude": "EVT?[10760]",
         "id": 10760,
@@ -6000,44 +6202,48 @@
     },
     "10762": {
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u7f51\u4e0a\u7684\u7c89\u4e1d\u5f88\u591a\uff0c\u4f60\u7684\u7f51\u7ea2\u6536\u5165\u751a\u81f3\u8d85\u8fc7\u4f60\u7684\u5de5\u8d44\u3002",
         "exclude": "EVT?[10762]",
+        "grade": 1,
         "id": 10762,
         "include": "EVT?[10750,10751]"
     },
     "10763": {
         "event": "\u4f60\u7684\u9879\u76ee\u5927\u83b7\u6210\u529f\u3002",
         "exclude": "EVT?[10763]",
+        "grade": 1,
         "id": 10763,
         "include": "EVT?[10586,10587]"
     },
     "10764": {
         "event": "\u5728\u4e00\u6b21\u91cd\u8981\u7684\u996d\u5c40\u4e2d\uff0c\u4f60\u4f5c\u4e3a\u7ffb\u8bd1\u51fa\u573a\u3002",
         "exclude": "EVT?[10764]",
         "id": 10764,
         "include": "(INT>2)&(EVT?[10586,10587])"
     },
     "10765": {
         "event": "\u4f60\u8d2d\u4e70\u4e86\u540d\u8f66\u540d\u8868\u3002",
         "exclude": "EVT?[10765]",
+        "grade": 1,
         "id": 10765,
         "include": "(MNY>7)&(EVT?[10586,10587])"
     },
     "10766": {
         "event": "\u4f60\u53c2\u52a0\u4e86\u516c\u53f8\u91cc\u7684\u65af\u8bfa\u514b\u6bd4\u8d5b\u3002",
         "exclude": "EVT?[10766]",
         "id": 10766,
         "include": "(STR>3)&(EVT?[10586,10587])"
     },
     "10767": {
         "event": "\u4f60\u4ec5\u51ed\u6bcf\u6708\u7684\u7406\u8d22\u6536\u5165\u5c31\u8d85\u8fc799%\u7684\u4eba\u4e86\u3002",
         "exclude": "EVT?[10767]",
+        "grade": 1,
         "id": 10767,
         "include": "(MNY>7)&(EVT?[10586,10587])"
     },
     "10768": {
         "branch": [
             "(EVT?[10010])&(EVT?[10007,10008]):30002",
             "TLT?[1135]:40062",
@@ -6051,100 +6257,115 @@
     "10769": {
         "event": "\u4f60\u9000\u4f11\u4e86\u3002",
         "exclude": "EVT?[10769]",
         "id": 10769,
         "include": "EVT?[10586,10587]"
     },
     "10770": {
-        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u4f60\u6361\u5230\u4e00\u5f20\u7eb8\u6761\uff0c\u4e0a\u9762\u5199\u7740\u201c\u5feb20\u4e2a\u7fa4\u90fd\u52a0\u6ee1\u4e86\uff0c\u4e0d\u52a0\u4e86\u4e0d\u52a0\u4e86\uff0c\u5173\u6ce8\u7b56\u5212\u7684\u8d34\u5427\u53f7\u795e\u6237\u5c0f\u5fb7\u6216\u8005B\u7ad9\u795e\u6237\u827e\u5170\u5fb7\u5427\uff0c\u4e0d\u8981\u79c1\u4fe1\u4e86\u6c42\u6c42\u4e86\u201c",
+        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u5feb20\u4e2a\u7fa4\u90fd\u52a0\u6ee1\u4e86\uff0c\u4e0d\u52a0\u4e86\u4e0d\u52a0\u4e86\uff0c\u5173\u6ce8\u7b56\u5212\u7684\u8d34\u5427\u53f7\u6216\u8005B\u7ad9\u8d26\u53f7\u795e\u6237\u5c0f\u5fb7\u5427",
         "exclude": "EVT?[10770]",
+        "grade": 2,
         "id": 10770,
         "include": "TLT?[1112]"
     },
     "10771": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u67d0\u7b56\u5212\u81ea\u5df1\u91cd\u5f00\u4e86500\u591a\u6b21\uff0c\u6700\u597d\u6210\u7ee9\u662f\u6b7b\u5728\u5fc3\u9b54\u52ab\uff0c\u5fc3\u6001\u5d29\u4e86\uff0c\u4e00\u76f4\u6ca1\u6210\u529f\u98de\u5347\u8fc7\u3002",
         "exclude": "EVT?[10771,10772]",
+        "grade": 2,
         "id": 10771,
         "include": "TLT?[1112]"
     },
     "10772": {
-        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u636e\u8bf4\u6309\u4e0b\u7279\u522b\u611f\u8c22\u6309\u94ae\uff0c\u518d\u6309\u4e0b\u6253\u8d4f\u6309\u94ae\uff0c\u53ef\u4ee5\u572824\u5c0f\u65f6\u5185\u8ba9\u81ea\u5df1\u7684\u540d\u5b57\u51fa\u73b0\u5728\u611f\u8c22\u540d\u5355\u4e0a\uff08\u96fe",
+        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u73b0\u5728BUG\u5f88\u591a\uff0c\u5e0c\u671b\u5927\u5bb6\u9047\u5230\u4e86BUG\u53ef\u4ee5\u901a\u77e5\u6211\u4eec\u3002BUG\u53ca\u610f\u89c1\u6536\u96c6Q\u7fa4\uff1a750452276",
         "exclude": "EVT?[10772,10771]",
+        "grade": 2,
         "id": 10772,
         "include": "TLT?[1112]"
     },
     "10773": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u636e\u8bf4\uff0c\u4fee\u4ed9\u8005\u662f\u771f\u5b9e\u5b58\u5728\u7684\u2026\u2026",
         "exclude": "EVT?[10773,10774]",
+        "grade": 2,
         "id": 10773,
         "include": "TLT?[1112]"
     },
     "10774": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u636e\u8bf4\uff0c\u6b63\u5e38\u4eba\u65e0\u8bba\u5982\u4f55\u90fd\u6d3b\u4e0d\u5230100\u5c81\uff0c\u9664\u975e\u2026\u2026\u6709\u4e2a\u5c0f\u76d2\u5b50\uff1f",
         "exclude": "EVT?[10774,10773]",
+        "grade": 2,
         "id": 10774,
         "include": "TLT?[1112]"
     },
     "10775": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u8003\u53e4\u5b66\u5bb6\u53d1\u73b0\u4e00\u7c92\u53e4\u4ee3\u7684\u836f\u4e38\uff0c\u770b\u4e0a\u53bb\u91d1\u707f\u707f\u7684\uff0c\u4e0d\u50cf\u51e1\u7269\u3002",
         "exclude": "EVT?[10775]",
+        "grade": 2,
         "id": 10775,
         "include": "TLT?[1112]"
     },
     "10776": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u4f60\u770b\u4e86\u4e00\u672c\u53e4\u4ee3\u7684\u7384\u5e7b\u5c0f\u8bf4\uff0c\u91cc\u9762\u8fbe\u5230\u5316\u795e\u671f\u9700\u8981\u609f\u900f\u6df7\u6c8c\u5927\u9053\u3002",
         "exclude": "EVT?[10776]",
+        "grade": 2,
         "id": 10776,
         "include": "TLT?[1112]"
     },
     "10777": {
-        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u6709\u4eba\u8bf4\u201c\u5982\u679c\u4f60\u5f88\u6709\u94b1\uff0c\u5c31\u51fa\u751f\u4e0d\u5230\u519c\u6751\uff1b\u5f88\u7a77\uff0c\u5c31\u51fa\u751f\u4e0d\u5230\u57ce\u5e02\u3002\u4e00\u4e2a\u731c\u6d4b\uff0c\u4e0d\u77e5\u9053\u5bf9\u4e0d\u5bf9\u3002\u201d",
+        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u73b0\u5b9e\u4e16\u754c\u5176\u5b9e\u6bd4\u6e38\u620f\u66f4\u9b54\u5e7b\u3002",
         "exclude": "EVT?[10777]",
+        "grade": 2,
         "id": 10777,
         "include": "TLT?[1112]"
     },
     "10778": {
-        "event": "\u3010\u7edd\u7edd\u5b50\u6d88\u606f\u3011\u4eca\u65e5\u4efd\u751c\u751c\u788e\u7247\u5df2\u52a0\u8f7d\u5b8c\u6bd5  \uff0c\u4e0d\u662f8\u20e3\ufe0f\uff0c\u5b9d\uff01\u6211\u4eca\u5929\u91cd\u5f00\u4eba\u751f\u4e86  \uff0c\u6211\u771f\u7684\u54ed\u6b7b\uff0c\u5462\u5462\u5462\uff0c\u8fd9\u5bb6\u7684\u4eba\u751f\u597d\u91cd\u5f00\u5230\u8dfajiojio\uff5e\uff5e\uff5e\u8fd9\u676f\u5c0f\u5e03\u4e01\u4e5f\u6709\u88ab\u60ca\u8273\u5230\u2049\ufe0f\u2049\ufe0f\u2049\ufe0f\u65e0\u8bed\u5b50\uff0c\u8def\u4e0a\u8fd8\u770b\u89c1\u4e00\u4e2aJava\u7537\uff0c\u5927\u65e0\u8bed\u4e8b\u4ef6\uff0c\u54d2\u54d2\u54d2\uff0c\u5c81\u6708\u6f2b\u957f \u90a3\u5c31\u4e00\u8d77\u62ef\u6551\u5730\u7403\u4e0e\u4e50\u8da3\u5427  ",
+        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u73b0\u5728\u5df2\u7ecf\u6ca1\u591a\u5c11\u6d3b\u8dc3\u73a9\u5bb6\u4e86\uff0c\u8fc7\u9635\u5b50\u4eba\u66f4\u5c11\u7684\u8bdd\uff0c\u6587\u6848\u662f\u4e0d\u662f\u53ef\u4ee5\u66f4\u52a0\u653e\u98de\u81ea\u6211\u4e86\uff08\u8bef",
         "exclude": "EVT?[10778]",
+        "grade": 2,
         "id": 10778,
         "include": "EVT?[10770,10771,10772,10773,10774,10775,10776,10777,10779,10780]"
     },
     "10779": {
-        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u9057\u4f20\u5b66\u5bb6\u8bf4\uff0c\u6700\u597d\u7684\u5929\u8d4b\u53ea\u67090.1%\u7684\u51e0\u7387\u51fa\u73b0\uff0c\u5176\u6b21\u7684\u5929\u8d4b\u662f1%\uff0c\u6bd4\u8f83\u597d\u7684\u5929\u8d4b\u662f10%\u3002",
+        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u4e0d\u4f1a\u5427\uff0c2023\u5e74\u4e86\u5c45\u7136\u8fd8\u6709\u4eba\u5728\u4eba\u751f\u91cd\u5f00\uff1f",
         "exclude": "EVT?[10779]",
+        "grade": 2,
         "id": 10779,
         "include": "TLT?[1112]"
     },
     "10780": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u4e13\u5bb6\u8ba4\u4e3a\uff0c\u4e00\u4e9b\u4e2d\u8001\u5e74\u4eba\u751f\u6d3b\u4e4f\u5473\uff0c\u53ea\u80fd\u770b\u65b0\u95fb\u5ea6\u65e5\uff0c\u662f\u56e0\u4e3a\u67d0\u4eba\u7f16\u4e0d\u51fa\u4e8b\u4ef6\u4e86\u3002",
         "exclude": "EVT?[10780]",
+        "grade": 2,
         "id": 10780,
         "include": "TLT?[1112]"
     },
     "10781": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u4e00\u5c45\u6c11\u88ab\u4e00\u8f86\u5931\u63a7\u7684\u6ce5\u5934\u8f66\u649e\u5230\uff0c\u4e0d\u5e78\u8eab\u4ea1\u3002\u636e\u76ee\u51fb\u8005\u79f0\uff0c\u53d7\u5bb3\u8005\u88ab\u649e\u540e\u66fe\u9ad8\u547c\u201c\u8fd9\u4e0d\u53ef\u80fd\uff0c\u6211\u662f\u4e09\u8f6c\u6e21\u52ab\u5927\u80fd\u201d\u4e4b\u7c7b\u7684\u8bdd\u3002",
         "exclude": "EVT?[10781]",
+        "grade": 2,
         "id": 10781,
         "include": "TLT?[1112]"
     },
     "10782": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u4f60\u770b\u4e86\u4e00\u672c\u7384\u5e7b\u5c0f\u8bf4\uff0c\u5c0f\u8bf4\u91cc\u60f3\u5ea6\u8fc7\u5929\u52ab\u9700\u8981\u609f\u900f\u5168\u90e8\u4e94\u884c\u5927\u9053\u548c\u4efb\u610f\u4e00\u79cd\u672c\u6e90\u5927\u9053\u3002",
         "exclude": "EVT?[10782]",
+        "grade": 2,
         "id": 10782,
         "include": "TLT?[1112]"
     },
     "10783": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u4e00\u540d\u4e0d\u523025\u5c81\u7684\u4f5c\u8005\u5f3a\u884c\u63cf\u5199\u5b8c\u5168\u4e0d\u61c2\u7684\u4e2d\u5e74\u548c\u5a5a\u540e\u751f\u6d3b\uff0c\u906d\u81f4\u5927\u91cf\u6279\u8bc4\u3002",
         "exclude": "EVT?[10783]",
+        "grade": 2,
         "id": 10783,
         "include": "TLT?[1112]"
     },
     "10784": {
         "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u67d0\u8fa3\u9e21\u6e38\u620f\u5341\u8fde\u62bd\u7adf\u7136\u6ca1\u6709\u4fdd\u5e95\uff0c\u5c31\u50cf\u5730\u7403online\u4e00\u6837\u3002",
         "exclude": "EVT?[10784]",
+        "grade": 2,
         "id": 10784,
         "include": "TLT?[1112]"
     },
     "10785": {
         "branch": [
             "STR<2:10000"
         ],
@@ -6177,36 +6398,39 @@
             "INT": 1,
             "MNY": 1,
             "SPR": 1,
             "STR": 1
         },
         "event": "\u4f60\u8fdb\u5165\u4e86\u4e00\u4e2a\u6e21\u52ab\u671f\u5927\u80fd\u7684\u4f20\u627f\u6d1e\u5e9c\u3002",
         "exclude": "EVT?[10787]",
+        "grade": 1,
         "id": 10787,
         "include": "(INT>5)&(TLT?[1048])",
         "postEvent": "\u867d\u7136\u6ca1\u80fd\u901a\u8fc7\u4f20\u627f\uff0c\u4f46\u83b7\u5f97\u4e86\u5c11\u91cf\u597d\u5904\u3002"
     },
     "10788": {
         "NoRandom": 1,
         "effect": {
             "CHR": 2,
             "INT": 20,
             "MNY": 2,
             "SPR": 2,
             "STR": 200
         },
         "event": "\u83b7\u5f97\u4e86\u4f20\u627f\u3002\u6240\u6709\u5c5e\u6027\u5927\u5e45\u63d0\u5347\u3002",
+        "grade": 2,
         "id": 10788
     },
     "10789": {
         "effect": {
             "INT": 100
         },
         "event": "\u4f60\u6361\u5230\u4e00\u4e2a\u7834\u788e\u7684\u4ed9\u5668\uff0c\u91cc\u9762\u6709\u4e2a\u77e5\u8bc6\u6e0a\u535a\u7684\u5668\u9b42\u3002",
         "exclude": "EVT?[10789]",
+        "grade": 2,
         "id": 10789,
         "include": "(MNY>13)&(TLT?[1048])",
         "postEvent": "\u4ece\u6b64\u667a\u529b\u4e0d\u518d\u662f\u4f60\u4fee\u884c\u8def\u4e0a\u7684\u95ee\u9898\u3002"
     },
     "10790": {
         "effect": {
             "STR": -1
@@ -6227,14 +6451,15 @@
         "exclude": "EVT?[10792]",
         "id": 10792,
         "include": "EVT?[10011]"
     },
     "10793": {
         "event": "\u4f60\u4eec\u5bb6\u4e70\u4e86\u98de\u8f66\uff0c\u5168\u7403\u62e5\u6709\u98de\u8f66\u7684\u4eba\u5f88\u5c11\u5f88\u5c11\u3002",
         "exclude": "EVT?[10793]",
+        "grade": 1,
         "id": 10793,
         "include": "EVT?[10011]"
     },
     "10794": {
         "effect": {
             "STR": -2
         },
@@ -6254,14 +6479,15 @@
         "exclude": "EVT?[10796]",
         "id": 10796,
         "include": "EVT?[10011]"
     },
     "10797": {
         "event": "\u5927\u592a\u7a7a\u822a\u884c\u65f6\u4ee3\u5230\u6765\u3002",
         "exclude": "EVT?[10797]",
+        "grade": 2,
         "id": 10797,
         "include": "EVT?[10011]"
     },
     "10798": {
         "event": "\u7ecf\u5e38\u6709\u5e74\u8f7b\u65f6\u7684\u719f\u4eba\u6765\u62dc\u8bbf\u4f60\u3002",
         "exclude": "EVT?[10798]",
         "id": 10798,
@@ -6272,26 +6498,29 @@
         "exclude": "EVT?[10799,10715]",
         "id": 10799,
         "include": "EVT?[10011]"
     },
     "10800": {
         "event": "\u4f60\u5bb6\u8bbe\u7f6e\u4e86\u6a21\u62df\u5916\u666f\uff0c\u53ef\u4ee5\u5b9e\u65f6\u663e\u793a\u4e16\u754c\u5404\u5730\u7684\u98ce\u5149\u3002",
         "exclude": "EVT?[10800]",
+        "grade": 1,
         "id": 10800,
         "include": "EVT?[10011]"
     },
     "10801": {
         "event": "\u4f60\u5bb6\u6362\u4e0a\u4e86\u81ea\u52a8\u5730\u677f\uff0c\u53ef\u4ee5\u81ea\u52a8\u6e05\u6d01\u3001\u79fb\u52a8\u3001\u53d8\u6e29\u7b49\u3002",
         "exclude": "EVT?[10801]",
+        "grade": 1,
         "id": 10801,
         "include": "EVT?[10011]"
     },
     "10802": {
         "event": "\u4f60\u5bb6\u6362\u4e0a\u4e86\u610f\u8bc6\u63a7\u5236\u5bb6\u5177\u3002\u8111\u4e2d\u601d\u8003\u5c31\u53ef\u4ee5\u63a7\u5236\u5bb6\u5177\u5bb6\u7535\u3002",
         "exclude": "EVT?[10802]",
+        "grade": 1,
         "id": 10802,
         "include": "EVT?[10011]"
     },
     "10803": {
         "event": "\u4f60\u611f\u53f9\u533b\u5b66\u53d1\u5c55\u7f13\u6162\uff0c\u81f3\u4eca\u4ecd\u672a\u653b\u514b\u764c\u75c7\u548c\u5fc3\u8840\u7ba1\u75be\u75c5\u3002",
         "exclude": "EVT?[10803]",
         "id": 10803,
@@ -6302,20 +6531,22 @@
         "exclude": "EVT?[10804]",
         "id": 10804,
         "include": "EVT?[10011]"
     },
     "10805": {
         "event": "\u4e2d\u56fd\u53ef\u63a7\u6838\u805a\u53d8\u6280\u672f\u5b8c\u5168\u6210\u719f\uff0c\u8fdb\u5165\u65e0\u9650\u80fd\u6e90\u7684\u65f6\u4ee3\u3002",
         "exclude": "EVT?[10805]",
+        "grade": 2,
         "id": 10805,
         "include": "EVT?[10011]"
     },
     "10806": {
         "event": "\u4eba\u7c7b\u51e0\u4e4e\u53ef\u4ee5\u5b8c\u5168\u63a7\u5236\u5929\u6c14\u3002",
         "exclude": "EVT?[10806]",
+        "grade": 2,
         "id": 10806,
         "include": "EVT?[10011,10010]"
     },
     "10807": {
         "event": "\u4f60\u8d8a\u6765\u8d8a\u559c\u6b22\u54f2\u5b66\u4e66\u7c4d\uff0c\u7ecf\u5e38\u770b\u300a\u9053\u5fb7\u7ecf\u300b\u548c\u540e\u73b0\u4ee3\u54f2\u5b66\u3002",
         "exclude": "EVT?[10807]",
         "id": 10807,
@@ -6371,23 +6602,25 @@
     },
     "10816": {
         "effect": {
             "STR": 20
         },
         "event": "\u4f60\u56e0\u4e3a\u5bb9\u8c8c\u88ab\u7834\u4f8b\u8fdb\u5165\u4e00\u5ea7\u6d1e\u5e9c\u3002\u4f53\u8d28\u5927\u5e45\u63d0\u5347\u3002",
         "exclude": "EVT?[10816]",
+        "grade": 1,
         "id": 10816,
         "include": "(CHR>13)&(TLT?[1048])"
     },
     "10817": {
         "effect": {
             "STR": 50
         },
         "event": "\u4f60\u6361\u5230\u5929\u9636\u7075\u5668\uff0c\u5b9e\u529b\u5927\u5e45\u63d0\u5347\u3002",
         "exclude": "EVT?[10817]",
+        "grade": 2,
         "id": 10817,
         "include": "TLT?[1048]"
     },
     "10818": {
         "event": "\u4f60\u548c\u4e00\u4f4d\u76f8\u540c\u5883\u754c\u7684\u4eba\u7ed3\u4e3a\u9053\u4fa3\u3002",
         "exclude": "EVT?[10818]",
         "id": 10818,
@@ -6402,35 +6635,37 @@
         "id": 10819,
         "include": "(TLT?[1048])&(EVT?[10818])"
     },
     "10820": {
         "effect": {
             "STR": -100
         },
-        "event": "\u4f60\u8d70\u706b\u5165\u9b54\uff0c\u4f53\u8d28\u5927\u5e45\u964d\u4f4e\u3002",
+        "event": "\u4f60\u8d70\u706b\u5165\u9b54\uff0c\u4f53\u8d28\u6781\u5927\u5e45\u964d\u4f4e\u3002",
         "id": 10820,
         "include": "TLT?[1048]"
     },
     "10821": {
         "effect": {
             "STR": -10
         },
         "event": "\u4f60\u8d70\u706b\u5165\u9b54\uff0c\u4f53\u8d28\u5927\u5e45\u964d\u4f4e\u3002",
         "id": 10821,
         "include": "TLT?[1048]"
     },
     "10822": {
         "event": "\u4f60\u4e0a\u4e86\u4e00\u4e2a\u6602\u8d35\u7684\u53cc\u8bed\u5e7c\u513f\u56ed\u3002",
         "exclude": "EVT?[10822]",
+        "grade": 1,
         "id": 10822,
         "include": "TLT?[1010]"
     },
     "10823": {
         "event": "\u4f60\u4e0a\u4e86\u4e00\u4e2a\u6602\u8d35\u7684\u53cc\u8bed\u5e7c\u513f\u56ed\u3002",
         "exclude": "EVT?[10823]",
+        "grade": 1,
         "id": 10823,
         "include": "(MNY>7)&(EVT?[10010])"
     },
     "10824": {
         "event": "\u4f60\u4e0a\u4e86\u4e00\u4e2a\u666e\u901a\u7684\u5e7c\u513f\u56ed\u3002",
         "exclude": "(MNY<8)&(EVT?[10824])",
         "id": 10824,
@@ -6559,20 +6794,22 @@
         "exclude": "EVT?[10840]",
         "id": 10840,
         "include": "EVT?[10010]"
     },
     "10841": {
         "event": "\u65f6\u95f4\u8df3\u8dc3\u3002",
         "exclude": "EVT?[10842]",
+        "grade": 2,
         "id": 10841,
         "include": "TLT?[1114]"
     },
     "10842": {
         "event": "\u65f6\u7a7a\u9519\u4e71\uff0c\u4f60\u4e2d\u9014\u88ab\u629b\u51fa\u3002",
         "exclude": "EVT?[10842]",
+        "grade": 1,
         "id": 10842,
         "include": "TLT?[1114]"
     },
     "10843": {
         "event": "\u4f60\u7684\u4f53\u8d28\u6781\u5ea6\u865a\u5f31\u3002",
         "exclude": "EVT?[10843]",
         "id": 10843,
@@ -6622,14 +6859,15 @@
         "exclude": "EVT?[10856,10857,10849,10850]",
         "id": 10850,
         "include": "EVT?[10822,10823]"
     },
     "10851": {
         "event": "\u4f60\u505a\u4e86\u667a\u5546\u6d4b\u8bd5\uff0c\u667a\u5546\u9ad8\u8fbe150\u3002",
         "exclude": "EVT?[10851]",
+        "grade": 2,
         "id": 10851,
         "include": "(INT>8)&(((MNY>7)&(EVT?[10010]))|(TLT?[1010]))"
     },
     "10852": {
         "event": "\u4f60\u5f00\u59cb\u5b66\u4e60\u6e38\u6cf3\u3002",
         "exclude": "EVT?[10852]",
         "id": 10852,
@@ -6640,20 +6878,22 @@
         "exclude": "EVT?[10853,10868]",
         "id": 10853,
         "include": "EVT?[10822,10823]"
     },
     "10854": {
         "event": "\u7238\u5988\u5e26\u4f60\u53bb\u65e5\u672c\u65c5\u6e38\u3002",
         "exclude": "EVT?[10854,10868,10869,11476]",
+        "grade": 1,
         "id": 10854,
         "include": "EVT?[10822,10823]"
     },
     "10855": {
         "event": "\u7238\u5988\u5e26\u4f60\u53bb\u7f8e\u56fd\u65c5\u6e38\u3002",
         "exclude": "EVT?[10855,10868,10869]",
+        "grade": 1,
         "id": 10855,
         "include": "EVT?[10822,10823]"
     },
     "10856": {
         "event": "\u4f60\u7684\u8bc6\u5b57\u91cf\u8fbe\u5230\u4e86300\u3002",
         "exclude": "EVT?[10856,10857,10849,10850]",
         "id": 10856,
@@ -6757,50 +6997,57 @@
         "exclude": "EVT?[10870]",
         "id": 10870,
         "include": "EVT?[10824]"
     },
     "10871": {
         "event": "\u4f60\u4e0a\u4e86\u4e2a\u540d\u724c\u5c0f\u5b66\u3002",
         "exclude": "EVT?[10871]",
+        "grade": 1,
         "id": 10871,
         "include": "EVT?[10822,10823]"
     },
     "10872": {
         "event": "\u4f60\u83b7\u5f97\u4e86\u673a\u5668\u4eba\u5927\u8d5b\u91d1\u5956\u3002",
         "exclude": "EVT?[10872]",
+        "grade": 2,
         "id": 10872,
         "include": "(INT>8)&(EVT?[10853])"
     },
     "10873": {
         "event": "\u4f60\u83b7\u5f97\u4e86\u4e09\u597d\u5b66\u751f\u3002",
         "exclude": "EVT?[10873]",
+        "grade": 1,
         "id": 10873,
         "include": "(INT>5)&(EVT?[10824])"
     },
     "10874": {
         "event": "\u4f60\u83b7\u5f97\u4e86\u4e09\u597d\u6807\u5175\u3002",
         "exclude": "EVT?[10874]",
+        "grade": 1,
         "id": 10874,
         "include": "(INT>6)&(EVT?[10824])"
     },
     "10875": {
         "event": "\u4f60\u83b7\u5f97\u4e86\u5e02\u4e09\u597d\u5b66\u751f\u3002",
         "exclude": "EVT?[10875]",
+        "grade": 1,
         "id": 10875,
         "include": "(INT>7)&(EVT?[10822,10823])"
     },
     "10876": {
         "event": "\u4f60\u83b7\u5f97\u4e86\u533a\u4e09\u597d\u6807\u5175\u3002",
         "exclude": "EVT?[10876]",
+        "grade": 1,
         "id": 10876,
         "include": "(INT>7)&(EVT?[10822,10823])"
     },
     "10877": {
         "event": "\u4f60\u5f53\u4e0a\u4e86\u73ed\u957f\u3002",
         "exclude": "EVT?[10877]",
+        "grade": 1,
         "id": 10877,
         "include": "EVT?[10010]"
     },
     "10878": {
         "event": "\u4f60\u5e2e\u73ed\u91cc\u51fa\u4e86\u4e00\u671f\u9ed1\u677f\u62a5\u3002",
         "exclude": "EVT?[10878]",
         "id": 10878,
@@ -6906,38 +7153,43 @@
         "exclude": "EVT?[10892]",
         "id": 10892,
         "include": "EVT?[10871]"
     },
     "10893": {
         "event": "\u4f60\u8fbe\u5230\u4e86\u94a2\u743410\u7ea7\u3002",
         "exclude": "EVT?[10893]",
+        "grade": 1,
         "id": 10893,
         "include": "EVT?[10847]"
     },
     "10894": {
         "event": "\u4f60\u96c5\u601d\u62ff\u52307.5\u5206\u3002",
         "exclude": "EVT?[10894,10895]",
+        "grade": 1,
         "id": 10894,
         "include": "(INT>7)&(EVT?[10871])"
     },
     "10895": {
         "event": "\u4f60\u7684\u82f1\u8bed\u8bcd\u6c47\u91cf\u8fbe\u523010000\u3002",
         "exclude": "EVT?[10895,10894]",
+        "grade": 1,
         "id": 10895,
         "include": "(INT>7)&(EVT?[10871])"
     },
     "10896": {
         "event": "\u4f60\u53c2\u52a0\u7f8e\u56fd\u6570\u5b66\u7ade\u8d5b\u83b7\u5f97\u4e00\u7b49\u5956\u3002",
         "exclude": "EVT?[10896]",
+        "grade": 1,
         "id": 10896,
         "include": "(INT>7)&(EVT?[10871])"
     },
     "10897": {
         "event": "\u4f60\u4eec\u5b66\u6821\u7ec4\u7ec7\u524d\u5f80\u5357\u6781\u4fee\u5b66\u65c5\u884c\u3002",
         "exclude": "EVT?[10897]",
+        "grade": 1,
         "id": 10897,
         "include": "EVT?[10871]"
     },
     "10898": {
         "event": "\u4f60\u7684\u7f8e\u8c8c\u5341\u5206\u60ca\u8273\u3002",
         "exclude": "EVT?[10898]",
         "id": 10898,
@@ -6996,14 +7248,15 @@
     },
     "10905": {
         "effect": {
             "SPR": 1
         },
         "event": "\u5bb6\u4eba\u9001\u4f60\u53bb\u56fd\u5916\u8bfb\u4e86\u4e00\u5e74\u3002",
         "exclude": "EVT?[10905]",
+        "grade": 1,
         "id": 10905,
         "include": "EVT?[10871]"
     },
     "10906": {
         "event": "\u4f60\u5bb6\u5f00\u59cb\u517b\u732b\u3002",
         "exclude": "EVT?[10906]",
         "id": 10906,
@@ -7223,20 +7476,22 @@
         "exclude": "EVT?[10937]",
         "id": 10937,
         "include": "(INT>8)&(EVT?[10010])"
     },
     "10938": {
         "event": "\u4f60\u989c\u503c\u51fa\u4f17\uff0c\u51c6\u5907\u8d70\u5a31\u4e50\u8def\u7ebf\u3002",
         "exclude": "EVT?[10938]",
+        "grade": 1,
         "id": 10938,
         "include": "(EVT?[10898])"
     },
     "10939": {
         "event": "\u4f60\u88ab\u4f53\u6821\u6559\u7ec3\u6316\u8d70\u3002",
         "exclude": "EVT?[10939]",
+        "grade": 1,
         "id": 10939,
         "include": "EVT?[10880]"
     },
     "10940": {
         "event": "\u4f60\u5347\u5165\u666e\u901a\u521d\u4e2d\u3002",
         "exclude": "EVT?[10940]",
         "id": 10940,
@@ -7247,14 +7502,15 @@
         "exclude": "EVT?[10941]",
         "id": 10941,
         "include": "EVT?[10871]"
     },
     "10942": {
         "event": "\u4f60\u7684\u6e38\u620f\u6280\u672f\u8fc7\u4eba\uff0c\u5728\u5b66\u6821\u5c0f\u6709\u540d\u6c14\u3002",
         "exclude": "EVT?[10942]",
+        "grade": 1,
         "id": 10942,
         "include": "(TLT?[1039])&(EVT?[10940])"
     },
     "10943": {
         "event": "\u4f60\u4e2d\u8003\u6ca1\u6709\u8003\u597d\u3002",
         "exclude": "EVT?[10943]",
         "id": 10943,
@@ -7271,14 +7527,15 @@
         "exclude": "EVT?[10945,10939,10258]",
         "id": 10945,
         "include": "(INT<7)&(EVT?[10940])"
     },
     "10946": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u4eba\u5927\u9644\u4e2d\u3002",
         "exclude": "EVT?[10946,10939]",
+        "grade": 1,
         "id": 10946,
         "include": "(TLT?[1010])&(INT>6)"
     },
     "10947": {
         "event": "\u8bad\u7ec3\u3002",
         "id": 10947,
         "include": "EVT?[10939]"
@@ -7300,14 +7557,15 @@
         "exclude": "EVT?[10949]",
         "id": 10949,
         "include": "EVT?[10948]"
     },
     "10950": {
         "event": "\u52a0\u5165\u5e74\u8f7b\u827a\u4eba\u56e2\u4f53\u51fa\u9053\u3002",
         "exclude": "EVT?[10950]",
+        "grade": 1,
         "id": 10950,
         "include": "EVT?[10948]"
     },
     "10951": {
         "event": "\u9047\u51b7\uff0c\u5f7b\u5e95\u88ab\u8d44\u672c\u5bb6\u653e\u5f03\u3002\u4f60\u9000\u5708\u4e86\u3002",
         "exclude": "EVT?[10951]",
         "id": 10951,
@@ -7348,35 +7606,39 @@
         "exclude": "EVT?[10957]",
         "id": 10957,
         "include": "EVT?[10954,10955]"
     },
     "10958": {
         "event": "\u5bb6\u4eba\u6295\u94b1\u5e2e\u4f60\u9020\u52bf\u3002",
         "exclude": "EVT?[10958]",
+        "grade": 1,
         "id": 10958,
         "include": "(MNY>7)&(EVT?[10938])"
     },
     "10959": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53c2\u4e0e\u9009\u79c0\u8282\u76ee\uff0c\u4e00\u4e3e\u7206\u7ea2\u3002",
         "exclude": "EVT?[10959]",
+        "grade": 2,
         "id": 10959,
         "include": "EVT?[10958]"
     },
     "10960": {
         "event": "\u4f60\u6210\u4e3a\u6700\u70ed\u95e8\u7684\u5c11\u5e74\u5929\u56e2C\u4f4d\u3002",
         "exclude": "EVT?[10960,10002]",
+        "grade": 2,
         "id": 10960,
         "include": "EVT?[10959]"
     },
     "10961": {
         "event": "\u4f60\u6210\u4e3a\u6700\u70ed\u95e8\u7684\u5c11\u5973\u5929\u56e2C\u4f4d\u3002",
         "exclude": "EVT?[10961,10001]",
+        "grade": 2,
         "id": 10961,
         "include": "EVT?[10959]"
     },
     "10962": {
         "event": "\u6f14\u51fa\u3001\u53c2\u52a0\u7efc\u827a\u8282\u76ee\u3002",
         "exclude": "EVT?[10962]",
         "id": 10962,
@@ -7384,20 +7646,22 @@
     },
     "10963": {
         "effect": {
             "MNY": 1
         },
         "event": "\u51fa\u6f14\u7535\u5f71\u300a\u6211\u7684\u53bf\u957f\u7236\u4eb2\u300b\uff0c\u70ed\u5ea6\u5927\u6da8\u3002",
         "exclude": "EVT?[10963]",
+        "grade": 1,
         "id": 10963,
         "include": "EVT?[10960,10961]"
     },
     "10964": {
         "event": "\u51fa\u6f14\u7535\u89c6\u5267\u300a\u5e78\u798f\u519c\u5bb6\u4e50\u300b\uff0c\u5e7f\u53d7\u597d\u8bc4\u3002",
         "exclude": "EVT?[10964]",
+        "grade": 1,
         "id": 10964,
         "include": "EVT?[10960,10961]"
     },
     "10965": {
         "effect": {
             "MNY": 1
         },
@@ -7405,14 +7669,15 @@
         "exclude": "EVT?[10965]",
         "id": 10965,
         "include": "EVT?[10960,10961]"
     },
     "10966": {
         "event": "\u4f60\u88ab\u5317\u4eac\u7535\u5f71\u5b66\u9662\u5f55\u53d6\u3002",
         "exclude": "EVT?[10966]",
+        "grade": 1,
         "id": 10966,
         "include": "EVT?[10960,10961]"
     },
     "10967": {
         "event": "\u4f60\u4f11\u95f2\u65f6\u95f4\u559c\u6b22\u8ffd\u65b0\u756a\u3002",
         "exclude": "EVT?[10967]",
         "id": 10967,
@@ -7423,20 +7688,22 @@
         "exclude": "EVT?[10968]",
         "id": 10968,
         "include": "EVT?[10940]"
     },
     "10969": {
         "event": "\u4f60\u5165\u4e86cos\u5708\u3002",
         "exclude": "EVT?[10969]",
+        "grade": 1,
         "id": 10969,
         "include": "(EVT?[10940])&(EVT?[10008,10007])"
     },
     "10970": {
         "event": "\u4f60\u7ecf\u5e38\u5973\u88c5\u3002",
         "exclude": "EVT?[10970,10002,10110,10111]",
+        "grade": 1,
         "id": 10970,
         "include": "EVT?[10969]"
     },
     "10971": {
         "event": "\u4f60\u7b2c\u4e00\u6b21\u770b\u9ec4\u4e66\u3002",
         "exclude": "EVT?[10971,10972,10973]",
         "id": 10971,
@@ -7566,14 +7833,15 @@
     },
     "10989": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u4e70\u5c0f\u5356\u90e8\u7684\u996e\u6599\u4e2d\u4e86\u518d\u6765\u4e00\u74f6\uff0c\u4e2d\u7684\u6253\u5f00\u53c8\u4e2d\u4e86\u518d\u6765\u4e00\u74f6\u3002",
         "exclude": "EVT?[10989,10990]",
+        "grade": 1,
         "id": 10989,
         "include": "EVT?[10940]"
     },
     "10990": {
         "event": "\u4f60\u5728\u5b66\u6821\u5c0f\u5356\u90e8\u4e70\u8fc7\u5f88\u591a\u6b21\u996e\u6599\uff0c\u4ece\u6765\u6ca1\u4e2d\u8fc7\u5956\u3002",
         "exclude": "EVT?[10990,10989]",
         "id": 10990,
@@ -7941,20 +8209,22 @@
     },
     "11046": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u593a\u5f97\u4e86\u5965\u8d5b\u91d1\u724c\u3002",
         "exclude": "EVT?[11046]",
+        "grade": 2,
         "id": 11046,
         "include": "(EVT?[11045,21045])&(INT>9)"
     },
     "11047": {
         "event": "\u4f60\u7ecf\u5e38\u53c2\u52a0\u5404\u79cd\u590f\u4ee4\u8425\u3002",
         "exclude": "EVT?[11047]",
+        "grade": 1,
         "id": 11047,
         "include": "EVT?[10941]"
     },
     "11048": {
         "event": "\u5b66\u6821\u91c7\u53d6\u6309\u6210\u7ee9\u6392\u8003\u573a\uff0c\u73ed\u4e0a\u91c7\u53d6\u6309\u6210\u7ee9\u6392\u5ea7\u4f4d\u3002",
         "exclude": "EVT?[11048]",
         "id": 11048,
@@ -8047,14 +8317,15 @@
     },
     "11062": {
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u53c2\u52a0\u4e00\u4e2a\u56fd\u9645\u6bd4\u8d5b\u83b7\u5f97\u4e00\u7b49\u5956\uff0c\u4e0a\u4e86\u5e74\u5ea6\u5f00\u5b66\u5178\u793c\u7684\u8868\u5f70\u3002",
         "exclude": "EVT?[11062]",
+        "grade": 2,
         "id": 11062,
         "include": "(EVT?[10946])&(INT>9)"
     },
     "11063": {
         "event": "\u867d\u7136\u4f60\u6bd4\u540c\u9f84\u4eba\u5f3a\u5f88\u591a\uff0c\u4f46\u4f60\u5468\u56f4\u603b\u6709\u5404\u65b9\u9762\u6bd4\u4f60\u90fd\u5f3a\u7684\u5927\u4f6c\u3002",
         "exclude": "EVT?[11063]",
         "id": 11063,
@@ -8065,79 +8336,89 @@
         "exclude": "EVT?[11064]",
         "id": 11064,
         "include": "EVT?[10946]"
     },
     "11065": {
         "event": "\u5b66\u6821\u63d0\u4f9b\u4e86\u5f88\u591a\u548c\u56fd\u5916\u540d\u6821\u4ea4\u6d41\u7684\u673a\u4f1a\u3002",
         "exclude": "EVT?[11065]",
+        "grade": 1,
         "id": 11065,
         "include": "EVT?[10946]"
     },
     "11066": {
         "event": "\u8001\u5e08\u8bf4\uff1a\u201c\u5c11\u58ee\u4e0d\u52aa\u529b\uff0c\u957f\u5927\u53bb\u9694\u58c1\u3002\u201d",
         "exclude": "EVT?[11066]",
         "id": 11066,
         "include": "EVT?[10946]"
     },
     "11067": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u5c11\u5e74\u73ed\uff0c\u63d0\u524d\u6b65\u5165\u5927\u5b66\u3002",
         "exclude": "EVT?[11067]",
+        "grade": 2,
         "id": 11067,
         "include": "(EVT?[10010])&(INT>9)"
     },
     "11068": {
         "event": "\u52aa\u529b\u5b66\u4e60\u3002",
         "id": 11068,
         "include": "EVT?[11067]"
     },
     "11069": {
         "event": "\u4f60\u51fa\u56fd\u7559\u5b66\u3002",
         "exclude": "EVT?[11069]",
+        "grade": 2,
         "id": 11069,
         "include": "EVT?[11067]"
     },
     "11070": {
         "event": "\u4f60\u524d\u5f80\u54c8\u4f5b\u5927\u5b66\u7559\u5b66\u3002",
         "exclude": "EVT?[11070]",
+        "grade": 2,
         "id": 11070,
         "include": "(EVT?[11067])&(TLT?[1073])"
     },
     "11071": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u6e05\u534e\u5927\u5b66\u3002",
         "exclude": "(EVT?[11071])|(TLT?[1107])",
+        "grade": 2,
         "id": 11071,
         "include": "((EVT?[10944,10945])&(INT>9))|(EVT?[10946])"
     },
     "11072": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u5317\u4eac\u5927\u5b66\u3002",
         "exclude": "EVT?[11072]",
+        "grade": 2,
         "id": 11072,
         "include": "((EVT?[10944,10945])&(INT>9))|(EVT?[10946])"
     },
     "11073": {
         "event": "\u4f60\u88ab\u4fdd\u9001\u6e05\u534e\u5927\u5b66\u3002",
         "exclude": "(EVT?[11073])|(TLT?[1107])",
+        "grade": 2,
         "id": 11073,
         "include": "EVT?[11046,11062]"
     },
     "11074": {
         "event": "\u4f60\u88ab\u4fdd\u9001\u5317\u4eac\u5927\u5b66\u3002",
         "exclude": "EVT?[11074]",
+        "grade": 2,
         "id": 11074,
         "include": "EVT?[11046,11062]"
     },
     "11075": {
         "event": "\u4f60\u8003\u4e0a\u4e00\u6240985\u5927\u5b66\u3002",
         "exclude": "EVT?[11075]",
+        "grade": 1,
         "id": 11075,
         "include": "(EVT?[10944,10945])&((INT>7)|(MNY>8))"
     },
     "11076": {
         "event": "\u4f60\u8003\u4e0a\u4e00\u6240211\u5927\u5b66\u3002",
         "exclude": "EVT?[11076]",
+        "grade": 1,
         "id": 11076,
         "include": "(EVT?[10944,10945])&((INT>6)|(MNY>7))"
     },
     "11077": {
         "event": "\u4f60\u8003\u4e0a\u4e00\u6240\u53cc\u975e\u672c\u79d1\u3002",
         "exclude": "EVT?[11077]",
         "id": 11077,
@@ -8294,14 +8575,15 @@
         "exclude": "EVT?[11100,11101,11102]",
         "id": 11102,
         "include": "(INT>7)&(EVT?[11077,11075,11076,11071,11072,11073,11074])"
     },
     "11103": {
         "event": "\u4f60\u4fdd\u7814\u4e86\u3002",
         "exclude": "EVT?[11103]",
+        "grade": 1,
         "id": 11103,
         "include": "EVT?[11102]"
     },
     "11104": {
         "event": "\u4f60\u6ca1\u62a2\u5230\u60f3\u9009\u4fee\u7684\u8bfe\u3002",
         "exclude": "EVT?[11104]",
         "id": 11104,
@@ -8451,14 +8733,15 @@
         "id": 11126,
         "include": "EVT?[11125]",
         "postEvent": "\u4f60\u6210\u4e3a\u4e86\u6253\u5de5\u4eba\u3002"
     },
     "11127": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u516c\u52a1\u5458\u3002",
         "exclude": "EVT?[11127,11123]",
+        "grade": 1,
         "id": 11127,
         "include": "EVT?[11125]"
     },
     "11128": {
         "event": "\u4f60\u5f00\u59cb\u76f8\u4eb2\u3002",
         "exclude": "(EVT?[11128,11171])|(TLT?[1027])",
         "id": 11128,
@@ -8553,14 +8836,15 @@
         "exclude": "EVT?[11142]",
         "id": 11142,
         "include": "EVT?[11123,11126]"
     },
     "11143": {
         "event": "\u5e74\u4f1a\u4e0a\uff0c\u4f60\u62bd\u5956\u62bd\u5230\u4e00\u53f0iphoneZ\u3002",
         "exclude": "EVT?[11143,11144,11145]",
+        "grade": 1,
         "id": 11143,
         "include": "EVT?[11123,11126]"
     },
     "11144": {
         "event": "\u5e74\u4f1a\u4e0a\uff0c\u4f60\u62bd\u5230\u4e00\u5f20\u739b\u838e\u62c9\u84825\u5143\u4ee3\u91d1\u5238\u3002",
         "exclude": "EVT?[11143,11144,11145]",
         "id": 11144,
@@ -8743,38 +9027,43 @@
         "exclude": "EVT?[11173]",
         "id": 11173,
         "include": "EVT?[11124]"
     },
     "11174": {
         "event": "\u4f60\u5f00\u4e86\u4e00\u5bb6\u4e92\u8054\u7f51\u516c\u53f8\u3002",
         "exclude": "EVT?[11174,11175,11176,11177,11178]",
+        "grade": 1,
         "id": 11174,
         "include": "EVT?[11124]"
     },
     "11175": {
         "event": "\u4f60\u5f00\u4e86\u4e00\u5bb6\u91d1\u878d\u516c\u53f8\u3002",
         "exclude": "EVT?[11174,11175,11176,11177,11178]",
+        "grade": 1,
         "id": 11175,
         "include": "EVT?[11124]"
     },
     "11176": {
         "event": "\u4f60\u5f00\u4e86\u4e00\u5bb6\u4e8c\u6b21\u5143\u516c\u53f8\u3002",
         "exclude": "EVT?[11174,11175,11176,11177,11178]",
+        "grade": 1,
         "id": 11176,
         "include": "(EVT?[11124])&(EVT?[10007,10008])"
     },
     "11177": {
         "event": "\u4f60\u5f00\u4e86\u4e00\u5bb6\u5b9e\u4e1a\u516c\u53f8\u3002",
         "exclude": "EVT?[11174,11175,11176,11177,11178]",
+        "grade": 1,
         "id": 11177,
         "include": "EVT?[11124]"
     },
     "11178": {
         "event": "\u4f60\u5f00\u4e86\u4e00\u5bb6\u65b0\u6280\u672f\u4ea7\u4e1a\u516c\u53f8\u3002",
         "exclude": "EVT?[11174,11175,11176,11177,11178]",
+        "grade": 1,
         "id": 11178,
         "include": "EVT?[11124]"
     },
     "11179": {
         "event": "\u4f60\u521b\u4e1a\u8fc7\u7a0b\u4e2d\u7ed3\u8bc6\u4e86\u8bb8\u591a\u5927\u4f6c\u3002",
         "exclude": "EVT?[11179]",
         "id": 11179,
@@ -8878,40 +9167,42 @@
     "11196": {
         "event": "\u4e2d\u56fd\u6210\u529f\u767b\u6708\u3002",
         "exclude": "EVT?[11196]",
         "id": 11196,
         "include": "EVT?[11127,11123,11126,11122,11124]"
     },
     "11197": {
-        "event": "\u6211\u56fd\u9996\u6b21\u593a\u5f97\u5965\u8fd0\u5956\u724c\u699c\u5956\u724c\u603b\u6570\u7b2c\u4e00\u3002",
+        "event": "\u5fae\u79ef\u5206\u6b63\u5f0f\u8fdb\u5165\u5c0f\u5b66\u6570\u5b66\u6559\u6750\u3002",
         "exclude": "EVT?[11197]",
         "id": 11197,
         "include": "EVT?[11127,11123,11126,11122,11124]"
     },
     "11198": {
-        "event": "\u4e3a\u51cf\u8f7b\u751f\u80b2\u8d1f\u62c5\uff0c\u56fd\u5bb6\u51fa\u53f0\u591a\u9879\u653f\u7b56\u3002",
+        "event": "\u4e13\u5bb6\u5efa\u8bae\u5c06\u4e2a\u7a0e\u8d77\u5f81\u70b9\u964d\u52300\u3002",
         "exclude": "EVT?[11198]",
         "id": 11198,
         "include": "EVT?[11127,11123,11126,11122,11124]"
     },
     "11199": {
         "event": "\u6211\u56fd\u5ba3\u5e03\u5efa\u6210\u793e\u4f1a\u4e3b\u4e49\u73b0\u4ee3\u5316\u5f3a\u56fd\u3002",
         "exclude": "EVT?[11199]",
+        "grade": 1,
         "id": 11199,
         "include": "EVT?[11127,11123,11126,11122,11124]"
     },
     "11200": {
-        "event": "\u6211\u56fd\u4eba\u5747GDP\u8d85\u8fc7\u97e9\u56fd\u3002",
+        "event": "\u5370\u5ea6\u5927\u91cf\u5927\u9f84\u7537\u5b50\u627e\u4e0d\u5230\u5bf9\u8c61\uff0c\u72af\u7f6a\u7387\u66b4\u589e\u3002",
         "exclude": "EVT?[11200]",
         "id": 11200,
         "include": "EVT?[11127,11123,11126,11122,11124]"
     },
     "11201": {
         "event": "\u4f60\u7684\u4e13\u8f91\u300a\u6697\u7ebf\u300b\u767b\u9876\u3002",
         "exclude": "EVT?[11201]",
+        "grade": 2,
         "id": 11201,
         "include": "EVT?[10966]"
     },
     "11202": {
         "event": "\u4f60\u6ca1\u6709\u65f6\u95f4\u4e0a\u8bfe\uff0c\u65f6\u95f4\u8868\u5b89\u6392\u5f97\u5f88\u6ee1\u3002",
         "exclude": "EVT?[11202]",
         "id": 11202,
@@ -9042,20 +9333,22 @@
         "exclude": "(EVT?[11220])|(TLT?[1044])",
         "id": 11220,
         "include": "(STR<2)&(EVT?[10010])"
     },
     "11221": {
         "event": "\u4f60\u4f4d\u5217\u5e74\u5ea6\u827a\u4eba\u6392\u884c\u7b2c3\u3002",
         "exclude": "EVT?[11221]",
+        "grade": 2,
         "id": 11221,
         "include": "EVT?[10966]"
     },
     "11222": {
         "event": "\u4f60\u540d\u5217\u5e74\u5ea6\u798f\u5e03\u65af\u5341\u5927\u4e2d\u56fd\u540d\u4eba\u3002",
         "exclude": "EVT?[11222]",
+        "grade": 2,
         "id": 11222,
         "include": "EVT?[10966]"
     },
     "11223": {
         "event": "\u6709\u8ba8\u538c\u7684\u79c1\u751f\u996d\u5f71\u54cd\u4f60\u7684\u751f\u6d3b\u3002",
         "exclude": "EVT?[11223]",
         "id": 11223,
@@ -9075,20 +9368,22 @@
         "exclude": "EVT?[11225]",
         "id": 11225,
         "include": "EVT?[10966]"
     },
     "11226": {
         "event": "\u4f60\u4e70\u4e86\u51e0\u8f86\u6570\u767e\u4e07\u3001\u4e0a\u5343\u4e07\u7684\u8c6a\u8f66\u3002",
         "exclude": "EVT?[11226]",
+        "grade": 1,
         "id": 11226,
         "include": "EVT?[10966]"
     },
     "11227": {
         "event": "\u4f60\u4e70\u4e86\u4e00\u680b\u5927\u522b\u5885\uff0c\u4e00\u5957\u6c64\u81e3\u4e00\u54c1\u3002",
         "exclude": "EVT?[11227]",
+        "grade": 1,
         "id": 11227,
         "include": "EVT?[10966]"
     },
     "11228": {
         "event": "\u56fd\u5bb6\u5f00\u59cb\u6253\u51fb\u5a31\u4e50\u5708\u3002",
         "exclude": "EVT?[11228]",
         "id": 11228,
@@ -9300,20 +9595,22 @@
         "exclude": "EVT?[11258,11218,10869]",
         "id": 11258,
         "include": "EVT?[10010]"
     },
     "11259": {
         "event": "\u4f60\u5f53\u4e0a\u4e86\u526f\u6559\u6388\u3002",
         "exclude": "EVT?[11259]",
+        "grade": 1,
         "id": 11259,
         "include": "EVT?[11162,11163]"
     },
     "11260": {
         "event": "\u4f60\u5f53\u4e0a\u4e86\u6b63\u6559\u6388\u3002",
         "exclude": "EVT?[11260]",
+        "grade": 1,
         "id": 11260,
         "include": "EVT?[11259]"
     },
     "11261": {
         "effect": {
             "SPR": -1
         },
@@ -9326,44 +9623,50 @@
         "branch": [
             "SPR<3:10062"
         ],
         "effect": {
             "SPR": -1
         },
         "event": "\u4f60\u5e38\u5e38\u56e0\u4e3a\u6027\u522b\u800c\u906d\u53d7\u66b4\u529b\u548c\u51b7\u66b4\u529b\u3002",
+        "exclude": "EVT?[11262,10062]",
         "id": 11262,
         "include": "(EVT?[10110,10111])&(EVT?[10009,10010])"
     },
     "11263": {
         "event": "\u53ef\u63a7\u6838\u805a\u53d8\u6280\u672f\u5b9e\u73b0\u3002\u5168\u7403\u8fc5\u901f\u5411\u65e0\u9650\u80fd\u6e90\u65f6\u4ee3\u8f6c\u53d8\u3002",
         "exclude": "EVT?[11263]",
+        "grade": 2,
         "id": 11263,
         "include": "EVT?[10010]"
     },
     "11264": {
         "event": "\u822a\u5929\u6280\u672f\u53d6\u5f97\u5de8\u5927\u7a81\u7834\u3002",
         "exclude": "EVT?[11264]",
+        "grade": 2,
         "id": 11264,
         "include": "EVT?[10010]"
     },
     "11265": {
         "event": "\u4f60\u524d\u5f80\u592a\u7a7a\u65c5\u884c\u3002",
         "exclude": "EVT?[11265]",
+        "grade": 2,
         "id": 11265,
         "include": "(STR>6)&(MNY>8)&(EVT?[11264,11263])"
     },
     "11266": {
         "event": "\u4f60\u524d\u5f80\u6708\u7403\u65c5\u884c\u3002",
         "exclude": "EVT?[11266]",
+        "grade": 2,
         "id": 11266,
         "include": "EVT?[11266]"
     },
     "11267": {
         "event": "\u4f60\u524d\u5f80\u706b\u661f\u65c5\u884c\u3002",
         "exclude": "EVT?[11267]",
+        "grade": 2,
         "id": 11267,
         "include": "EVT?[11267]"
     },
     "11268": {
         "branch": [
             "TLT?[1135]:40062",
             "EVT?[10010]:10000"
@@ -9372,48 +9675,53 @@
         "exclude": "EVT?[11268]",
         "id": 11268,
         "include": "EVT?[11264]"
     },
     "11269": {
         "event": "\u751f\u4ea7\u8d44\u6599\u6240\u6709\u5236\u6b63\u5728\u6df1\u523b\u6539\u53d8\uff0c\u8bb8\u591a\u56fd\u5bb6\u5411\u793e\u4f1a\u4e3b\u4e49\u56fd\u5bb6\u8fc7\u6e21\u3002",
         "exclude": "EVT?[11269]",
+        "grade": 1,
         "id": 11269,
         "include": "EVT?[11263]"
     },
     "11270": {
         "event": "\u4e13\u5bb6\u58f0\u79f0\u71c3\u6599\u662f\u8d44\u672c\u4e3b\u4e49\u793e\u4f1a\u7684\u57fa\u7840\uff0c\u53ef\u63a7\u6838\u805a\u53d8\u662f\u5171\u4ea7\u4e3b\u4e49\u793e\u4f1a\u7684\u57fa\u7840\u3002",
         "exclude": "EVT?[11270]",
         "id": 11270,
         "include": "EVT?[11263]"
     },
     "11271": {
         "event": "\u5404\u4e2a\u4ea7\u4e1a\u90fd\u53d6\u5f97\u4e86\u5de8\u5927\u7684\u7a81\u7834\uff0c\u4e00\u5e74\u7684\u8fdb\u6b65\u9876\u8fc7\u53bb10\u5e74\u3002",
         "exclude": "EVT?[11271]",
+        "grade": 1,
         "id": 11271,
         "include": "EVT?[11263]"
     },
     "11272": {
         "event": "\u7535\u529b\u5f7b\u5e95\u514d\u8d39\u3002",
         "exclude": "EVT?[11272]",
+        "grade": 2,
         "id": 11272,
         "include": "EVT?[11263]",
         "postEvent": "\u6240\u6709\u71c3\u6cb9\u71c3\u6c14\u90fd\u88ab\u7535\u529b\u53d6\u4ee3\u3002"
     },
     "11273": {
         "event": "\u4f60\u7684\u516c\u53f8\u5236\u9020\u51fa\u53ef\u690d\u5165\u5927\u8111\u7684\u82af\u7247\u3002\u53ef\u4ee5\u663e\u8457\u63d0\u5347\u4eba\u7c7b\u8bb0\u5fc6\u529b\u3002",
         "exclude": "EVT?[11273]",
+        "grade": 1,
         "id": 11273,
         "include": "(EVT?[11124])&(EVT?[11263])"
     },
     "11274": {
         "effect": {
             "INT": 2
         },
         "event": "\u4f60\u7814\u53d1\u51fa\u53ef\u690d\u5165\u5927\u8111\u7684\u82af\u7247\u3002\u53ef\u4ee5\u76f4\u63a5\u5c06\u77e5\u8bc6\u4fe1\u606f\u690d\u5165\u5927\u8111\u3002",
         "exclude": "EVT?[11274]",
+        "grade": 2,
         "id": 11274,
         "include": "(EVT?[11162,11163])&(EVT?[11263])",
         "postEvent": "\u4f60\u5f80\u81ea\u5df1\u5927\u8111\u690d\u5165\u4e86\uff0c\u667a\u529b\u663e\u8457\u63d0\u5347\u3002"
     },
     "11275": {
         "effect": {
             "MNY": 1
@@ -9451,38 +9759,41 @@
         "exclude": "EVT?[11278,11318]",
         "id": 11278,
         "include": "(INT<2)&(EVT?[10010])"
     },
     "11279": {
         "event": "\u4f60\u5347\u5b98\u4e86\u3002",
         "exclude": "EVT?[11279]",
+        "grade": 1,
         "id": 11279,
         "include": "EVT?[11127]"
     },
     "11280": {
         "event": "\u4f60\u7ecf\u5e38\u5728\u7f51\u4e0a\u6652\u751f\u6d3b\u3002",
         "exclude": "EVT?[11280]",
         "id": 11280,
         "include": "(MNY>4)&(EVT?[10010])"
     },
     "11281": {
         "event": "Web3.0\u65f6\u4ee3\u5b8c\u5168\u5230\u6765\u3002",
         "exclude": "EVT?[11281]",
+        "grade": 1,
         "id": 11281,
         "include": "EVT?[10010]"
     },
     "11282": {
         "event": "6G\u4fe1\u53f7\u8986\u76d6\u5168\u7403\u5927\u591a\u6570\u5730\u533a\u3002",
         "exclude": "EVT?[11282]",
         "id": 11282,
         "include": "EVT?[10010]"
     },
     "11283": {
         "event": "\u624b\u673a\u6d88\u4ea1\u4e86\uff0c\u53d6\u800c\u4ee3\u4e4b\u7684\u662f\u5168\u606f\u6295\u5f71\u3002",
         "exclude": "EVT?[11283]",
+        "grade": 1,
         "id": 11283,
         "include": "EVT?[10010]"
     },
     "11284": {
         "event": "\u636e\u8bf4\u4f20\u9001\u88c5\u7f6e\u6b63\u5728\u7814\u5236\u4e2d\u3002",
         "exclude": "EVT?[11284]",
         "id": 11284,
@@ -9499,54 +9810,59 @@
         "event": "\u4f60\u7684\u751f\u6d3b\u65e5\u65b0\u6708\u5f02\uff0c\u611f\u89c9\u65f6\u4ee3\u98de\u901f\u524d\u8fdb\u7740\u3002",
         "id": 11286,
         "include": "EVT?[11263,11281,11282,11283,11285]"
     },
     "11287": {
         "event": "\u865a\u62df\u73b0\u5b9e\u6280\u672f\u53d6\u5f97\u5de8\u5927\u7a81\u7834\u3002",
         "exclude": "EVT?[11287]",
+        "grade": 2,
         "id": 11287,
         "include": "EVT?[11272,11184]"
     },
     "11288": {
         "event": "\u7b2c\u4e00\u4e2a\u53ef\u771f\u5b9e\u8fdb\u5165\u7684\u865a\u62df\u4e16\u754c\u51fa\u73b0\u4e86\u3002",
         "exclude": "EVT?[11288]",
+        "grade": 2,
         "id": 11288,
         "include": "EVT?[11287]",
         "postEvent": "\u5168\u4eba\u7c7b\u75af\u72c2\u4e86\u3002"
     },
     "11289": {
         "event": "\u4f60\u7ec8\u65e5\u6c89\u8ff7\u5728\u865a\u62df\u4e16\u754c\u4e4b\u4e2d\u3002",
         "exclude": "EVT?[11289]",
+        "grade": 1,
         "id": 11289,
         "include": "(MNY<9)&(EVT?[11288])",
         "postEvent": "\u865a\u62df\u4e16\u754c\u4e2d\u7684\u65f6\u95f4\u8fc7\u5f97\u6bd4\u73b0\u5b9e\u6162\u3002"
     },
     "11290": {
         "effect": {
             "CHR": -1,
             "INT": -1,
             "SPR": 1,
             "STR": -1
         },
         "event": "\u4f60\u4f9d\u9760\u751f\u547d\u7ef4\u6301\u88c5\u7f6e\u6d3b\u7740\u3002\u6240\u6709\u65f6\u95f4\u90fd\u5728\u865a\u62df\u4e2d\u5ea6\u8fc7\u3002",
         "exclude": "EVT?[11290]",
+        "grade": 1,
         "id": 11290,
         "include": "EVT?[11289]",
         "postEvent": "\u4e0d\u8fc7\u4e16\u754c\u4e0a\u5927\u591a\u6570\u666e\u901a\u4eba\u90fd\u548c\u4f60\u4e00\u6837\u3002"
     },
     "11291": {
         "branch": [
             "(STR<0)&(INT<0):10000"
         ],
         "effect": {
             "INT": -1,
             "SPR": 1,
             "STR": -1
         },
         "event": "\u5916\u754c\u4e00\u5e74\uff0c\u865a\u62df\u4e16\u754c\u4e2d\u5341\u5e74\u3002",
+        "grade": 1,
         "id": 11291,
         "include": "EVT?[11290]",
         "postEvent": "\u73b0\u5b9e\u4e2d\u7684\u4f60\u8d8a\u6765\u8d8a\u865a\u5f31\uff0c\u865a\u62df\u4e2d\u7684\u4f60\u8d8a\u6765\u8d8a\u5feb\u4e50\u3002"
     },
     "11292": {
         "event": "\u4f60\u5f00\u59cb\u6295\u8d44\u641e\u865a\u62df\u73b0\u5b9e\u3002",
         "exclude": "EVT?[11292]",
@@ -9574,20 +9890,22 @@
     },
     "11296": {
         "branch": [
             "INT>10:21296"
         ],
         "event": "\u9ad8\u8d85\u7684\u6d1e\u5bdf\u529b\u4f7f\u4f60\u53d1\u73b0\uff1a\u73b0\u5b9e\u4e16\u754c\u662f\u865a\u62df\u7684\u3002",
         "exclude": "EVT?[11296]",
+        "grade": 3,
         "id": 11296,
-        "include": "(INT>10)&(EVT?[11288])"
+        "include": "((INT>10)&(EVT?[11288]))|(TLT?[2022])"
     },
     "11297": {
         "event": "\u6211\u56fd\u8fdb\u5165\u5171\u4ea7\u4e3b\u4e49\u793e\u4f1a\u3002",
         "exclude": "EVT?[11297,11287,10448]",
+        "grade": 2,
         "id": 11297,
         "include": "EVT?[11263]"
     },
     "11298": {
         "event": "\u7b2c\u4e09\u6b21\u4e16\u754c\u5927\u6218\u7206\u53d1\u3002",
         "exclude": "EVT?[11298]",
         "id": 11298,
@@ -9601,45 +9919,50 @@
         "exclude": "EVT?[11299]",
         "id": 11299,
         "include": "(EVT?[11263])&(EVT?[11298])"
     },
     "11300": {
         "event": "\u63a2\u7d22\u98de\u8239\u53d1\u73b0\u4e86\u6709\u4f4e\u7b49\u751f\u547d\u7684\u5730\u5916\u884c\u661f\u3002",
         "exclude": "EVT?[11300]",
+        "grade": 1,
         "id": 11300,
         "include": "EVT?[11264]"
     },
     "11301": {
         "event": "\u4eba\u7c7b\u6d3e\u9063\u8239\u961f\u53bb\u5730\u5916\u884c\u661f\u8fdb\u884c\u6539\u9020\u5de5\u4f5c\uff0c\u4fbf\u4e8e\u672a\u6765\u6b96\u6c11\u3002",
         "exclude": "EVT?[11301]",
+        "grade": 1,
         "id": 11301,
         "include": "EVT?[11300]"
     },
     "11302": {
         "event": "\u79d1\u5b66\u5bb6\u58f0\u79f0\u5916\u661f\u4e0a\u53ef\u80fd\u6709\u672a\u77e5\u7684\u81f4\u547d\u7ec6\u83cc\u6216\u75c5\u6bd2\uff0c\u53bb\u4e86\u5c31\u4e0d\u53ef\u8d38\u7136\u8fd4\u56de\u3002",
         "exclude": "EVT?[11302]",
         "id": 11302,
         "include": "EVT?[11300]"
     },
     "11303": {
         "event": "\u4eba\u7c7b\u53c8\u53d1\u73b0\u53e6\u5916\u4e09\u4e2a\u6709\u751f\u547d\u7684\u5730\u5916\u884c\u661f\u3002",
         "exclude": "EVT?[11303]",
+        "grade": 1,
         "id": 11303,
         "include": "EVT?[11300]"
     },
     "11304": {
         "event": "\u6709\u5916\u661f\u4eba\u4e58\u98de\u8239\u6765\u5230\u5730\u7403\u60f3\u8981\u5360\u9886\u5730\u7403\uff0c\u5374\u4e0d\u77e5\u88ab\u8c01\u77ac\u95f4\u6d88\u706d\u3002",
         "exclude": "EVT?[11304]",
+        "grade": 1,
         "id": 11304,
         "include": "EVT?[11300]",
         "postEvent": "\u6709\u4f20\u95fb\u79f0\u5730\u7403\u4e0a\u65e9\u5c31\u6709\u66f4\u5f3a\u5927\u7684\u5916\u661f\u4eba\u5728\u4e86\u3002"
     },
     "11305": {
         "event": "\u764c\u75c7\u88ab\u653b\u514b\u4e86\u3002",
         "exclude": "EVT?[11305]",
+        "grade": 1,
         "id": 11305,
         "include": "EVT?[10010]"
     },
     "11306": {
         "branch": [
             "EVT?[10010]:10000"
         ],
@@ -9692,14 +10015,15 @@
         "event": "\u4f60\u7684\u5b69\u5b50\u53bb\u4e16\u3002",
         "exclude": "EVT?[11311]",
         "id": 11311,
         "include": "EVT?[11240]"
     },
     "11312": {
         "branch": [
+            "TLT?[1135]:40062",
             "EVT?[10010]:10000"
         ],
         "event": "\u4f60\u88ab\u4eba\u8c0b\u6740\u4e86\u3002",
         "exclude": "EVT?[11312]",
         "id": 11312,
         "include": "EVT?[11124]"
     },
@@ -9771,14 +10095,15 @@
         "event": "\u4f60\u83b7\u5f97\u4e86\u51cf\u5211\uff0c\u63d0\u524d\u51fa\u72f1\u3002",
         "exclude": "EVT?[11321,11322]",
         "id": 11322,
         "include": "(EVT?[11320])&(TLT?[1117])"
     },
     "11323": {
         "branch": [
+            "TLT?[1135]:40062",
             "EVT?[10010]:10000"
         ],
         "event": "\u4f60\u5728\u72f1\u4e2d\u88ab\u4eba\u6253\u6b7b\u3002",
         "exclude": "EVT?[11321,11322]",
         "id": 11323,
         "include": "(STR<6)&(EVT?[11320])"
     },
@@ -9793,14 +10118,15 @@
     },
     "11325": {
         "branch": [
             "(MNY<8)&(SPR<8):21315"
         ],
         "event": "\u6709\u4e00\u4e2a\u6309\u94ae\uff0c\u6309\u4e0b\u53bb\u540e\u4f60\u80fd\u5f97\u5230\u5927\u91cf\u91d1\u94b1\uff0c\u4f46\u4eba\u7c7b\u57281000\u5e74\u5185\u4f1a\u706d\u4ea1\u3002",
         "exclude": "EVT?[11325]",
+        "grade": 2,
         "id": 11325,
         "include": "EVT?[10010]",
         "postEvent": "\u4f60\u6ca1\u6309\u3002"
     },
     "11326": {
         "event": "\u79d1\u5b66\u5bb6\u53d1\u73b0\uff0c\u6709\u4e00\u9897\u76f4\u5f8420\u5343\u7c73\u7684\u5c0f\u884c\u661f\u53ef\u80fd\u5728990\u5e74\u540e\u63a5\u8fd1\u5730\u7403\u3002",
         "exclude": "EVT?[11326]",
@@ -9813,186 +10139,208 @@
         "exclude": "EVT?[11327]",
         "id": 11327,
         "include": "EVT?[21315]"
     },
     "11328": {
         "event": "\u51fa\u73b0\u4e86\u53ef\u4ee5\u5728\u865a\u62df\u4e16\u754c\u4e2d\u521b\u9020\u865a\u62df\u4e16\u754c\u7684\u865a\u62df\u6e38\u620f\u3002",
         "exclude": "EVT?[11328]",
+        "grade": 1,
         "id": 11328,
         "include": "EVT?[11287]"
     },
     "11329": {
         "event": "\u4f60\u4e00\u5929\u6709\u534a\u6570\u65f6\u95f4\u6ce1\u5728\u865a\u62df\u4e16\u754c\u4e2d\u3002",
         "exclude": "EVT?[11293]",
+        "grade": 1,
         "id": 11329,
         "include": "EVT?[11287]"
     },
     "11330": {
         "event": "\u4ea4\u901a\u5f7b\u5e95\u514d\u8d39\u4e86\u3002",
         "exclude": "EVT?[11330]",
+        "grade": 1,
         "id": 11330,
         "include": "EVT?[11263]"
     },
     "11331": {
         "event": "\u4f60\u53bb\u4e16\u754c\u5404\u5730\u65c5\u6e38\u3002",
         "exclude": "EVT?[11332,11333,11334]",
+        "grade": 1,
         "id": 11331,
         "include": "EVT?[11330]"
     },
     "11332": {
         "event": "\u4f60\u5b9a\u5c45\u7a7a\u95f4\u7ad9\u3002",
         "exclude": "EVT?[11332,11333,11334]",
+        "grade": 2,
         "id": 11332,
         "include": "EVT?[11265]"
     },
     "11333": {
         "event": "\u4f60\u5b9a\u5c45\u6708\u7403\u3002",
         "exclude": "EVT?[11332,11333,11334]",
+        "grade": 2,
         "id": 11333,
         "include": "EVT?[11266]"
     },
     "11334": {
         "event": "\u4f60\u5b9a\u5c45\u706b\u661f\u3002",
         "exclude": "EVT?[11332,11333,11334]",
+        "grade": 2,
         "id": 11334,
         "include": "EVT?[11267]"
     },
     "11335": {
         "effect": {
             "INT": -1,
             "STR": 1
         },
         "event": "\u2593#\u2593\u2026\u2026*\u2593\u2593\u2593\u2299\u2593&\u2593\u2593\u2593\u2593\uffe5\uff08\u2593\u2593\u2593*-+\u2593\u2593",
+        "grade": 2,
         "id": 11335,
         "include": "TLT?[1128]"
     },
     "11336": {
         "effect": {
             "INT": -1,
             "MNY": 1
         },
         "event": "\u2593\u2593\u2593\u2593\u2593\u2593\u2593&\u2026\u2026\u2593\u2196\u2593\u2593\u2593\u2593\u2593&*\uffe5\u2593\u221e\u2593\u2593\u2593\u2593",
+        "grade": 2,
         "id": 11336,
         "include": "TLT?[1128]"
     },
     "11337": {
         "effect": {
             "INT": -1,
             "SPR": 1
         },
         "event": "\u2593\u2593\u2593\u2593*\u2593*\u2593\u2593&\u2593^\u2593^\u2593\u2593\u2593\u2593\u2299\u2593\u2593\u2593\u2593\u2593&",
+        "grade": 2,
         "id": 11337,
         "include": "TLT?[1128]"
     },
     "11338": {
         "effect": {
             "CHR": 1,
             "INT": -1
         },
         "event": "\uffe5%\u2593\u2593\u2593\u221e\u2593\u2593\u2593\u2593\u2593\u2593\u2593\uff08\uff08**",
+        "grade": 2,
         "id": 11338,
         "include": "TLT?[1128]"
     },
     "11339": {
         "effect": {
             "CHR": 2,
             "INT": -1
         },
         "event": "\u2593\uffe5@\u221e\u2593\u2593\u2593\u2593\u2571\u2572\u2593\u2196\u2593\u2593\u2593\u2593\u2593\u2593@@\u2593\u2593\u2593\u2593",
+        "grade": 2,
         "id": 11339,
         "include": "TLT?[1128]"
     },
     "11340": {
         "effect": {
             "INT": -1,
             "STR": 2
         },
         "event": "\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2026\u2026&*%+-*",
+        "grade": 2,
         "id": 11340,
         "include": "TLT?[1128]"
     },
     "11341": {
         "effect": {
             "INT": -1,
             "MNY": 2
         },
-        "event": "\u2593\u300b\u300a\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u300b\u300b\u2593",
+        "event": "\u2593 \u2593 \u2593 \u2593 \u2593 \u2593\r\n\u2593 \u2593 \u2593 \u2593 \u2593 \uff0c\r\n\u2593 \u2593 \u2593 \u2593 \uff0c\r\n\u2593 \u2593 \u2593 \u2593 \u2593 \u2593 \u2593\r\n\u2593 \u2593 ",
+        "grade": 2,
         "id": 11341,
         "include": "TLT?[1128]"
     },
     "11342": {
         "effect": {
             "INT": -1,
             "SPR": 2
         },
         "event": "\u2593\u2593\u2593\u201c{}|\u2593\u2593\u2593\u2593\u2593\u2593\u2014\u2593\u2593\u2593\u2593&",
+        "grade": 2,
         "id": 11342,
         "include": "TLT?[1128]"
     },
     "11343": {
         "effect": {
             "INT": -1,
             "STR": 3
         },
         "event": "\uff1a\u2593\u2593\u2593\uff1a\u221e\u2593\u2593\u2593\u2593\u2593\u2593\u2026\u2026\u2571\u2572\u2593\u2593\u2593\u2593\u300b",
+        "grade": 2,
         "id": 11343,
         "include": "TLT?[1128]"
     },
     "11344": {
         "effect": {
             "CHR": 3,
             "INT": -1
         },
         "event": "\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\uff01~\u2593\uff01\u2593+\u2593=\u2593\u2018",
+        "grade": 2,
         "id": 11344,
         "include": "TLT?[1128]"
     },
     "11345": {
         "effect": {
             "INT": -1,
             "MNY": 3
         },
         "event": "\uff1b\u2019\u2593\u2571\u2572\uff0c\u2593\u0419*-\u2593\u2593\u2593",
+        "grade": 2,
         "id": 11345,
         "include": "TLT?[1128]"
     },
     "11346": {
         "effect": {
             "INT": -1,
             "SPR": 3
         },
         "event": "\uff1b\u3010\u2593\u3011\u2581\u2582\u2583\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u2593\u3001\u3001\u2593\u2593\u2593\u2593\u2593\uff1f",
+        "grade": 2,
         "id": 11346,
         "include": "TLT?[1128]"
     },
     "11347": {
         "branch": [
             "TLT?[1128]:10000"
         ],
         "effect": {
             "INT": -1
         },
         "event": "\u2581\u2582\u2583\u2584\u2585\u2586\u2587\u2588\u2587\u2586\u2585\u2584\u2583\u2582\u2581",
+        "grade": 2,
         "id": 11347,
         "include": "TLT?[1128]"
     },
     "11348": {
         "branch": [
             "TLT?[1128]:10000"
         ],
         "effect": {
             "INT": -1
         },
         "event": "\u2605\u2606\u2191\u25ce\u00a4\u2605\u2606\u25ce\u2191\u00a4\u2605\u2606\u25ce\u00a4\u25ce\u2191\u00a4\u2605\u2606\u2191",
+        "grade": 2,
         "id": 11348,
         "include": "TLT?[1128]"
     },
     "11349": {
         "event": "\u4f60\u6ca1\u6709\u8fd9\u6bb5\u8bb0\u5fc6\u3002",
         "exclude": "EVT?[20349]",
+        "grade": 1,
         "id": 11349,
         "include": "TLT?[1129]"
     },
     "11350": {
         "event": "\u5a5a\u540e\u4f60\u7684\u4e08\u592b\u6ca1\u6709\u4e4b\u524d\u5bf9\u4f60\u90a3\u4e48\u597d\u4e86\u3002",
         "exclude": "EVT?[10001,11294,11350,11357,11358,11359,11360,11361,11362,11363,11295]|((EVT?[10002])&(TLT?[1026]))",
         "id": 11350,
@@ -10324,14 +10672,15 @@
     },
     "11401": {
         "effect": {
             "MNY": 1
         },
         "event": "\u4f60\u4e70\u5f69\u7968\u4e2d\u4e86\u5956\u3002\u5bb6\u5883\u56de\u6696\u3002",
         "exclude": "EVT?[11401]",
+        "grade": 1,
         "id": 11401,
         "include": "(MNY<3)&(EVT?[10010])"
     },
     "11402": {
         "event": "\u56e0\u4e3a\u5f88\u6709\u94b1\uff0c\u603b\u662f\u6709\u4eba\u548c\u4f60\u5bb6\u6500\u4eb2\u621a\u3002",
         "exclude": "EVT?[11402]",
         "id": 11402,
@@ -10400,15 +10749,15 @@
     "11413": {
         "event": "\u56e0\u4e3a\u76f8\u8c8c\u4e0d\u4f73\uff0c\u751f\u6d3b\u4e2d\u5e73\u6dfb\u4e86\u4e0d\u5c11\u9ebb\u70e6\u3002",
         "exclude": "EVT?[11413]",
         "id": 11413,
         "include": "(CHR<4)&(EVT?[10010])"
     },
     "11414": {
-        "event": "\u751f\u7269\u5b66\u5bb6\u7a81\u7834\u6027\u5b8c\u6210\u4e86\u732b\u72d7\u6742\u4ea4\u5b9e\u9a8c\u3002",
+        "event": "\u4eca\u5e74\u8003\u7814\u4eba\u6570\u7a81\u78341\u5343\u4e07\u3002",
         "exclude": "EVT?[11414]",
         "id": 11414,
         "include": "EVT?[10010]"
     },
     "11415": {
         "event": "\u53cd\u73af\u4fdd\u56e2\u4f53\u5728\u897f\u65b9\u56fd\u5bb6\u6e38\u884c\u3002",
         "exclude": "EVT?[11415]",
@@ -10424,21 +10773,22 @@
     "11417": {
         "event": "\u4e00\u4f4d\u54f2\u5b66\u5bb6\u5f00\u8f9f\u4e86\u865a\u62df\u4e3b\u4e49\u54f2\u5b66\uff0c\u4ece\u4e16\u754c\u662f\u865a\u62df\u6e38\u620f\u4e3a\u8d77\u70b9\u5efa\u6784\u4e86\u6574\u4e2a\u4f53\u7cfb\u3002",
         "exclude": "EVT?[11417,11263,11288]",
         "id": 11417,
         "include": "EVT?[10010]"
     },
     "11418": {
-        "event": "\u56fd\u5bb6\u7edf\u4e00\u5168\u56fd\u6237\u53e3\u3002",
+        "event": "\u4e00\u5e74\u4e2d\u6709100\u591a\u540d\u660e\u661f\u56e0\u5077\u7a0e\u88ab\u7f5a\u3002",
         "exclude": "EVT?[11418]",
         "id": 11418,
-        "include": "EVT?[10010]"
+        "include": "EVT?[10010]",
+        "postEvent": "\u56fd\u5bb6\u5f00\u59cb\u5927\u529b\u6574\u6cbb\uff0c\u5a31\u4e50\u5708\u9010\u6e10\u8d70\u5411\u8870\u4ea1\u3002"
     },
     "11419": {
-        "event": "\u56fd\u5bb6\u8fdb\u4e00\u6b65\u63a8\u51fa\u9650\u5236\u672a\u6210\u5e74\u4eba\u6d88\u8d39\u7684\u6cd5\u6848\u3002",
+        "event": "\u5370\u5ea6\u7a81\u53d1\u4e25\u91cd\u4f20\u67d3\u75c5\uff0c\u706b\u846c\u573a\u7206\u6ee1\u3002",
         "exclude": "EVT?[11419]",
         "id": 11419,
         "include": "EVT?[10010]"
     },
     "11420": {
         "event": "\u751f\u7269\u5b66\u5bb6\u5ba3\u79f0\uff0c\u56e0\u4e3a\u4eba\u7c7b\u8fc7\u4e8e\u4f9d\u8d56\u4eba\u9020\u5de5\u5177\uff0c\u4eba\u7c7b\u5929\u751f\u7684\u5de5\u5177\u773c\u8033\u624b\u811a\u7b49\u5df2\u7ecf\u505c\u6b62\u8fdb\u5316\u4e86\u3002",
         "exclude": "EVT?[11420]",
@@ -10461,31 +10811,30 @@
         "event": "\u7f8e\u56fd\u4e3a\u4fdd\u62a4\u4eba\u6743\uff0c\u7981\u6b62\u51fa\u7248\u4ee5\u201c\u4ed6\u4eba\u7684\u51fa\u4e11\u6216\u4e0d\u5e78\u201d\u4f5c\u4e3a\u7b11\u70b9\u7684\u4f5c\u54c1\u3002",
         "exclude": "EVT?[11423]",
         "id": 11423,
         "include": "EVT?[10010]",
         "postEvent": "\u8c10\u97f3\u6897\u5f00\u59cb\u7edf\u6cbb\u5f71\u89c6\u754c\u3002"
     },
     "11424": {
-        "event": "\u8c03\u67e5\u663e\u793a\uff0c84%\u7684\u4eba\u8ba4\u4e3a\u81ea\u5df1\u7684\u989c\u503c\u662f\u201c\u4e2d\u4e0a\u201d\u3002",
-        "exclude": "EVT?[11424,11425,11426,11263,11288]",
+        "event": "\u67d0\u9ad8\u6821\u591a\u540d\u540c\u5b66\u5728\u5bbf\u820d\u9ad8\u5531\u56fd\u9645\u6b4c\uff0c\u6821\u9886\u5bfc\u8fc5\u901f\u9501\u5b9a\u8fd9\u4e9b\u540c\u5b66\u6240\u5728\u5bdd\u5ba4\u5e76\u4e0a\u95e8\u5bf9\u4ed6\u4eec\u8fdb\u884c\u4e86\u8868\u5f70\u548c\u9f13\u52b1\u3002",
+        "exclude": "EVT?[11424]",
         "id": 11424,
         "include": "EVT?[10010]"
     },
     "11425": {
-        "event": "\u8c03\u67e5\u663e\u793a\uff0c50%\u7684\u4eba\u8ba4\u4e3a\u81ea\u5df1\u6bd4\u5927\u591a\u6570\u4eba\u591a\u70b9\u513f\u5c0f\u806a\u660e\uff0c\u53e6\u591630%\u7684\u4eba\u8ba4\u4e3a\u81ea\u5df1\u7684\u667a\u5546\u663e\u8457\u4f18\u4e8e\u8eab\u8fb9\u7684\u4eba\u3002",
-        "exclude": "EVT?[11424,11425,11426,11263,11288]",
+        "event": "\u7814\u7a76\u53d1\u73b0\uff0c\u7f51\u7edc\u89c6\u9891\u5e73\u5747\u65f6\u957f\u5728\u8fc7\u53bb10\u5e74\u95f4\u964d\u4f4e\u4e8650%\u3002",
+        "exclude": "EVT?[11425]",
         "id": 11425,
         "include": "EVT?[10010]"
     },
     "11426": {
-        "event": "\u8c03\u67e5\u663e\u793a\uff0c75%\u7684\u4eba\u8ba4\u4e3a\u81ea\u5df1\u7684\u4eba\u54c1\u597d\u8fc7\u7edd\u5927\u591a\u6570\u4eba\u3002",
-        "exclude": "EVT?[11424,11425,11426,11263,11288]",
+        "event": "\u636e\u62a5\u9053\uff0c\u7f8e\u56fd\u5bcc\u8c6a\u5728\u745e\u58eb\u94f6\u884c\u5b58\u6b3e\u8fbe\u6570\u5343\u4ebf\u7f8e\u5143\uff0c\u5f15\u53d1\u7f8e\u56fd\u5e73\u6c11\u4e0d\u6ee1\u3002",
+        "exclude": "EVT?[11426]",
         "id": 11426,
-        "include": "EVT?[10010]",
-        "postEvent": "\u4e13\u5bb6\u8868\u793a\u53ef\u80fd\u4e0e\u62a5\u9053\u72af\u7f6a\u7684\u65b0\u95fb\u8fc7\u591a\u6709\u5173\u3002"
+        "include": "EVT?[10010]"
     },
     "11427": {
         "event": "\u4f60\u524d\u4e24\u5e74\u5f00\u59cb\u4f7f\u7528\u7684\u4e00\u4e2a\u5c0f\u4f17\u7ebf\u4e0a\u793e\u4ea4\u5e73\u53f0\uff0c\u73b0\u5728\u7a81\u7136\u706b\u4e86\u3002",
         "exclude": "EVT?[11427,11263,11288]",
         "id": 11427,
         "include": "EVT?[10010]",
         "postEvent": "\u4f46\u4f60\u611f\u89c9\u5e73\u53f0\u5185\u7684\u73af\u5883\u4e00\u4e0b\u5b50\u4e4c\u70df\u7634\u6c14\u8d77\u6765\uff0c\u4f60\u5f88\u6000\u5ff5\u4e24\u5e74\u524d\u7684\u6837\u5b50\u3002"
@@ -10495,49 +10844,50 @@
         "exclude": "EVT?[11428]",
         "id": 11428,
         "include": "EVT?[10010]"
     },
     "11429": {
         "event": "\u6709\u7814\u7a76\u8868\u660e\uff0c\u5386\u53f2\u4e0a\u6240\u6709\u7684\u751f\u547d\u90fd\u53ef\u4ee5\u7b97\u6210\u4e00\u4e2a\u4e2a\u4f53\u7684\u4e00\u90e8\u5206\u3002",
         "exclude": "EVT?[11429]",
+        "grade": 1,
         "id": 11429,
         "include": "EVT?[10010]"
     },
     "11430": {
-        "event": "\u8bfa\u8d1d\u5c14\u5956\u6682\u505c\u4e3e\u529e\u3002",
+        "event": "\u8c03\u67e5\u663e\u793a\uff0c84%\u7684\u4eba\u8ba4\u4e3a\u81ea\u5df1\u7684\u989c\u503c\u662f\u201c\u4e2d\u4e0a\u201d\u3002",
         "exclude": "EVT?[11430]",
         "id": 11430,
         "include": "EVT?[10010]"
     },
     "11431": {
-        "event": "\u6b27\u76df\u5408\u5e76\u6210\u4e86\u4e00\u4e2a\u56fd\u5bb6\u3002",
+        "event": "\u4e2d\u8003\u5206\u6d41\u88ab\u53d6\u6d88\u3002",
         "exclude": "EVT?[11431]",
         "id": 11431,
         "include": "EVT?[10010]"
     },
     "11432": {
         "event": "\u5370\u5ea6\u6210\u4e3a\u4e86\u8054\u5408\u56fd\u7b2c\u516d\u5e38\u3002",
-        "exclude": "EVT?[11432,11433]",
+        "exclude": "EVT?[11432]",
         "id": 11432,
         "include": "EVT?[10010]"
     },
     "11433": {
-        "event": "\u8054\u5408\u56fd\u89e3\u6563\u4e86\u3002",
+        "event": "\u67d0\u4e13\u5bb6\u5728\u8fdb\u884c\u300a\u4fdd\u62a4\u73af\u5883\u3001\u4e0d\u8981\u5403\u8089\u300b\u7684\u6f14\u8bb2\u540e\uff0c\u88ab\u4eba\u610f\u5916\u62cd\u5230\u8fdb\u5165\u4e86\u4e00\u5bb6\u70e4\u8089\u5e97\u3002",
         "exclude": "EVT?[11433]",
         "id": 11433,
         "include": "EVT?[10010]"
     },
     "11434": {
         "event": "\u671d\u9c9c\u7edf\u4e00\u97e9\u56fd\u3002",
         "exclude": "EVT?[11434]",
         "id": 11434,
         "include": "EVT?[10010]"
     },
     "11435": {
-        "event": "\u6559\u5e08\u884c\u4e1a\u8d8a\u6765\u8d8a\u53d7\u5230\u91cd\u89c6\uff0c\u6559\u5e08\u5de5\u8d44\u663e\u8457\u63d0\u9ad8\u3002",
+        "event": "\u67d0\u5730\u653f\u5e9c\u63a8\u51fa\u5e02\u6c11\u6210\u5c31\u7cfb\u7edf\uff0c\u7ed3\u5a5a\u88ab\u8bbe\u4e3a\u4f20\u8bf4\u7ea7\u6210\u5c31\uff0c\u5f15\u53d1\u5927\u6279\u5e74\u8f7b\u4eba\u524d\u53bb\u9886\u8bc1\u3002",
         "exclude": "EVT?[11435]",
         "id": 11435,
         "include": "EVT?[10010]"
     },
     "11436": {
         "event": "\u56fd\u5bb6\u5ba3\u5e03\u6f14\u5458\u6b4c\u624b\u6536\u5165\u9700\u6309\u5de5\u8d44\u53d1\u653e\uff0c\u4e14\u4e0d\u5f97\u8d85\u8fc7\u5f53\u5730\u516c\u52a1\u5458\u5e73\u5747\u5de5\u8d44\u7684\u4e09\u500d\u3002",
         "exclude": "EVT?[11436]",
@@ -10556,19 +10906,18 @@
         "id": 11438,
         "include": "EVT?[10010]"
     },
     "11439": {
         "event": "\u4e16\u754c\u7b2c\u4e00\u4e2a\u516b\u661f\u7ea7\u9152\u5e97\u5728\u7a7a\u95f4\u7ad9\u5efa\u6210\u3002",
         "exclude": "EVT?[11439,11263,11288]",
         "id": 11439,
-        "include": "EVT?[10010]",
-        "postEvent": "\u5728\u4e0a\u9762\u80fd\u770b\u5230\u516b\u5927\u884c\u661f\u3002"
+        "include": "EVT?[10010]"
     },
     "11440": {
-        "event": "\u5e7f\u5dde\u51fa\u73b0\u5341\u51e0\u5e73\u65b9\u516c\u91cc\u5927\u7684\u5de8\u578b\u87d1\u8782\u3002",
+        "event": "\u4e13\u5bb6\u5efa\u8bae\uff0c\u653f\u5e9c\u5e94\u5f53\u4e3a\u4e13\u5bb6\u63d0\u4f9b\u4fdd\u9556\uff0c\u907f\u514d\u4e13\u5bb6\u88ab\u66b4\u6c11\u6253\u6b7b\u3002",
         "exclude": "EVT?[11440]",
         "id": 11440,
         "include": "EVT?[10010]"
     },
     "11441": {
         "event": "\u67d0\u6e38\u620f\u516c\u53f8\u5411\u6559\u4f1a\u51fa\u8d44\uff0c\u5c06\u5723\u7ecf\u4e2d\u7684\u201c\u8bfa\u4e9a\u201d\u51a0\u540d\u6210\u201c\u660e\u65e5\u201d\u3002",
         "exclude": "EVT?[11441]",
@@ -10584,15 +10933,15 @@
     "11443": {
         "event": "\u7531\u4e8e\u201c\u7f29\u5199\u6548\u5e94\u201d\uff0c\u6c49\u8bed\u5df2\u7ecf\u7b80\u5316\u4e3a\u7eaf\u5b57\u6bcd\u8bed\u8a00\u3002",
         "exclude": "EVT?[11443]",
         "id": 11443,
         "include": "EVT?[10010]"
     },
     "11444": {
-        "event": "\u7f8e\u56fd\u5c06\u5c0f\u5b66\u5165\u5b66\u5e74\u9f84\u63a8\u8fdf\u523010-12\u5c81\u3002",
+        "event": "\u4e13\u5bb6\u5efa\u8bae\u63d0\u9ad8\u623f\u4ef7\u3002",
         "exclude": "EVT?[11444]",
         "id": 11444,
         "include": "EVT?[10010]"
     },
     "11445": {
         "event": "\u672c\u5730\u4e00\u9189\u9152\u7537\u5b50\u8def\u8fb9\u88ab\u4eba\u4fb5\u72af\uff0c\u5a92\u4f53\u79f0\u539f\u56e0\u662f\u5176\u8863\u7740\u66b4\u9732\u3002",
         "exclude": "EVT?[11445,11263,11288]",
@@ -10615,364 +10964,389 @@
     "11448": {
         "event": "\u7269\u7406\u5b66\u5bb6\u53d1\u73b0\u5730\u7403\u53ef\u80fd\u771f\u7684\u662f\u5b87\u5b99\u7684\u4e2d\u5fc3\u3002",
         "exclude": "EVT?[11448]",
         "id": 11448,
         "include": "EVT?[10010]"
     },
     "11449": {
-        "event": "\u524d\u9886\u5bfc\u4eba\u6253\u7834\u6700\u957f\u5bff\u7684\u4eba\u5409\u5c3c\u65af\u7eaa\u5f55\u3002",
+        "event": "\u7ebd\u7ea6\u65f6\u62a5\u516c\u5e03\u7f8e\u56fd\u5e74\u5ea6\u5341\u5927\u7f51\u7edc\u6d41\u884c\u8bed\u3002",
         "exclude": "EVT?[11449]",
         "id": 11449,
-        "include": "EVT?[10010]"
+        "include": "EVT?[10010]",
+        "postEvent": "\u7f8e\u56fd\u7f51\u6c11\u5e76\u4e0d\u63a5\u53d7\uff0c\u8ba4\u4e3a\u5b98\u65b9\u7684\u6d41\u884c\u8bed\u592a\u8131\u79bb\u7fa4\u4f17\u3002"
     },
     "11450": {
         "event": "\u4e00\u9897\u5c0f\u884c\u661f\u5373\u5c06\u51fb\u4e2d\u5730\u7403\u65f6\u7a81\u7136\u6298\u8fd4\u79bb\u5f00\u3002",
         "exclude": "EVT?[11450]",
         "id": 11450,
         "include": "EVT?[10010]",
         "postEvent": "\u4e13\u5bb6\u79f0\u53ef\u80fd\u6709\u4eba\u8bb8\u4e86\u4ec0\u4e48\u79bb\u8c31\u7684\u613f\u671b\u3002"
     },
     "11451": {
         "effect": {
             "STR": 80
         },
         "event": "\u4f60\u4f7f\u7528\u9b54\u6cd5\u68d2\uff0c\u53d8\u8eab\u6210\u4e86\u9b54\u6cd5\u5c11\u5973\u3002",
+        "exclude": "EVT?[11451]",
+        "grade": 3,
         "id": 11451,
-        "include": "(TLT?[1131])&(EVT?[10002,20053,10111])&(EVT?[10007,10008])",
+        "include": "(TLT?[1131])&(EVT?[10002,20053,10111])&(EVT?[10007,10008,20007,20008])",
         "postEvent": "\u4f60\u53d8\u5f3a\u4e86\uff0c\u4f46\u4ece\u6b64\u4f60\u8981\u5c65\u884c\u8eab\u4e3a\u9b54\u6cd5\u5c11\u5973\u7684\u4f7f\u547d\u2026\u2026"
     },
     "11452": {
         "event": "\u4f60\u548c\u4eba\u7c7b\u770b\u4e0d\u89c1\u7684\u602a\u7269\u6218\u6597\u3002",
         "exclude": "EVT?[21457]",
+        "grade": 1,
         "id": 11452,
         "include": "EVT?[11451]"
     },
     "11453": {
         "event": "\u4f60\u5b88\u62a4\u7740\u8fd9\u4e2a\u661f\u7403\u3002",
         "exclude": "EVT?[21457]",
+        "grade": 1,
         "id": 11453,
         "include": "EVT?[11451]"
     },
     "11454": {
         "event": "\u4f60\u4e0d\u518d\u662f\u5c11\u5973\uff0c\u9b54\u6cd5\u68d2\u79bb\u5f00\u4e86\u4f60\u5bfb\u627e\u4e0b\u4e00\u4e2a\u4e3b\u4eba\u3002",
         "exclude": "EVT?[21457,11454]",
+        "grade": 1,
         "id": 11454,
         "include": "EVT?[11451]",
         "postEvent": "\u4f60\u7684\u9b54\u6cd5\u5c11\u5973\u751f\u6daf\u7ed3\u675f\u4e86\uff0c\u9b54\u529b\u4e5f\u90fd\u6d88\u6563\u4e86\uff0c\u4f60\u53d8\u56de\u4e86\u666e\u901a\u4eba\u3002"
     },
     "11455": {
         "branch": [
             "STR<88:10000"
         ],
         "event": "\u4f60\u548c\u4fb5\u5165\u5730\u7403\u7684\u94f6\u6cb3\u5e1d\u738b\u6218\u6597\u3002\u5b83\u5341\u5206\u5f3a\u5927\u3002",
         "exclude": "EVT?[11455,21457]",
+        "grade": 2,
         "id": 11455,
         "include": "EVT?[11456]",
         "postEvent": "\u4f46\u4f60\u8fd8\u662f\u8d62\u4e86\u3002"
     },
     "11456": {
         "event": "\u4e00\u4e2a\u5916\u661f\u4eba\u6765\u5730\u7403\u5ba3\u79f0\u8981\u7edf\u6cbb\u5730\u7403\uff0c\u88ab\u4f60\u79d2\u6740\u3002",
         "exclude": "EVT?[11456,21457]",
+        "grade": 1,
         "id": 11456,
         "include": "EVT?[11451]"
     },
     "11457": {
         "branch": [
             "INT<5:21457"
         ],
         "event": "\u4f60\u906d\u5230\u4e86\u89e6\u624b\u5973\u738b\u7684\u653b\u51fb\u3002",
         "exclude": "EVT?[11457,21457]",
+        "grade": 2,
         "id": 11457,
         "include": "EVT?[11451]",
         "postEvent": "\u4f60\u6d88\u706d\u4e86\u89e6\u624b\u5973\u738b\u3002"
     },
     "11458": {
         "event": "\u4f60\u5728\u5730\u7403\u4e0a\u8086\u610f\u7834\u574f\u3002",
+        "grade": 1,
         "id": 11458,
         "include": "EVT?[21457]"
     },
     "11459": {
         "event": "\u4f60\u5f15\u8bf1\u5176\u4ed6\u9b54\u6cd5\u5c11\u5973\u6076\u5815\u3002",
+        "grade": 1,
         "id": 11459,
         "include": "EVT?[21457]"
     },
     "11460": {
         "event": "\u4f60\u6467\u6bc1\u4e86\u7f8e\u56fd\u3002",
         "exclude": "EVT?[11460]",
+        "grade": 2,
         "id": 11460,
         "include": "EVT?[21457]"
     },
     "11461": {
         "event": "\u4f60\u6467\u6bc1\u4e86\u82f1\u56fd\u3002",
         "exclude": "EVT?[11461]",
+        "grade": 2,
         "id": 11461,
         "include": "EVT?[21457]"
     },
     "11462": {
         "event": "\u6cd5\u56fd\u81e3\u670d\u5728\u4f60\u88d9\u4e0b\u3002",
         "exclude": "EVT?[11462]",
+        "grade": 2,
         "id": 11462,
         "include": "EVT?[21457]"
     },
     "11463": {
         "event": "\u4f60\u6d88\u706d\u4e86\u65e5\u672c\u6240\u6709\u7684\u7537\u6027\u3002",
         "exclude": "EVT?[11463,11476]",
+        "grade": 2,
         "id": 11463,
         "include": "EVT?[21457]"
     },
     "11464": {
         "event": "\u4f60\u6467\u6bc1\u4e86\u4fc4\u7f57\u65af\u3002",
         "exclude": "EVT?[11464]",
+        "grade": 2,
         "id": 11464,
         "include": "EVT?[21457]"
     },
     "11465": {
         "branch": [
             "STR<88:10000"
         ],
         "effect": {
             "STR": 88
         },
         "event": "\u4f60\u906d\u9047\u4e86\u4e00\u4e2a\u5f3a\u5927\u7684\u9b54\u6cd5\u5c11\u5973\u3002",
         "exclude": "EVT?[11465]",
+        "grade": 2,
         "id": 11465,
         "include": "EVT?[21457]",
         "postEvent": "\u4f60\u62fc\u5c3d\u5168\u529b\u6740\u6b7b\u4e86\u5bf9\u65b9,\u5e76\u5438\u53d6\u4e86\u5979\u7684\u9b54\u529b\u3002"
     },
     "11466": {
         "branch": [
             "STR<100:10000"
         ],
         "event": "\u4e00\u4e2a\u4f1a\u98de\u7684\u4eba\u5bf9\u4f60\u51fa\u624b\uff0c\u4ed6\u79f0\u81ea\u5df1\u662f\u7b51\u57fa\u671f\u4fee\u58eb\u3002",
         "exclude": "EVT?[11466]",
+        "grade": 2,
         "id": 11466,
         "include": "EVT?[21457]",
         "postEvent": "\u82e6\u6218\u540e\u4f60\u6740\u6b7b\u4e86\u5bf9\u65b9\u3002"
     },
     "11467": {
         "branch": [
             "STR<2000:10000"
         ],
         "event": "\u4e00\u4e2a\u4f1a\u98de\u7684\u4eba\u5bf9\u4f60\u51fa\u624b\uff0c\u4ed6\u79f0\u81ea\u5df1\u662f\u6e21\u52ab\u671f\u4fee\u58eb\u3002",
         "exclude": "EVT?[11467]",
+        "grade": 2,
         "id": 11467,
         "include": "EVT?[21457]",
         "postEvent": "\u4f60\u8fd8\u6ca1\u770b\u6e05\u5bf9\u65b9\u600e\u4e48\u51fa\u624b\u5c31\u5931\u53bb\u4e86\u610f\u8bc6\u3002"
     },
     "11468": {
         "effect": {
             "AGE": -5
         },
         "event": "\u65f6\u5149\u7a81\u7136\u5012\u6d41\u4e86\u3002",
+        "grade": 2,
         "id": 11468,
         "include": "TLT?[1133]"
     },
     "11469": {
         "effect": {
             "AGE": -50
         },
         "event": "\u4f60\u7a81\u7136\u56de\u5230\u4e86\u5e74\u8f7b\u7684\u65f6\u5019\u3002",
         "exclude": "EVT?[11469]",
+        "grade": 2,
         "id": 11469,
         "include": "TLT?[1132]"
     },
     "11470": {
         "event": "\u4e3a\u7ef4\u62a4\u7f51\u7edc\u6587\u660e\u73af\u5883\uff0c\u65e5\u672c\u5c06\u88ab\u548c\u8c10\u4e3a\u6708\u672c\u3002",
         "exclude": "EVT?[11470,11476]",
         "id": 11470
     },
     "11471": {
-        "event": "\u8d85\u7ea7\u7ba1\u7406\u5458\uff08Admin\uff09\u5df2\u88ab\u51fb\u8d25\u3002",
+        "event": "\u4e13\u5bb6\u5efa\u8bae\uff0c\u5982\u679c\u4eba\u751f\u4e0d\u5982\u610f\u53ef\u4ee5\u5c1d\u8bd5\u91cd\u5f00\uff0c\u4e3a\u51cf\u8f7b\u517b\u8001\u91d1\u538b\u529b\u505a\u51fa\u8d21\u732e\u3002",
         "exclude": "EVT?[11471]",
         "id": 11471,
         "include": "EVT?[10010]"
     },
     "11472": {
-        "event": "4\u670810\u53f7\uff0c\u4e00\u4e9b\u5144\u5f1f\u4eec\u5931\u53bb\u4e86\u5bb6\u56ed\uff0c\u53ea\u7559\u4e0b\u4e86\u90a3\u6bb5\u8bdd\uff0c\u6697\u53f7\u4e0d\u53d8\uff0c\u6c5f\u6e56\u518d\u89c1\uff0c\u6ef4\uff0c\u6ef4\u6ef4\u3002\u5929\u738b\u76d6\u5730\u864e\u2026\u2026",
+        "event": "\u67d0\u4e92\u8054\u7f51\u5927\u5382\u5f00\u53d1\u7684\u81ea\u52a8\u7f16\u7a0bAI\uff0c\u5728\u4e0a\u7ebf\u4e09\u5929\u540e\u8fc7\u52b3\u731d\u6b7b\u3002",
         "exclude": "EVT?[11472]",
         "id": 11472,
         "include": "EVT?[10010]"
     },
     "11473": {
-        "event": "\u636e\u4e00\u4f4d\u8d44\u6df1\u6e38\u620f\u5236\u4f5c\u8005\u900f\u9732\uff1a\u67d0\u6e38\u620f\u7684\u7b2c\u516d\u4ee3\u4f5c\u54c1\u6b63\u5728\u7d27\u5bc6\u5236\u4f5c\u5f53\u4e2d\uff0c\u4ed6\u4eec\u5df2\u7ecf\u5efa\u597d\u4e86\u6587\u4ef6\u5939\uff0c\u786e\u5b9a\u6d88\u606f\u53ef\u9760\u3002",
+        "event": "\u79e6\u59cb\u7687\u9675\u88ab\u6253\u5f00\uff0c\u5893\u7a74\u91cc\u9762\u662f\u7a7a\u7684\u3002",
         "exclude": "EVT?[11473]",
         "id": 11473,
         "include": "EVT?[10010]"
     },
     "11474": {
-        "event": "\u6e7e\u533a\u7a0b\u5e8f\u5458\u5efa\u56fd\uff0c\u7981\u6b62\u53d8\u66f4\u9700\u6c42\u88ab\u5217\u5165\u5baa\u6cd5\u3002",
+        "event": "\u653f\u5e9c\u5c06\u6e38\u620f\u4e2d\u7684\u62bd\u5361\u8ba4\u5b9a\u4e3a\u8d4c\u535a\u884c\u4e3a\u3002",
         "exclude": "EVT?[11474]",
         "id": 11474
     },
     "11475": {
-        "effect": {
-            "STR": 1
-        },
-        "event": "\u4f60\u53bb\u542c\u4e86\u4e00\u573a\u7535\u5b50\u7ba1\u98ce\u7434\u97f3\u4e50\u4f1a\uff0c\u611f\u89c9\u81ea\u5df1\u7684\u6d2a\u8352\u4e4b\u529b\u6b63\u5728\u89c9\u9192",
+        "event": "\u4e00\u56fe\u4e66\u9986\u53d1\u751f\u706b\u707e\uff0c\u9664\u535a\u4eba\u4f20\u4e4b\u5916\u7684\u5176\u4ed6\u4e66\u7c4d\u5168\u90e8\u711a\u6bc1\u3002",
         "exclude": "EVT?[11475]",
         "id": 11475,
         "include": "(MNY>7)&(EVT?[10010])"
     },
     "11476": {
         "event": "\u5c0f\u65e5\u5b50\u8fc7\u5f97\u4e0d\u9519\u7684\u56fd\u5bb6\u8ba4\u7956\u5f52\u5b97\uff0c\u5f52\u5316\u4e3a\u6052\u6851\u7701\u3002",
         "exclude": "EVT?[11476,11497,11498]",
         "id": 11476
     },
     "11477": {
-        "event": "\u67d0\u5b59\u59d3\u6f2b\u753b\u5bb6\u6c89\u8ff7\u6478\u9c7c\uff0c\u6700\u7ec8\u653e\u5f03\u6f2b\u753b\u3002\u610f\u5916\u4e2d\u5956\u4e00\u4ebf\u540e\uff0c\u9192\u6765\u53d1\u73b0\u662f\u505a\u68a6\u3002",
+        "event": "\u4e00\u540d\u5143\u5b87\u5b99\u4e3b\u64ad\u9003\u7a0e138\u4ebf\uff0c\u6253\u7834\u5386\u53f2\u8bb0\u5f55\u3002",
         "exclude": "EVT?[11477]",
         "id": 11477,
-        "include": "EVT?[10009]"
+        "include": "EVT?[10432]"
     },
     "11478": {
-        "event": "\u67d0\u7f51\u7ea2\u5929\u5929\u5fd9\u4e8e\u76f8\u4eb2\uff0c\u5bfc\u81f4\u7c89\u4e1d\u4e0d\u6ee1\uff0c\u6700\u7ec8\u4e0d\u5f97\u4e0d\u516c\u5f00\u5ba3\u5e03\u81ea\u5df1\u8f6c\u6295\u72ec\u8eab\u4e3b\u4e49\u3002",
+        "event": "\u4e13\u5bb6\u5efa\u8bae\uff0c\u519c\u6c11\u53ef\u4ee5\u5728\u7701\u4f1a\u4e70\u623f\uff0c\u6bcf\u5929\u5750\u9ad8\u94c1\u56de\u8001\u5bb6\u79cd\u7530\u3002",
         "exclude": "EVT?[11478]",
         "id": 11478,
         "include": "EVT?[10009]"
     },
     "11479": {
-        "event": "\u53ef\u4ee5\u81ea\u4e3b\u53d1\u660e\u7684\u53d1\u660e\u673a\u88ab\u53d1\u660e\uff0c\u5947\u602a\u7684\u53d1\u660e\u5145\u65a5\u4e16\u754c\uff0c\u5f15\u53d1\u4e86\u707e\u96be\u3002",
+        "event": "\u5370\u5ea6\u4eba\u53e3\u8d85\u8d8a\u4e2d\u56fd\u3002",
         "exclude": "EVT?[11479]",
         "id": 11479,
         "include": "EVT?[10010]"
     },
     "11480": {
-        "event": "\u56fd\u8db3\u593a\u5f97\u4e16\u754c\u676f\u3002",
+        "event": "\u5b66\u672f\u754c\u666e\u904d\u5f00\u59cb\u4f7f\u7528AI\u6765\u5199\u8bba\u6587\uff0c\u8bba\u6587\u4ea7\u91cf\u7206\u53d1\u5f0f\u589e\u957f\u3002",
         "exclude": "EVT?[11480]",
         "id": 11480
     },
     "11481": {
-        "event": "\u865a\u62df\u5076\u50cf\u738b\u52a0\u7136\u5728\u4e00\u6b21\u76f4\u64ad\u4e2d\u5ba3\u5e03\u4e0e\u540c\u4e8b\u675c\u5411\u7897\u6210\u4e3a\u604b\u4eba\u3002",
+        "event": "\u67d0\u9ad8\u6821\u88ab\u66dd\u5149\u53ef\u4ee5\u8d70\u540e\u95e8\u8fdb\u5165\u540e\uff0c\u5f00\u59cb\u660e\u7801\u6807\u4ef7\u552e\u5356\u540d\u989d\u3002",
         "exclude": "EVT?[11481]",
         "id": 11481,
         "include": "EVT?[10010]"
     },
     "11482": {
-        "event": "\u6c11\u95f4\u4e00\u6b3e\u540d\u4e3a\u201c\u4eba\u751f\u91cd\u5f00\u6a21\u62df\u5668\u201d\u7684\u6e38\u620f\u6b63\u5728\u5174\u8d77\uff0c\u5f15\u8d77\u70ed\u8bae\u3002",
+        "event": "\u4e24\u4f4d\u8457\u540d\u4eba\u5de5\u667a\u80fd\u5076\u50cf\u7684\u4e0d\u6b63\u5f53\u7537\u5973\u5173\u7cfb\u88ab\u66dd\u5149\uff0c\u5176\u4e2d\u4e00\u4f4d\u5220\u5e93\u81ea\u6740\u4e86\u3002",
         "exclude": "EVT?[11482]",
         "id": 11482,
-        "include": "EVT?[10009]"
+        "include": "EVT?[11481]"
     },
     "11483": {
-        "event": "\u4e00\u4f4d\u6253\u6c14\u7403\u644a\u8001\u677f\u88ab\u53d1\u73b0\u7adf\u662f\u5730\u4e0b\u519b\u706b\u5927\u4ea8\u3002",
+        "event": "\u7531\u4e8e\u4e2d\u56fd\u4f01\u4e1a\u7684\u5927\u529b\u8d44\u52a9\uff0c\u4e16\u754c\u676f\u5c06\u5165\u56f4\u540d\u989d\u6570\u91cf\u63d0\u9ad8\u5230\u4e86108\u3002",
         "exclude": "EVT?[11483]",
         "id": 11483,
         "include": "EVT?[10011]"
     },
     "11484": {
-        "event": "\u4eba\u7c7b\u53d1\u73b0\u5b9c\u5c45\u7c7b\u5730\u884c\u661f\uff0c\u88ab\u547d\u540d\u4e3a\u4e0d\u5403\u9999\u83dc\u661f27\u53f7\u3002",
+        "event": "\u56fd\u5185\u4e92\u8054\u7f51\u4f01\u4e1a\u5927\u5e45\u6269\u62db\uff0c\u4e1a\u754c\u4e00\u7247\u7e41\u8363\u3002",
         "exclude": "EVT?[11484]",
         "id": 11484
     },
     "11485": {
-        "event": "\u6709\u79d1\u7814\u7ec4\u7ec7\u5ba3\u79f0\uff0c\u4eba\u7c7b\u6709\u80fd\u529b\u91cd\u5851\u5927\u81ea\u7136\u98df\u7269\u7f51\uff0c\u521b\u9020\u4e00\u4e2a\u6ca1\u6709\u98df\u8089\u52a8\u7269\u7684\u65b0\u751f\u6001\u5e73\u8861\u3002\u5927\u6982\u9700\u8981\u4e00\u4e07\u5e74\u5230\u4e00\u5343\u4e07\u5e74\u3002",
+        "event": "\u5168\u7403\u4eba\u53e3\u8dcc\u783480\u4ebf\u3002",
         "exclude": "EVT?[11485]",
         "id": 11485
     },
     "11486": {
-        "event": "\u80a1\u5e02\u5927\u6da8\uff0cP\u80a1\u76f4\u51b2\u4e00\u4e07\u70b9\u3002",
+        "event": "\u5e74\u5ea6\u5341\u5927\u6d41\u884c\u6b4c\u516c\u5e03\uff0c\u4f60\u53d1\u73b0\u4e00\u9996\u4e5f\u6ca1\u542c\u8fc7\u3002",
         "exclude": "EVT?[11486]",
         "id": 11486,
         "include": "EVT?[10010]"
     },
     "11487": {
-        "event": "\u4eba\u7c7b\u9996\u6b213D\u6253\u5370\u6708\u7403\u3002\u4ece\u6b64\u5929\u4e0a\u6709\u4e86\u4e24\u4e2a\u6708\u4eae\u3002",
+        "event": "\u636e\u62a5\u9053\uff0c\u7f8e\u56fd\u4e00\u5f69\u6c11\u4e2d\u5f69\u7968800\u4ebf\u7f8e\u5143\uff0c\u540e\u88ab\u66dd\u5149\u662f\u56e0\u7f8e\u56fd\u5f69\u7968\u6ede\u9500\u800c\u7f16\u9020\u51fa\u7684\u5047\u65b0\u95fb\u3002",
         "exclude": "EVT?[11487]",
         "id": 11487
     },
     "11488": {
-        "event": "\u53d7\u6c14\u5019\u5f71\u54cd\uff0c\u4e00\u53ea\u91ce\u732a\u649e\u6b7b\u4e86\u4e00\u53ea\u5e1d\u738b\u87f9\u3002",
+        "event": "\u7f8e\u56fd\u9ec4\u77f3\u516c\u56ed\u706b\u5c71\u7206\u53d1\u3002\u5168\u7403\u5e73\u5747\u6c14\u6e29\u4e0b\u964d1\u6444\u6c0f\u5ea6\u3002",
         "exclude": "EVT?[11488]",
         "id": 11488,
         "include": "EVT?[10009]"
     },
     "11489": {
-        "event": "\u4e16\u754c\u4e0a\u9996\u4e2a\u6ca1\u6709\u5a5a\u59fb\u7684\u56fd\u5bb6\u51fa\u73b0\u4e86\u3002",
+        "effect": {
+            "SPR": -1
+        },
+        "event": "\u4f60\u611f\u89c9\u81ea\u5df1\u8d8a\u6765\u8d8a\u96be\u4ece\u5a31\u4e50\u6d3b\u52a8\u4e2d\u83b7\u5f97\u4e50\u8da3\u4e86\u3002",
         "exclude": "EVT?[11489]",
         "id": 11489
     },
     "11490": {
-        "event": "\u56fd\u5185\u72ec\u7acb\u6e38\u620f\u5de5\u4f5c\u5ba4\u8054\u76df\u5236\u4f5c\u76843A\u6e38\u620f\u5927\u4f5c\u65a9\u83b7TAG\u5e74\u5ea6\u6e38\u620f\u3002",
+        "effect": {
+            "INT": 1
+        },
+        "event": "\u4f60\u559c\u6b22\u8bfb\u9053\u5fb7\u7ecf\u548c\u5e84\u5b50\u3002",
         "exclude": "EVT?[11490]",
         "id": 11490,
-        "include": "EVT?[10010]"
+        "include": "TLT?[1048]"
     },
     "11491": {
-        "event": "\u56fd\u4e52\u5728\u5bf9\u5916\u661f\u4eba\u7684\u6bd4\u8d5b\u4e2d\u5b8c\u80dc\u5bf9\u624b\uff0c\u4e3a\u661f\u7cfb\u5916\u4ea4\u505a\u51fa\u5de8\u5927\u8d21\u732e\u3002",
+        "event": "\u65e5\u672c\u516c\u5e03\u5e74\u5ea6\u6c49\u5b57\uff1a\u5bc4\u3002",
         "exclude": "EVT?[11491]",
         "id": 11491,
-        "include": "EVT?[10090,10700]"
+        "include": "EVT?[10010]"
     },
     "11492": {
-        "effect": {
-            "MNY": 2
-        },
-        "event": "\u4f60\u88ab\u65e0\u4eba\u9a7e\u9a76\u8f66\u649e\u4f24\u4e86\uff0c\u83b7\u5f97\u5927\u91cf\u8d54\u507f\u3002",
+        "event": "\u636e\u8c03\u67e5\uff0c\u6211\u56fd\u653f\u5e9c\u516c\u4fe1\u529b\u8fbe\u5230\u5386\u53f2\u6700\u9ad8\u70b9\u3002",
         "exclude": "EVT?[11492]",
         "id": 11492,
-        "include": "EVT?[10010]"
+        "include": "EVT?[10010]",
+        "postEvent": "\u636e\u7ea6\u7ff0\u970d\u666e\u91d1\u65af\u5927\u5b66\u7814\u7a76\u8868\u660e\uff0c\u7f8e\u56fd\u653f\u5e9c\u516c\u4fe1\u529b\u4ecd\u5728\u6301\u7eed\u4e0b\u964d\u3002"
     },
     "11493": {
-        "event": "\u9a6c\u65af\u514b\u5ba3\u5e03\u7279\u65af\u62c9\u8fdb\u519b\u989c\u8272\u9886\u57df\uff0c\u7528\u6237\u6388\u6743\u540e\u53ef\u4ee5\u76f4\u63a5\u901a\u8fc7\u8f66\u5185\u6444\u50cf\u5934\u8fdb\u884c\u5f55\u5236\u548c\u53d1\u5e03\u3002",
+        "event": "\u7f8e\u56fd\u67d0\u5dde\u7acb\u6cd5\uff0c\u8981\u6c42\u6240\u6709\u5fc3\u7406\u6d4b\u8bd5\u5728\u5f00\u59cb\u524d\u90fd\u9700\u8981\u6807\u6ce8\u5df4\u7eb3\u59c6\u6548\u5e94\u8b66\u544a\u3002",
         "exclude": "EVT?[11493]",
         "id": 11493,
-        "include": "EVT?[10009]"
+        "include": "EVT?[10011]"
     },
     "11494": {
-        "event": "\u706b\u661f\u5ba3\u79f0\u5373\u5c06\u767b\u9646\u671d\u9c9c\u3002",
+        "event": "\u97e9\u56fd\u4eba\u53e3\u76f4\u7ebf\u4e0b\u6ed1\uff0c\u97e9\u56fd\u653f\u5e9c\u5ba3\u5e03\u5373\u5c06\u542f\u52a8\u201c\u706b\u79cd\u201d\u8ba1\u5212\u3002",
         "exclude": "EVT?[11494]",
         "id": 11494,
         "include": "EVT?[10009]"
     },
     "11495": {
-        "event": "\u9996\u4e2a\u7981\u6b62\u8feb\u5bb3\u7a0b\u5e8f\u5458\u6cd5\u6848\u751f\u6548\u3002",
+        "event": "\u4e3a\u57f9\u517b\u9633\u521a\u4e4b\u6c14\uff0c\u6709\u5173\u4e13\u5bb6\u5efa\u8bae\u7981\u6b62\u7537\u6027\u5750\u7740\u5c0f\u4fbf\u3002",
         "exclude": "EVT?[11495]",
         "id": 11495,
-        "include": "EVT?[10010]"
+        "include": "EVT?[10009]"
     },
     "11496": {
-        "event": "\u8d8a\u5357\u5ba3\u5e03\u6bd2\u54c1\u5408\u6cd5\u5316\uff0c\u56e0\u4e3a\u53ef\u4ee5\u7ed9\u56fd\u5bb6\u521b\u9020\u5927\u91cf\u7a0e\u6536\uff0c\u63d0\u4f9b\u5927\u91cf\u5de5\u4f5c\u5c97\u4f4d\u3002",
+        "event": "\u5168\u5e74\u6240\u6709\u5f71\u89c6\u4f5c\u54c1\u7684\u4e3b\u89d2\u5747\u662f\u5c11\u6570\u4eba\u7fa4\u3002",
         "exclude": "EVT?[11496]",
         "id": 11496,
-        "include": "EVT?[10009]"
+        "include": "EVT?[10011]"
     },
     "11497": {
-        "event": "\u5916\u661f\u8230\u961f\u9020\u8bbf\uff0c\u89c2\u770b\u4e1c\u4eac\u5965\u8fd0\u4f1a\u5f00\u5e55\u5f0f\u540e\u8fde\u591c\u9003\u79bb\u5730\u7403\u3002",
-        "exclude": "EVT?[11497,11476,11491]",
+        "event": "\u7535\u5546\u5e73\u53f0\u8bbe\u7acb2.29\u8d2d\u7269\u8282\u3002\u81f3\u6b64\u7ec8\u4e8e\u5168\u5e74366\u5929\u5168\u90e8\u90fd\u662f\u8d2d\u7269\u8282\u3002",
+        "exclude": "EVT?[11497]",
         "id": 11497
     },
     "11498": {
-        "event": "\u65e5\u672c\u5927\u91cf\u5c45\u6c11\u56e0\u6838\u5e9f\u6c34\u53d8\u5f02\uff0c\u4e3a\u9632\u6b62\u75c5\u6bd2\u4f20\u64ad\u7f8e\u56fd\u5411\u65e5\u672c\u629b\u4e0b\u4e24\u9897\u539f\u5b50\u5f39\u3002",
-        "exclude": "EVT?[11476,11498]",
+        "event": "\u82f1\u56fd\u5c06\u6c49\u8bed\u8bbe\u4e3a\u5fc5\u4fee\u8bfe\u7a0b\u3002",
+        "exclude": "EVT?[11498]",
         "id": 11498,
         "include": "EVT?[10009]"
     },
     "11499": {
         "event": "\u8003\u53e4\u961f\u5728\u8499\u53e4\u4e00\u5e26\u53d1\u6398\u51fa\u4e00\u5177\u4e1c\u664b\u65f6\u671f\u9a6c\u7684\u9057\u9aa8\uff0c\u4e13\u5bb6\u6307\u51fa\u9a6c\u7684\u4e3b\u4eba\u6b63\u662f\u664b\u5143\u5e1d\u53f8\u9a6c\u777f\u3002",
         "exclude": "EVT?[11499]",
         "id": 11499,
         "include": "EVT?[10010]"
     },
     "11500": {
         "effect": {
-            "STR": -1
+            "SPR": -1
         },
-        "event": "\u8def\u8fc7\u7a7a\u5730\uff0c\u88ab\u6253\u7fbd\u6bdb\u7403\u7684\u5927\u5988\u4e00\u8bb0\u65cb\u98ce\u6263\u6740\u6253\u6655\u4e86\u8fc7\u53bb\u3002",
-        "exclude": "EVT?[11500]",
+        "event": "\u4f60\u611f\u89c9\u4e16\u754c\u65e5\u65b0\u6708\u5f02\uff0c\u5404\u79cd\u5927\u4e8b\u4e0d\u65ad\u53d1\u751f\uff0c\u4f46\u597d\u50cf\u53c8\u90fd\u4e0e\u4f60\u7684\u751f\u6d3b\u65e0\u5173\u3002",
+        "exclude": "EVT?[11500,11501]",
         "id": 11500,
-        "include": "(EVT?[10010])&(STR<4)"
+        "include": "MNY<4"
     },
     "11501": {
-        "event": "\u56fd\u5bb6\u964d\u4f4e\u6e38\u620f\u7248\u53f7\u9650\u5236\uff0c\u592a\u7237\u7237\u751f\u524d\u5728\u7b49\u7684\u6e38\u620f\u7ec8\u4e8e\u53d1\u552e\u4e86\u3002",
-        "exclude": "EVT?[11501]",
+        "effect": {
+            "SPR": 1
+        },
+        "event": "\u4f60\u611f\u89c9\u4e16\u754c\u65e5\u65b0\u6708\u5f02\uff0c\u5bf9\u672a\u6765\u65e0\u9650\u53ef\u80fd\u7684\u90a3\u4efd\u597d\u5947\u652f\u6301\u7740\u4f60\u7ee7\u7eed\u6d3b\u4e0b\u53bb\u3002",
+        "exclude": "EVT?[11500,11501]",
         "id": 11501,
-        "include": "(EVT?[10010])&(MNY>4)"
+        "include": "SPR<4"
     },
     "11502": {
-        "event": "\u4e3a\u9632\u8303\u661f\u9645\u5165\u4fb5\u548c\u6838\u4e8b\u6545\u5e26\u6765\u7684\u53d8\u5f02\u751f\u7269\uff0c\u51e0\u5927\u56fd\u7275\u5934\u6210\u7acb\u5730\u7403\u548c\u5e73\u8054\u5408\u7ec4\u7ec7\u3002",
+        "event": "\u5c71\u4e1c\u7701\u5ba3\u5e03\u672c\u7701\u7537\u6027\u5e73\u5747\u8eab\u9ad8\u8fbe\u52301\u7c738\u3002\r\n\u5404\u5927\u793e\u4ea4\u5e73\u53f0\u4e0a\u6240\u5728\u5730\u6807\u6ce8\u4e3a\u5c71\u4e1c\u7701\u7684\u7537\u6027\u8d26\u6237\u6570\u91cf\u6fc0\u589e\u3002",
         "exclude": "EVT?[11502]",
         "id": 11502,
         "include": "EVT?[10010]"
     },
     "20007": {
         "NoRandom": 1,
         "event": "\u4f60\u559c\u6b22\u770b\u753b\u9762\u4eba\u8bbe\u597d\u770b\u7684\u52a8\u6f2b\u3002",
@@ -11012,14 +11386,15 @@
     },
     "20037": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u8f7b\u677e\u6253\u4e0a\u4e86\u738b\u8005\u3002",
+        "grade": 1,
         "id": 20037
     },
     "20038": {
         "NoRandom": 1,
         "event": "\u4f60\u6253\u4e0a\u4e86\u9ec4\u91d1\u6bb5\u4f4d\u3002",
         "id": 20038
     },
@@ -11041,14 +11416,15 @@
     "20054": {
         "effect": {
             "CHR": 1,
             "SPR": 1
         },
         "event": "\u4f60\u559c\u6b22\u4e0a\u4e86\u5973\u88c5\u3002",
         "exclude": "EVT?[20054]",
+        "grade": 1,
         "id": 20054,
         "include": "EVT?[20053]"
     },
     "20055": {
         "branch": [
             "MNY<6:20056"
         ],
@@ -11080,22 +11456,24 @@
     },
     "20091": {
         "NoRandom": 1,
         "effect": {
             "CHR": 5
         },
         "event": "\u4f60\u53d1\u660e\u4e86\u989c\u503c\u63d0\u5347\u673a\uff0c\u5927\u5e45\u63d0\u9ad8\u4e86\u989c\u503c\u3002",
+        "grade": 2,
         "id": 20091
     },
     "20092": {
         "NoRandom": 1,
         "effect": {
             "MNY": 2
         },
         "event": "\u4f60\u53d1\u660e\u4e86\u8bb8\u591a\u6709\u7528\u7684\u5c0f\u4e1c\u897f\uff0c\u5356\u4e86\u4e0d\u5c11\u94b1\u3002",
+        "grade": 1,
         "id": 20092
     },
     "20186": {
         "NoRandom": 1,
         "event": "\u4f60\u7684\u6027\u683c\u4e5f\u5f88\u53db\u9006\uff0c\u548c\u4ed6\u4eec\u4e00\u89c1\u5982\u6545\u3002",
         "id": 20186
     },
@@ -11131,38 +11509,41 @@
     },
     "20323": {
         "effect": {
             "STR": 10
         },
         "event": "\u7956\u4f20\u7684\u5c0f\u76d2\u5b50\u4e2d\u6563\u51fa\u4e86\u5947\u602a\u7684\u6c14\u4f53\u3002",
         "exclude": "EVT?[20323]",
+        "grade": 2,
         "id": 20323,
         "include": "TLT?[1048]",
         "postEvent": "\u4f60\u611f\u89c9\u81ea\u5df1\u4f53\u8d28\u63d0\u5347\u4e86\u3002"
     },
     "20332": {
         "branch": [
             "STR<88:10000"
         ],
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u906d\u5230\u4e86\u4e00\u4e2a\u6076\u5815\u7684\u9b54\u6cd5\u5c11\u5973\uff0c\u5e76\u5c55\u5f00\u6218\u6597\u3002",
         "exclude": "EVT?[20332]",
+        "grade": 1,
         "id": 20332,
         "include": "TLT?[1048]",
         "postEvent": "\u4f60\u6218\u80dc\u4e86\u5979\u3002"
     },
     "20333": {
         "effect": {
             "INT": 10,
             "STR": 100
         },
         "event": "\u4f60\u610f\u5916\u5f97\u5230\u4e86\u4e00\u4e2a\u5143\u5a74\u4fee\u58eb\u7684\u4f20\u627f\u3002",
         "exclude": "EVT?[20333]",
+        "grade": 2,
         "id": 20333,
         "include": "(INT>9)&(TLT?[1048])"
     },
     "20334": {
         "branch": [
             "STR>20:20335"
         ],
@@ -11171,14 +11552,15 @@
         "id": 20334,
         "include": "TLT?[1048]",
         "postEvent": "\u6ca1\u6709\u6210\u529f\u3002"
     },
     "20335": {
         "NoRandom": 1,
         "event": "\u4f60\u901a\u8fc7\u5927\u6bd4\uff0c\u6210\u4e3a\u4e86\u5916\u95e8\u5f1f\u5b50\u3002",
+        "grade": 1,
         "id": 20335
     },
     "20336": {
         "branch": [
             "(STR>30)&(INT>7):20337",
             "(STR<25)&(INT<5):10000"
         ],
@@ -11191,14 +11573,15 @@
     "20337": {
         "NoRandom": 1,
         "effect": {
             "MNY": 2,
             "STR": 20
         },
         "event": "\u4f60\u987a\u5229\u5b8c\u6210\u4efb\u52a1\uff0c\u83b7\u5f97\u5956\u52b1\u3002",
+        "grade": 1,
         "id": 20337
     },
     "20338": {
         "effect": {
             "CHR": 5
         },
         "event": "\u4f60\u670d\u7528\u4e86\u5b97\u95e8\u53d1\u653e\u7684\u517b\u989c\u4e39\u3002\u989c\u503c\u63d0\u5347\u3002",
@@ -11231,27 +11614,28 @@
     },
     "20342": {
         "branch": [
             "STR>119:20343",
             "STR<120:10000"
         ],
         "event": "\u4f60\u627e\u5230\u4e86\u90a3\u4e2a\u6740\u5bb3\u5c0f\u5e08\u59b9\u7684\u4fee\u58eb\uff0c\u5e76\u4e0e\u4e4b\u6218\u6597\u3002",
-        "exclude": "EVT?[20342]",
+        "exclude": "EVT?[20342,20343]",
         "id": 20342,
         "include": "EVT?[20341]"
     },
     "20343": {
         "NoRandom": 1,
         "branch": [
             "TLT?[1129]:20349"
         ],
         "effect": {
             "STR": 5
         },
         "event": "\u4f60\u65a9\u6740\u4e86\u7b51\u57fa\u4fee\u58eb\uff0c\u83b7\u5f97\u5c11\u91cf\u5b9d\u7269\uff0c\u548c\u5c0f\u5e08\u59b9\u7684\u4e00\u679a\u6212\u6307\u3002",
+        "grade": 1,
         "id": 20343
     },
     "20344": {
         "branch": [
             "STR>30:20345"
         ],
         "event": "\u4f60\u53c2\u52a0\u5b97\u95e8\u5185\u90e8\u5927\u6bd4\u3002",
@@ -11264,14 +11648,15 @@
         "NoRandom": 1,
         "effect": {
             "MNY": 1,
             "SPR": 1,
             "STR": 5
         },
         "event": "\u4f60\u664b\u5347\u6210\u4e86\u5185\u95e8\u5f1f\u5b50\u3002",
+        "grade": 1,
         "id": 20345
     },
     "20346": {
         "branch": [
             "STR>150:20348",
             "STR>100:20347"
         ],
@@ -11285,42 +11670,109 @@
         "NoRandom": 1,
         "effect": {
             "MNY": 1,
             "SPR": 1,
             "STR": 10
         },
         "event": "\u4f60\u664b\u5347\u6210\u4e86\u6838\u5fc3\u5f1f\u5b50\u3002",
+        "grade": 1,
         "id": 20347
     },
     "20348": {
         "NoRandom": 1,
         "effect": {
             "MNY": 2,
             "SPR": 1,
             "STR": 20
         },
         "event": "\u4f60\u88ab\u5b97\u95e8\u957f\u8001\u6536\u4e3a\u4eb2\u4f20\u5f1f\u5b50\u3002",
+        "grade": 2,
         "id": 20348
     },
     "20349": {
         "NoRandom": 1,
         "effect": {
             "STR": -5
         },
         "event": "\u4f60\u60b2\u4f24\u653b\u5fc3\u8d70\u706b\u5165\u9b54\uff0c\u4eba\u683c\u4e5f\u56e0\u6b64\u5408\u5e76\u4e86\u3002",
+        "grade": 2,
         "id": 20349
     },
+    "20361": {
+        "NoRandom": 1,
+        "event": "\u622a\u6740\u8005\u53d1\u73b0\u4f60\u6bd4\u4ed6\u8fd8\u7a77\uff0c\u76f4\u547c\u6666\u6c14\uff0c\u653e\u4e86\u4f60\u4e00\u9a6c\u3002",
+        "id": 20361
+    },
+    "20362": {
+        "NoRandom": 1,
+        "effect": {
+            "STR": 50
+        },
+        "event": "\u622a\u6740\u8005\u88ab\u4f60\u53cd\u6740\u3002\u5f97\u5230\u5927\u91cf\u5b9d\u7269\uff0c\u4f53\u8d28\u63d0\u5347\u3002",
+        "grade": 1,
+        "id": 20362
+    },
+    "20363": {
+        "NoRandom": 1,
+        "branch": [
+            "STR>500:20362",
+            "EVT?[20364]:20361",
+            "TLT?[1048]:10000"
+        ],
+        "event": "\u4f60\u5728\u62cd\u5356\u884c\u5916\u906d\u5230\u4e86\u622a\u6740\u3002",
+        "id": 20363
+    },
+    "20364": {
+        "NoRandom": 1,
+        "branch": [
+            "CHR<3:20363"
+        ],
+        "effect": {
+            "SPR": -1
+        },
+        "event": "\u4f60\u592a\u7a77\u4e86\uff0c\u4ec0\u4e48\u4e5f\u6ca1\u62cd\u5230\u3002",
+        "id": 20364
+    },
+    "20365": {
+        "NoRandom": 1,
+        "branch": [
+            "CHR<3:20363"
+        ],
+        "effect": {
+            "INT": 10,
+            "MNY": -5,
+            "STR": 10
+        },
+        "event": "\u4f60\u62cd\u5230\u4e86\u4e00\u7bc7\u529f\u6cd5\u3002\u4f53\u8d28\u548c\u667a\u529b\u63d0\u5347\u3002",
+        "grade": 1,
+        "id": 20365
+    },
+    "20366": {
+        "NoRandom": 1,
+        "branch": [
+            "CHR<3:20363"
+        ],
+        "effect": {
+            "MNY": -1,
+            "SPR": 5,
+            "STR": 100
+        },
+        "event": "\u5176\u4ed6\u4eba\u4e0d\u8ba4\u8bc6\u4e0a\u53e4\u5947\u7269\uff0c\u88ab\u4f60\u4f4e\u4ef7\u62cd\u5230\u3002\r\n\u4f53\u8d28\u548c\u5feb\u4e50\u5927\u5e45\u63d0\u5347\u3002",
+        "grade": 2,
+        "id": 20366
+    },
     "20367": {
         "effect": {
             "INT": 100,
             "SPR": 10,
             "STR": 1000
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u4e00\u6761\u5929\u9053\uff01",
         "exclude": "EVT?[20367]",
+        "grade": 3,
         "id": 20367,
         "include": "(EVT?[10365])&((TLT?[1033,1122])|(EVT?[10715]))",
         "postEvent": "\u5c5e\u6027\u5927\u5e45\u63d0\u5347\u3002"
     },
     "20369": {
         "branch": [
             "STR>0:10000"
@@ -11331,80 +11783,88 @@
     },
     "20380": {
         "effect": {
             "STR": 50
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u5251\u9053\u3002",
         "exclude": "EVT?[20380]",
+        "grade": 2,
         "id": 20380,
         "include": "(EVT?[10365])&(INT>100)",
         "postEvent": "\u4f53\u8d28\u63d0\u5347\u3002"
     },
     "20381": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u96f7\u7535\u5927\u9053\u3002",
         "exclude": "EVT?[20381]",
+        "grade": 2,
         "id": 20381,
         "include": "(EVT?[10365])&(INT>100)",
         "postEvent": "\u53ef\u4ee5\u62b5\u6d88\u7b2c\u4e5d\u91cd\u96f7\u52ab\u3002"
     },
     "20382": {
         "effect": {
             "INT": 20,
             "SPR": 2,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u4eba\u9053\u3002",
         "exclude": "EVT?[20382]",
+        "grade": 2,
         "id": 20382,
         "include": "(EVT?[10365])&(INT>100)",
         "postEvent": "\u4f60\u609f\u900f\u4e86\u4f1f\u5927\u7684\u9a6c\u514b\u601d\u4e3b\u4e49\u3002"
     },
     "20383": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u98ce\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[20383]",
+        "grade": 2,
         "id": 20383,
         "include": "(EVT?[10365])&(INT>100)",
         "postEvent": "\u4f60\u53ef\u4ee5\u4f7f\u7528\u98ce\u5143\u7d20\u529b\u98de\u884c\u4e86\u3002\u4f46\u4f60\u672c\u6765\u5c31\u53ef\u4ee5\u98de\u3002"
     },
     "20384": {
         "event": "\u4f60\u609f\u51fa\u4e86\u7a7a\u624b\u9053\u3002",
         "exclude": "EVT?[20384]",
+        "grade": 2,
         "id": 20384,
         "include": "(EVT?[10365])&(INT>100)",
         "postEvent": "\u597d\u50cf\u6ca1\u4ec0\u4e48\u7528\u3002"
     },
     "20390": {
         "effect": {
             "AGE": -100
         },
         "event": "\u4f60\u5728\u7ef4\u6301\u81ea\u8eab\u60c5\u51b5\u4e0d\u53d8\u7684\u524d\u63d0\u4e0b\uff0c\u8fd0\u7528\u65f6\u95f4\u5927\u9053\u56de\u5230\u4e86100\u5e74\u524d\u3002",
         "exclude": "EVT?[20390]",
+        "grade": 3,
         "id": 20390,
         "include": "EVT?[10387]"
     },
     "20408": {
         "event": "\u4f60\u89c9\u9192\u524d\u4e16\u8bb0\u5fc6\uff0c\u91cd\u65b0\u8e0f\u4e0a\u4fee\u884c\u8def\u3002",
+        "grade": 3,
         "id": 20408,
         "include": "(TLT?[1134])&(EVT?[10391])"
     },
     "20409": {
         "NoRandom": 1,
         "effect": {
             "AGE": -500,
             "STR": -1000
         },
         "event": "\u4f60\u6ca1\u6709\u625b\u8fc7\u8fd9\u4e00\u52ab\u3002\u7075\u9b42\u788e\u7247\u4fa5\u5e78\u9003\u51fa\uff0c\u4f60\u8f6c\u4e16\u91cd\u751f\u4e86\u3002",
+        "grade": 3,
         "id": 20409,
         "postEvent": "\u8eab\u4f53\u53d8\u5f31\uff0c\u8bb0\u5fc6\u5c3d\u5931\uff0c\u4f46\u4f60\u7684\u9053\u4e4b\u5883\u754c\u8fd8\u5728\u3002"
     },
     "20410": {
         "NoRandom": 1,
         "effect": {
             "SPR": 2
@@ -11469,15 +11929,15 @@
     "20422": {
         "NoRandom": 1,
         "event": "\u76f4\u89c9\u544a\u8bc9\u4f60\u4e8b\u60c5\u6ca1\u8fd9\u4e48\u7b80\u5355\u3002",
         "id": 20422
     },
     "20423": {
         "NoRandom": 1,
-        "event": "\u6709\u77e5\u60c5\u4eba\u544a\u8bc9\u4f60\u4e0d\u662f\u4ea4\u901a\u4e8b\u6545\uff0c\u597d\u50cf\u662f\u4e00\u4e2a\u5728\u5929\u4e0a\u98de\u7684\u4eba\u2026\u2026",
+        "event": "\u6709\u77e5\u60c5\u4eba\u544a\u8bc9\u4f60\u4e0d\u662f\u4ea4\u901a\u4e8b\u6545\uff0c\u597d\u50cf\u662f\u4e00\u4e2a\u5728\u5929\u4e0a\u98de\u7684\u4eba\u9020\u6210\u7684\u2026\u2026",
         "id": 20423
     },
     "20425": {
         "NoRandom": 1,
         "event": "\u4f60\u610f\u8bc6\u5230\u8fd9\u573a\u5730\u9707\u5e76\u4e0d\u5bfb\u5e38\u2026\u2026",
         "id": 20425
     },
@@ -11569,27 +12029,30 @@
         "NoRandom": 1,
         "event": "\u4f60\u7a81\u7136\u611f\u89c9\u4eba\u751f\u65e0\u61be\u4e86\u3002",
         "id": 20460
     },
     "20461": {
         "NoRandom": 1,
         "event": "\u4f60\u8d2d\u4e70\u4e86\u4e00\u672c\u300a\u4ed9\u8109\u56fe\u5f55\u300b\u3002",
+        "grade": 2,
         "id": 20461
     },
     "20462": {
         "NoRandom": 1,
         "event": "\u4f60\u8d2d\u4e70\u4e86\u4e00\u672c\u300a\u5143\u795e\u4e0d\u706d\u300b\u3002",
+        "grade": 2,
         "id": 20462
     },
     "20529": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u62ff\u4e86\u7b2c\u4e00\u540d\u3002",
+        "grade": 1,
         "id": 20529
     },
     "20534": {
         "NoRandom": 1,
         "branch": [
             "TLT?[1108]:10000"
         ],
@@ -11603,22 +12066,24 @@
     },
     "20558": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u8fc7\u4eba\u7684\u989c\u503c\u548c\u821e\u6280\u8ba9\u4f60\u6210\u4e3a\u4e07\u4f17\u77a9\u76ee\u3002",
+        "grade": 1,
         "id": 20558
     },
     "20565": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u7684\u521b\u4e1a\u6700\u6210\u529f\u3002",
+        "grade": 1,
         "id": 20565
     },
     "20567": {
         "branch": [
             "TLT?[1135]:40062",
             "EVT?[10011]:10000"
         ],
@@ -11659,26 +12124,28 @@
         "NoRandom": 1,
         "event": "\u867d\u7136\u6bd4\u5e73\u65f6\u505a\u7684\u96be\uff0c\u4f46\u8fd8\u662f\u90fd\u505a\u51fa\u6765\u4e86\u3002",
         "id": 20575
     },
     "20576": {
         "NoRandom": 1,
         "event": "\u4f60\u8eab\u624b\u654f\u6377\uff0c\u4fa5\u5e78\u9003\u5f97\u4e00\u547d\u3002",
+        "grade": 2,
         "id": 20576
     },
     "20577": {
         "NoRandom": 1,
         "branch": [
             "EVT?[10505]:10000"
         ],
         "event": "\u4f60\u4e0a\u53bb\u6311\u8845\u4ed6\u4eec\uff0c\u88ab\u4e00\u7fa4\u4eba\u6301\u68b0\u56f4\u6bb4\u3002",
         "id": 20577
     },
     "20580": {
         "event": "\u4f60\u8003\u4e0a\u4e86\u54c8\u4f5b\u5927\u5b66\u3002",
+        "grade": 2,
         "id": 20580,
         "include": "(TLT?[1073])&(INT>5)&(EVT?[10011])"
     },
     "20596": {
         "NoRandom": 1,
         "event": "\u5f88\u5feb\u4f60\u4eec\u4fbf\u786e\u5b9a\u4e86\u5173\u7cfb\u3002",
         "id": 20596
@@ -11704,16 +12171,17 @@
     },
     "20759": {
         "NoRandom": 1,
         "event": "\u88ab\u5929\u4ef7\u6d77\u9c9c\u5751\u4e86\u4e0d\u5c11\u94b1\u3002",
         "id": 20759
     },
     "20770": {
-        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u76d7\u7248\u6a2a\u884c\uff0c\u5e0c\u671b\u5927\u5bb6\u591a\u5e2e\u5fd9\u4e3e\u62a5\u76d7\u7248",
+        "event": "\u3010\u7edd\u5bc6\u6d88\u606f\u3011\u66f4\u65b0\u540e\u7b2c\u4e00\u6b21\u53ef\u80fd\u52a0\u8f7d\u4f1a\u6bd4\u8f83\u6162\u3002",
         "exclude": "EVT?[20770]",
+        "grade": 2,
         "id": 20770,
         "include": "TLT?[1112]"
     },
     "20917": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
@@ -11723,22 +12191,24 @@
     },
     "21011": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u88ab\u8bc4\u4e3a\u73ed\u82b1\u3002",
+        "grade": 1,
         "id": 21011
     },
     "21012": {
         "NoRandom": 1,
         "effect": {
             "SPR": 1
         },
         "event": "\u4f60\u88ab\u8bc4\u4e3a\u6821\u8349\u3002",
+        "grade": 1,
         "id": 21012
     },
     "21015": {
         "event": "\u5b66\u6821\u98df\u5802\u63a8\u51fa\u4e86\u65b0\u83dc\uff1a\u751f\u714e\u5305\u7092\u9505\u8d34.",
         "exclude": "EVT?[10944,11015,11016,11017,11018,11019,11020,21015]",
         "id": 21015,
         "include": "EVT?[10940]"
@@ -11782,119 +12252,146 @@
     },
     "21296": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21297"
         ],
         "event": "\u7a81\u7136\uff0c\u65f6\u95f4\u505c\u6b62\u4e86\u3002",
+        "grade": 3,
         "id": 21296
     },
     "21297": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21298"
         ],
         "event": "\u4f60\u5411\u4e0b\u65b9\u8dd1\uff0c\u60f3\u8981\u9003\u79bb\u8fd9\u4e2a\u4e16\u754c\u3002",
+        "grade": 3,
         "id": 21297
     },
     "21298": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21299"
         ],
         "event": "\u8dd1",
+        "grade": 3,
         "id": 21298
     },
     "21299": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21300"
         ],
         "event": "         \u8dd1",
+        "grade": 3,
         "id": 21299
     },
     "21300": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21301"
         ],
         "event": "                    \u8dd1",
+        "grade": 3,
         "id": 21300
     },
     "21301": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21302"
         ],
         "event": "            \u8dd1",
+        "grade": 3,
         "id": 21301
     },
     "21302": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21303"
         ],
         "event": "   \u8dd1",
+        "grade": 3,
         "id": 21302
     },
     "21303": {
         "NoRandom": 1,
         "branch": [
             "INT>10:21304"
         ],
         "event": "             \u8dd1",
+        "grade": 3,
         "id": 21303
     },
     "21304": {
         "NoRandom": 1,
         "event": "                        \u8dd1 ",
+        "grade": 3,
         "id": 21304
     },
     "21305": {
         "branch": [
             "INT>10:21306"
         ],
         "event": "\u4f60\u7684\u884c\u4e3a\u7ec8\u4e8e\u89e6\u53d1\u4e86\u8fd9\u4e2a\u6ee1\u662fBUG\u7684\u865a\u62df\u4e16\u754c\u7684\u9632\u536b\u673a\u5236\u3002",
         "exclude": "EVT?[21305]",
+        "grade": 3,
         "id": 21305,
         "include": "EVT?[21304]"
     },
     "21306": {
         "NoRandom": 1,
         "branch": [
             "CHR>5:21307",
             "CHR<6:21308"
         ],
         "event": "\u4e16\u754c\u5f00\u59cb\u5bf9\u4f60\u505a\u51fa\u5ba1\u5224\u3002",
+        "grade": 3,
         "id": 21306
     },
     "21307": {
         "NoRandom": 1,
         "event": "\u4f60\u76f8\u8c8c\u8fd8\u53ef\u4ee5\uff0c\u4e16\u754c\u51b3\u5b9a\u62b9\u53bb\u4f60\u8fd9\u6bb5\u8bb0\u5fc6\u8ba9\u4f60\u7ee7\u7eed\u751f\u6d3b\u3002",
+        "grade": 3,
         "id": 21307
     },
     "21308": {
         "NoRandom": 1,
         "branch": [
             "CHR<6:10000"
         ],
         "event": "\u4f60\u76f8\u8c8c\u4e0d\u884c\uff0c\u4e16\u754c\u51b3\u5b9a\u6d88\u706d\u4f60\u3002",
+        "grade": 3,
         "id": 21308
     },
     "21315": {
         "NoRandom": 1,
         "effect": {
             "MNY": 3
         },
         "event": "\u4f60\u6309\u4e86\u3002\u4f60\u83b7\u5f97\u4e86\u5927\u91cf\u91d1\u94b1\u3002",
+        "grade": 2,
         "id": 21315
     },
+    "21326": {
+        "event": "\u79d1\u5b66\u5bb6\u8ba4\u4e3a\u5f57\u661f\u7531\u5927\u51b0\u6784\u6210\u3002",
+        "exclude": "EVT?[21326]",
+        "id": 21326,
+        "include": "EVT?[10010]"
+    },
+    "21327": {
+        "event": "\u4e00\u9897\u56de\u5f52\u5468\u671f996\u5e74\u7684\u5f57\u661f\u63a5\u8fd1\u5730\u7403\u3002",
+        "exclude": "EVT?[21327]",
+        "id": 21327,
+        "include": "EVT?[21315]"
+    },
     "21457": {
         "NoRandom": 1,
         "event": "\u4f60\u610f\u5fd7\u529b\u4e0d\u8db3\uff0c\u88ab\u8bf1\u5bfc\u6076\u5815\u4e86\u3002",
+        "grade": 2,
         "id": 21457,
         "postEvent": "\u4f60\u53d8\u6210\u4e86\u89e6\u624b\u9b54\u5973\uff0c\u4ece\u6b64\u4e3a\u5973\u738b\u6548\u529b\u3002"
     },
     "30001": {
         "branch": [
             "STR<3:10000",
             "STR>2:30002"
@@ -11905,26 +12402,28 @@
     },
     "30002": {
         "NoRandom": 1,
         "effect": {
             "LIF": -1
         },
         "event": "\u4f60\u7a7f\u8d8a\u5230\u4e86\u5f02\u4e16\u754c\u3002",
+        "grade": 2,
         "id": 30002,
         "postEvent": "\u4f60\u5728\u539f\u5148\u4e16\u754c\u7684\u4eba\u751f\u7ed3\u675f\u4e86\u3002"
     },
     "40001": {
         "effect": {
             "CHR": 5,
             "INT": 5,
             "SPR": 3,
             "STR": 5
         },
         "event": "\u4f60\u6253\u5f00\u5c0f\u76d2\u5b50\uff0c\u83b7\u5f97\u7ec3\u6c14\u6cd5\u95e8\uff0c\u4f46\u4f60\u53d1\u73b0\u4e5e\u4e10\u7ed9\u4f60\u7684\u300a\u4ed9\u8109\u56fe\u5f55\u300b\u66f4\u52a0\u9ad8\u660e\uff0c\u662f\u4f20\u8bf4\u4e2d\u7684\u592a\u53e4\u4fee\u884c\u6cd5\u95e8\u3002",
         "exclude": "EVT?[40001,40003]",
+        "grade": 3,
         "id": 40001,
         "include": "(TLT?[1048])&(EVT?[20461])",
         "postEvent": "\u4f60\u4fee\u70bc\u592a\u53e4\u6cd5\u95e8\uff0c\u7a81\u7834\u5230\u51c0\u606f\u524d\u671f\u3002\u5bff\u5143\u63d0\u5347\u5230500\u5e74\u3002"
     },
     "40002": {
         "effect": {
             "STR": 5
@@ -11936,41 +12435,45 @@
     },
     "40003": {
         "effect": {
             "STR": 10
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51c0\u606f\u4e2d\u671f\u3002",
         "exclude": "EVT?[40003]",
+        "grade": 1,
         "id": 40003,
         "include": "(EVT?[40001,40061])&(STR>100)"
     },
     "40004": {
         "effect": {
             "STR": 10
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51c0\u606f\u540e\u671f\u3002",
         "exclude": "EVT?[40004]",
+        "grade": 1,
         "id": 40004,
         "include": "(EVT?[40003])&(STR>200)"
     },
     "40005": {
         "effect": {
             "STR": 10
         },
         "event": "\u4f60\u7a81\u7834\u5230\u51c0\u606f\u5dc5\u5cf0\u3002",
         "exclude": "EVT?[40005]",
+        "grade": 1,
         "id": 40005,
         "include": "(EVT?[40004])&(STR>300)"
     },
     "40006": {
         "effect": {
             "STR": 20
         },
         "event": "\u4f60\u95ef\u5165\u4e00\u5904\u79d8\u5883\uff0c\u593a\u5f97\u5927\u91cf\u8d44\u6e90\u3002",
         "exclude": "EVT?[40010]",
+        "grade": 1,
         "id": 40006,
         "include": "EVT?[40001,40003,40061]"
     },
     "40007": {
         "effect": {
             "CHR": 1
         },
@@ -11992,23 +12495,25 @@
     "40009": {
         "effect": {
             "INT": 2,
             "STR": 10
         },
         "event": "\u4f60\u65a9\u6740\u4e86\u4e00\u4e2a\u7b51\u57fa\u4fee\u58eb\uff0c\u5f97\u5230\u5b9d\u7269\u3002",
         "exclude": "EVT?[40010]",
+        "grade": 1,
         "id": 40009,
         "include": "(EVT?[40001,40061])&(STR>100)"
     },
     "40010": {
         "effect": {
             "STR": 20
         },
         "event": "\u4f60\u8fdb\u884c\u65e0\u57a2\u7b51\u57fa\uff0c\u5b9e\u529b\u8fdc\u80dc\u4e8e\u5bfb\u5e38\u7b51\u57fa\u3002",
         "exclude": "EVT?[40010]",
+        "grade": 2,
         "id": 40010,
         "include": "(EVT?[40005])&(STR>500)",
         "postEvent": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u524d\u671f\u3002"
     },
     "40011": {
         "effect": {
             "STR": 10
@@ -12020,118 +12525,130 @@
     },
     "40012": {
         "effect": {
             "STR": 30
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u4e2d\u671f\u3002",
         "exclude": "EVT?[40012]",
+        "grade": 1,
         "id": 40012,
         "include": "(EVT?[40010])&(STR>800)"
     },
     "40013": {
         "effect": {
             "STR": 30
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u540e\u671f\u3002",
         "exclude": "EVT?[40013]",
+        "grade": 1,
         "id": 40013,
         "include": "(EVT?[40012])&(STR>1200)"
     },
     "40014": {
         "effect": {
             "STR": 30
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7b51\u57fa\u5dc5\u5cf0\u3002",
         "exclude": "EVT?[40014]",
+        "grade": 1,
         "id": 40014,
         "include": "(EVT?[40013])&(STR>1600)"
     },
     "40015": {
         "effect": {
             "INT": 10,
             "STR": 100
         },
         "event": "\u4f60\u53c2\u52a0\u7b51\u57fa\u5929\u624d\u6218\uff0c\u593a\u5f97\u7b2c\u4e00\u3002",
         "exclude": "EVT?[40015,40023]",
+        "grade": 2,
         "id": 40015,
         "include": "EVT?[40010]",
         "postEvent": "\u5f97\u5230\u5927\u91cf\u5956\u52b1\u3002\u5e76\u88ab\u4e00\u4f4d\u6e21\u52ab\u5927\u80fd\u6536\u4e3a\u4eb2\u4f20\u3002"
     },
     "40016": {
         "event": "\u4f60\u89c9\u9192\u4e00\u822c\u5143\u5a74\u671f\u624d\u6709\u7684\u795e\u8bc6\u3002",
         "exclude": "EVT?[40016,40023]",
+        "grade": 2,
         "id": 40016,
         "include": "EVT?[40010]"
     },
     "40017": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u706b\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[40017]",
+        "grade": 2,
         "id": 40017,
         "include": "EVT?[40010]"
     },
     "40018": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u91d1\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[40018]",
+        "grade": 2,
         "id": 40018,
         "include": "EVT?[40010]"
     },
     "40019": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u6728\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[40019]",
+        "grade": 2,
         "id": 40019,
         "include": "EVT?[40010]"
     },
     "40020": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u6c34\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[40020]",
+        "grade": 2,
         "id": 40020,
         "include": "EVT?[40010]"
     },
     "40021": {
         "effect": {
             "INT": 20,
             "STR": 20
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u571f\u4e4b\u5927\u9053\u3002",
         "exclude": "EVT?[40021]",
+        "grade": 2,
         "id": 40021,
         "include": "EVT?[40010]"
     },
     "40022": {
         "effect": {
             "STR": 20
         },
         "event": "\u5b8c\u7f8e\u6dec\u4f53\uff0c\u4f53\u8d28\u5927\u5e45\u63d0\u5347\u3002",
         "exclude": "EVT?[40023]",
+        "grade": 2,
         "id": 40022,
         "include": "EVT?[40010]"
     },
     "40023": {
         "effect": {
             "INT": 30,
             "STR": 50
         },
         "event": "\u4f60\u4f53\u5185\u7075\u606f\u6c47\u805a\u6210\u4e39\u6d77\uff0c\u53c8\u590d\u5f52\u6d41\u8f6c\u5468\u8eab\u7ecf\u8109\uff0c\u5f62\u6210\u7075\u8109\u3002",
         "exclude": "EVT?[40023]",
+        "grade": 2,
         "id": 40023,
         "include": "(EVT?[40014])&(STR>2000)",
         "postEvent": "\u4f60\u7a81\u7834\u5230\u7075\u8109\u524d\u671f\u3002"
     },
     "40024": {
         "effect": {
             "INT": 10,
@@ -12154,76 +12671,83 @@
     "40026": {
         "effect": {
             "INT": 30,
             "STR": 50
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7075\u8109\u4e2d\u671f\u3002",
         "exclude": "EVT?[40026]",
+        "grade": 1,
         "id": 40026,
         "include": "(EVT?[40023])&(INT>500)",
         "postEvent": "\u4e39\u6d77\u4e2d\u51dd\u805a\u51fa\u4e24\u9897\u91d1\u4e39\u3002"
     },
     "40027": {
         "effect": {
             "INT": 30,
             "STR": 50
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7075\u8109\u540e\u671f\u3002",
         "exclude": "EVT?[40027]",
+        "grade": 1,
         "id": 40027,
         "include": "(EVT?[40023])&(INT>1000)",
         "postEvent": "\u4e39\u6d77\u4e2d\u51dd\u805a\u51fa\u56db\u9897\u91d1\u4e39\u3002"
     },
     "40028": {
         "effect": {
             "INT": 30,
             "STR": 100
         },
         "event": "\u4f60\u7a81\u7834\u5230\u7075\u8109\u5dc5\u5cf0\u3002",
         "exclude": "EVT?[40028]",
+        "grade": 1,
         "id": 40028,
         "include": "(EVT?[40023])&(INT>2000)",
         "postEvent": "\u4e39\u6d77\u4e2d\u51dd\u805a\u51fa\u516b\u9897\u91d1\u4e39\u3002"
     },
     "40029": {
         "effect": {
             "INT": 50,
             "STR": 200
         },
         "event": "\u4f60\u65a9\u6740\u4e86\u4e00\u4f4d\u6e21\u52ab\u671f\u4fee\u58eb\u3002\u83b7\u5f97\u5927\u91cf\u8d44\u6e90\u3002",
         "exclude": "EVT?[40039]",
+        "grade": 2,
         "id": 40029,
         "include": "(EVT?[40023])&(STR>2000)"
     },
     "40030": {
         "effect": {
             "INT": 20,
             "STR": 100
         },
         "event": "\u4f60\u65a9\u6740\u4e00\u4f4d\u5143\u5a74\u4fee\u58eb\uff0c\u83b7\u5f97\u5927\u91cf\u8d44\u6e90\u3002",
         "exclude": "EVT?[40039]",
+        "grade": 2,
         "id": 40030,
         "include": "(EVT?[40023])&(STR>1000)"
     },
     "40031": {
         "effect": {
             "INT": 50,
             "STR": 500
         },
         "event": "\u4f60\u6467\u6bc1\u4e86\u4e00\u4e2a\u9b54\u9053\u5b97\u95e8\uff0c\u65a9\u6740\u6570\u4f4d\u707e\u52ab\u5883\u9b54\u4fee\u3002",
         "exclude": "EVT?[40039]",
+        "grade": 2,
         "id": 40031,
         "include": "(EVT?[40023])&(STR>2000)"
     },
     "40032": {
         "effect": {
             "INT": 100
         },
         "event": "\u4f60\u9047\u5230\u4e00\u4f4d\u4f2a\u4ed9\u5883\u7684\u9b42\u4fee\uff0c\u4ed6\u60f3\u593a\u820d\u4f60\uff0c\u88ab\u4f60\u53cd\u6740\u3002",
         "exclude": "EVT?[40032,40039]",
+        "grade": 2,
         "id": 40032,
         "include": "(EVT?[40023])&(INT>1000)"
     },
     "40033": {
         "branch": [
             "STR>1:10000"
         ],
@@ -12235,54 +12759,59 @@
     "40034": {
         "effect": {
             "INT": 50,
             "STR": 50
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u7a7a\u95f4\u5927\u9053\u3002",
         "exclude": "EVT?[40034]",
+        "grade": 3,
         "id": 40034,
         "include": "EVT?[40010]"
     },
     "40035": {
         "effect": {
             "INT": 50,
             "STR": 50
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u65f6\u95f4\u5927\u9053\u3002",
         "exclude": "EVT?[40035]",
+        "grade": 3,
         "id": 40035,
         "include": "EVT?[40010]"
     },
     "40036": {
         "effect": {
             "INT": 100,
             "STR": 100
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u6df7\u6c8c\u5927\u9053\u3002",
         "exclude": "EVT?[40036]",
+        "grade": 3,
         "id": 40036,
         "include": "EVT?[40010]"
     },
     "40037": {
         "effect": {
             "INT": 75,
             "STR": 75
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u751f\u547d\u5927\u9053\u3002",
         "exclude": "EVT?[40037]",
+        "grade": 3,
         "id": 40037,
         "include": "EVT?[40010]"
     },
     "40038": {
         "effect": {
             "INT": 75,
             "STR": 75
         },
         "event": "\u4f60\u609f\u51fa\u4e86\u6bc1\u706d\u5927\u9053\u3002",
         "exclude": "EVT?[40038]",
+        "grade": 3,
         "id": 40038,
         "include": "EVT?[40010]"
     },
     "40039": {
         "branch": [
             "EVT?[40028]:40040"
         ],
@@ -12294,14 +12823,15 @@
         "exclude": "EVT?[40039]",
         "id": 40039,
         "include": "(EVT?[40028])&(EVT?[40036])"
     },
     "40040": {
         "NoRandom": 1,
         "event": "\u4f60\u6495\u88c2\u4e16\u754c\u4e4b\u58c1\uff0c\u8e0f\u788e\u865a\u7a7a\u800c\u53bb\u3002",
+        "grade": 3,
         "id": 40040
     },
     "40041": {
         "branch": [
             "STR>1:10000"
         ],
         "event": "\u5bff\u5143\u7ec8\u3002",
@@ -12339,157 +12869,174 @@
         "id": 40046,
         "include": "EVT?[40042]",
         "postEvent": "\u6ca1\u6709\u627e\u5230\u4ec0\u4e48\u6709\u7528\u7684\u4e1c\u897f\u3002"
     },
     "40047": {
         "event": "\u4f60\u95ef\u5165\u4e86\u4e00\u5904\u8fdc\u53e4\u6218\u573a\u9057\u8ff9\u3002",
         "exclude": "EVT?[40047,40051]",
+        "grade": 2,
         "id": 40047,
         "include": "EVT?[40042]",
         "postEvent": "\u4f60\u627e\u5230\u4e86\u4e00\u4e9b\u53e4\u7c4d\u3002\u4e0a\u9762\u63cf\u8ff0\u4e86\u53e4\u4ed9\u754c\u7834\u788e\u524d\u7684\u6837\u5b50\uff0c\u4f60\u53d1\u73b0\u90a3\u65f6\u7684\u4e3b\u6d41\u4fee\u884c\u6cd5\u95e8\u4e0d\u6b62\u300a\u4ed9\u8109\u56fe\u5f55\u300b\u4e00\u79cd\uff0c\u8fd8\u6709\u65e0\u9700\u6e21\u52ab\u7684\u300a\u65e0\u4e0a\u5999\u9053\u6587\u59cb\u771f\u7ecf\u300b\u3002"
     },
     "40048": {
         "event": "\u4f60\u95ef\u5165\u4e86\u4e00\u5904\u8fdc\u53e4\u6218\u573a\u9057\u8ff9\u3002",
         "exclude": "EVT?[40048,40051]",
+        "grade": 2,
         "id": 40048,
         "include": "EVT?[40047]",
         "postEvent": "\u4f60\u627e\u5230\u4e86\u4e00\u4e9b\u53e4\u7c4d\u3002\u4e0a\u9762\u63cf\u8ff0\u4e86\u300a\u65e0\u4e0a\u5999\u9053\u6587\u59cb\u771f\u7ecf\u300b\u7684\u5883\u754c\u5212\u5206\uff1a\u51e1\u4fd7-\u6e05\u51c0-\u5408\u4e00-\u65e0\u76f8-\u5165\u9053-\u7fbd\u5316\u3002\u5165\u9053\u4e4b\u540e\u609f\u51fa\u5168\u90e8\u672c\u6e90\u5927\u9053\u540e\u5373\u53ef\u76f4\u63a5\u98de\u5347\uff0c\u65e0\u9700\u6e21\u52ab\u3002"
     },
     "40049": {
         "event": "\u4f60\u95ef\u5165\u4e86\u4e00\u5904\u8fdc\u53e4\u6218\u573a\u9057\u8ff9\u3002",
         "exclude": "EVT?[40049,40051]",
+        "grade": 3,
         "id": 40049,
         "include": "EVT?[40048]",
         "postEvent": "\u5f97\u5230\u4e86\u300a\u65e0\u4e0a\u5999\u9053\u6587\u59cb\u771f\u7ecf\u300b\u4fee\u884c\u6cd5\u95e8\u3002\u4f60\u5f00\u59cb\u8f6c\u4fee\uff0c\u8e0f\u5165\u5165\u9053\u5883\u3002"
     },
     "40050": {
         "effect": {
             "LIF": -1
         },
         "event": "\u4f60\u609f\u900f\u5168\u90e8\u672c\u6e90\u5927\u9053\uff0c\u8e0f\u5165\u7fbd\u5316\u5883\uff0c\u98de\u5347\u4ed9\u754c\u3002",
+        "grade": 3,
         "id": 40050,
         "include": "(EVT?[40049])&(EVT?[40038])&(EVT?[40037])&(EVT?[40035])&(EVT?[40034])",
         "postEvent": "\u4f60\u4f5c\u4e3a\u201c\u4eba\u201d\u7684\u4e00\u751f\u7ed3\u675f\u4e86\u3002"
     },
     "40051": {
         "event": "\u4f60\u6765\u5230\u4e00\u4e2a\u7834\u788e\u7684\u661f\u7403\u4e0a\uff0c\u5f97\u5230\u4e00\u672c\u5f02\u754c\u4fee\u884c\u6cd5\u95e8\u300a\u661f\u5c18\u5e7b\u706d\u300b\u3002",
         "exclude": "EVT?[40051,40049]",
+        "grade": 3,
         "id": 40051,
         "include": "EVT?[40044]",
         "postEvent": "\u4f60\u5c1d\u8bd5\u7406\u89e3\u5f02\u754c\u6587\u5b57\u3002"
     },
     "40052": {
         "event": "\u6309\u300a\u661f\u5c18\u5e7b\u706d\u300b\u7684\u8bf4\u6cd5\uff0c\u90a3\u4e9b\u5f02\u754c\u751f\u547d\u4e0d\u4fee\u91d1\u4e39\uff0c\u800c\u662f\u5c06\u91d1\u4e39\u8f6c\u5316\u4e3a\u592a\u9634\u592a\u9633\uff0c\u4e4b\u540e\u518d\u8fdb\u884c\u6781\u5ea6\u5371\u9669\u7684\u788e\u4e39\uff0c\u8fdb\u5165\u51e1\u5c18\u671f\u3002\u51e1\u5c18\u671f\u975e\u5e38\u5f31\u5c0f\uff0c\u6210\u529f\u5ea6\u8fc7\u540e\u4fbf\u662f\u661f\u5c18\u5883\uff0c\u5b9e\u529b\u51cc\u9a7e\u4e8e\u4ed9\u4e4b\u4e0a\u3002",
         "exclude": "EVT?[40052]",
+        "grade": 3,
         "id": 40052,
         "include": "EVT?[40051]",
         "postEvent": "\u4f60\u5f00\u59cb\u8f6c\u4fee\u5f02\u754c\u6cd5\u95e8\u3002"
     },
     "40053": {
         "effect": {
             "STR": 900
         },
         "event": "\u4f60\u6210\u529f\u5c06\u4e39\u6d77\u51dd\u805a\u6210\u4e00\u9897\u592a\u9633\uff0c\u516b\u9897\u91d1\u4e39\u8f6c\u5316\u4e3a\u516b\u5927\u592a\u9634\u3002",
         "exclude": "EVT?[40053]",
+        "grade": 3,
         "id": 40053,
         "include": "EVT?[40052]"
     },
     "40054": {
         "branch": [
             "STR>3999:40055",
             "STR<4000:10000"
         ],
         "event": "\u4f60\u5f00\u59cb\u8fdb\u884c\u788e\u4e39\u3002\u4f60\u5f00\u59cb\u788e\u592a\u9634\u3002",
         "exclude": "EVT?[40054]",
+        "grade": 3,
         "id": 40054,
         "include": "EVT?[40053]"
     },
     "40055": {
         "NoRandom": 1,
         "branch": [
             "STR>4499:40056",
             "STR<4500:10000"
         ],
         "event": "\u4f60\u5f00\u59cb\u788e\u592a\u9633\u3002",
+        "grade": 3,
         "id": 40055
     },
     "40056": {
         "NoRandom": 1,
         "branch": [
             "TMS>999:40058",
             "TMS<1000:40057"
         ],
         "event": "\u788e\u4e39\u6210\u529f\uff0c\u4f60\u8e0f\u5165\u51e1\u5c18\u671f\u3002\u9700\u8981\u8fdb\u884c\u5343\u4e16\u8f6e\u56de\u540e\u518d\u6b21\u788e\u4e39\u6210\u529f\uff0c\u624d\u80fd\u664b\u5347\u661f\u5c18\u5883\u3002",
+        "grade": 3,
         "id": 40056
     },
     "40057": {
         "NoRandom": 1,
         "branch": [
             "TMS<1000:10000"
         ],
         "event": "\u4f60\u8fd8\u672a\u6ee1\u5343\u4e16\u8f6e\u56de\uff0c\u4e8e\u662f\u4f60\u518d\u6b21\u8fdb\u5165\u4e86\u8f6e\u56de\u4e4b\u4e2d\u3002",
+        "grade": 3,
         "id": 40057
     },
     "40058": {
         "NoRandom": 1,
         "effect": {
             "CHR": 1000,
             "INT": 1000,
             "MNY": 1000,
             "SPR": 1000,
             "STR": 1000
         },
         "event": "\u4f60\u5df2\u6ee1\u5343\u4e16\u8f6e\u56de\uff0c\u8e0f\u5165\u661f\u5c18\u5883\u3002\u4f60\u5df2\u4e0d\u518d\u662f\u4eba\uff0c\u751a\u81f3\u4e5f\u4e0d\u662f\u4ed9\u3002\u4f60\u5f7b\u5e95\u4ece\u8f6e\u56de\u4e4b\u4e2d\u8d85\u8131\u4e86",
+        "grade": 3,
         "id": 40058
     },
     "40059": {
         "effect": {
             "LIF": -1
         },
         "event": "\u2026\u2026\u5417\uff1f",
+        "grade": 3,
         "id": 40059,
         "include": "EVT?[40058]"
     },
     "40060": {
         "event": "\u4f60\u7559\u4e0b\u4e00\u5ea7\u4f20\u627f\u6d1e\u5e9c\u3002",
         "exclude": "(AEVT?[40061])|(EVT?[40039,40060])",
+        "grade": 1,
         "id": 40060,
         "include": "EVT?[40028]",
         "postEvent": "\u4f60\u628a\u300a\u4ed9\u8109\u56fe\u5f55\u300b\u6cd5\u95e8\u7559\u4e0b\u4e86\u3002"
     },
     "40061": {
         "effect": {
             "CHR": 2,
             "INT": 2,
             "STR": 2
         },
         "event": "\u4f60\u8fdb\u5165\u4e00\u5904\u4f20\u627f\u6d1e\u5e9c\uff0c\u5f97\u5230\u4e86\u592a\u53e4\u4fee\u884c\u6cd5\u95e8\u300a\u4ed9\u8109\u56fe\u5f55\u300b\u3002",
         "exclude": "(AEVT?[40061])|(EVT?[40001])",
+        "grade": 3,
         "id": 40061,
         "include": "AEVT?[40060]",
         "postEvent": "\u4f60\u8f6c\u4fee\u592a\u53e4\u6cd5\u95e8\uff0c\u8fbe\u5230\u51c0\u606f\u524d\u671f\u3002"
     },
     "40062": {
         "NoRandom": 1,
         "branch": [
             "EVT?[20462]:40063",
             "EVT![20462]:40064"
         ],
         "effect": {
             "SPR": 1
         },
         "event": "\u5728\u4f60\u6b7b\u524d\u4e00\u523b\uff0c\u7075\u9b42\u4e0d\u77e5\u4e3a\u4f55\u8131\u79bb\u4e86\u8eab\u4f53\u3002",
+        "grade": 3,
         "id": 40062
     },
     "40063": {
         "NoRandom": 1,
         "effect": {
             "INT": 5
         },
         "event": "\u6839\u636e\u4e4b\u524d\u770b\u8fc7\u7684\u300a\u5143\u795e\u4e0d\u706d\u300b\uff0c\u4f60\u7a33\u56fa\u4e86\u9b42\u9b44\uff0c\u5e76\u4e14\u6210\u529f\u8de8\u5165\u8131\u80ce\u5883\uff0c\u5f00\u59cb\u4fee\u70bc\u9b42\u4fee\u6cd5\u95e8\u3002",
+        "grade": 3,
         "id": 40063
     },
     "40064": {
         "NoRandom": 1,
         "effect": {
             "STR": -9999
         },
@@ -12565,14 +13112,15 @@
         "exclude": "EVT?[40075,40084]",
         "id": 40074,
         "include": "EVT?[40063]"
     },
     "40075": {
         "event": "\u4f60\u7a81\u7834\u5230\u795e\u6e38\u5883\u3002",
         "exclude": "EVT?[40075,40084]",
+        "grade": 2,
         "id": 40075,
         "include": "(EVT?[40063])&(INT>50)"
     },
     "40076": {
         "effect": {
             "INT": 3
         },
@@ -12590,14 +13138,15 @@
         "exclude": "EVT?[40078,40084]",
         "id": 40077,
         "include": "EVT?[40075]"
     },
     "40078": {
         "event": "\u4f60\u7a81\u7834\u5230\u4f2a\u4ed9\u5883\u3002",
         "exclude": "EVT?[40078,40084]",
+        "grade": 2,
         "id": 40078,
         "include": "(EVT?[40063])&(INT>500)",
         "postEvent": "\u9b42\u4fee\u6c38\u8fdc\u4e0d\u53ef\u80fd\u6210\u4ed9\uff0c\u6700\u7ec8\u90fd\u53ea\u80fd\u5c1d\u8bd5\u593a\u820d\uff0c\u5426\u5219\u4f1a\u968f\u7740\u65f6\u95f4\u6d88\u6563\u3002"
     },
     "40079": {
         "event": "\u4f60\u5230\u5904\u5bfb\u627e\u9002\u5408\u7684\u593a\u820d\u5bf9\u8c61\u3002",
         "exclude": "EVT?[40083,40084]",
@@ -12633,20 +13182,22 @@
     },
     "40083": {
         "branch": [
             "EVT?[40078]:10365"
         ],
         "event": "\u4f60\u5c1d\u8bd5\u593a\u820d\u4e00\u4f4d\u91d1\u4e39\u4e5d\u5c42\u4fee\u58eb\uff0c\u6210\u529f\u4e86\u3002",
         "exclude": "EVT?[40083,40084]",
+        "grade": 3,
         "id": 40083,
         "include": "EVT?[40079]"
     },
     "40084": {
         "branch": [
             "EVT?[40075]:40003"
         ],
         "event": "\u4f60\u5c1d\u8bd5\u593a\u820d\u4e00\u4f4d\u51c0\u606f\u4fee\u58eb\uff0c\u6210\u529f\u4e86\u3002",
         "exclude": "EVT?[40078,40084]",
+        "grade": 3,
         "id": 40084,
         "include": "EVT?[40075]"
     }
 }
```

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/resources/talents.json` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/talents.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996575342465752%*

 * *Differences: {"'1136'": "{'effect': {replace: OrderedDict([('MNY', 10)])}}"}*

```diff
@@ -1177,15 +1177,15 @@
         "grade": 3,
         "id": 1135,
         "name": "\u8f6e\u56de\u4e4b\u5916"
     },
     "1136": {
         "description": "\u5bb6\u5883+10",
         "effect": {
-            "INT": -5
+            "MNY": 10
         },
         "grade": 0,
         "id": 1136,
         "name": "\u8d2a\u5a6a"
     },
     "1137": {
         "condition": "(AGE?[100])&(TMS>99)",
```

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/talent.py` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/talent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import random
 from pathlib import Path
-from typing import Dict, List, Iterator
+from typing import Dict, Iterator, List
 
 from .property import Property
 from .utils import parse_condition
 
 
 class Talent:
     def __init__(self, data):
```

### Comparing `nonebot_plugin_remake-0.2.7/nonebot_plugin_remake/utils.py` & `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.2.7/setup.py` & `nonebot_plugin_remake-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,71 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-remake
+Version: 0.3.0
+Summary: 适用于 Nonebot2 的人生重开模拟器插件
+Home-page: https://github.com/noneplugin/nonebot-plugin-remake
+License: MIT
+Author: meetwq
+Author-email: meetwq@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-remake
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_remake']
+# nonebot-plugin-remake
 
-package_data = \
-{'': ['*'], 'nonebot_plugin_remake': ['resources/*']}
+适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的人生重开模拟器
 
-install_requires = \
-['nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0', 'nonebot2>=2.0.0-beta.4,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-remake',
-    'version': '0.2.7',
-    'description': '适用于 Nonebot2 的人生重开模拟器插件',
-    'long_description': '# nonebot-plugin-remake\n\n适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的人生重开模拟器\n\n这垃圾人生一秒也不想待了？立即重开！\n\n\n### 安装\n\n- 使用 nb-cli\n\n```\nnb plugin install nonebot_plugin_remake\n```\n\n- 使用 pip\n\n```\npip install nonebot_plugin_remake\n```\n\n本插件使用了 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) 的 `send_group_forward_msg` 和 `send_private_forward_msg` 接口 来发送合并转发消息，\n\n发送私聊合并转发消息需要使用 `v1.0.0-rc2` 版本以上的 go-cqhttp\n\n\n### 使用\n\n#### 触发方式：\n\n**以下命令需要加[命令前缀](https://v2.nonebot.dev/docs/api/config#Config-command_start) (默认为`/`)，可自行设置为空**\n\n```\n@机器人 remake/liferestart/人生重开/人生重来\n```\n\n\n#### 示例：\n\n<div align="left">\n  <img src="https://s2.loli.net/2022/01/15/rahwIWFfuvLGPgm.jpg" width="400" />\n</div>\n\n\n### 特别感谢\n\n- [cc004/lifeRestart-py](https://github.com/cc004/lifeRestart-py) lifeRestart game in python\n\n- [DaiShengSheng/lifeRestart_bot](https://github.com/DaiShengSheng/lifeRestart_bot) 适用于HoshinoBot下的人生重来模拟器插件\n',
-    'author': 'meetwq',
-    'author_email': 'meetwq@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/noneplugin/nonebot-plugin-remake',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+这垃圾人生一秒也不想待了？立即重开！
 
 
-setup(**setup_kwargs)
+### 安装
+
+- 使用 nb-cli
+
+```
+nb plugin install nonebot_plugin_remake
+```
+
+- 使用 pip
+
+```
+pip install nonebot_plugin_remake
+```
+
+本插件使用了 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) 的 `send_group_forward_msg` 和 `send_private_forward_msg` 接口 来发送合并转发消息，
+
+发送私聊合并转发消息需要使用 `v1.0.0-rc2` 版本以上的 go-cqhttp
+
+
+### 使用
+
+#### 触发方式：
+
+**以下命令需要加[命令前缀](https://v2.nonebot.dev/docs/api/config#Config-command_start) (默认为`/`)，可自行设置为空**
+
+```
+@机器人 remake/liferestart/人生重开/人生重来
+```
+
+
+#### 示例：
+
+<div align="left">
+  <img src="https://s2.loli.net/2022/01/15/rahwIWFfuvLGPgm.jpg" width="400" />
+</div>
+
+
+### 特别感谢
+
+- [cc004/lifeRestart-py](https://github.com/cc004/lifeRestart-py) lifeRestart game in python
+
+- [DaiShengSheng/lifeRestart_bot](https://github.com/DaiShengSheng/lifeRestart_bot) 适用于HoshinoBot下的人生重来模拟器插件
+
```

