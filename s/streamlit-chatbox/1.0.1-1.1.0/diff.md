# Comparing `tmp/streamlit_chatbox-1.0.1-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5921 bytes, number of entries: 8
+Zip file size: 6077 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Jul-30 13:49 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     4563 b- defN 23-Jul-31 01:26 streamlit_chatbox/elements.py
+-rw-rw-rw-  2.0 fat     4431 b- defN 23-Aug-01 03:38 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-31 01:37 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat     3655 b- defN 23-Aug-01 00:23 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     4452 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      677 b- defN 23-Aug-01 00:25 streamlit_chatbox-1.0.1.dist-info/RECORD
-8 files, 14172 bytes uncompressed, 4729 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 fat     4423 b- defN 23-Aug-01 03:38 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      677 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/RECORD
+8 files, 14773 bytes uncompressed, 4885 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.0.1.dist-info/METADATA
+Filename: streamlit_chatbox-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.0.1.dist-info/WHEEL
+Filename: streamlit_chatbox-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.0.1.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.0.1.dist-info/RECORD
+Filename: streamlit_chatbox-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/elements.py

```diff
@@ -27,30 +27,30 @@
                 "format": "mp4",
             },
             "image": {
                 "use_column_width": "auto",
             },
         }
         self._set_default_kwargs()
-        self._element = None
+        self._dg = None
         self._place_holder = None
 
     def _set_default_kwargs(self) -> None:
         if default := self._defualt_kwargs.get(self._output_method):
             for k, v in default.items():
                 self._kwargs.setdefault(k, v)
 
     def __call__(self) -> st._DeltaGenerator:
-        # assert self._element is None, "Every element can be rendered once only."
+        # assert self._dg is None, "Every element can be rendered once only."
         self._place_holder = st.empty()
         output_method = getattr(self._place_holder, self._output_method)
         assert callable(
             output_method), f"The attribute st.{self._output_mehtod} is not callable."
-        self._element = output_method(*self._args, **self._kwargs)
-        return self._element
+        self._dg = output_method(*self._args, **self._kwargs)
+        return self._dg
 
 
 class OutputElement(Element):
     def __init__(self,
                  content: Union[str, bytes] = "",
                  output_method: str = "markdown",
                  title: str = "",
@@ -74,27 +74,25 @@
 
     def __repr__(self) -> str:
         method = self._output_method.capitalize()
         return f"{method} Element:\n{self._content}"
 
     def update_element(
         self,
-        element: Union["OutputElement", str],
+        element: "OutputElement",
         streaming: Optional[bool] = None,
     ) -> st._DeltaGenerator:
         assert self._place_holder is not None, "You must render the element before setting new element."
-        if isinstance(element, str):
-            element = Markdown(element)
-            if streaming is None:
-                streaming = True
-        if streaming and isinstance(element, Markdown):
-            element._content += " ▌"
         with self._place_holder:
-            self._element = element()
-        return self._element
+            self._dg = element()
+        return self._dg
+
+    def attrs_from(self, target):
+        for attr in ["_in_expander", "_expanded", "_title"]:
+            setattr(self, attr, getattr(target, attr))
 
 
 class InputElement(Element):
     pass
 
 
 class Markdown(OutputElement):
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## streamlit_chatbox/messages.py

```diff
@@ -88,14 +88,35 @@
     def output_messages(self):
         for msg in self.history:
             avatar = self._user_avatar if msg["role"] == "user" else self._assistant_avatar
             with st.chat_message(msg["role"], avatar=avatar):
                 for element in msg["elements"]:
                     element()
 
+    def update_msg(
+        self,
+        element: Union["OutputElement", str],
+        element_index: int = -1,
+        history_index: int = -1,
+        streaming: Optional[bool] = None,
+    ) -> st._DeltaGenerator:
+        if isinstance(element, str):
+            element = Markdown(element)
+            if streaming is None:
+                streaming = True
+        if streaming and isinstance(element, Markdown):
+            element._content += " ▌"
+        old_element = self.history[history_index]["elements"][element_index]
+        dg = old_element.update_element(
+            element, streaming
+        )
+        element.attrs_from(old_element)
+        self.history[history_index]["elements"][element_index] = element
+        return dg
+
 
 class FakeLLM:
     def _answer(self, query: str) -> str:
         answer = f"this is my answer for your question:\n\n{query}"
         docs = ["reference 1", "reference 2", "reference 3"]
         return answer, docs
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `streamlit_chatbox-1.0.1.dist-info/METADATA` & `streamlit_chatbox-1.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.0.1
+Version: 1.1.0
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.24.0)
@@ -49,15 +49,15 @@
 
 llm = FakeLLM()
 chat_box = ChatBox()
 
 with st.sidebar:
     st.subheader('start to chat using streamlit')
     streaming = st.checkbox('streaming', True)
-    in_expander = st.checkbox('show messages in expander', False)
+    in_expander = st.checkbox('show messages in expander', True)
     show_history = st.checkbox('show history', False)
 
 chat_box.output_messages()
 
 if query := st.chat_input('input your question here'):
     chat_box.user_say(query)
     if streaming:
@@ -70,19 +70,18 @@
                 Markdown("", in_expander=in_expander, title="references"),
             ]
         )
         time.sleep(1)
         text = ""
         for x, docs in generator:
             text += x
-            elements[0].update_element(text)
-            elements[1].update_element("\n\n".join(docs), streaming=False)
+            chat_box.update_msg(text, 0, streaming=True)
+            chat_box.update_msg("\n\n".join(docs), 1, streaming=False)
         # update the element without focus
-        elements[0].update_element(text, streaming=False)
-        elements[0] = Markdown(text)
+        chat_box.update_msg(text, 0, streaming=False)
     else:
         text, docs = llm.chat(query)
         chat_box.ai_say(
             [
                 Markdown(text, in_expander=in_expander,
                          expanded=True, title="answer"),
                 Markdown("\n\n".join(docs), in_expander=in_expander,
```

## Comparing `streamlit_chatbox-1.0.1.dist-info/RECORD` & `streamlit_chatbox-1.1.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 streamlit_chatbox/__init__.py,sha256=okS4bZ1sk5ma0Nawlw07pLxVR_INKIqCQQFqvzkzR4A,392
-streamlit_chatbox/elements.py,sha256=rC12Gv0WrZVKMPIh61KIBdw6fkuMM4I4V6FSKHV21Z8,4563
+streamlit_chatbox/elements.py,sha256=G5qNHFANT_KgLtZ9BMDZ7rcCFx6gmoeXaomMfF-3iFU,4431
 streamlit_chatbox/flows.py,sha256=RvtStf1em9vGPp_sj8V7xHKbBiI5_p58RAFuvEMq2-c,323
-streamlit_chatbox/messages.py,sha256=Kgt9ek-EA_CpmDK4kLQfo6yJk1ew19Qfzpk0tRDECGY,3655
-streamlit_chatbox-1.0.1.dist-info/METADATA,sha256=By1JclVTh14N6FqrHoJ4MSfptNys5C-QTskOcaVBvsk,4452
-streamlit_chatbox-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-streamlit_chatbox-1.0.1.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
-streamlit_chatbox-1.0.1.dist-info/RECORD,,
+streamlit_chatbox/messages.py,sha256=U549KtBonkt6yOYvbkymCcHl640P-HEAmEv2WPa-2Es,4423
+streamlit_chatbox-1.1.0.dist-info/METADATA,sha256=UxBfVIzIRlyy0eKCN0Z33DbnxwhQe0ziyD22hqchWTM,4417
+streamlit_chatbox-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+streamlit_chatbox-1.1.0.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
+streamlit_chatbox-1.1.0.dist-info/RECORD,,
```

