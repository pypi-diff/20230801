# Comparing `tmp/chrisbase-0.4.2.tar.gz` & `tmp/chrisbase-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisbase-0.4.2.tar", last modified: Fri Jul 21 02:05:30 2023, max compression
+gzip compressed data, was "chrisbase-0.4.3.tar", last modified: Tue Aug  1 01:47:19 2023, max compression
```

## Comparing `chrisbase-0.4.2.tar` & `chrisbase-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:05:30.073789 chrisbase-0.4.2/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-07-21 00:41:05.000000 chrisbase-0.4.2/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-07-21 02:05:30.073789 chrisbase-0.4.2/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-07-21 00:41:05.000000 chrisbase-0.4.2/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-07-21 00:41:05.000000 chrisbase-0.4.2/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      990 2023-07-21 02:05:30.073789 chrisbase-0.4.2/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:05:30.073789 chrisbase-0.4.2/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:05:30.073789 chrisbase-0.4.2/src/chrisbase/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 00:41:05.000000 chrisbase-0.4.2/src/chrisbase/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-07-21 00:41:05.000000 chrisbase-0.4.2/src/chrisbase/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2622 2023-07-21 01:57:26.000000 chrisbase-0.4.2/src/chrisbase/data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    24356 2023-07-21 00:41:05.000000 chrisbase-0.4.2/src/chrisbase/io.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-07-21 00:41:05.000000 chrisbase-0.4.2/src/chrisbase/morp.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1279 2023-07-21 00:41:05.000000 chrisbase-0.4.2/src/chrisbase/net.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-07-21 00:41:05.000000 chrisbase-0.4.2/src/chrisbase/time.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5122 2023-07-21 00:41:05.000000 chrisbase-0.4.2/src/chrisbase/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:05:30.073789 chrisbase-0.4.2/src/chrisbase.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-07-21 02:05:30.000000 chrisbase-0.4.2/src/chrisbase.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      474 2023-07-21 02:05:30.000000 chrisbase-0.4.2/src/chrisbase.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-21 02:05:30.000000 chrisbase-0.4.2/src/chrisbase.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-07-21 02:05:30.000000 chrisbase-0.4.2/src/chrisbase.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      169 2023-07-21 02:05:30.000000 chrisbase-0.4.2/src/chrisbase.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-07-21 02:05:30.000000 chrisbase-0.4.2/src/chrisbase.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-21 02:05:29.000000 chrisbase-0.4.2/src/chrisbase.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:47:19.049459 chrisbase-0.4.3/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-07-21 02:23:59.000000 chrisbase-0.4.3/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-08-01 01:47:19.049459 chrisbase-0.4.3/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-07-21 02:23:59.000000 chrisbase-0.4.3/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-07-21 02:23:59.000000 chrisbase-0.4.3/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      990 2023-08-01 01:47:19.049459 chrisbase-0.4.3/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:47:19.049459 chrisbase-0.4.3/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:47:19.049459 chrisbase-0.4.3/src/chrisbase/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 02:23:59.000000 chrisbase-0.4.3/src/chrisbase/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-07-21 02:23:59.000000 chrisbase-0.4.3/src/chrisbase/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11079 2023-07-27 08:01:47.000000 chrisbase-0.4.3/src/chrisbase/data.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    21167 2023-07-27 07:59:27.000000 chrisbase-0.4.3/src/chrisbase/io.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-07-21 02:23:59.000000 chrisbase-0.4.3/src/chrisbase/morp.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      505 2023-07-26 22:58:26.000000 chrisbase-0.4.3/src/chrisbase/net.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-07-21 02:23:59.000000 chrisbase-0.4.3/src/chrisbase/time.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9798 2023-07-28 07:33:28.000000 chrisbase-0.4.3/src/chrisbase/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:47:19.049459 chrisbase-0.4.3/src/chrisbase.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-08-01 01:47:19.000000 chrisbase-0.4.3/src/chrisbase.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      474 2023-08-01 01:47:19.000000 chrisbase-0.4.3/src/chrisbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-08-01 01:47:19.000000 chrisbase-0.4.3/src/chrisbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-08-01 01:47:19.000000 chrisbase-0.4.3/src/chrisbase.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      169 2023-08-01 01:47:19.000000 chrisbase-0.4.3/src/chrisbase.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-08-01 01:47:19.000000 chrisbase-0.4.3/src/chrisbase.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-08-01 01:47:18.000000 chrisbase-0.4.3/src/chrisbase.egg-info/zip-safe
```

### Comparing `chrisbase-0.4.2/LICENSE` & `chrisbase-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.2/PKG-INFO` & `chrisbase-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.4.2
+Version: 0.4.3
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrisbase-0.4.2/setup.cfg` & `chrisbase-0.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrisbase
-version = 0.4.2
+version = 0.4.3
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrisbase
 description = A base tool for python programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrisbase-0.4.2/src/chrisbase/io.py` & `chrisbase-0.4.3/src/chrisbase/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,36 +3,88 @@
 import os
 import shutil
 import socket
 import subprocess
 import sys
 import traceback
 import warnings
-from datetime import datetime, timedelta
+from ipaddress import IPv4Address
 from itertools import chain
-from logging import getLogger
 from pathlib import Path
 from time import sleep
-from typing import Optional, Iterable
+from typing import Iterable
 
+import netifaces
 import pandas as pd
 from chrisdict import AttrDict
 from tabulate import tabulate
 
-from chrisbase.time import from_timestamp, str_delta
-from chrisbase.util import tupled, SP, NO, OX
+from chrisbase.time import from_timestamp
+from chrisbase.util import tupled, NO, OX
 
 logger = logging.getLogger(__name__)
 sys_stdout = sys.stdout
 sys_stderr = sys.stderr
 
 
 class LoggingFormat:
-    CHECK: str = ' ┇ '.join(['%(asctime)s', '%(levelname)-8s', '%(name)48s', '%(message)s'])
-    DEBUG: str = ' ┇ '.join(['%(pathname)120s:%(lineno)-5d', '%(asctime)s', '%(levelname)-8s', '%(name)48s', '%(message)s'])
+    CHECK_48: str = ' ┇ '.join(['%(asctime)s', '%(levelname)-8s', '%(name)48s', '%(message)s'])
+    CHECK_36: str = ' ┇ '.join(['%(asctime)s', '%(levelname)-8s', '%(name)36s', '%(message)s'])
+    CHECK_24: str = ' ┇ '.join(['%(asctime)s', '%(levelname)-8s', '%(name)24s', '%(message)s'])
+    DEBUG_48: str = ' ┇ '.join(['%(pathname)120s:%(lineno)-5d', '%(asctime)s', '%(levelname)-8s', '%(name)48s', '%(message)s'])
+    DEBUG_36: str = ' ┇ '.join(['%(pathname)90s:%(lineno)-5d', '%(asctime)s', '%(levelname)-8s', '%(name)36s', '%(message)s'])
+    DEBUG_24: str = ' ┇ '.join(['%(pathname)60s:%(lineno)-5d', '%(asctime)s', '%(levelname)-8s', '%(name)24s', '%(message)s'])
+
+
+class MuteStd:
+    def __init__(self, out=None, err=None, flush_sec=0.0, mute_warning=None, mute_logger=None):
+        self.mute = open(os.devnull, 'w')
+        self.stdout = out or self.mute
+        self.stderr = err or self.mute
+        self.preout = sys.stdout
+        self.preerr = sys.stderr
+        self.flush_sec = flush_sec
+        assert isinstance(mute_logger, (type(None), str, list, tuple, set))
+        assert isinstance(mute_warning, (type(None), str, list, tuple, set))
+        self.mute_logger = tupled(mute_logger)
+        self.mute_warning = tupled(mute_warning)
+
+    def __enter__(self):
+        try:
+            self.mute_logger = [logging.getLogger(x) for x in self.mute_logger] if self.mute_logger else None
+            if self.mute_logger:
+                for x in self.mute_logger:
+                    x.disabled = True
+                    x.propagate = False
+            if self.mute_warning:
+                for x in self.mute_warning:
+                    warnings.filterwarnings('ignore', category=UserWarning, module=x)
+            flush_or(self.preout, self.preerr, sec=self.flush_sec if self.flush_sec else None)
+            sys.stdout = self.stdout
+            sys.stderr = self.stderr
+        except Exception as e:
+            print(f"[MuteStd.__enter__()] [{type(e)}] {e}", file=sys_stderr)
+            exit(11)
+
+    def __exit__(self, *exc_info):
+        try:
+            flush_or(self.stdout, self.stderr, sec=self.flush_sec if self.flush_sec else None)
+            if self.mute_logger:
+                for x in self.mute_logger:
+                    x.disabled = False
+                    x.propagate = True
+            if self.mute_warning:
+                for x in self.mute_warning:
+                    warnings.filterwarnings('default', category=UserWarning, module=x)
+            sys.stdout = self.preout
+            sys.stderr = self.preerr
+            self.mute.close()
+        except Exception as e:
+            print(f"[MuteStd.__exit__()] [{type(e)}] {e}", file=sys_stderr)
+            exit(22)
 
 
 def cwd(path=None) -> Path:
     if not path:
         return Path.cwd()
     else:
         os.chdir(path)
@@ -147,151 +199,14 @@
     for out in outs:
         if out and not out.closed:
             out.flush()
             if sec and sec > 0.001:
                 sleep(sec)
 
 
-class MuteStd:
-    def __init__(self, out=None, err=None, flush_sec=0.0, mute_warning=None, mute_logger=None):
-        self.mute = open(os.devnull, 'w')
-        self.stdout = out or self.mute
-        self.stderr = err or self.mute
-        self.preout = sys.stdout
-        self.preerr = sys.stderr
-        self.flush_sec = flush_sec
-        assert isinstance(mute_logger, (type(None), str, list, tuple, set))
-        assert isinstance(mute_warning, (type(None), str, list, tuple, set))
-        self.mute_logger = tupled(mute_logger)
-        self.mute_warning = tupled(mute_warning)
-
-    def __enter__(self):
-        try:
-            self.mute_logger = [getLogger(x) for x in self.mute_logger] if self.mute_logger else None
-            if self.mute_logger:
-                for x in self.mute_logger:
-                    x.disabled = True
-                    x.propagate = False
-            if self.mute_warning:
-                for x in self.mute_warning:
-                    warnings.filterwarnings('ignore', category=UserWarning, module=x)
-            flush_or(self.preout, self.preerr, sec=self.flush_sec if self.flush_sec else None)
-            sys.stdout = self.stdout
-            sys.stderr = self.stderr
-        except Exception as e:
-            print(f"[MuteStd.__enter__()] [{type(e)}] {e}", file=sys_stderr)
-            exit(11)
-
-    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
-        try:
-            flush_or(self.stdout, self.stderr, sec=self.flush_sec if self.flush_sec else None)
-            if self.mute_logger:
-                for x in self.mute_logger:
-                    x.disabled = False
-                    x.propagate = True
-            if self.mute_warning:
-                for x in self.mute_warning:
-                    warnings.filterwarnings('default', category=UserWarning, module=x)
-            sys.stdout = self.preout
-            sys.stderr = self.preerr
-            self.mute.close()
-        except Exception as e:
-            print(f"[MuteStd.__exit__()] [{type(e)}] {e}", file=sys_stderr)
-            exit(22)
-
-
-class JobTimer:
-    def __init__(self, name=None, prefix=None, postfix=None, verbose=False, mt=0, mb=0, pt=0, pb=0, rt=0, rb=0, rc='-',
-                 flush_sec=None, mute_loggers=None, mute_warning=None):
-        self.name = name
-        self.prefix = prefix if prefix and len(prefix) > 0 else None
-        self.postfix = postfix if postfix and len(postfix) > 0 else None
-        self.flush_sec = flush_sec
-        self.mt: int = mt
-        self.mb: int = mb
-        self.pt: int = pt
-        self.pb: int = pb
-        self.rt: int = rt
-        self.rb: int = rb
-        self.rc: str = rc
-        self.verbose: bool = verbose
-        assert isinstance(mute_loggers, (type(None), str, list, tuple, set))
-        assert isinstance(mute_warning, (type(None), str, list, tuple, set))
-        self.mute_loggers = tupled(mute_loggers)
-        self.mute_warning = tupled(mute_warning)
-        self.t1: Optional[datetime] = datetime.now()
-        self.t2: Optional[datetime] = datetime.now()
-        self.td: Optional[timedelta] = self.t2 - self.t1
-
-    def __enter__(self):
-        try:
-            self.mute_loggers = [getLogger(x) for x in self.mute_loggers] if self.mute_loggers else None
-            if self.mute_loggers:
-                for x in self.mute_loggers:
-                    x.disabled = True
-                    x.propagate = False
-            if self.mute_warning:
-                for x in self.mute_warning:
-                    warnings.filterwarnings('ignore', category=UserWarning, module=x)
-            flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
-            if self.verbose:
-                if self.mt > 0:
-                    for _ in range(self.mt):
-                        logger.info('')
-                if self.rt > 0:
-                    for _ in range(self.rt):
-                        logger.info(hr(c=self.rc))
-                if self.name:
-                    logger.info(f'{self.prefix + SP if self.prefix else NO}[INIT] {self.name}{SP + self.postfix if self.postfix else NO}')
-                    if self.rt > 0:
-                        for _ in range(self.rt):
-                            logger.info(hr(c=self.rc))
-                if self.pt > 0:
-                    for _ in range(self.pt):
-                        logger.info('')
-                flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
-            self.t1 = datetime.now()
-            return self
-        except Exception as e:
-            logger.error(f"[JobTimer.__enter__()] [{type(e)}] {e}")
-            exit(11)
-
-    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
-        try:
-            self.t2 = datetime.now()
-            self.td = self.t2 - self.t1
-            flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
-            if self.verbose:
-                if self.pb > 0:
-                    for _ in range(self.pb):
-                        logger.info('')
-                if self.rb > 0:
-                    for _ in range(self.rb):
-                        logger.info(hr(c=self.rc))
-                if self.name:
-                    logger.info(f'{self.prefix + SP if self.prefix else NO}[EXIT] {self.name}{SP + self.postfix if self.postfix else NO} ($={str_delta(self.td)})')
-                    if self.rb > 0:
-                        for _ in range(self.rb):
-                            logger.info(hr(c=self.rc))
-                if self.mb > 0:
-                    for _ in range(self.mb):
-                        logger.info('')
-                flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
-            if self.mute_loggers:
-                for x in self.mute_loggers:
-                    x.disabled = False
-                    x.propagate = True
-            if self.mute_warning:
-                for x in self.mute_warning:
-                    warnings.filterwarnings('default', category=UserWarning, module=x)
-        except Exception as e:
-            logger.error(f"[JobTimer.__exit__()] [{type(e)}] {e}")
-            exit(22)
-
-
 def exists_or(path):
     path = Path(path)
     return path if path.exists() else None
 
 
 def first_path_or(path):
     try:
@@ -590,14 +505,15 @@
         if with_column_name:
             print('\t'.join(keys), file=out)
         for row in chain([first], rows):
             print('\t'.join(map(str, [row[k] for k in keys])), file=out)
 
 
 def run_command(*args, title=None, mt=0, mb=0, pt=0, pb=0, rt=0, rb=0, rc='-', bare=True, verbose=True, real=True):
+    from chrisbase.data import JobTimer
     with JobTimer(name=None if bare else f"run_command({title})" if title else f"run_command{args}",
                   verbose=verbose, mt=mt, mb=mb, pt=pt, pb=pb, rt=rt, rb=rb, rc=rc) as scope:
         if real:
             subprocess.run(list(map(str, args)), stdout=None if verbose else scope.mute, stderr=None if verbose else scope.mute)
 
 
 def read_command_out(*args):
@@ -643,14 +559,28 @@
 def get_hostaddr(default="127.0.0.1") -> str:
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as st:
         st.connect(("8.8.8.8", 80))
         r = first_or(st.getsockname())
         return r if r else default
 
 
+def yield_local_addrs():
+    for inf in netifaces.interfaces():
+        inf_addrs = netifaces.ifaddresses(inf).get(netifaces.AF_INET)
+        if inf_addrs:
+            for inf_addr in [x.get('addr') for x in inf_addrs]:
+                if inf_addr and IPv4Address(inf_addr).is_global:
+                    yield inf_addr
+
+
+def get_ip_addrs():
+    local_addrs = list(yield_local_addrs())
+    return local_addrs, len(local_addrs)
+
+
 def prepend_to_global_path(*xs):
     os.environ['PATH'] = os.pathsep.join(map(str, xs)) + os.pathsep + os.environ['PATH']
 
 
 def append_to_global_path(*xs):
     os.environ['PATH'] = os.environ['PATH'] + os.pathsep + os.pathsep.join(map(str, xs))
 
@@ -692,18 +622,19 @@
         handlers.append(h)
         if existing_content:
             h.stream.write(existing_content)
     assert len(handlers) > 0, f"Empty handlers: filename={filename}, filemode={filemode}, stream={stream}"
     return handlers
 
 
-def update_existing_handlers(handlers):
+def update_existing_handlers(handlers, debug=False):
     for x in logging.Logger.manager.loggerDict.values():
         if isinstance(x, logging.Logger):
             if len(x.handlers) > 0:
                 for h in x.handlers:
                     if isinstance(h, logging.FileHandler):
                         h.stream.close()
                     x.removeHandler(h)
                 for h in handlers:
                     x.addHandler(h)
-                logger.debug(f"logging.getLogger({x.name:<20s}) = Logger(level={x.level}, handlers={x.handlers}, disabled={x.disabled}, propagate={x.propagate}, parent={x.parent})")
+                if debug:
+                    logger.debug(f"logging.getLogger({x.name:<20s}) = Logger(level={x.level}, handlers={x.handlers}, disabled={x.disabled}, propagate={x.propagate}, parent={x.parent})")
```

### Comparing `chrisbase-0.4.2/src/chrisbase/morp.py` & `chrisbase-0.4.3/src/chrisbase/morp.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.2/src/chrisbase/time.py` & `chrisbase-0.4.3/src/chrisbase/time.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.2/src/chrisbase.egg-info/PKG-INFO` & `chrisbase-0.4.3/src/chrisbase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.4.2
+Version: 0.4.3
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

