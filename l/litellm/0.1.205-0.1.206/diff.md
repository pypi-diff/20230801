# Comparing `tmp/litellm-0.1.205.tar.gz` & `tmp/litellm-0.1.206.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.205.tar", last modified: Tue Aug  1 01:52:10 2023, max compression
+gzip compressed data, was "litellm-0.1.206.tar", last modified: Tue Aug  1 18:36:17 2023, max compression
```

## Comparing `litellm-0.1.205.tar` & `litellm-0.1.206.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:52:10.700031 litellm-0.1.205/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 01:51:52.000000 litellm-0.1.205/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 01:52:10.700031 litellm-0.1.205/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-01 01:51:52.000000 litellm-0.1.205/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:52:10.700031 litellm-0.1.205/litellm/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-01 01:51:52.000000 litellm-0.1.205/litellm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-08-01 01:51:52.000000 litellm-0.1.205/litellm/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-08-01 01:51:52.000000 litellm-0.1.205/litellm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:52:10.700031 litellm-0.1.205/litellm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:52:10.700031 litellm-0.1.205/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 01:51:52.000000 litellm-0.1.205/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:17.224927 litellm-0.1.206/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 18:36:00.000000 litellm-0.1.206/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 18:36:17.220927 litellm-0.1.206/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-01 18:36:00.000000 litellm-0.1.206/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:17.220927 litellm-0.1.206/litellm/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-01 18:36:00.000000 litellm-0.1.206/litellm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-08-01 18:36:00.000000 litellm-0.1.206/litellm/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-08-01 18:36:00.000000 litellm-0.1.206/litellm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:17.220927 litellm-0.1.206/litellm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:36:17.224927 litellm-0.1.206/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 18:36:00.000000 litellm-0.1.206/setup.py
```

### Comparing `litellm-0.1.205/LICENSE` & `litellm-0.1.206/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.205/README.md` & `litellm-0.1.206/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,23 @@
 
 a simple & light 100 line package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
 - guarantees consistent output, text responses will always be available at `['choices'][0]['message']['content']`
 
-Read the docs - https://litellm.readthedocs.io/en/latest/
 # usage
-## installation
-```
-pip install litellm
-```
 
-Stable version
+Read the docs - https://litellm.readthedocs.io/en/latest/
+
+## quick start
 ```
-pip install litellm==0.1.1
+pip install litellm
 ```
 
-* Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
 ```python
 from litellm import completion
 
 ## set ENV variables
 # ENV variables can be set in .env file, too. Example in .env.example
 os.environ["OPENAI_API_KEY"] = "openai key"
 os.environ["COHERE_API_KEY"] = "cohere key"
@@ -43,14 +39,20 @@
 
 # azure openai call
 response = completion("chatgpt-test", messages, azure=True)
 
 # openrouter call
 response = completion("google/palm-2-codechat-bison", messages)
 ```
+Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
+
+Stable version
+```
+pip install litellm==0.1.1
+```
 
 # hosted version
 - [Grab time if you want access 👋](https://calendly.com/d/4mp-gd3-k5k/berriai-1-1-onboarding-litellm-hosted-version)
 
 # why did I build this 
 - **Need for simplicity**: My code started to get extremely complicated managing & translating calls between Azure, OpenAI, Cohere
```

### Comparing `litellm-0.1.205/litellm/__init__.py` & `litellm-0.1.206/litellm/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 ]
 
 ####### EMBEDDING MODELS ###################
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
 
-from .utils import client, logging  # Import all the symbols from main.py
+from .utils import client, logging, exception_type  # Import all the symbols from main.py
 from .main import *  # Import all the symbols from main.py
```

### Comparing `litellm-0.1.205/litellm/main.py` & `litellm-0.1.206/litellm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any
 from func_timeout import func_set_timeout, FunctionTimedOut
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 import traceback
 import dotenv
 import traceback
 import litellm
-from litellm import client, logging
+from litellm import client, logging, exception_type
 from litellm import success_callback, failure_callback
 import random
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
 
 
@@ -116,15 +116,15 @@
       response = openai.Completion.create(
           model=model,
           prompt = prompt
       )
     elif "replicate" in model:
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
-      if not os.environ.get("REPLICATE_API_TOKEN") and  os.environ.get("REPLICATE_API_KEY"):
+      if not os.environ.get("REPLICATE_API_TOKEN") and os.environ.get("REPLICATE_API_KEY"):
         replicate_api_token = os.environ.get("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
       prompt = " ".join([message["content"] for message in messages])
       input = {"prompt": prompt}
       if max_tokens != float('inf'):
         input["max_length"] = max_tokens # for t5 models 
         input["max_new_tokens"] = max_tokens # for llama2 models 
@@ -203,15 +203,15 @@
       )
       new_response = {
           "choices": [
               {
                   "finish_reason": "stop",
                   "index": 0,
                   "message": {
-                      "content": response[0],
+                      "content": response[0].text,
                       "role": "assistant"
                   }
               }
           ],
       }
       response = new_response
 
@@ -242,16 +242,18 @@
       )
     else: 
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       args = locals()
       raise ValueError(f"No valid completion model args passed in - {args}")
     return response
   except Exception as e:
-    logging(model=model, input=messages, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
-    raise e
+    # log the original exception
+    logging(model=model, input=messages, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn, exception=e)
+    ## Map to OpenAI Exception
+    raise exception_type(model=model, original_exception=e)
 
 
 ### EMBEDDING ENDPOINTS ####################
 @client
 @func_set_timeout(60, allowOverride=True) ## https://pypi.org/project/func-timeout/
 def embedding(model, input=[], azure=False, forceTimeout=60, logger_fn=None):
   response = None
```

