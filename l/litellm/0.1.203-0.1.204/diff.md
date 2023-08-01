# Comparing `tmp/litellm-0.1.203.tar.gz` & `tmp/litellm-0.1.204.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.203.tar", last modified: Mon Jul 31 20:25:56 2023, max compression
+gzip compressed data, was "litellm-0.1.204.tar", last modified: Tue Aug  1 00:48:52 2023, max compression
```

## Comparing `litellm-0.1.203.tar` & `litellm-0.1.204.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:25:56.800485 litellm-0.1.203/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 20:25:42.000000 litellm-0.1.203/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 20:25:56.800485 litellm-0.1.203/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-31 20:25:42.000000 litellm-0.1.203/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:25:56.800485 litellm-0.1.203/litellm/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 20:25:42.000000 litellm-0.1.203/litellm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-07-31 20:25:42.000000 litellm-0.1.203/litellm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:25:56.800485 litellm-0.1.203/litellm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 20:25:56.000000 litellm-0.1.203/litellm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 20:25:56.000000 litellm-0.1.203/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:25:56.000000 litellm-0.1.203/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-31 20:25:56.000000 litellm-0.1.203/litellm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 20:25:56.000000 litellm-0.1.203/litellm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:25:56.800485 litellm-0.1.203/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 20:25:42.000000 litellm-0.1.203/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:48:52.024226 litellm-0.1.204/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 00:48:29.000000 litellm-0.1.204/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 00:48:52.024226 litellm-0.1.204/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-01 00:48:29.000000 litellm-0.1.204/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:48:52.024226 litellm-0.1.204/litellm/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 00:48:29.000000 litellm-0.1.204/litellm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19254 2023-08-01 00:48:29.000000 litellm-0.1.204/litellm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:48:52.024226 litellm-0.1.204/litellm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:48:52.024226 litellm-0.1.204/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 00:48:29.000000 litellm-0.1.204/setup.py
```

### Comparing `litellm-0.1.203/LICENSE` & `litellm-0.1.204/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.203/README.md` & `litellm-0.1.204/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.203/litellm/main.py` & `litellm-0.1.204/litellm/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -78,42 +78,127 @@
         except Exception as e:
           traceback_exception = traceback.format_exc()
           my_thread = threading.Thread(target=handle_failure, args=(e, traceback.format_exc(), args, kwargs)) # don't interrupt execution of main thread
           my_thread.start()
           raise e
     return wrapper
 
+
+def get_optional_params(
+    # 12 optional params
+    functions = [],
+    function_call = "",
+    temperature = 1,
+    top_p = 1,
+    n = 1,
+    stream = False,
+    stop = None,
+    max_tokens = float('inf'),
+    presence_penalty = 0,
+    frequency_penalty = 0,
+    logit_bias = {},
+    user = "",
+):
+  optional_params = {}
+  if functions != []:
+      optional_params["functions"] = functions
+  if function_call != "":
+      optional_params["function_call"] = function_call
+  if temperature != 1:
+      optional_params["temperature"] = temperature
+  if top_p != 1:
+      optional_params["top_p"] = top_p
+  if n != 1:
+      optional_params["n"] = n
+  if stream:
+      optional_params["stream"] = stream
+  if stop != None:
+      optional_params["stop"] = stop
+  if max_tokens != float('inf'):
+      optional_params["max_tokens"] = max_tokens
+  if presence_penalty != 0:
+      optional_params["presence_penalty"] = presence_penalty
+  if frequency_penalty != 0:
+      optional_params["frequency_penalty"] = frequency_penalty
+  if logit_bias != {}:
+      optional_params["logit_bias"] = logit_bias
+  if user != "":
+      optional_params["user"] = user
+  return optional_params
+
 ####### COMPLETION ENDPOINTS ################
 #############################################
 @client
-@func_set_timeout(60, allowOverride=True) ## https://pypi.org/project/func-timeout/ - timeouts, in case calls hang (e.g. Azure)
-def completion(model, messages, max_tokens=None, *, forceTimeout=60, azure=False, logger_fn=None): # ,*,.. requires optional params like forceTimeout, azure and logger_fn to be passed in as keyword arguments
+@func_set_timeout(180, allowOverride=True) ## https://pypi.org/project/func-timeout/ - timeouts, in case calls hang (e.g. Azure)
+def completion(
+    model, messages, # required params
+    # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
+    functions=[], function_call="", # optional params
+    temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
+    presence_penalty=0, frequency_penalty=0, logit_bias={}, user="",
+    # Optional liteLLM function params
+    *, forceTimeout=60, azure=False, logger_fn=None, verbose=False
+  ):
   try:
+    # check if user passed in any of the OpenAI optional params
+    optional_params = get_optional_params(
+      functions=functions, function_call=function_call, 
+      temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
+      presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user
+    )
     if azure == True:
       # azure configs
       openai.api_type = "azure"
       openai.api_base = os.environ.get("AZURE_API_BASE")
       openai.api_version = os.environ.get("AZURE_API_VERSION")
       openai.api_key = os.environ.get("AZURE_API_KEY")
       ## LOGGING
-      logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
+      logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = openai.ChatCompletion.create(
         engine=model,
-        messages = messages
+        messages = messages,
+        **optional_params
+      )
+    elif model in open_ai_chat_completion_models:
+      openai.api_type = "openai"
+      openai.api_base = "https://api.openai.com/v1"
+      openai.api_version = None
+      openai.api_key = os.environ.get("OPENAI_API_KEY")
+      ## LOGGING
+      logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
+
+      ## COMPLETION CALL
+      response = openai.ChatCompletion.create(
+        model=model,
+        messages = messages,
+        **optional_params
+      )
+    elif model in open_ai_text_completion_models:
+      openai.api_type = "openai"
+      openai.api_base = "https://api.openai.com/v1"
+      openai.api_version = None
+      openai.api_key = os.environ.get("OPENAI_API_KEY")
+      prompt = " ".join([message["content"] for message in messages])
+      ## LOGGING
+      logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
+      ## COMPLETION CALL
+      response = openai.Completion.create(
+          model=model,
+          prompt = prompt
       )
-    elif "replicate" in model: 
+    elif "replicate" in model:
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
       if not os.environ.get("REPLICATE_API_TOKEN") and  os.environ.get("REPLICATE_API_KEY"):
         replicate_api_token = os.environ.get("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
       prompt = " ".join([message["content"] for message in messages])
       input = {"prompt": prompt}
-      if max_tokens:
+      if max_tokens != float('inf'):
         input["max_length"] = max_tokens # for t5 models 
         input["max_new_tokens"] = max_tokens # for llama2 models 
       ## LOGGING
       logging(model=model, input=input, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
       ## COMPLETION CALL
       output = replicate.run(
         model,
@@ -143,17 +228,18 @@
             prompt += f"{HUMAN_PROMPT}{message['content']}"
           else:
             prompt += f"{AI_PROMPT}{message['content']}"
         else:
           prompt += f"{HUMAN_PROMPT}{message['content']}"
       prompt += f"{AI_PROMPT}"
       anthropic = Anthropic()
-      if max_tokens:
+      # check if user passed in max_tokens != float('inf')
+      if max_tokens != float('inf'):
         max_tokens_to_sample = max_tokens
-      else: 
+      else:
         max_tokens_to_sample = 300 # default in Anthropic docs https://docs.anthropic.com/claude/reference/client-libraries
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
       ## COMPLETION CALL
       completion = anthropic.completions.create(
           model=model,
           prompt=prompt,
@@ -193,42 +279,16 @@
                       "content": response[0],
                       "role": "assistant"
                   }
               }
           ],
       }
       response = new_response
-
-    elif model in open_ai_chat_completion_models:
-      openai.api_type = "openai"
-      openai.api_base = "https://api.openai.com/v1"
-      openai.api_version = None
-      openai.api_key = os.environ.get("OPENAI_API_KEY")
-      ## LOGGING
-      logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
-      ## COMPLETION CALL
-      response = openai.ChatCompletion.create(
-          model=model,
-          messages = messages
-      )
-    elif model in open_ai_text_completion_models:
-      openai.api_type = "openai"
-      openai.api_base = "https://api.openai.com/v1"
-      openai.api_version = None
-      openai.api_key = os.environ.get("OPENAI_API_KEY")
-      prompt = " ".join([message["content"] for message in messages])
-      ## LOGGING
-      logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
-      ## COMPLETION CALL
-      response = openai.Completion.create(
-          model=model,
-          prompt = prompt
-      )
-    else: 
-      logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
+    else:
+      raise Exception(f"Model '{model}' not found. Please check your model name and try again.")
     return response
   except Exception as e:
     logging(model=model, input=messages, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
     raise e
 
 
 ### EMBEDDING ENDPOINTS ####################
```

