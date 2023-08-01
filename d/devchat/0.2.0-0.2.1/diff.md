# Comparing `tmp/devchat-0.2.0.tar.gz` & `tmp/devchat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.2.0.tar", max compression
+gzip compressed data, was "devchat-0.2.1.tar", max compression
```

## Comparing `devchat-0.2.0.tar` & `devchat-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-07-05 11:57:19.300520 devchat-0.2.0/LICENSE
--rw-r--r--   0        0        0     5267 2023-07-13 11:26:05.138364 devchat-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 11:57:31.893875 devchat-0.2.0/devchat/__init__.py
--rw-r--r--   0        0        0     9475 2023-07-22 04:20:24.586852 devchat-0.2.0/devchat/_cli.py
--rw-r--r--   0        0        0     4503 2023-07-21 16:39:59.449026 devchat-0.2.0/devchat/assistant.py
--rw-r--r--   0        0        0     1676 2023-07-21 16:39:59.449400 devchat-0.2.0/devchat/chat.py
--rw-r--r--   0        0        0      758 2023-07-23 12:18:04.254562 devchat-0.2.0/devchat/message.py
--rw-r--r--   0        0        0      248 2023-07-05 11:57:51.466105 devchat-0.2.0/devchat/openai/__init__.py
--rw-r--r--   0        0        0     3558 2023-07-23 12:18:04.254963 devchat-0.2.0/devchat/openai/openai_chat.py
--rw-r--r--   0        0        0     3293 2023-07-23 12:18:04.255359 devchat-0.2.0/devchat/openai/openai_message.py
--rw-r--r--   0        0        0    10706 2023-07-23 12:18:04.255807 devchat-0.2.0/devchat/openai/openai_prompt.py
--rw-r--r--   0        0        0     8874 2023-07-21 16:39:59.450857 devchat-0.2.0/devchat/prompt.py
--rw-r--r--   0        0        0     9872 2023-07-23 12:18:04.256202 devchat-0.2.0/devchat/store.py
--rw-r--r--   0        0        0     6778 2023-07-23 02:09:55.769806 devchat-0.2.0/devchat/utils.py
--rw-r--r--   0        0        0     1154 2023-07-23 12:25:42.216663 devchat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6557 1970-01-01 00:00:00.000000 devchat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 11:57:19.300520 devchat-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5267 2023-07-13 11:26:05.138364 devchat-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 11:57:31.893875 devchat-0.2.1/devchat/__init__.py
+-rw-r--r--   0        0        0     9493 2023-08-01 05:53:42.349789 devchat-0.2.1/devchat/_cli.py
+-rw-r--r--   0        0        0     4503 2023-07-21 16:39:59.449026 devchat-0.2.1/devchat/assistant.py
+-rw-r--r--   0        0        0     1676 2023-07-21 16:39:59.449400 devchat-0.2.1/devchat/chat.py
+-rw-r--r--   0        0        0      758 2023-07-23 12:18:04.254562 devchat-0.2.1/devchat/message.py
+-rw-r--r--   0        0        0      248 2023-07-05 11:57:51.466105 devchat-0.2.1/devchat/openai/__init__.py
+-rw-r--r--   0        0        0     3558 2023-07-31 23:46:29.233957 devchat-0.2.1/devchat/openai/openai_chat.py
+-rw-r--r--   0        0        0     3293 2023-07-23 12:18:04.255359 devchat-0.2.1/devchat/openai/openai_message.py
+-rw-r--r--   0        0        0    10686 2023-08-01 05:53:42.350169 devchat-0.2.1/devchat/openai/openai_prompt.py
+-rw-r--r--   0        0        0     8953 2023-08-01 05:53:42.350409 devchat-0.2.1/devchat/prompt.py
+-rw-r--r--   0        0        0     9872 2023-07-23 12:18:04.256202 devchat-0.2.1/devchat/store.py
+-rw-r--r--   0        0        0     6821 2023-08-01 05:53:42.350632 devchat-0.2.1/devchat/utils.py
+-rw-r--r--   0        0        0     1154 2023-08-01 05:53:42.350865 devchat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6557 1970-01-01 00:00:00.000000 devchat-0.2.1/PKG-INFO
```

### Comparing `devchat-0.2.0/LICENSE` & `devchat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/README.md` & `devchat-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/devchat/_cli.py` & `devchat-0.2.1/devchat/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,16 +174,16 @@
             if 'tokens-per-prompt' in config:
                 assistant.token_limit = config['tokens-per-prompt']
 
             functions_data = None
             if functions is not None:
                 with open(functions, 'r', encoding="utf-8") as f_file:
                     functions_data = json.load(f_file)
-            assistant.make_prompt(content, instruct_contents, context_contents,
-                                  functions_data, parent, reference,
+            assistant.make_prompt(content, instruct_contents, context_contents, functions_data,
+                                  parent=parent, references=reference,
                                   function_name=function_name)
 
             for response in assistant.iterate_response():
                 click.echo(response, nl=False)
         else:
             click.echo(f"Error: Invalid LLM in configuration '{provider}'", err=True)
             sys.exit(os.EX_DATAERR)
```

### Comparing `devchat-0.2.0/devchat/assistant.py` & `devchat-0.2.1/devchat/assistant.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/devchat/chat.py` & `devchat-0.2.1/devchat/chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/devchat/message.py` & `devchat-0.2.1/devchat/message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/devchat/openai/openai_chat.py` & `devchat-0.2.1/devchat/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/devchat/openai/openai_message.py` & `devchat-0.2.1/devchat/openai/openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/devchat/openai/openai_prompt.py` & `devchat-0.2.1/devchat/openai/openai_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 import json
 import math
 from typing import List, Optional
 from devchat.prompt import Prompt
 from devchat.message import Message
 from devchat.utils import update_dict, get_logger
-from devchat.utils import message_tokens, response_tokens
+from devchat.utils import openai_message_tokens, openai_response_tokens
 from .openai_message import OpenAIMessage
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class OpenAIPrompt(Prompt):
@@ -44,16 +44,19 @@
         if self.new_context:
             combined += [update_dict(msg.to_dict(), 'content',
                                      f"<context>\n{msg.content}\n</context>")
                          for msg in self.new_context]
         return combined
 
     def input_messages(self, messages: List[dict]):
+        self._request_tokens = 0
         state = "new_instruct"
         for message_data in messages:
+            self._request_tokens += openai_message_tokens(message_data, self.model)
+
             message = OpenAIMessage.from_dict(message_data)
 
             if state == "new_instruct":
                 if message.role == "system" and not message.content.startswith("<context>"):
                     self._new_messages[Message.INSTRUCT].append(message)
                 else:
                     state = "history_context"
@@ -90,39 +93,39 @@
     def append_new(self, message_type: str, content: str,
                    available_tokens: int = math.inf) -> bool:
         if message_type not in (Message.INSTRUCT, Message.CONTEXT):
             raise ValueError(f"Current messages cannot be of type {message_type}.")
         # New instructions and context are of the system role
         message = OpenAIMessage(content=content, role='system')
 
-        num_tokens = message_tokens(message.to_dict(), self.model)
+        num_tokens = openai_message_tokens(message.to_dict(), self.model)
         if num_tokens > available_tokens:
             return False
 
         self._new_messages[message_type].append(message)
         self._request_tokens += num_tokens
         return True
 
     def set_functions(self, functions, available_tokens: int = math.inf):
-        num_tokens = message_tokens({"functions": json.dumps(functions)}, self.model)
+        num_tokens = openai_message_tokens({"functions": json.dumps(functions)}, self.model)
         if num_tokens > available_tokens:
             return False
 
         self._new_messages[Message.FUNCTION] = functions
         self._request_tokens += num_tokens
         return True
 
     def get_functions(self):
         return self._new_messages.get(Message.FUNCTION, None)
 
     def _prepend_history(self, message_type: str, message: Message,
                          token_limit: int = math.inf) -> bool:
         if message_type == Message.INSTRUCT:
             raise ValueError("History messages cannot be of type INSTRUCT.")
-        num_tokens = message_tokens(message.to_dict(), self.model)
+        num_tokens = openai_message_tokens(message.to_dict(), self.model)
         if num_tokens > token_limit - self._request_tokens:
             return False
         self._history_messages[message_type].insert(0, message)
         self._request_tokens += num_tokens
         return True
 
     def prepend_history(self, prompt: 'OpenAIPrompt', token_limit: int = math.inf) -> bool:
@@ -141,15 +144,15 @@
     def set_request(self, content: str, function_name: Optional[str] = None) -> int:
         if not content.strip():
             raise ValueError("The request cannot be empty.")
         message = OpenAIMessage(content=content,
                                 role=('user' if not function_name else 'function'),
                                 name=function_name)
         self._new_messages['request'] = message
-        self._request_tokens += message_tokens(message.to_dict(), self.model)
+        self._request_tokens += openai_message_tokens(message.to_dict(), self.model)
 
     def set_response(self, response_str: str):
         """
         Parse the API response string and set the Prompt object's attributes.
 
         Args:
             response_str (str): The JSON-formatted response string from the chat API.
@@ -217,22 +220,15 @@
                             delta['function_call']['arguments']
 
             if finish_reason:
                 self._response_reasons[index] = finish_reason
         return delta_content
 
     def _count_response_tokens(self) -> int:
-        if self._response_tokens:
-            return self._response_tokens
-
-        total = 0
-        for response_message in self.responses:
-            total += response_tokens(response_message.to_dict(), self.model)
-        self._response_tokens = total
-        return total
+        return sum(openai_response_tokens(resp.to_dict(), self.model) for resp in self.responses)
 
     def _validate_model(self, response_data: dict):
         if not response_data['model'].startswith(self.model):
             raise ValueError(f"Model mismatch: expected '{self.model}', "
                              f"got '{response_data['model']}'")
 
     def _timestamp_from_dict(self, response_data: dict):
```

### Comparing `devchat-0.2.0/devchat/prompt.py` & `devchat-0.2.1/devchat/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,24 +46,24 @@
     references: List[str] = field(default_factory=list)
     _timestamp: int = None
     _request_tokens: int = 0
     _response_tokens: int = 0
     _response_reasons: List[str] = field(default_factory=list)
     _hash: str = None
 
-    def _check_complete(self) -> bool:
+    def _complete_for_hash(self) -> bool:
         """
         Check if the prompt is complete for hashing.
 
         Returns:
             bool: Whether the prompt is complete.
         """
-        if not self.request or not self._request_tokens or not self.responses:
-            logger.warning("Incomplete prompt: request = %s (%d), response = %s",
-                           self.request, self._request_tokens, self.responses)
+        if not self.request or not self.responses:
+            logger.warning("Incomplete prompt: request = %s, response = %s",
+                           self.request, self.responses)
             return False
 
         if not self._response_tokens:
             return False
 
         return True
 
@@ -85,14 +85,16 @@
 
     @property
     def request_tokens(self) -> int:
         return self._request_tokens
 
     @property
     def response_tokens(self) -> int:
+        if not self._response_tokens:
+            self._response_tokens = self._count_response_tokens()
         return self._response_tokens
 
     @abstractmethod
     def _count_response_tokens(self) -> int:
         """
         Calculate the number of tokens used in the responses.
         """
@@ -179,21 +181,21 @@
     def finalize_hash(self) -> str:
         """
         Calculate and set the hash of the prompt.
 
         Returns:
             str: The hash of the prompt. None if the prompt is incomplete.
         """
-        if not self._check_complete():
+        if not self._complete_for_hash():
             self._hash = None
 
         if self._hash:
             return self._hash
 
-        self._count_response_tokens()
+        self._response_tokens = self._count_response_tokens()
 
         data = asdict(self)
         data.pop('_hash')
         string = str(tuple(sorted(data.items())))
         self._hash = hashlib.sha256(string.encode('utf-8')).hexdigest()
         return self._hash
```

### Comparing `devchat-0.2.0/devchat/store.py` & `devchat-0.2.1/devchat/store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.0/devchat/utils.py` & `devchat-0.2.1/devchat/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """
     Update a dictionary with a key-value pair and return the dictionary.
     """
     dict_to_update[key] = value
     return dict_to_update
 
 
-def message_tokens(message: dict, model: str) -> int:
+def openai_message_tokens(message: dict, model: str) -> int:
     """Returns the number of tokens used by a message."""
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError as err:
         raise ValueError(f"Invalid model {model} for tiktoken.") from err
 
     num_tokens = 0
@@ -187,16 +187,17 @@
     else:
         num_tokens += 3
         tokens_per_name = 1
 
     for key, value in message.items():
         if key == 'function_call':
             value = json.dumps(value)
-        num_tokens += len(encoding.encode(value))
+        if value:
+            num_tokens += len(encoding.encode(value))
         if key == "name":
             num_tokens += tokens_per_name
     return num_tokens
 
 
-def response_tokens(message: dict, model: str) -> int:
+def openai_response_tokens(message: dict, model: str) -> int:
     """Returns the number of tokens used by a response."""
-    return message_tokens(message, model)
+    return openai_message_tokens(message, model)
```

### Comparing `devchat-0.2.0/pyproject.toml` & `devchat-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devchat"
-version = "0.2.0"
+version = "0.2.1"
 description = "DevChat is an open-source tool that helps developers write prompts to generate code and documentation."
 authors = ["DevChat Team <hello@devchat.ai>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/devchat-ai/devchat"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `devchat-0.2.0/PKG-INFO` & `devchat-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat
-Version: 0.2.0
+Version: 0.2.1
 Summary: DevChat is an open-source tool that helps developers write prompts to generate code and documentation.
 Home-page: https://github.com/devchat-ai/devchat
 License: Apache-2.0
 Author: DevChat Team
 Author-email: hello@devchat.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

