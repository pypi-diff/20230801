# Comparing `tmp/ai_chat_chain-0.1.1.tar.gz` & `tmp/ai_chat_chain-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_chat_chain-0.1.1.tar", max compression
+gzip compressed data, was "ai_chat_chain-0.1.2.tar", max compression
```

## Comparing `ai_chat_chain-0.1.1.tar` & `ai_chat_chain-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.1.1/ai_chat/__init__.py
--rw-r--r--   0        0        0     4973 2023-08-01 16:16:55.848731 ai_chat_chain-0.1.1/ai_chat/chat.py
--rw-r--r--   0        0        0      136 2023-08-01 02:01:47.995647 ai_chat_chain-0.1.1/ai_chat/defaults.py
--rw-r--r--   0        0        0     1082 2023-08-01 19:16:20.659048 ai_chat_chain-0.1.1/ai_chat/openai.py
--rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.1.1/ai_chat/store/__init__.py
--rw-r--r--   0        0        0     1043 2023-08-01 17:00:50.526537 ai_chat_chain-0.1.1/ai_chat/store/base.py
--rw-r--r--   0        0        0     5127 2023-08-01 15:38:29.361570 ai_chat_chain-0.1.1/ai_chat/store/sqlite.py
--rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.1.1/ai_chat/store/supabase.py
--rw-r--r--   0        0        0     1390 2023-08-01 02:31:01.169745 ai_chat_chain-0.1.1/ai_chat/types.py
--rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.1.1/ai_chat/util.py
--rw-r--r--   0        0        0      851 2023-08-01 19:24:19.082737 ai_chat_chain-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      907 2023-08-01 17:08:52.775187 ai_chat_chain-0.1.1/README.md
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 ai_chat_chain-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.1.2/ai_chat/__init__.py
+-rw-r--r--   0        0        0     4973 2023-08-01 16:16:55.848731 ai_chat_chain-0.1.2/ai_chat/chat.py
+-rw-r--r--   0        0        0      136 2023-08-01 02:01:47.995647 ai_chat_chain-0.1.2/ai_chat/defaults.py
+-rw-r--r--   0        0        0     1082 2023-08-01 19:16:20.659048 ai_chat_chain-0.1.2/ai_chat/openai.py
+-rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.1.2/ai_chat/store/__init__.py
+-rw-r--r--   0        0        0     1043 2023-08-01 17:00:50.526537 ai_chat_chain-0.1.2/ai_chat/store/base.py
+-rw-r--r--   0        0        0     5127 2023-08-01 15:38:29.361570 ai_chat_chain-0.1.2/ai_chat/store/sqlite.py
+-rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.1.2/ai_chat/store/supabase.py
+-rw-r--r--   0        0        0     1390 2023-08-01 02:31:01.169745 ai_chat_chain-0.1.2/ai_chat/types.py
+-rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.1.2/ai_chat/util.py
+-rw-r--r--   0        0        0      851 2023-08-01 19:28:49.658093 ai_chat_chain-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      907 2023-08-01 17:08:52.775187 ai_chat_chain-0.1.2/README.md
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 ai_chat_chain-0.1.2/PKG-INFO
```

### Comparing `ai_chat_chain-0.1.1/ai_chat/chat.py` & `ai_chat_chain-0.1.2/ai_chat/chat.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/ai_chat/openai.py` & `ai_chat_chain-0.1.2/ai_chat/openai.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/ai_chat/store/base.py` & `ai_chat_chain-0.1.2/ai_chat/store/base.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/ai_chat/store/sqlite.py` & `ai_chat_chain-0.1.2/ai_chat/store/sqlite.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/ai_chat/store/supabase.py` & `ai_chat_chain-0.1.2/ai_chat/store/supabase.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/ai_chat/types.py` & `ai_chat_chain-0.1.2/ai_chat/types.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/ai_chat/util.py` & `ai_chat_chain-0.1.2/ai_chat/util.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/pyproject.toml` & `ai_chat_chain-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-chat-chain"
-version = "0.1.1"
+version = "0.1.2"
 description = "maintain chat conversation state"
 authors = ["erik aronesty <erik@q32.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_chat"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_chat_chain-0.1.1/README.md` & `ai_chat_chain-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.1/PKG-INFO` & `ai_chat_chain-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-chat-chain
-Version: 0.1.1
+Version: 0.1.2
 Summary: maintain chat conversation state
 License: MIT
 Author: erik aronesty
 Author-email: erik@q32.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

