# Comparing `tmp/litellm-0.1.206.tar.gz` & `tmp/litellm-0.1.207.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.206.tar", last modified: Tue Aug  1 18:36:17 2023, max compression
+gzip compressed data, was "litellm-0.1.207.tar", last modified: Tue Aug  1 21:45:31 2023, max compression
```

## Comparing `litellm-0.1.206.tar` & `litellm-0.1.207.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:17.224927 litellm-0.1.206/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 18:36:00.000000 litellm-0.1.206/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 18:36:17.220927 litellm-0.1.206/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-01 18:36:00.000000 litellm-0.1.206/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:17.220927 litellm-0.1.206/litellm/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-01 18:36:00.000000 litellm-0.1.206/litellm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-08-01 18:36:00.000000 litellm-0.1.206/litellm/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-08-01 18:36:00.000000 litellm-0.1.206/litellm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:17.220927 litellm-0.1.206/litellm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 18:36:17.000000 litellm-0.1.206/litellm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:36:17.224927 litellm-0.1.206/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 18:36:00.000000 litellm-0.1.206/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:45:31.413084 litellm-0.1.207/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 21:45:15.000000 litellm-0.1.207/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 21:45:31.413084 litellm-0.1.207/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-01 21:45:15.000000 litellm-0.1.207/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:45:31.409083 litellm-0.1.207/litellm/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:45:31.413084 litellm-0.1.207/litellm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:45:31.413084 litellm-0.1.207/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 21:45:15.000000 litellm-0.1.207/setup.py
```

### Comparing `litellm-0.1.206/LICENSE` & `litellm-0.1.207/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.206/README.md` & `litellm-0.1.207/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # *🚅 litellm*
 [![PyPI Version](https://img.shields.io/pypi/v/litellm.svg)](https://pypi.org/project/litellm/)
 [![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.1-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/BerriAI/litellm/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/BerriAI/litellm/tree/main)
 [![ New Relea Tests](https://github.com/BerriAI/litellm/actions/workflows/tests.yml/badge.svg)](https://github.com/BerriAI/litellm/actions/workflows/tests.yml)
 [![Publish to PyPI](https://github.com/BerriAI/litellm/actions/workflows/publish_pypi.yml/badge.svg?branch=main)](https://github.com/BerriAI/litellm/actions/workflows/publish_pypi.yml) ![Downloads](https://img.shields.io/pypi/dm/litellm)
 
 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 a simple & light 100 line package to call OpenAI, Azure, Cohere, Anthropic API Endpoints
```

### Comparing `litellm-0.1.206/litellm/__init__.py` & `litellm-0.1.207/litellm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 ]
 
 ####### EMBEDDING MODELS ###################
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
 
+from .timeout import timeout
 from .utils import client, logging, exception_type  # Import all the symbols from main.py
 from .main import *  # Import all the symbols from main.py
```

### Comparing `litellm-0.1.206/litellm/main.py` & `litellm-0.1.207/litellm/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import os, openai, cohere, replicate, sys
 from typing import Any
-from func_timeout import func_set_timeout, FunctionTimedOut
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 import traceback
 import dotenv
 import traceback
 import litellm
-from litellm import client, logging, exception_type
-from litellm import success_callback, failure_callback
+from litellm import client, logging, exception_type, timeout, success_callback, failure_callback
 import random
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
-
-
 def get_optional_params(
     # 12 optional params
     functions = [],
     function_call = "",
     temperature = 1,
     top_p = 1,
     n = 1,
@@ -55,23 +51,23 @@
   if user != "":
       optional_params["user"] = user
   return optional_params
 
 ####### COMPLETION ENDPOINTS ################
 #############################################
 @client
-@func_set_timeout(180, allowOverride=True) ## https://pypi.org/project/func-timeout/ - timeouts, in case calls hang (e.g. Azure)
+@timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def completion(
     model, messages, # required params
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     functions=[], function_call="", # optional params
     temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
     presence_penalty=0, frequency_penalty=0, logit_bias={}, user="",
     # Optional liteLLM function params
-    *, forceTimeout=60, azure=False, logger_fn=None, verbose=False
+    *, force_timeout=60, azure=False, logger_fn=None, verbose=False
   ):
   try:
     # check if user passed in any of the OpenAI optional params
     optional_params = get_optional_params(
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user
@@ -250,16 +246,16 @@
     logging(model=model, input=messages, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn, exception=e)
     ## Map to OpenAI Exception
     raise exception_type(model=model, original_exception=e)
 
 
 ### EMBEDDING ENDPOINTS ####################
 @client
-@func_set_timeout(60, allowOverride=True) ## https://pypi.org/project/func-timeout/
-def embedding(model, input=[], azure=False, forceTimeout=60, logger_fn=None):
+@timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
+def embedding(model, input=[], azure=False, force_timeout=60, logger_fn=None):
   response = None
   if azure == True:
     # azure configs
     openai.api_type = "azure"
     openai.api_base = os.environ.get("AZURE_API_BASE")
     openai.api_version = os.environ.get("AZURE_API_VERSION")
     openai.api_key = os.environ.get("AZURE_API_KEY")
```

### Comparing `litellm-0.1.206/litellm/utils.py` & `litellm-0.1.207/litellm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,138 +97,147 @@
           my_thread.start()
           raise e
     return wrapper
 
 ####### HELPER FUNCTIONS ################
 def set_callbacks(callback_list):
   global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel
-  for callback in callback_list:
-    if callback == "sentry":
-      try:
-          import sentry_sdk
-      except ImportError:
-          print_verbose("Package 'sentry_sdk' is missing. Installing it...")
-          subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'sentry_sdk'])
-          import sentry_sdk
-      sentry_sdk_instance = sentry_sdk
-      sentry_sdk_instance.init(dsn=os.environ.get("SENTRY_API_URL"), traces_sample_rate=float(os.environ.get("SENTRY_API_TRACE_RATE")))
-      capture_exception = sentry_sdk_instance.capture_exception
-      add_breadcrumb = sentry_sdk_instance.add_breadcrumb 
-    elif callback == "posthog":
-      try:
-          from posthog import Posthog
-      except ImportError:
-          print_verbose("Package 'posthog' is missing. Installing it...")
-          subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'posthog'])
-          from posthog import Posthog
-      posthog = Posthog(
-        project_api_key=os.environ.get("POSTHOG_API_KEY"),
-        host=os.environ.get("POSTHOG_API_URL"))
-    elif callback == "slack":
-      try:
-          from slack_bolt import App
-      except ImportError:
-          print_verbose("Package 'slack_bolt' is missing. Installing it...")
-          subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'slack_bolt'])
-          from slack_bolt import App
-      slack_app = App(
-        token=os.environ.get("SLACK_API_TOKEN"),
-        signing_secret=os.environ.get("SLACK_API_SECRET")
-      )
-      alerts_channel = os.environ["SLACK_API_CHANNEL"]
-      print_verbose(f"Initialized Slack App: {slack_app}")
+  try:
+    for callback in callback_list:
+      if callback == "sentry":
+        try:
+            import sentry_sdk
+        except ImportError:
+            print_verbose("Package 'sentry_sdk' is missing. Installing it...")
+            subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'sentry_sdk'])
+            import sentry_sdk
+        sentry_sdk_instance = sentry_sdk
+        sentry_sdk_instance.init(dsn=os.environ.get("SENTRY_API_URL"), traces_sample_rate=float(os.environ.get("SENTRY_API_TRACE_RATE")))
+        capture_exception = sentry_sdk_instance.capture_exception
+        add_breadcrumb = sentry_sdk_instance.add_breadcrumb 
+      elif callback == "posthog":
+        try:
+            from posthog import Posthog
+        except ImportError:
+            print_verbose("Package 'posthog' is missing. Installing it...")
+            subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'posthog'])
+            from posthog import Posthog
+        posthog = Posthog(
+          project_api_key=os.environ.get("POSTHOG_API_KEY"),
+          host=os.environ.get("POSTHOG_API_URL"))
+      elif callback == "slack":
+        try:
+            from slack_bolt import App
+        except ImportError:
+            print_verbose("Package 'slack_bolt' is missing. Installing it...")
+            subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'slack_bolt'])
+            from slack_bolt import App
+        slack_app = App(
+          token=os.environ.get("SLACK_API_TOKEN"),
+          signing_secret=os.environ.get("SLACK_API_SECRET")
+        )
+        alerts_channel = os.environ["SLACK_API_CHANNEL"]
+        print_verbose(f"Initialized Slack App: {slack_app}")
+  except:
+    pass
 
 
 def handle_failure(exception, traceback_exception, args, kwargs):
     global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel
-    print_verbose(f"handle_failure args: {args}")
-    print_verbose(f"handle_failure kwargs: {kwargs}")
-    
+    try:
+      print_verbose(f"handle_failure args: {args}")
+      print_verbose(f"handle_failure kwargs: {kwargs}")
+      
+      success_handler = additional_details.pop("success_handler", None)
+      failure_handler = additional_details.pop("failure_handler", None)
+      
+      additional_details["Event_Name"] = additional_details.pop("failed_event_name", "litellm.failed_query")
+      print_verbose(f"self.failure_callback: {litellm.failure_callback}")
+
+      print_verbose(f"additional_details: {additional_details}")
+      for callback in litellm.failure_callback:
+        try:
+          if callback == "slack":
+            slack_msg = "" 
+            if len(kwargs) > 0: 
+              for key in kwargs: 
+                slack_msg += f"{key}: {kwargs[key]}\n"
+            if len(args) > 0:
+              for i, arg in enumerate(args):
+                slack_msg += f"LiteLLM_Args_{str(i)}: {arg}"
+            for detail in additional_details: 
+              slack_msg += f"{detail}: {additional_details[detail]}\n"
+            slack_msg += f"Traceback: {traceback_exception}"
+            slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
+          elif callback == "sentry":
+            capture_exception(exception)
+          elif callback == "posthog": 
+            print_verbose(f"inside posthog, additional_details: {len(additional_details.keys())}")
+            ph_obj = {}
+            if len(kwargs) > 0: 
+              ph_obj = kwargs
+            if len(args) > 0:
+              for i, arg in enumerate(args):
+                ph_obj["litellm_args_" + str(i)] = arg
+            for detail in additional_details:
+              ph_obj[detail] = additional_details[detail]
+            event_name = additional_details["Event_Name"]
+            print_verbose(f"ph_obj: {ph_obj}")
+            print_verbose(f"PostHog Event Name: {event_name}")
+            if "user_id" in additional_details:
+              posthog.capture(additional_details["user_id"], event_name, ph_obj)
+            else: # PostHog calls require a unique id to identify a user - https://posthog.com/docs/libraries/python
+              unique_id = str(uuid.uuid4())
+              posthog.capture(unique_id, event_name)
+              print_verbose(f"successfully logged to PostHog!")
+        except:
+          print_verbose(f"Error Occurred while logging failure: {traceback.format_exc()}")
+          pass
+      
+      if failure_handler and callable(failure_handler):
+        call_details = {
+          "exception": exception,
+          "additional_details": additional_details
+        }
+        failure_handler(call_details)
+      pass
+    except:
+      pass
+
+def handle_success(*args, **kwargs):
+  try:
     success_handler = additional_details.pop("success_handler", None)
     failure_handler = additional_details.pop("failure_handler", None)
-    
-    additional_details["Event_Name"] = additional_details.pop("failed_event_name", "litellm.failed_query")
-    print_verbose(f"self.failure_callback: {litellm.failure_callback}")
-
-    print_verbose(f"additional_details: {additional_details}")
-    for callback in litellm.failure_callback:
+    additional_details["Event_Name"] = additional_details.pop("successful_event_name", "litellm.succes_query")
+    for callback in litellm.success_callback:
       try:
-        if callback == "slack":
-          slack_msg = "" 
-          if len(kwargs) > 0: 
-            for key in kwargs: 
-              slack_msg += f"{key}: {kwargs[key]}\n"
-          if len(args) > 0:
-            for i, arg in enumerate(args):
-              slack_msg += f"LiteLLM_Args_{str(i)}: {arg}"
-          for detail in additional_details: 
-            slack_msg += f"{detail}: {additional_details[detail]}\n"
-          slack_msg += f"Traceback: {traceback_exception}"
-          slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
-        elif callback == "sentry":
-          capture_exception(exception)
-        elif callback == "posthog": 
-          print_verbose(f"inside posthog, additional_details: {len(additional_details.keys())}")
+        if callback == "posthog":
           ph_obj = {}
-          if len(kwargs) > 0: 
-            ph_obj = kwargs
-          if len(args) > 0:
-            for i, arg in enumerate(args):
-              ph_obj["litellm_args_" + str(i)] = arg
           for detail in additional_details:
             ph_obj[detail] = additional_details[detail]
           event_name = additional_details["Event_Name"]
-          print_verbose(f"ph_obj: {ph_obj}")
-          print_verbose(f"PostHog Event Name: {event_name}")
           if "user_id" in additional_details:
             posthog.capture(additional_details["user_id"], event_name, ph_obj)
           else: # PostHog calls require a unique id to identify a user - https://posthog.com/docs/libraries/python
             unique_id = str(uuid.uuid4())
-            posthog.capture(unique_id, event_name)
-            print_verbose(f"successfully logged to PostHog!")
+            posthog.capture(unique_id, event_name, ph_obj)
+          pass
+        elif callback == "slack":
+          slack_msg = "" 
+          for detail in additional_details: 
+            slack_msg += f"{detail}: {additional_details[detail]}\n"
+          slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
       except:
-        print_verbose(f"Error Occurred while logging failure: {traceback.format_exc()}")
         pass
-    
-    if failure_handler and callable(failure_handler):
-      call_details = {
-        "exception": exception,
-        "additional_details": additional_details
-      }
-      failure_handler(call_details)
-    pass
 
-def handle_success(*args, **kwargs):
-  success_handler = additional_details.pop("success_handler", None)
-  failure_handler = additional_details.pop("failure_handler", None)
-  additional_details["Event_Name"] = additional_details.pop("successful_event_name", "litellm.succes_query")
-  for callback in litellm.success_callback:
-    try:
-      if callback == "posthog":
-        ph_obj = {}
-        for detail in additional_details:
-          ph_obj[detail] = additional_details[detail]
-        event_name = additional_details["Event_Name"]
-        if "user_id" in additional_details:
-          posthog.capture(additional_details["user_id"], event_name, ph_obj)
-        else: # PostHog calls require a unique id to identify a user - https://posthog.com/docs/libraries/python
-          unique_id = str(uuid.uuid4())
-          posthog.capture(unique_id, event_name, ph_obj)
-        pass
-      elif callback == "slack":
-        slack_msg = "" 
-        for detail in additional_details: 
-          slack_msg += f"{detail}: {additional_details[detail]}\n"
-        slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
-    except:
-      pass
-  
-  if success_handler and callable(success_handler):
-    success_handler(args, kwargs)
-  pass
+    if success_handler and callable(success_handler):
+      success_handler(args, kwargs)
+    pass
+  except:
+    pass
 
 
 def exception_type(model, original_exception):
     if isinstance(original_exception, OpenAIError):
         # Handle the OpenAIError
         raise original_exception
     elif model:
```

