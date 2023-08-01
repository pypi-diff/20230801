# Comparing `tmp/nonebot_plugin_savepic-0.1.0.tar.gz` & `tmp/nonebot_plugin_savepic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_savepic-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_savepic-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_savepic-0.1.0.tar` & `nonebot_plugin_savepic-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1060 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/LICENSE
--rw-r--r--   0        0        0     3770 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/README.md
--rw-r--r--   0        0        0     5135 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/__init__.py
--rw-r--r--   0        0        0      600 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/config.py
--rw-r--r--   0        0        0      846 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/migrations/1a654e02179b_.py
--rw-r--r--   0        0        0      581 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/model.py
--rw-r--r--   0        0        0     4948 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/pic_sql.py
--rw-r--r--   0        0        0      971 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/rule.py
--rw-r--r--   0        0        0      489 2023-08-01 21:36:23.651085 nonebot_plugin_savepic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1984 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/README.md
+-rw-r--r--   0        0        0     5606 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/__init__.py
+-rw-r--r--   0        0        0      181 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/config.py
+-rw-r--r--   0        0        0      846 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/migrations/1a654e02179b_.py
+-rw-r--r--   0        0        0      581 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/model.py
+-rw-r--r--   0        0        0     4948 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/pic_sql.py
+-rw-r--r--   0        0        0      971 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/rule.py
+-rw-r--r--   0        0        0      490 2023-08-01 21:52:34.712039 nonebot_plugin_savepic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2621 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_savepic-0.1.0/LICENSE` & `nonebot_plugin_savepic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/__init__.py` & `nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,30 @@
 
 from asyncpg.exceptions import InvalidRegularExpressionError
 
 from .config import Config
 from .pic_sql import savepic, rename, delete, write_pic, randpic, load_pic, select_pic
 from .rule import PIC_AMDIN
 
+from nonebot.plugin import PluginMetadata
+
+__plugin_meta__ = PluginMetadata(
+    name="Savepic",
+    description="表情包保存",
+    usage="""用法:
+/savepic <文件名> <图片>
+/savepic -g <文件名> <全局图片>
+/savepic -d <文件名> 删除图图片
+/savepic -m <原文件名> <新文件名> 重命名图片
+/randpic <关键词> 随机图片
+<文件名> 发送图片""",
+    config=Config,
+    homepage="https://github.com/Yan-Zero/nonebot-plugin-savepic"
+)
+
 INVALID_FILENAME_CHARACTERS = r'\/:*?"<>|'
 
 global_config = get_driver().config
 p_config = Config.parse_obj(global_config)
 
 rpic = on_command("randpic", aliases={"随机图"}, priority=5)
 @rpic.handle()
```

### Comparing `nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/migrations/1a654e02179b_.py` & `nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/migrations/1a654e02179b_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/model.py` & `nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/pic_sql.py` & `nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/pic_sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.0/nonebot_plugin_savepic/rule.py` & `nonebot_plugin_savepic-0.1.1/nonebot_plugin_savepic/rule.py`

 * *Files identical despite different names*

