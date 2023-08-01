# Comparing `tmp/streamlit_chatbox-1.0.0-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5642 bytes, number of entries: 8
+Zip file size: 5921 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Jul-30 13:49 streamlit_chatbox/__init__.py
 -rw-rw-rw-  2.0 fat     4563 b- defN 23-Jul-31 01:26 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-31 01:37 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat     2793 b- defN 23-Jul-31 01:27 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     4454 b- defN 23-Jul-31 01:44 streamlit_chatbox-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 01:44 streamlit_chatbox-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-31 01:44 streamlit_chatbox-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      677 b- defN 23-Jul-31 01:44 streamlit_chatbox-1.0.0.dist-info/RECORD
-8 files, 13312 bytes uncompressed, 4450 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 fat     3655 b- defN 23-Aug-01 00:23 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     4452 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      677 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/RECORD
+8 files, 14172 bytes uncompressed, 4729 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.0.0.dist-info/METADATA
+Filename: streamlit_chatbox-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.0.0.dist-info/WHEEL
+Filename: streamlit_chatbox-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.0.0.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.0.0.dist-info/RECORD
+Filename: streamlit_chatbox-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/messages.py

```diff
@@ -14,14 +14,42 @@
         self._assistant_avatar = assistant_avatar
         st.session_state.setdefault(self._session_name, [])
 
     @property
     def history(self):
         return st.session_state.get(self._session_name, [])
 
+    def filter_history(
+        self,
+        history_len: int,
+        filter: Callable = None,
+    ) -> List:
+        def default_filter(index, msg):
+            '''
+            filter text messages only with the format {"role":role, "content":content}
+            '''
+            content = [x._content for x in msg["elements"] if x._output_method in ["markdown", "text"]]
+            return {
+                "role": msg["role"],
+                "content": "\n\n".join(content),
+            }
+
+        if filter is None:
+            filter = default_filter
+
+        result = []
+        for msg in self.history[-1::-1]:
+            filtered = filter(msg)
+            if filtered is not None:
+                result.insert(0, filtered)
+                if len(result) >= history_len:
+                    break
+
+        return result
+
     def _prepare_elements(
         self,
         elements: Union[OutputElement, str, List[Union[OutputElement, str]]],
     ) -> List[OutputElement]:
         if isinstance(elements, str):
             elements = [Markdown(elements)]
         elif isinstance(elements, OutputElement):
```

## Comparing `streamlit_chatbox-1.0.0.dist-info/METADATA` & `streamlit_chatbox-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.0.0
+Version: 1.0.1
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.24.0)
@@ -20,14 +20,16 @@
 This package(>=1.0.0) will focus on wrapper of official chat elements to make chat with LLMs more convenient.
 
 # Chatbox component for streamlit
 
 A Streamlit component to show chat messages.
 It's basiclly a wrapper of streamlit officeial elements including the chat elemnts.
 
+![demo](https://github.com/liunux4odoo/streamlit-chatbox/blob/master/demo.gif?raw=true)
+
 ## Features
 
 - support streaming output.
 - support markdown/image/video/audio messages, and all streamlit elements could be supported by customized `OutputElement`.
 - output multiple messages at once, and make them collapsable.
 
 This make it easy to chat with langchain LLMs in streamlit.
@@ -99,17 +101,14 @@
         Audio('https://sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4'))
 
 if show_history:
     st.write(chat_box.history)
 
 ```
 
-![demo](https://github.com/liunux4odoo/streamlit-chatbox/blob/master/demo.gif?raw=true)
-
-
 ## Todos
 
 - [x] wrapper of official chat elements
 - [ ] input messages: (this depends on the official st.chat_input improvement by #7069)
 	- [x] TEXT
 	- [ ] IMAGE
 		- [ ] file upload
```

## Comparing `streamlit_chatbox-1.0.0.dist-info/RECORD` & `streamlit_chatbox-1.0.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 streamlit_chatbox/__init__.py,sha256=okS4bZ1sk5ma0Nawlw07pLxVR_INKIqCQQFqvzkzR4A,392
 streamlit_chatbox/elements.py,sha256=rC12Gv0WrZVKMPIh61KIBdw6fkuMM4I4V6FSKHV21Z8,4563
 streamlit_chatbox/flows.py,sha256=RvtStf1em9vGPp_sj8V7xHKbBiI5_p58RAFuvEMq2-c,323
-streamlit_chatbox/messages.py,sha256=wzfpzWie1V3wBAAddy4YaWlHmzmkPaO9qVZ8ALl3ut0,2793
-streamlit_chatbox-1.0.0.dist-info/METADATA,sha256=_gEQpq6HWkig_XHbSWSt6XP_1LjSsDwYRfCryN1Mi8s,4454
-streamlit_chatbox-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-streamlit_chatbox-1.0.0.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
-streamlit_chatbox-1.0.0.dist-info/RECORD,,
+streamlit_chatbox/messages.py,sha256=Kgt9ek-EA_CpmDK4kLQfo6yJk1ew19Qfzpk0tRDECGY,3655
+streamlit_chatbox-1.0.1.dist-info/METADATA,sha256=By1JclVTh14N6FqrHoJ4MSfptNys5C-QTskOcaVBvsk,4452
+streamlit_chatbox-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+streamlit_chatbox-1.0.1.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
+streamlit_chatbox-1.0.1.dist-info/RECORD,,
```

