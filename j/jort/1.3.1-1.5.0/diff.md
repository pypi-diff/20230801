# Comparing `tmp/jort-1.3.1.tar.gz` & `tmp/jort-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jort-1.3.1.tar", last modified: Thu Jun 22 05:54:06 2023, max compression
+gzip compressed data, was "jort-1.5.0.tar", last modified: Tue Aug  1 19:53:54 2023, max compression
```

## Comparing `jort-1.3.1.tar` & `jort-1.5.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 05:54:06.747008 jort-1.3.1/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.3.1/LICENSE
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4280 2023-06-22 05:54:06.747008 jort-1.3.1/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3825 2023-06-22 05:52:26.000000 jort-1.3.1/README.md
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 05:54:06.739008 jort-1.3.1/jort/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      331 2023-06-22 00:12:17.000000 jort-1.3.1/jort/__init__.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1372 2023-06-22 00:12:17.000000 jort-1.3.1/jort/_config.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       21 2023-06-22 05:53:07.000000 jort-1.3.1/jort/_version.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3112 2023-05-27 04:28:06.000000 jort-1.3.1/jort/checkpoint.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1378 2023-05-27 04:28:06.000000 jort-1.3.1/jort/datetime_utils.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      152 2023-05-23 01:48:58.000000 jort-1.3.1/jort/exceptions.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    11030 2023-06-22 00:12:17.000000 jort-1.3.1/jort/jort_exe.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     9259 2023-06-22 00:12:17.000000 jort-1.3.1/jort/reporting_callbacks.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     7663 2023-06-22 00:12:17.000000 jort-1.3.1/jort/track_cli.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    11059 2023-06-22 05:43:14.000000 jort-1.3.1/jort/tracker.py
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-06-22 05:54:06.747008 jort-1.3.1/jort.egg-info/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4280 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      386 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/SOURCES.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/dependency_links.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       43 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/entry_points.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      153 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/requires.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-06-22 05:54:06.000000 jort-1.3.1/jort.egg-info/top_level.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-06-22 05:54:06.747008 jort-1.3.1/setup.cfg
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      967 2023-06-22 00:12:17.000000 jort-1.3.1/setup.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-08-01 19:53:54.448586 jort-1.5.0/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.5.0/LICENSE
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4558 2023-08-01 19:53:54.448586 jort-1.5.0/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4103 2023-08-01 19:52:38.000000 jort-1.5.0/README.md
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-08-01 19:53:54.440586 jort-1.5.0/jort/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      431 2023-08-01 19:52:38.000000 jort-1.5.0/jort/__init__.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       21 2023-08-01 19:52:38.000000 jort-1.5.0/jort/_version.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3087 2023-08-01 19:52:38.000000 jort-1.5.0/jort/block.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    11091 2023-08-01 19:52:38.000000 jort-1.5.0/jort/config.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2027 2023-08-01 19:52:38.000000 jort-1.5.0/jort/database.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1378 2023-05-27 04:28:06.000000 jort-1.5.0/jort/datetime_utils.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      152 2023-05-23 01:48:58.000000 jort-1.5.0/jort/exceptions.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3358 2023-08-01 19:52:38.000000 jort-1.5.0/jort/jort_exe.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     9318 2023-08-01 19:52:38.000000 jort-1.5.0/jort/reporting_callbacks.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     7761 2023-08-01 19:52:38.000000 jort-1.5.0/jort/track_cli.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)    14513 2023-08-01 19:52:38.000000 jort-1.5.0/jort/tracker.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-08-01 19:53:54.448586 jort-1.5.0/jort.egg-info/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4558 2023-08-01 19:53:53.000000 jort-1.5.0/jort.egg-info/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      397 2023-08-01 19:53:53.000000 jort-1.5.0/jort.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-08-01 19:53:53.000000 jort-1.5.0/jort.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       43 2023-08-01 19:53:53.000000 jort-1.5.0/jort.egg-info/entry_points.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      167 2023-08-01 19:53:53.000000 jort-1.5.0/jort.egg-info/requires.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-08-01 19:53:53.000000 jort-1.5.0/jort.egg-info/top_level.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-08-01 19:53:54.448586 jort-1.5.0/setup.cfg
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      967 2023-06-22 00:12:17.000000 jort-1.5.0/setup.py
```

### Comparing `jort-1.3.1/LICENSE` & `jort-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jort-1.3.1/PKG-INFO` & `jort-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jort
-Version: 1.3.1
+Version: 1.5.0
 Summary: Script profiler with checkpoints
 Home-page: https://github.com/bbrzycki/jort
 Author: Bryan Brzycki
 Author-email: bbrzycki@berkeley.edu
 Project-URL: Source, https://github.com/bbrzycki/jort
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,25 +12,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jort
 [![PyPI version](https://badge.fury.io/py/jort.svg)](https://badge.fury.io/py/jort) 
 [![Documentation Status](https://readthedocs.org/projects/jort/badge/?version=latest)](https://jort.readthedocs.io/en/latest/?badge=latest)
 
-Track, profile, and notify at custom checkpoints in your coding scripts. Time new and existing shell commands with a convenient command line tool. Save and view details of finished jobs with a local database.
+* Track, profile, and notify at custom blocks in your coding scripts. 
+* Time new and existing shell commands with a convenient command line tool. 
+* Save and view details of finished jobs with a local database.
+![jort help message](jort_help.png)
 
 ## Installation
 ```
 pip install jort
 ```
 
 ## Script Timing
-Use the `Tracker` to create named checkpoints throughout your code. Checkpoints need `start` and `stop` calls, and 
+Use the `Tracker` to create named blocks throughout your code. Blocks need `start` and `stop` calls, and 
 multiple iterations are combined to summarize how long it takes to complete each leg. The `report` function
-prints the results from all checkpoints. If `stop` is not supplied a checkpoint name, the tracker will close and calculate elapsed time from the last open checkpoint (i.e. last in, first out).
+prints the results from all blocks. If `stop` is not supplied a block name, the tracker will close and calculate elapsed time from the last open block (i.e. last in, first out).
 ```
 import jort
 from time import sleep
 
 tr = jort.Tracker()
 
 tr.start('my_script')
@@ -46,14 +49,16 @@
 
 The printed report appears as:
 ```
 my_script | 11.0 s ± 0.0 s per iteration, n = 1
 sleep_1s | 1.0 s ± 0.0 s per iteration, n = 10
 ```
 
+Alternatively, you can use single line checkpoints with `tr.checkpoint()`, which create timing blocks that close at the start of the next checkpoint. Note that you must use another `tr.stop()` call to end the final checkpoint block.
+
 ### Function Decorators
 `jort` supports timing functions with decorators, via `Tracker.track`. As in the first example:
 ```
 @tr.track
 def my_script():
     sleep(1)
     for _ in range(10):
@@ -81,28 +86,29 @@
 
 For SMS text and e-mail notifications, you can enter credentials with the command `jort config`. 
 
 SMS handling is done through Twilio, which offers a [free trial tier](https://support.twilio.com/hc/en-us/articles/223136107-How-does-Twilio-s-Free-Trial-work-). As of now, `jort` handles notifications locally, so you need to add your own credentials for each service. 
 
 ## Saving to Database
 
-`jort` allows you to save details of finished jobs to a local database. To save all checkpoints to database, use the `to_db` keyword. You can also optionally group jobs under a common "session" by specifying the `session_name` keyword:
+`jort` allows you to save details of finished jobs to a local database. To save all blocks to database, use the `to_db` keyword. You can also optionally group jobs under a common "session" by specifying the `session_name` keyword:
 ```
 tr = jort.Tracker(to_db=True, session_name="my_session")
 ```
-If you do not want every checkpoint to be saved, you can specify manually:
+If you do not want every block to be saved, you can specify manually:
 ```
 tr.stop('my_script', to_db=True)
 
 @tr.track(to_db=True)
 def my_script():
     [...]
 ```
 
 ## Command Line Timing
+![jort track help](jort_track_help.png)
 
 To track a new command, you can run:
 ```
 jort track your_command
 ```
 If the target command uses its own options, place quotes around the full command.
 ```
```

### Comparing `jort-1.3.1/README.md` & `jort-1.5.0/jort.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,39 @@
+Metadata-Version: 2.1
+Name: jort
+Version: 1.5.0
+Summary: Script profiler with checkpoints
+Home-page: https://github.com/bbrzycki/jort
+Author: Bryan Brzycki
+Author-email: bbrzycki@berkeley.edu
+Project-URL: Source, https://github.com/bbrzycki/jort
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # jort
 [![PyPI version](https://badge.fury.io/py/jort.svg)](https://badge.fury.io/py/jort) 
 [![Documentation Status](https://readthedocs.org/projects/jort/badge/?version=latest)](https://jort.readthedocs.io/en/latest/?badge=latest)
 
-Track, profile, and notify at custom checkpoints in your coding scripts. Time new and existing shell commands with a convenient command line tool. Save and view details of finished jobs with a local database.
+* Track, profile, and notify at custom blocks in your coding scripts. 
+* Time new and existing shell commands with a convenient command line tool. 
+* Save and view details of finished jobs with a local database.
+![jort help message](jort_help.png)
 
 ## Installation
 ```
 pip install jort
 ```
 
 ## Script Timing
-Use the `Tracker` to create named checkpoints throughout your code. Checkpoints need `start` and `stop` calls, and 
+Use the `Tracker` to create named blocks throughout your code. Blocks need `start` and `stop` calls, and 
 multiple iterations are combined to summarize how long it takes to complete each leg. The `report` function
-prints the results from all checkpoints. If `stop` is not supplied a checkpoint name, the tracker will close and calculate elapsed time from the last open checkpoint (i.e. last in, first out).
+prints the results from all blocks. If `stop` is not supplied a block name, the tracker will close and calculate elapsed time from the last open block (i.e. last in, first out).
 ```
 import jort
 from time import sleep
 
 tr = jort.Tracker()
 
 tr.start('my_script')
@@ -32,14 +49,16 @@
 
 The printed report appears as:
 ```
 my_script | 11.0 s ± 0.0 s per iteration, n = 1
 sleep_1s | 1.0 s ± 0.0 s per iteration, n = 10
 ```
 
+Alternatively, you can use single line checkpoints with `tr.checkpoint()`, which create timing blocks that close at the start of the next checkpoint. Note that you must use another `tr.stop()` call to end the final checkpoint block.
+
 ### Function Decorators
 `jort` supports timing functions with decorators, via `Tracker.track`. As in the first example:
 ```
 @tr.track
 def my_script():
     sleep(1)
     for _ in range(10):
@@ -67,28 +86,29 @@
 
 For SMS text and e-mail notifications, you can enter credentials with the command `jort config`. 
 
 SMS handling is done through Twilio, which offers a [free trial tier](https://support.twilio.com/hc/en-us/articles/223136107-How-does-Twilio-s-Free-Trial-work-). As of now, `jort` handles notifications locally, so you need to add your own credentials for each service. 
 
 ## Saving to Database
 
-`jort` allows you to save details of finished jobs to a local database. To save all checkpoints to database, use the `to_db` keyword. You can also optionally group jobs under a common "session" by specifying the `session_name` keyword:
+`jort` allows you to save details of finished jobs to a local database. To save all blocks to database, use the `to_db` keyword. You can also optionally group jobs under a common "session" by specifying the `session_name` keyword:
 ```
 tr = jort.Tracker(to_db=True, session_name="my_session")
 ```
-If you do not want every checkpoint to be saved, you can specify manually:
+If you do not want every block to be saved, you can specify manually:
 ```
 tr.stop('my_script', to_db=True)
 
 @tr.track(to_db=True)
 def my_script():
     [...]
 ```
 
 ## Command Line Timing
+![jort track help](jort_track_help.png)
 
 To track a new command, you can run:
 ```
 jort track your_command
 ```
 If the target command uses its own options, place quotes around the full command.
 ```
```

### Comparing `jort-1.3.1/jort/checkpoint.py` & `jort-1.5.0/jort/block.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import numpy as np
 from . import datetime_utils
 
 
-class Checkpoint(object):
+class Block(object):
     """
-    Checkpoint object to mark start, stop, and elapsed times.
+    Block object to mark start, stop, and elapsed times.
 
     Start and stop times are in ISO format, while elapsed times are in seconds.
 
     Parameters
     ----------
     name : string
-        Checkpoint name
+        Block name
 
-    :ivar name: checkpoint name
+    :ivar name: block name
     :ivar starts: list of start times
     :ivar stops: list of stop times
     :ivar elapsed: list of elapsed times
     """
     def __init__(self, name):
         self.name = name 
         self.starts = [] 
@@ -26,15 +26,15 @@
         
     def _get_elapsed(self):
         self.elapsed = [datetime_utils.get_runtime(t1, t2) 
                         for (t1, t2) in zip(self.starts, self.stops)]
         
     def add_times(self, start, stop):
         """
-        Store start, stop, and elpased times to checkpoint.
+        Store start, stop, and elpased times to block.
 
         Parameters
         ----------
         start : string
             ISO date of start
         stop : string
             ISO date of stop
```

### Comparing `jort-1.3.1/jort/datetime_utils.py` & `jort-1.5.0/jort/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `jort-1.3.1/jort/reporting_callbacks.py` & `jort-1.5.0/jort/reporting_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from email import encoders
 from email.mime.base import MIMEBase
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email.mime.application import MIMEApplication
 import twilio.rest
 import humanfriendly
-from . import _config
+from . import config
 from . import exceptions
 
 
 class Callback(ABC):
     """
     Abstract base class for notification callbacks.
     """
@@ -70,28 +70,28 @@
     def execute(self, payload):
         print(self.format_message(payload))
 
 
 class EmailNotification(Callback):
     """
     Send email notifications to and from your email account. Requires login 
-    credentials, which can be entered at the command line via :code:`jort -i`.
+    credentials, which can be entered at the command line via :code:`jort config`.
     """
     def __init__(self, email=None):
-        config_data = _config.get_config_data()
+        config_data = config._get_config_data()
         self.email = config_data.get("email")
-        self.smtp_server = config_data.get("smtp_server")
-        self.email_password = config_data.get("email_password")
         if email is not None:
             self.email = email
+        self.email_password = config_data.get("email_password")
+        self.smtp_server = config_data.get("smtp_server")
 
         if self.email_password is None:
-            raise exceptions.JortCredentialException("Missing email password, add with `jort -i` command")
+            raise exceptions.JortCredentialException("Missing email password, add with `jort config email` command")
         if self.smtp_server is None:
-            raise exceptions.JortException("Missing SMTP server, add with `jort -i` command")
+            raise exceptions.JortException("Missing SMTP server, add with `jort config email` command")
         if self.email is None:
             raise exceptions.JortException("Missing email")
 
     def format_message(self, payload):
         if payload["machine"] is not None:
             machine_text = f' on machine {payload["machine"]}'
             html_machine_text = f' on machine <strong>{payload["machine"]}</strong>'
@@ -167,15 +167,15 @@
         email_data = self.format_message(payload)
 
         message = MIMEMultipart("alternative")
         message.attach(MIMEText(email_data["body"], "plain"))
         message.attach(MIMEText(email_data["html_body"], "html"))
 
         if payload["stdout_fn"] is not None:
-            stdout_path = f'{_config.JORT_DIR}/{payload["stdout_fn"]}'
+            stdout_path = os.path.join(config._get_data_dir(), payload["stdout_fn"])
             with open(stdout_path, "r") as f:
                 attachment = MIMEApplication(f.read(), _subtype="txt")
             attachment.add_header("Content-Disposition", "attachment", filename="output.txt")
 
             message_mix = MIMEMultipart("mixed")
             message_mix.attach(message)
             message_mix.attach(attachment)
@@ -191,29 +191,29 @@
             server.login(self.email, self.email_password)
             server.sendmail(message["From"], message["To"], message.as_string())
 
 
 class TextNotification(Callback):
     """
     Send SMS notifications to and from numbers managed by your Twilio account. Requires 
-    Twilio credentials, which can be entered at the command line via :code:`jort -i`.
+    Twilio credentials, which can be entered at the command line via :code:`jort config`.
     """
     def __init__(self, receive_number=None):
-        config_data = _config.get_config_data()
+        config_data = config._get_config_data()
         self.receive_number = config_data.get("twilio_receive_number")
+        if receive_number is not None:
+            self.receive_number = receive_number
         self.send_number = config_data.get("twilio_send_number")
         self.twilio_account_sid = config_data.get("twilio_account_sid")
         self.twilio_auth_token = config_data.get("twilio_auth_token")
-        if receive_number is not None:
-            self.receive_number = receive_number
 
         if self.twilio_account_sid is None or self.twilio_auth_token is None:
-            raise exceptions.JortCredentialException("Missing Twilio credentials, add with `jort -i` command")
+            raise exceptions.JortCredentialException("Missing Twilio credentials, add with `jort config text` command")
         if self.send_number is None:
-            raise exceptions.JortException("Missing Twilio sending number, add with `jort -i` command")
+            raise exceptions.JortException("Missing Twilio sending number, add with `jort config text` command")
         if self.receive_number is None:
             raise exceptions.JortException("Missing receiving number")
 
     def format_message(self, payload):
         if payload["status"] == "success":
             return (
                 f'Your job `{payload["name"]}` successfully completed '
```

### Comparing `jort-1.3.1/jort/track_cli.py` & `jort-1.5.0/jort/track_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import sys
 import time
 import sqlite3
 import contextlib
 import shlex
 import subprocess
 import uuid
+import shutil
 import psutil
 import shortuuid
 from tqdm import tqdm
 from pprint import pprint
 
 from . import tracker
 from . import datetime_utils
-from . import _config
+from . import config
 from . import reporting_callbacks
+from . import exceptions
 
 
 def track_new(command,
               use_shell=False,
               store_stdout=False,
               save_filename=None,
               to_db=False,
@@ -38,15 +40,15 @@
     use_shell : bool, optional
         Option to use shell execution for subprocess
     store_stdout : bool, optional
         Option to write command output to file
     save_filename : str, optional
         Filename to which to save command output
     to_db : bool, optional
-        Save all checkpoints to database
+        Save all blocks to database
     session_name : str, optional
         Name of job session, if saving jobs to database
     unique : bool, optional
         Whether to skip job, if already successfully run and stored in database
     send_text : bool, optional
         Option to send SMS notification on completion
     send_email : bool, optional
@@ -54,44 +56,47 @@
     verbose : bool, optional
         Option to control how much information is printed in stdout
     update_period : int, optional
         Number of seconds between each payload update and stdout write. If 
         :code:`update_period=-1`, as default, the only update occurs on completion.
     """
     callbacks = [reporting_callbacks.PrintReport()]
-    if send_text:
-        callbacks.append(reporting_callbacks.TextNotification())
     if send_email:
         callbacks.append(reporting_callbacks.EmailNotification())
+    if send_text:
+        callbacks.append(reporting_callbacks.TextNotification())
 
     # Key for storing stdout text to file
     if save_filename or store_stdout:
         stdout_fn = f"{shortuuid.uuid()}.txt"
-        stdout_path = f"{_config.JORT_DIR}/{stdout_fn}"
+        stdout_path = os.path.join(config._get_data_dir(), stdout_fn)
     else:
         stdout_fn = None
 
     tr = tracker.Tracker(to_db=to_db, session_name=session_name)
     if unique:
-        with contextlib.closing(sqlite3.connect(f"{_config.JORT_DIR}/jort.db")) as con:
-            cur = con.cursor()
-            sql = (
-                "SELECT status FROM jobs WHERE session_id == ? AND job_name == ?"
-            )
-            res = cur.execute(sql, (tr.session_id, command))
-            for row in res.fetchall():
-                status = row[0]
-                if status == "success":
-                    print("Found matching job that completed successfully; skipping...")
-                    con.close()
-                    return
+        try: 
+            with contextlib.closing(sqlite3.connect(config._get_database_path())) as con:
+                cur = con.cursor()
+                sql = (
+                    "SELECT status FROM jobs WHERE session_id = ? AND job_name = ?"
+                )
+                res = cur.execute(sql, (tr.session_id, command))
+                for row in res.fetchall():
+                    status = row[0]
+                    if status == "success":
+                        print("Found matching job that completed successfully; skipping...")
+                        con.close()
+                        return
+        except sqlite3.OperationalError as e:
+            raise exceptions.JortException("Missing database - make sure to initialize with `jort.init()` or `jort init`") from e 
 
     tr.start(name=command)
 
-    payload = tr.open_checkpoint_payloads[command]
+    payload = tr.open_block_payloads[command]
 
     payload['stdout_fn'] = stdout_fn
 
     # ACTUALLY START SUBPROCESS
     my_env = os.environ.copy()
     my_env["PYTHONUNBUFFERED"] = "1"
 
@@ -115,15 +120,15 @@
 
     # Create stdout file
     if verbose:
         pprint(payload)
     if save_filename or store_stdout:
         with open(stdout_path, "a+") as f:
             f.write(f"{command}\n")
-            f.write(f"--\n")
+            f.write(f"----\n")
 
     buffer = ""
     temp_start = time.time()
     for line in p.stdout:
         if update_period > 0 and time.time() - temp_start >= update_period:
             if verbose:
                 print("Buffered! (Not sent)", [buffer])
@@ -163,21 +168,16 @@
     # print("")
     # if payload["runtime"] < 10:
     #     sys.exit("Job exited in 10 seconds -- no need to track!")
 
     if verbose:
         pprint(payload)
 
-    if save_filename or store_stdout:
-        if save_filename:
-            subprocess.call(["cp", stdout_path, save_filename])
-        try:
-            subprocess.call(["rm", stdout_path])
-        except Exception as e:
-            raise e
+    if save_filename:
+        shutil.move(stdout_path, save_filename)
 
 
 def track_existing(pid,
                    to_db=False,
                    session_name=None,
                    send_text=False,
                    send_email=False,
@@ -187,43 +187,43 @@
     Track execution time and details of existing command line process.
 
     Parameters
     ----------
     pid : int
         Process ID of existing process
     to_db : bool, optional
-        Save all checkpoints to database
+        Save all blocks to database
     session_name : str, optional
         Name of job session, if saving jobs to database
     send_text : bool, optional
         Option to send SMS notification on completion
     send_email : bool, optional
         Option to send e-mail notification on completion
     verbose : bool, optional
         Option to control how much information is printed in stdout
     update_period : int, optional
         Number of seconds between each payload update. If 
         :code:`update_period=-1`, as default, the only update occurs on completion.
     """
     callbacks = [reporting_callbacks.PrintReport()]
-    if send_text:
-        callbacks.append(reporting_callbacks.TextNotification())
     if send_email:
         callbacks.append(reporting_callbacks.EmailNotification())
+    if send_text:
+        callbacks.append(reporting_callbacks.TextNotification())
 
     # Does not support stdout tracking
     stdout_fn = None
 
     # Create process based on PID and grab relevant information
     p = psutil.Process(pid)
     command = " ".join(p.cmdline())
 
     tr = tracker.Tracker(to_db=to_db, session_name=session_name)
     tr.start(name=command, date_created=datetime_utils.get_iso_date(p.create_time()))
-    payload = tr.open_checkpoint_payloads[command]
+    payload = tr.open_block_payloads[command]
 
     if verbose:
         pprint(payload)
 
     temp_start = time.time()
 
     while p.is_running():
```

### Comparing `jort-1.3.1/jort/tracker.py` & `jort-1.5.0/jort/tracker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,68 @@
+import os
 import sys
+import linecache
 import time
 import sqlite3
 import logging
 import traceback
 import functools
 import shortuuid
 import contextlib
+import socket
+import inspect
 
-from . import _config
-from . import checkpoint
+from . import config
+from . import block
 from . import datetime_utils
+from . import exceptions
         
 
+def _get_linenumber():
+        call_frame = inspect.getframeinfo(inspect.stack()[2][0])
+        return call_frame.lineno
+
+
 class Tracker(object):
     """
     A class to time sections of Python scripts by creating and closing timing
-    checkpoints. 
+    blocks. 
 
     Parameters
     ----------
+    session_name : str, optional
+        Name of job session, if saving jobs to database
     log_name : str
         Filename for timing logs
     verbose : int, optional
         Options for verbosity. 0 for none, 1 for INFO, and 2 for DEBUG.
     to_db : bool, optional
-        Save all checkpoint runtime details to database
-    session_name : str, optional
-        Name of job session, if saving jobs to database
+        Save all block runtime details to database
 
     :ivar date_created: time of initialization
     :ivar machine: name of local machine
-    :ivar checkpoints: dict of Checkpoints
-    :ivar open_checkpoint_payloads: dict of job status payloads for open Checkpoints
+    :ivar blocks: dict of Blocks
+    :ivar open_block_payloads: dict of job status payloads for open Blocks
     :ivar log_name: log filename
-    :iver to_db: option to save all checkpoints to database
+    :iver to_db: option to save all blocks to database
     :iver session_name: name of job session
     """
-    def __init__(self, log_name="tracker.log", verbose=0, to_db=False, session_name=None):
+    def __init__(self, session_name=None, log_name="tracker.log", verbose=0, to_db=False):
         self.date_created = datetime_utils.get_iso_date()
-        self.machine = _config.get_config_data().get("machine")
-        self.checkpoints = {}
-        self.open_checkpoint_payloads = {}
+        self.machine = socket.gethostname() #config._get_config_data().get("machine")
+        self.blocks = {}
+        self.open_block_payloads = {}
 
         # Manage session name, id; if session name is provided, get the id from db
-        self.to_db = to_db
         self.session_name = session_name
         self.session_id = shortuuid.uuid()
-
-        with contextlib.closing(sqlite3.connect(f"{_config.JORT_DIR}/jort.db")) as con:
-            cur = con.cursor()
-            if self.session_name is not None:
-                sql = "SELECT session_id FROM sessions WHERE session_name == ?"
-                res = cur.execute(sql, (self.session_name,))
-                row = res.fetchone()
-                if row is not None:
-                    self.session_id = row[0]
-            else:
-                self.session_name = self.session_id
-                if self.to_db:
-                    sql = (
-                        "INSERT INTO sessions VALUES(?, ?)"
-                    )
-                    cur.execute(sql, (self.session_id, self.session_name))
-                    con.commit()
+        self.session_configured = False
+        self.to_db = to_db
+        if self.to_db:
+            self._configure_db_session()
 
         self.log_name = log_name
         if verbose != 0:
             print(f"Starting session `{self.session_name}`")
             # if verbose == 1:
             #     level = logging.INFO
             # else:
@@ -76,209 +72,311 @@
             # handlers = [file_handler, stdout_handler]
 
             # logging.basicConfig(level=level,
             #                     format="%(asctime)s %(name)-15s %(levelname)-8s %(message)s",
             #                     handlers=handlers, 
             #                     force=True)
         
-    def start(self, name=None, date_created=None):
+    def _configure_db_session(self):
+        """
+        Manage session name and id. If session name is provided, get the id from database.
         """
-        Open checkpoint and start timer. Creates initial job status payload for use
+        try:
+            with contextlib.closing(sqlite3.connect(config._get_database_path())) as con:
+                cur = con.cursor()
+                if self.session_name is not None:
+                    sql = "SELECT session_id FROM sessions WHERE session_name = ?"
+                    res = cur.execute(sql, (self.session_name,))
+                    row = res.fetchone()
+                    if row is not None:
+                        self.session_id = row[0]
+                else:
+                    self.session_name = self.session_id
+                    sql = (
+                        "INSERT INTO sessions VALUES(?, ?)"
+                    )
+                    cur.execute(sql, (self.session_id, self.session_name))
+                    con.commit()
+            self.session_configured = True
+        except sqlite3.OperationalError as e:
+            raise exceptions.JortException("Missing database - make sure to initialize with `jort.init()` or `jort init`") from e
+
+    def checkpoint(self, name=None, callbacks=[], to_db=False):
+        """
+        A checkpoint opens a timing block that closes at the next checkpoint.
+        Note that the last checkpoint needs to be closed with stop().
+        """
+        # First close any existing checkpoints
+        for ckpt_name, payload in self.open_block_payloads.copy().items():
+            if payload["is_checkpoint"]:
+                self.stop(name=ckpt_name, callbacks=callbacks, to_db=to_db)
+        
+        if name is None:
+            name = f"Checkpoint - line {_get_linenumber()}"
+        
+        self.start(name=name, is_checkpoint=True)
+
+    def start(self, name=None, date_created=None, is_checkpoint=False):
+        """
+        Open block and start timer. Creates initial job status payload for use
         with notifications.
 
         Parameters
         ----------
         name : str
-            Checkpoint name
+            Block name
         date_created : str, optional
             For an existing process, instead set this input as the creation date
+        is_checkpoint : bool, optional
+            Whether block start is a checkpoint (stops at next checkpoint)
         """
         if name is None:
             name = "Misc"
         name = str(name)
-        if name in self.open_checkpoint_payloads:
-            raise RuntimeError(f"Open checkpoint named {name} already exists")
+        if name in self.open_block_payloads:
+            raise RuntimeError(f"Open block named {name} already exists")
         
         if date_created is not None:
             start = date_created
         else:
             start = datetime_utils.get_iso_date()
         now = datetime_utils.get_iso_date()
 
-        self.open_checkpoint_payloads[name] = {
+        self.open_block_payloads[name] = {
             "user_id": None,
             "job_id": shortuuid.uuid(),
             "session_id": self.session_id,
             "name": name,
             "long_name": name,
             "status": "running",
             "machine": self.machine,
             "date_created": start,
             "date_modified": now,
             "runtime": datetime_utils.get_runtime(start, now),
             "stdout_fn": None,
             "unread": True,
             "error_message": None,
+            "is_checkpoint": is_checkpoint,
         }
-        if name not in self.checkpoints:
-            self.checkpoints[name] = checkpoint.Checkpoint(name)
+        if name not in self.blocks:
+            self.blocks[name] = block.Block(name)
         logger = logging.getLogger(f"{name}.start")
         logger.debug("Profiling block started.")
         
     def stop(self, name=None, callbacks=[], to_db=False):
         """
-        Close checkpoint and stop timer. Store start, stop, and elapsed times.
+        Close block and stop timer. Store start, stop, and elapsed times.
         Process job status payload and execute notification callbacks.
 
-        If checkpoint name isn't supplied, get the most recent checkpoint (last
+        If block name isn't supplied, get the most recent block (last
         in, first out; LIFO).
 
         Parameters
         ----------
         name : str, optional
-            Checkpoint name
+            Block name
         callbacks : list, optional
             List of optional notification callbacks
         to_db : bool, optional
-            Save checkpoint runtime details to database
+            Save block runtime details to database
         """
         if name is None:
-            name = list(self.open_checkpoint_payloads.keys())[-1]
-        elif name not in self.open_checkpoint_payloads:
-            raise KeyError(f"No open checkpoint named {name}")
+            name = list(self.open_block_payloads.keys())[-1]
+        elif name not in self.open_block_payloads:
+            raise KeyError(f"No open block named {name}")
 
-        payload = self.open_checkpoint_payloads.pop(name)
+        payload = self.open_block_payloads.pop(name)
         if payload["status"] == "running":
             payload["status"] = "success"
         start = payload["date_created"]
         stop = datetime_utils._update_payload_times(payload)
-        self.checkpoints[name].add_times(start, stop)
+        self.blocks[name].add_times(start, stop)
 
         logger = logging.getLogger(f"{name}.stop")
         logger.debug("Profiling block stopped.")
-        formatted_runtime = checkpoint.format_reported_times(self.checkpoints[name].elapsed[-1])
+        formatted_runtime = block.format_reported_times(self.blocks[name].elapsed[-1])
         logger.info(f"Elapsed time: {formatted_runtime}")
 
         if self.to_db or to_db:
-            with contextlib.closing(sqlite3.connect(f"{_config.JORT_DIR}/jort.db")) as con:
-                cur = con.cursor()
-                # Make sure session info is included in db
-                sql = (
-                    "INSERT OR IGNORE INTO sessions VALUES(?, ?)"
-                )
-                cur.execute(sql, (self.session_id, self.session_name))
-                # Insert job into db
-                sql = (
-                    "INSERT INTO jobs VALUES("
-                    "    :job_id,"
-                    "    :session_id,"
-                    "    :name,"
-                    "    :status,"
-                    "    :machine,"
-                    "    :date_created,"
-                    "    :date_modified,"
-                    "    :runtime,"
-                    "    :stdout_fn,"
-                    "    :error_message"
-                    ")"
-                )
-                cur.execute(sql, payload)
-                job_id = cur.lastrowid
-                con.commit()
+            if not self.session_configured:
+                self._configure_db_session()
+            try:
+                with contextlib.closing(sqlite3.connect(config._get_database_path())) as con:
+                    cur = con.cursor()
+                    # Make sure session info is included in db
+                    sql = (
+                        "INSERT OR IGNORE INTO sessions VALUES(?, ?)"
+                    )
+                    cur.execute(sql, (self.session_id, self.session_name))
+                    # Insert job into db
+                    sql = (
+                        "INSERT INTO jobs VALUES("
+                        "    :job_id,"
+                        "    :session_id,"
+                        "    :name,"
+                        "    :status,"
+                        "    :machine,"
+                        "    :date_created,"
+                        "    :date_modified,"
+                        "    :runtime,"
+                        "    :stdout_fn,"
+                        "    :error_message"
+                        ")"
+                    )
+                    cur.execute(sql, payload)
+                    job_id = cur.lastrowid
+                    con.commit()
+            except sqlite3.OperationalError as e:
+                raise exceptions.JortException("Missing database - make sure to initialize with `jort.init()` or `jort init`") from e
 
         for callback in callbacks:
             callback.execute(payload=payload)
         
     def remove(self, name=None):
         """
-        Option to remove checkpoint start instead of completing a profiling
+        Option to remove block start instead of completing a profiling
         set, such as on catching an error.
 
         Parameters
         ----------
         name : str, optional
-            Checkpoint name
+            Block name
         """
         if name is None:
-            name = list(self.open_checkpoint_payloads.keys())[-1]
+            name = list(self.open_block_payloads.keys())[-1]
         
-        if name in self.open_checkpoint_payloads:
-            payload = self.open_checkpoint_payloads.pop(name)
+        if name in self.open_block_payloads:
+            payload = self.open_block_payloads.pop(name)
             logger = logging.getLogger(f"{name}.remove")
             logger.debug("Profiling block removed.")
         
     def clear_open(self):
         """
-        Clear all open checkpoints / open job status payloads.
+        Clear all open blocks / open job status payloads.
         """
-        self.open_checkpoint_payloads = {}
+        self.open_block_payloads = {}
 
     def raise_error(self):
         """
-        Update information payload with error details for the outermost checkpoint,
+        Update information payload with error details for the outermost block,
         to only be used within the except block during exception handling.
         """
-        name = list(self.open_checkpoint_payloads.keys())[0]
-        payload = self.open_checkpoint_payloads[name]
+        name = list(self.open_block_payloads.keys())[0]
+        payload = self.open_block_payloads[name]
         payload["status"] = "error"
         payload["error_message"] = traceback.format_exc().strip().split('\n')[-1]
         raise
 
     def track(self, f=None, callbacks=[], to_db=False, report=False):
         """
-        Function wrapper for tracker, to be used as a decorator. Creates a checkpoint
+        Function wrapper for tracker, to be used as a decorator. Creates a block
         with the input function's name. 
 
-        Without parameters / evaluation, the decorator simply creates the checkpoint 
+        Without parameters / evaluation, the decorator simply creates the block 
         and times the input function. With parameters, this method can execute 
         callbacks and print a report. 
 
         Parameters
         ----------
         f : func, optional
             Function to decorate
         callbacks : list, optional
             List of optional notification callbacks
         to_db : bool, optional
-            Save checkpoint runtime details to database
+            Save block runtime details to database
         report : bool, optional
             Option to print tracker report at function completion
         """
         assert callable(f) or f is None
         def decorator(func):
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
                 self.start(name=func.__qualname__)
                 try:
                     result = func(*args, **kwargs)
                 except Exception as e:
-                    payload = self.open_checkpoint_payloads[func.__qualname__]
+                    payload = self.open_block_payloads[func.__qualname__]
                     payload["status"] = "error"
                     payload["error_message"] = traceback.format_exc().strip().split('\n')[-1]
                     raise
                 finally:
                     self.stop(name=func.__qualname__, callbacks=callbacks, to_db=to_db)
                     if report:
                         self.report()
                 return result
             return wrapper
         return decorator(f) if f else decorator
         
     def report(self, dec=1):
         """
-        Print formatted runtime statistics for all checkpoints.
+        Print formatted runtime statistics for all blocks.
 
         Parameters
         ----------
         dec : int
             Decimal precision
         """
-        for name in self.checkpoints:
-            ckpt = self.checkpoints[name]
-            print(ckpt.report(dec=dec))
+        print()
+        print(f"Session: {self.session_name}")
+        for name in self.blocks:
+            block = self.blocks[name]
+            print(block.report(dec=dec))
+        print()
+
+    def exec(self, code_string):
+        """
+        Code string can be a series of statements, separated by newlines.
+        """
+        lines = [line.strip() for line in code_string.strip().split('\n')]
+        for line in lines:
+            self.start(name=line)
+            exec(line)
+            self.stop()
+
+
+    def auto_line_monitor(self):
+        self.first_monitor_pass = True
+        class SetTrace(object):
+            def __init__(self_, func):
+                self_.func = func
+
+            def __enter__(self_):
+                sys.setprofile(self_.func)
+                return self_
+
+            def __exit__(self_, ext_type, exc_value, traceback):
+                try:
+                    self.stop()
+                except IndexError:
+                    pass
+                sys.setprofile(None)
+
+        def monitor(frame, event, arg):
+            if event == "line":
+                if not self.first_monitor_pass:
+                    try:
+                        self.stop()
+                    except IndexError:
+                        pass
+                else:
+                    self.first_monitor_pass = False
+                lineno = frame.f_lineno
+                filename = frame.f_globals["__file__"]
+                if (filename.endswith(".pyc") or
+                    filename.endswith(".pyo")):
+                    filename = filename[:-1]
+                name = frame.f_globals["__name__"]
+                line = linecache.getline(filename, lineno)
+                if 'import' in line:
+                    self.start(line.strip())
+                print("%s:%s: %s" % (name, lineno, line.rstrip()))
+            return monitor
+        return SetTrace(monitor)
+
+    
             
             
 def track(f=None, callbacks=[], to_db=False, report=True):
     """
     Independent function wrapper, to be used as a decorator, that creates a one-off
     tracker.
     
@@ -289,12 +387,12 @@
     Parameters
     ----------
     f : func, optional
         Function to decorate
     callbacks : list, optional
         List of optional notification callbacks
     to_db : bool, optional
-        Save checkpoint runtime details to database
+        Save block runtime details to database
     report : bool, optional
         Option to print tracker report at function completion
     """
     return Tracker(verbose=0).track(f=f, callbacks=callbacks, to_db=to_db, report=report)
```

### Comparing `jort-1.3.1/jort.egg-info/PKG-INFO` & `jort-1.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-Metadata-Version: 2.1
-Name: jort
-Version: 1.3.1
-Summary: Script profiler with checkpoints
-Home-page: https://github.com/bbrzycki/jort
-Author: Bryan Brzycki
-Author-email: bbrzycki@berkeley.edu
-Project-URL: Source, https://github.com/bbrzycki/jort
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # jort
 [![PyPI version](https://badge.fury.io/py/jort.svg)](https://badge.fury.io/py/jort) 
 [![Documentation Status](https://readthedocs.org/projects/jort/badge/?version=latest)](https://jort.readthedocs.io/en/latest/?badge=latest)
 
-Track, profile, and notify at custom checkpoints in your coding scripts. Time new and existing shell commands with a convenient command line tool. Save and view details of finished jobs with a local database.
+* Track, profile, and notify at custom blocks in your coding scripts. 
+* Time new and existing shell commands with a convenient command line tool. 
+* Save and view details of finished jobs with a local database.
+![jort help message](jort_help.png)
 
 ## Installation
 ```
 pip install jort
 ```
 
 ## Script Timing
-Use the `Tracker` to create named checkpoints throughout your code. Checkpoints need `start` and `stop` calls, and 
+Use the `Tracker` to create named blocks throughout your code. Blocks need `start` and `stop` calls, and 
 multiple iterations are combined to summarize how long it takes to complete each leg. The `report` function
-prints the results from all checkpoints. If `stop` is not supplied a checkpoint name, the tracker will close and calculate elapsed time from the last open checkpoint (i.e. last in, first out).
+prints the results from all blocks. If `stop` is not supplied a block name, the tracker will close and calculate elapsed time from the last open block (i.e. last in, first out).
 ```
 import jort
 from time import sleep
 
 tr = jort.Tracker()
 
 tr.start('my_script')
@@ -46,14 +35,16 @@
 
 The printed report appears as:
 ```
 my_script | 11.0 s ± 0.0 s per iteration, n = 1
 sleep_1s | 1.0 s ± 0.0 s per iteration, n = 10
 ```
 
+Alternatively, you can use single line checkpoints with `tr.checkpoint()`, which create timing blocks that close at the start of the next checkpoint. Note that you must use another `tr.stop()` call to end the final checkpoint block.
+
 ### Function Decorators
 `jort` supports timing functions with decorators, via `Tracker.track`. As in the first example:
 ```
 @tr.track
 def my_script():
     sleep(1)
     for _ in range(10):
@@ -81,28 +72,29 @@
 
 For SMS text and e-mail notifications, you can enter credentials with the command `jort config`. 
 
 SMS handling is done through Twilio, which offers a [free trial tier](https://support.twilio.com/hc/en-us/articles/223136107-How-does-Twilio-s-Free-Trial-work-). As of now, `jort` handles notifications locally, so you need to add your own credentials for each service. 
 
 ## Saving to Database
 
-`jort` allows you to save details of finished jobs to a local database. To save all checkpoints to database, use the `to_db` keyword. You can also optionally group jobs under a common "session" by specifying the `session_name` keyword:
+`jort` allows you to save details of finished jobs to a local database. To save all blocks to database, use the `to_db` keyword. You can also optionally group jobs under a common "session" by specifying the `session_name` keyword:
 ```
 tr = jort.Tracker(to_db=True, session_name="my_session")
 ```
-If you do not want every checkpoint to be saved, you can specify manually:
+If you do not want every block to be saved, you can specify manually:
 ```
 tr.stop('my_script', to_db=True)
 
 @tr.track(to_db=True)
 def my_script():
     [...]
 ```
 
 ## Command Line Timing
+![jort track help](jort_track_help.png)
 
 To track a new command, you can run:
 ```
 jort track your_command
 ```
 If the target command uses its own options, place quotes around the full command.
 ```
```

### Comparing `jort-1.3.1/setup.py` & `jort-1.5.0/setup.py`

 * *Files identical despite different names*

