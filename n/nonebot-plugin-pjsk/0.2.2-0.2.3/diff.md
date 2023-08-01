# Comparing `tmp/nonebot_plugin_pjsk-0.2.2.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.2.tar", last modified: Fri Jul 28 16:21:00 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.3.tar", last modified: Tue Aug  1 12:36:54 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.2.tar` & `nonebot_plugin_pjsk-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-28 16:20:41.039194 nonebot_plugin_pjsk-0.2.2/LICENSE
--rw-r--r--   0        0        0     3764 2023-07-28 16:20:41.039194 nonebot_plugin_pjsk-0.2.2/README.md
--rw-r--r--   0        0        0      889 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     7573 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0     1076 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0     7535 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     4002 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2351 2023-07-28 16:20:41.119195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1811 2023-07-28 16:21:00.639484 nonebot_plugin_pjsk-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-01 12:36:31.066187 nonebot_plugin_pjsk-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4076 2023-08-01 12:36:31.066187 nonebot_plugin_pjsk-0.2.3/README.md
+-rw-r--r--   0        0        0      889 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     8436 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0     1163 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0    11101 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     4002 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2351 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1787 2023-08-01 12:36:54.346318 nonebot_plugin_pjsk-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.2/LICENSE` & `nonebot_plugin_pjsk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.2/README.md` & `nonebot_plugin_pjsk-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -103,15 +103,16 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-插件有配置项，但是一般情况下无需更改，请自行查看 [config.py](./nonebot_plugin_pjsk/config.py) 文件
+见 [config.py](./nonebot_plugin_pjsk/config.py) 文件  
+插件开箱即用，如无需要则无须配置
 
 ## 🎉 使用
 
 直接使用指令 `pjsk` 进入交互创建模式；  
 使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助
 
 ### 效果图
@@ -146,14 +147,22 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.3
+
+- 限制了贴纸文本大小，以免 Bot 瞬间爆炸
+- 未提供字体大小时适应性调节 ([#14](https://github.com/Agnes4m/nonebot_plugin_pjsk/issues/14))
+- 参数 `--rotate` 改为提供角度值，正数为顺时针旋转
+- 将指令帮助渲染为图片发送（可以关）
+- 丢掉了 `pil-utils` 依赖
+
 ### 0.2.2
 
 - 修改了 0.2.1 版的交互创建模式的触发方式
 - 试验性地支持了 Emoji
 
 ### 0.2.1
```

#### html2text {}

```diff
@@ -10,27 +10,32 @@
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½®
-æä»¶æéç½®é¡¹ï¼ä½æ¯ä¸è¬æåµä¸æ éæ´æ¹ï¼è¯·èªè¡æ¥ç
-[config.py](./nonebot_plugin_pjsk/config.py) æä»¶ ## ð ä½¿ç¨
+"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½® è§ [config.py](./
+nonebot_plugin_pjsk/config.py) æä»¶
+æä»¶å¼ç®±å³ç¨ï¼å¦æ éè¦åæ é¡»éç½® ## ð ä½¿ç¨
 ç´æ¥ä½¿ç¨æä»¤ `pjsk` è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h`
 äºè§£ä½¿ç¨ Shell-Like æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾
 ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example](./readme/example-interact.png)   ä½¿ç¨
 Shell-Like æä»¤ ![example](./readme/example.png)  ## ð ç¢ç¢å¿µ -
 ~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
 å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æ issue æè [å ç¾¤](https://
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.2
-- ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.3
+- éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
+æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
+nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
+æ¹ä¸ºæä¾è§åº¦å¼ï¼æ­£æ°ä¸ºé¡ºæ¶éæè½¬ -
+å°æä»¤å¸®å©æ¸²æä¸ºå¾çåéï¼å¯ä»¥å³ï¼ - ä¸¢æäº `pil-utils`
+ä¾èµ ### 0.2.2 - ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
 è¯éªæ§å°æ¯æäº Emoji ### 0.2.1 - æ´æ¹æä»¤ `pjskåè¡¨`
 çäº¤äºæ¹å¼ ### 0.2.0 - éææä»¶
```

### Comparing `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __plugin_meta__ = PluginMetadata(
     name="Sekai Stickers",
     description="基于 NoneBot2 的 Project Sekai 表情包制作插件",
     usage="直接使用指令 `pjsk` 进入交互创建模式；\n使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/__main__.py` & `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,114 +4,138 @@
 from nonebot.exception import ParserExit
 from nonebot.internal.adapter import Message
 from nonebot.matcher import Matcher
 from nonebot.params import Arg, ArgPlainText, CommandArg, ShellCommandArgs
 from nonebot.rule import ArgumentParser, Namespace
 from nonebot.typing import T_State
 from nonebot_plugin_saa import Image, MessageFactory, MessageSegmentFactory, Text
+from numpy import rad2deg
 
+from .config import config
 from .draw import (
     DEFAULT_FONT_WEIGHT,
     DEFAULT_LINE_SPACING,
     DEFAULT_STROKE_WIDTH,
+    TextTooLargeError,
     draw_sticker,
     get_all_characters,
     get_character_stickers,
     i2b,
+    render_help_image,
+    use_image_cache,
 )
 from .resource import select_or_get_random
 from .utils import ResolveValueError, resolve_value
 
 cmd_sticker_list = on_command(
     "pjsk列表",
     aliases={"啤酒烧烤列表", "pjsk表情列表", "啤酒烧烤表情列表"},
     state={"interact": False},
 )
 
-cmd_generate_parser = ArgumentParser(
-    "pjsk",
-    description="Project Sekai 表情生成",
-    epilog="Tip：大部分有默认值的数值参数都可以用 `^` 开头指定相对于默认值的偏移量",
-)
-cmd_generate_parser.add_argument("text", nargs="*", help="添加的文字，为空时进入交互模式")
+cmd_generate_parser = ArgumentParser("pjsk")
+cmd_generate_parser.add_argument("text", nargs="*", help="添加的文字，为空时使用默认值")
 cmd_generate_parser.add_argument(
     "-i",
     "--id",
     help="表情 ID，可以通过指令 `pjsk列表` 查询，不提供时则随机选择",
 )
 cmd_generate_parser.add_argument("-x", help="文字的中心 x 坐标")
 cmd_generate_parser.add_argument("-y", help="文字的中心 y 坐标")
-cmd_generate_parser.add_argument(
-    "-r",
-    "--rotate",
-    type=str,
-    help="文字旋转的角度，单位为 `(ROTATE / 10) 弧度`",
-)
-cmd_generate_parser.add_argument("-s", "--size", help="文字的大小")
+cmd_generate_parser.add_argument("-r", "--rotate", help="文字旋转的角度")
+cmd_generate_parser.add_argument("-s", "--size", help="文字的大小，不指定时会以默认大小为最大值自动调整")
 cmd_generate_parser.add_argument("-w", "--weight", help="文本粗细")
 cmd_generate_parser.add_argument("--stroke-width", help="文本描边宽度")
 cmd_generate_parser.add_argument("--line-spacing", help="文本行间距")
 
 cmd_generate = on_shell_command(
     "pjsk",
     parser=cmd_generate_parser,
     aliases={"啤酒烧烤"},
     priority=2,
 )
 
 
+HELP = (
+    "Project Sekai 表情生成\n"
+    "\n"
+    f"{cmd_generate_parser.format_help()}\n"
+    "\n"
+    "Tips：\n"
+    "- 大部分有默认值的数值参数都可以用 ^ 开头指定相对于默认值的偏移量\n"
+    "- 不提供任何指令参数时会进入交互创建模式"
+)
+
+
+async def handle_exit(matcher: Matcher, arg: str):
+    if arg in ("0", "q", "e", "quit", "exit", "退出"):
+        await matcher.finish("已退出交互创建模式")
+
+
+def format_error(error: Exception) -> str:
+    if isinstance(error, ResolveValueError):
+        return f"提供的参数值 `{error.args[0]}` 解析出错"
+    if isinstance(error, TextTooLargeError):
+        return "你给的参数是不是有点太逆天了 😅"
+    logger.opt(exception=error).error("Error occurred while drawing sticker")
+    return "生成表情时出错，请检查后台日志"
+
+
 # failed to parse args
 @cmd_generate.handle()
 async def _(matcher: Matcher, foo: ParserExit = ShellCommandArgs()):
     if not foo.message:
         return
+
     if foo.status == 0:
-        await matcher.finish(foo.message)
+        if config.pjsk_help_as_image:
+            try:
+                img = await use_image_cache(render_help_image, "help", "JPEG")(HELP)
+            except Exception:
+                logger.exception("Error occurred while rendering help image")
+                await matcher.finish("生成帮助图片时出错，请检查后台日志")
+            await MessageFactory([Image(img)]).finish(reply=True)
+
+        await matcher.finish(HELP)
+
     await matcher.finish(f"参数解析出错：{foo.message}")
 
 
 # command or enter interact mode handler
 @cmd_generate.handle()
 async def _(matcher: Matcher, args: Namespace = ShellCommandArgs()):
     if not any(vars(args).values()):  # 没有任何参数
         matcher.skip()  # 跳过该 handler 进入交互模式
 
     sticker_id: Optional[str] = args.id
     selected_sticker = select_or_get_random(sticker_id)
     if not selected_sticker:
         await matcher.finish("没有找到对应 ID 的表情")
 
-    texts: Optional[List[str]] = args.text
+    texts: List[str] = args.text
     default_text = selected_sticker.default_text
     try:
         image = await draw_sticker(
             selected_sticker,
-            text=" ".join(texts) if texts else default_text.text,
+            text=" ".join(texts),  # if texts else default_text.text,
             x=resolve_value(args.x, default_text.x),
             y=resolve_value(args.y, default_text.y),
-            rotate=resolve_value(args.rotate, default_text.r),
+            rotate=resolve_value(args.rotate, rad2deg(default_text.r / 10)),
             font_size=resolve_value(args.size, default_text.s),
             stroke_width=resolve_value(args.stroke_width, DEFAULT_STROKE_WIDTH),
             line_spacing=resolve_value(args.line_spacing, DEFAULT_LINE_SPACING, float),
             font_weight=resolve_value(args.weight, DEFAULT_FONT_WEIGHT),
+            auto_adjust=args.size is None,
         )
-    except ResolveValueError as e:
-        await matcher.finish(f"提供的参数值 `{e.args[0]}` 解析出错")
-    except Exception:
-        logger.exception("Error occurred while drawing sticker")
-        await matcher.finish("生成表情时出错，请检查后台日志")
+    except Exception as e:
+        await matcher.finish(format_error(e))
 
     await MessageFactory([Image(i2b(image))]).finish(reply=True)
 
 
-async def handle_exit(matcher: Matcher, arg: str):
-    if arg in ("0", "q", "e", "quit", "exit", "退出"):
-        await matcher.finish("已退出交互创建模式")
-
-
 # interact mode or sticker list
 @cmd_sticker_list.handle()
 async def _(matcher: Matcher, arg: Message = CommandArg()):
     if arg.extract_plain_text().strip():
         matcher.set_arg("character", arg)
 
 
@@ -196,13 +220,16 @@
     sticker_id: str = ArgPlainText(),
     text: str = ArgPlainText(),
 ):
     sticker_info = select_or_get_random(sticker_id)
     assert sticker_info is not None
 
     try:
-        image = await draw_sticker(sticker_info, text=text)
-    except Exception:
-        logger.exception("Error occurred while drawing sticker")
-        await matcher.finish("生成表情时出错，请检查后台日志")
+        image = await draw_sticker(
+            sticker_info,
+            text=text,
+            auto_adjust=True,
+        )
+    except Exception as e:
+        await matcher.finish(format_error(e))
 
     await MessageFactory([Image(i2b(image))]).finish(reply=True)
```

### Comparing `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,17 @@
         "https://raw.gitmirror.com/TheOriginalAyaka/sekai-stickers/main/"
     )
     pjsk_repo_prefix: str = "https://raw.gitmirror.com/Agnes4m/nonebot_plugin_pjsk/main/"
 
     pjsk_emoji_source: str = "Apple"
     """Emoji 来源，可选值见 https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/imagetext_py.pyi#L217"""
 
+    pjsk_help_as_image: bool = True
+    """是否将帮助信息作为图片发送"""
+
     @validator("pjsk_assets_prefix", "pjsk_repo_prefix")
     def check_url(cls, v):  # noqa: N805
         if not v.startswith(("http://", "https://")):
             raise ValueError("URL must start with http:// or https://")
         if not v.endswith("/"):
             v = f"{v}/"
         return v
```

### Comparing `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.2/pyproject.toml` & `nonebot_plugin_pjsk-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.2"
+version = "0.2.3"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-plugin-send-anything-anywhere>=0.2.7",
     "imagetext-py>=2.1.3",
-    "pil-utils>=0.1.7",
     "httpx>=0.24.1",
     "numpy>=1.25.1",
     "anyio>=3.7.1",
 ]
 requires-python = ">=3.9,<4.0"
 keywords = [
     "pjsk",
```

### Comparing `nonebot_plugin_pjsk-0.2.2/PKG-INFO` & `nonebot_plugin_pjsk-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
 Requires-Dist: imagetext-py>=2.1.3
-Requires-Dist: pil-utils>=0.1.7
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: numpy>=1.25.1
 Requires-Dist: anyio>=3.7.1
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 -->
 
@@ -129,15 +128,16 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-插件有配置项，但是一般情况下无需更改，请自行查看 [config.py](./nonebot_plugin_pjsk/config.py) 文件
+见 [config.py](./nonebot_plugin_pjsk/config.py) 文件  
+插件开箱即用，如无需要则无须配置
 
 ## 🎉 使用
 
 直接使用指令 `pjsk` 进入交互创建模式；  
 使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助
 
 ### 效果图
@@ -172,14 +172,22 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.3
+
+- 限制了贴纸文本大小，以免 Bot 瞬间爆炸
+- 未提供字体大小时适应性调节 ([#14](https://github.com/Agnes4m/nonebot_plugin_pjsk/issues/14))
+- 参数 `--rotate` 改为提供角度值，正数为顺时针旋转
+- 将指令帮助渲染为图片发送（可以关）
+- 丢掉了 `pil-utils` 依赖
+
 ### 0.2.2
 
 - 修改了 0.2.1 版的交互创建模式的触发方式
 - 试验性地支持了 Emoji
 
 ### 0.2.1
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.2 Summary: Project
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.3 Summary: Project
 Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
 https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Project-URL:
 Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk Requires-Python:
 <4.0,>=3.9 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-
-anything-anywhere>=0.2.7 Requires-Dist: imagetext-py>=2.1.3 Requires-Dist: pil-
-utils>=0.1.7 Requires-Dist: httpx>=0.24.1 Requires-Dist: numpy>=1.25.1
-Requires-Dist: anyio>=3.7.1 Description-Content-Type: text/markdown
+anything-anywhere>=0.2.7 Requires-Dist: imagetext-py>=2.1.3 Requires-Dist:
+httpx>=0.24.1 Requires-Dist: numpy>=1.25.1 Requires-Dist: anyio>=3.7.1
+Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç» ### Wonderhoy! ![Wonderhoy](./readme/wonderhoy.png) ## ð¿
 å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
@@ -24,27 +24,32 @@
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½®
-æä»¶æéç½®é¡¹ï¼ä½æ¯ä¸è¬æåµä¸æ éæ´æ¹ï¼è¯·èªè¡æ¥ç
-[config.py](./nonebot_plugin_pjsk/config.py) æä»¶ ## ð ä½¿ç¨
+"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½® è§ [config.py](./
+nonebot_plugin_pjsk/config.py) æä»¶
+æä»¶å¼ç®±å³ç¨ï¼å¦æ éè¦åæ é¡»éç½® ## ð ä½¿ç¨
 ç´æ¥ä½¿ç¨æä»¤ `pjsk` è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h`
 äºè§£ä½¿ç¨ Shell-Like æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾
 ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example](./readme/example-interact.png)   ä½¿ç¨
 Shell-Like æä»¤ ![example](./readme/example.png)  ## ð ç¢ç¢å¿µ -
 ~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
 å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æ issue æè [å ç¾¤](https://
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.2
-- ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.3
+- éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
+æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
+nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
+æ¹ä¸ºæä¾è§åº¦å¼ï¼æ­£æ°ä¸ºé¡ºæ¶éæè½¬ -
+å°æä»¤å¸®å©æ¸²æä¸ºå¾çåéï¼å¯ä»¥å³ï¼ - ä¸¢æäº `pil-utils`
+ä¾èµ ### 0.2.2 - ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
 è¯éªæ§å°æ¯æäº Emoji ### 0.2.1 - æ´æ¹æä»¤ `pjskåè¡¨`
 çäº¤äºæ¹å¼ ### 0.2.0 - éææä»¶
```

