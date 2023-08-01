# Comparing `tmp/nonebot_plugin_searchbiliinfo-1.7.8.tar.gz` & `tmp/nonebot_plugin_searchbiliinfo-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_searchbiliinfo-1.7.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_searchbiliinfo-1.7.9.tar", max compression
```

## Comparing `nonebot_plugin_searchbiliinfo-1.7.8.tar` & `nonebot_plugin_searchbiliinfo-1.7.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_searchbiliinfo-1.7.8/LICENSE
--rw-r--r--   0        0        0   105452 2023-06-19 10:48:02.172801 nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/__init__.py
--rw-r--r--   0        0        0   356769 2023-03-07 03:59:53.911011 nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/data.py
--rw-r--r--   0        0        0  6937547 2023-02-20 03:35:57.148057 nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/data_medal.py
--rw-r--r--   0        0        0     3484 2023-02-24 08:29:21.055074 nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/html/composition_page.html
--rw-r--r--   0        0        0     1264 2023-06-19 10:50:13.596632 nonebot_plugin_searchbiliinfo-1.7.8/pyproject.toml
--rw-r--r--   0        0        0    30735 2023-06-19 10:48:58.114644 nonebot_plugin_searchbiliinfo-1.7.8/README.md
--rw-r--r--   0        0        0    31225 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_searchbiliinfo-1.7.9/LICENSE
+-rw-r--r--   0        0        0   105350 2023-08-01 08:58:42.651409 nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/__init__.py
+-rw-r--r--   0        0        0   356769 2023-03-07 03:59:53.911011 nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/data.py
+-rw-r--r--   0        0        0  6937547 2023-02-20 03:35:57.148057 nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/data_medal.py
+-rw-r--r--   0        0        0     3484 2023-02-24 08:29:21.055074 nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/html/composition_page.html
+-rw-r--r--   0        0        0     1264 2023-08-01 09:04:06.602965 nonebot_plugin_searchbiliinfo-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0    30735 2023-06-19 10:48:58.114644 nonebot_plugin_searchbiliinfo-1.7.9/README.md
+-rw-r--r--   0        0        0    31225 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.9/PKG-INFO
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/LICENSE` & `nonebot_plugin_searchbiliinfo-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/__init__.py` & `nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         nonebot.logger.info(temp)
         await catch_str1.finish(Message(f'{msg}'), reply_message=True)
 
     nonebot.logger.debug("src_uid:" + src_uid + " tgt_uid:" + tgt_uid)
 
     await catch_str1.send("正在获取数据中，请耐心等待...", reply_message=True)
 
-    url = 'https://ukamnads.icu/api/search/user/detail?uid=' + src_uid + '&target=' + tgt_uid + \
+    url = 'https://danmakus.com/api/search/user/detail?uid=' + src_uid + '&target=' + tgt_uid + \
             '&pagenum=' + page + '&pagesize=' + page_size
     info_json = await common_get_return_json(url)
 
     if info_json == None:
         msg = '果咩，查询信息失败喵~API寄了喵'
         await catch_str1.finish(Message(f'{msg}'), reply_message=True)
 
@@ -323,15 +323,15 @@
         msg = '查询不到用户名为：' + src_uid + ' 的相关信息。\nError code：' + str(temp["code"])
         await catch_str11.finish(Message(f'{msg}'), reply_message=True)
 
     nonebot.logger.debug("src_uid:" + src_uid + " tgt_uid:" + tgt_uid)
 
     await catch_str11.send("正在获取数据中，请耐心等待...", reply_message=True)
 
-    url = 'https://ukamnads.icu/api/search/user/detail?uid=' + src_uid + '&target=' + tgt_uid + \
+    url = 'https://danmakus.com/api/search/user/detail?uid=' + src_uid + '&target=' + tgt_uid + \
             '&pagenum=' + page + '&pagesize=' + page_size
     info_json = await common_get_return_json(url)
 
     if info_json == None:
         msg = '果咩，查询信息失败喵~API寄了喵'
         await catch_str11.finish(Message(f'{msg}'), reply_message=True)
 
@@ -395,15 +395,15 @@
     else:
         nonebot.logger.info(temp)
         msg = '查询不到用户名为：' + content + ' 的相关信息。\nError code：' + str(temp["code"])
         await catch_str.finish(Message(f'{msg}'), reply_message=True)
 
     await catch_str.send("正在获取数据中，请耐心等待...", reply_message=True)
 
-    url = 'https://ukamnads.icu/api/search/user/channel?uid=' + content
+    url = 'https://danmakus.com/api/search/user/channel?uid=' + content
     user_info_json = await common_get_return_json(url)
 
     if user_info_json == None:
         msg = '果咩，查询用户信息失败喵~API寄了喵'
         await catch_str2.finish(Message(f'{msg}'), reply_message=True)
 
     try:
@@ -457,15 +457,15 @@
         nonebot.logger.info(temp)
         msg = '查询不到：' + content + ' 的相关信息。\nError code：' + str(temp["code"])
         await catch_str26.finish(Message(f'{msg}'), reply_message=True)
 
     await catch_str26.send("正在获取数据中，请耐心等待...", reply_message=True)
 
     
-    url = 'https://ukamnads.icu/api/search/user/channel?uid=' + content
+    url = 'https://danmakus.com/api/search/user/channel?uid=' + content
     user_info_json = await common_get_return_json(url)
 
     if user_info_json == None:
         msg = '果咩，查询用户信息失败喵~API寄了喵'
         await catch_str26.finish(Message(f'{msg}'), reply_message=True)
 
     try:
@@ -530,15 +530,15 @@
     else:
         nonebot.logger.info(temp)
         msg = '查询不到用户名为：' + src_uid + ' 的相关信息。\nError code：' + str(temp["code"])
         await catch_str3.finish(Message(f'{msg}'), reply_message=True)
 
     await catch_str3.send("正在获取数据中，请耐心等待...", reply_message=True)
 
-    url = 'https://ukamnads.icu/api/info/channel?cid=' + src_uid
+    url = 'https://danmakus.com/api/info/channel?cid=' + src_uid
     info_json = await common_get_return_json(url)
 
     if info_json == None:
         msg = '查询用户：' + src_uid + '失败，API寄了喵'
         await catch_str3.finish(Message(f'{msg}'), reply_message=True)
 
     try:
@@ -665,15 +665,15 @@
         "3": "舰长",
     }
 
     income_type_ch = INCOME_TYPE_CHS.get(income_type, "礼物")
 
     await catch_str4.send("正在获取数据中，请耐心等待...", reply_message=True)
 
-    url = 'https://ukamnads.icu/api/info/channel?cid=' + src_uid
+    url = 'https://danmakus.com/api/info/channel?cid=' + src_uid
     live_json = await common_get_return_json(url)
 
     try:
         # 判断返回代码
         if live_json['code'] != 200:
             msg = '查询用户：' + src_uid + ' 直播信息失败，请检查拼写或者是API寄了\nError code：' + str(live_json["code"])
             await catch_str4.finish(Message(f'{msg}'), reply_message=True)
@@ -700,15 +700,15 @@
               "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;总直播时长:" + totalLivehour + "h\n\n" + \
               "| 时间 | uid | 昵称 | 内容 | 价格 |\n" \
               "| :-----| :-----| :-----| :-----| :-----|\n"
 
     # nonebot.logger.info(out_str)
 
     # 获取当场直播信息
-    url = 'https://ukamnads.icu/api/info/live?liveid=' + live_id + '&type=' + income_type + '&uid='
+    url = 'https://danmakus.com/api/info/live?liveid=' + live_id + '&type=' + income_type + '&uid='
     info_json = await common_get_return_json(url)
 
     if info_json == None:
         msg = '查询用户：' + src_uid + ' 场次数据失败，API寄了喵'
         await catch_str4.finish(Message(f'{msg}'), reply_message=True)
 
     try:
@@ -1200,15 +1200,15 @@
         await catch_str14.finish(Message(f'{msg}'), reply_message=True)
 
     await catch_str14.send("正在获取数据中，请耐心等待...", reply_message=True)
 
     try:
         async with get_new_page(viewport={"width": 1040, "height": 2500}) as page:
             await page.goto(
-                "https://ukamnads.icu/user/" + content,
+                "https://danmakus.com/user/" + content,
                 timeout=2 * 60 * 1000,
                 wait_until="networkidle",
             )
             temp_path = "./data/danmakus.com_user" + await get_current_timestamp_seconds() + ".png"
             pic = await page.screenshot(full_page=True, path=temp_path)
 
         await catch_str14.finish(MessageSegment.image(pic))
@@ -1238,15 +1238,15 @@
         await catch_str15.finish(Message(f'{msg}'), reply_message=True)
 
     await catch_str15.send("正在获取数据中，请耐心等待...", reply_message=True)
 
     try:
         async with get_new_page(viewport={"width": 850, "height": 2000}) as page:
             await page.goto(
-                "https://ukamnads.icu/channel/" + content,
+                "https://danmakus.com/channel/" + content,
                 timeout=2 * 60 * 1000,
                 wait_until="networkidle",
             )
             temp_path = "./data/danmakus.com_channel" + await get_current_timestamp_seconds() + ".png"
             pic = await page.screenshot(full_page=True, path=temp_path)
 
         await catch_str15.finish(MessageSegment.image(pic))
@@ -1275,15 +1275,15 @@
         msg = '查询不到：' + content + ' 的相关信息。\nError code：' + str(temp["code"])
         await catch_str39.finish(Message(f'{msg}'), reply_message=True)
 
     await catch_str39.send("正在获取数据中，请耐心等待...", reply_message=True)
 
     try:
         async with get_new_page(viewport={"width": 1000, "height": 1200}) as page:
-            url = "https://ukamnads.icu/analyze/" + content + "?startTime=1669874804320&endTime=" + await get_current_timestamp_seconds(1)
+            url = "https://danmakus.com/analyze/" + content + "?startTime=1669874804320&endTime=" + await get_current_timestamp_seconds(1)
             # print(url)
             await page.goto(
                 url,
                 timeout=2 * 60 * 1000,
                 wait_until="networkidle",
             )
             # 等待页面加载完成
@@ -1591,27 +1591,27 @@
             await page.goto(
                 "https://laplace.live/user/" + content,
                 timeout=2 * 60 * 1000,
                 wait_until="networkidle"
             )
             # 等待页面加载完成
             await page.wait_for_selector('.info', timeout=60 * 1000)
-            # 删除小作文
-            click_js = 'let p_arr=document.getElementsByClassName("Home_xl__sAgvD")[0].getElementsByTagName("p");for(let i=0;i<(p_arr.length-1);i++){setTimeout(function(){p_arr[0].remove()},100)}'
-            # 执行 JavaScript 代码
-            result = await page.evaluate(click_js)
-            click_js = 'let details=document.getElementsByClassName("jsx-1561ee057cab7771 Home_scrollableContent__6y8XH Home_xl__sAgvD")[0].getElementsByTagName("details");' \
+            # # 删除小作文
+            # click_js = 'let p_arr=document.getElementsByClassName("Home_xl__sAgvD")[0].getElementsByTagName("p");for(let i=0;i<(p_arr.length-1);i++){setTimeout(function(){p_arr[0].remove()},100)}'
+            # # 执行 JavaScript 代码
+            # result = await page.evaluate(click_js)
+            click_js = 'let details=document.getElementsByTagName("details");' \
                 'let len=details.length;for(var i=0;i<len;i++){details[i].getElementsByTagName("summary")[0].click();};' \
                 'document.getElementsByClassName("player")[0].remove();'
             # 执行 JavaScript 代码
             result = await page.evaluate(click_js)
             nonebot.logger.debug(result)
             # 修改长度已显示
             await page.wait_for_selector('.following-list')
-            click_js = 'let len=document.getElementsByClassName("jsx-5797876f0d745d6c following-list").length;for(var i=0;i<len;i++){document.getElementsByClassName("jsx-5797876f0d745d6c following-list")[i].style.maxHeight="2000px"}'
+            click_js = 'let len=document.getElementsByClassName("following-list").length;for(var i=0;i<len;i++){document.getElementsByClassName("following-list")[i].style.maxHeight="2000px"}'
             result = await page.evaluate(click_js)
             nonebot.logger.debug(result)
             await asyncio.sleep(3)
             temp_path = "./data/laplace.live_user" + await get_current_timestamp_seconds() + ".png"
             pic = await page.screenshot(full_page=True, path=temp_path)
 
         await catch_str23.finish(MessageSegment.image(pic))
@@ -2091,15 +2091,16 @@
     try:
         async with get_new_page(viewport={"width": 530, "height": 29999}) as page:
             await page.goto(
                 "https://laplace.live/dd",
                 timeout=2 * 60 * 1000,
                 wait_until="networkidle",
             )
-            await page.wait_for_selector('.jsx-a9b5b32e4de3b53c')
+            await page.wait_for_selector('.btn')
+            await page.wait_for_timeout(1)
             click_js = 'document.getElementById("' + radio_sort + '").click();document.getElementById("showVup").click()'
             # 执行 JavaScript 代码
             result = await page.evaluate(click_js)
             nonebot.logger.debug(result)
             await page.wait_for_selector('.item')
             # 渲染比较慢，建议多等等，等待个10秒
             await page.wait_for_timeout(10)
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/data.py` & `nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/data_medal.py` & `nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/data_medal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/nonebot_plugin_searchBiliInfo/html/composition_page.html` & `nonebot_plugin_searchbiliinfo-1.7.9/nonebot_plugin_searchBiliInfo/html/composition_page.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/pyproject.toml` & `nonebot_plugin_searchbiliinfo-1.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-searchbiliinfo"
-version = "1.7.8"
+version = "1.7.9"
 description = "A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）"
 authors = ["Ikaros <327209194@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_searchbiliinfo"}]
 homepage = "https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo"
 repository = "https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo"
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/README.md` & `nonebot_plugin_searchbiliinfo-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.8/PKG-INFO` & `nonebot_plugin_searchbiliinfo-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-searchbiliinfo
-Version: 1.7.8
+Version: 1.7.9
 Summary: A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）
 Home-page: https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo
 License: MIT
 Author: Ikaros
 Author-email: 327209194@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-searchbiliinfo Version: 1.7.8
+Metadata-Version: 2.1 Name: nonebot-plugin-searchbiliinfo Version: 1.7.9
 Summary: A plugin for nonebot2. Query Bilibili user
 informationï¼ä¸ä¸ªNonebot2çæä»¶ï¼bç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ãç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDï¼ä¸»æ­è¥æ¶æ¦åï¼æ¥æåï¼æ¥çå­ç­ãï¼
 Home-page: https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo License:
 MIT Author: Ikaros Author-email: 327209194@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

