# Comparing `tmp/encab-0.0.8.tar.gz` & `tmp/encab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encab-0.0.8.tar", last modified: Mon Jul 31 13:02:33 2023, max compression
+gzip compressed data, was "encab-0.0.9.tar", last modified: Tue Aug  1 11:32:09 2023, max compression
```

## Comparing `encab-0.0.8.tar` & `encab-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.557084 encab-0.0.8/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.8/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5048 2023-07-31 13:02:33.557084 encab-0.0.8/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4489 2023-07-31 13:00:37.000000 encab-0.0.8/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-07-31 11:48:15.000000 encab-0.0.8/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-31 13:02:33.557084 encab-0.0.8/setup.cfg
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.545084 encab-0.0.8/src/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.549084 encab-0.0.8/src/encab/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.8/src/encab/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.8/src/encab/__main__.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.553084 encab-0.0.8/src/encab/common/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1935 2023-07-31 12:19:35.000000 encab-0.0.8/src/encab/common/log_stream.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4168 2023-07-31 12:20:55.000000 encab-0.0.8/src/encab/common/process.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11911 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/config.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8252 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/encab.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.557084 encab-0.0.8/src/encab/ext/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.8/src/encab/ext/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5995 2023-07-31 12:27:13.000000 encab-0.0.8/src/encab/ext/log_sanitizer.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9694 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/ext/startup_script.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.8/src/encab/ext/validation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.8/src/encab/extensions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5574 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/program.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10172 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/program_state.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3203 2023-07-16 12:24:46.000000 encab-0.0.8/src/encab/programs.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.553084 encab-0.0.8/src/encab.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5048 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      585 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-08-01 11:32:09.190313 encab-0.0.9/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.9/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5048 2023-08-01 11:32:09.190313 encab-0.0.9/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4489 2023-08-01 09:20:54.000000 encab-0.0.9/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-08-01 09:20:48.000000 encab-0.0.9/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-08-01 11:32:09.190313 encab-0.0.9/setup.cfg
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-08-01 11:32:09.178313 encab-0.0.9/src/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-08-01 11:32:09.182313 encab-0.0.9/src/encab/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.9/src/encab/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.9/src/encab/__main__.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-08-01 11:32:09.186313 encab-0.0.9/src/encab/common/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1977 2023-08-01 11:25:09.000000 encab-0.0.9/src/encab/common/log_stream.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5274 2023-08-01 11:23:00.000000 encab-0.0.9/src/encab/common/process.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11911 2023-07-31 12:31:36.000000 encab-0.0.9/src/encab/config.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8252 2023-08-01 09:21:16.000000 encab-0.0.9/src/encab/encab.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-08-01 11:32:09.190313 encab-0.0.9/src/encab/ext/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.9/src/encab/ext/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5995 2023-07-31 12:27:13.000000 encab-0.0.9/src/encab/ext/log_sanitizer.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9694 2023-07-31 12:31:36.000000 encab-0.0.9/src/encab/ext/startup_script.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.9/src/encab/ext/validation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.9/src/encab/extensions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5574 2023-07-31 12:31:36.000000 encab-0.0.9/src/encab/program.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10172 2023-07-31 12:31:36.000000 encab-0.0.9/src/encab/program_state.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3203 2023-07-16 12:24:46.000000 encab-0.0.9/src/encab/programs.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-08-01 11:32:09.186313 encab-0.0.9/src/encab.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5048 2023-08-01 11:32:09.000000 encab-0.0.9/src/encab.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      585 2023-08-01 11:32:09.000000 encab-0.0.9/src/encab.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-08-01 11:32:09.000000 encab-0.0.9/src/encab.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-08-01 11:32:09.000000 encab-0.0.9/src/encab.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-08-01 11:32:09.000000 encab-0.0.9/src/encab.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-08-01 11:32:09.000000 encab-0.0.9/src/encab.egg-info/top_level.txt
```

### Comparing `encab-0.0.8/LICENSE` & `encab-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/PKG-INFO` & `encab-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.8
+Version: 0.0.9
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.8
+   INFO  encab: encab 0.0.9
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -104,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.8
+INFO  encab: encab 0.0.9
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -177,15 +177,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.8
+   INFO  encab: encab 0.0.9
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.8/README.md` & `encab-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.8
+   INFO  encab: encab 0.0.9
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -89,15 +89,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.8
+INFO  encab: encab 0.0.9
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -162,15 +162,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.8
+   INFO  encab: encab 0.0.9
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.8/pyproject.toml` & `encab-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encab"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sebastian Kuebeck", email="sebastian.kuebeck@encab.io" },
 ]
 description = "Process manager"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `encab-0.0.8/src/encab/common/log_stream.py` & `encab-0.0.9/src/encab/common/log_stream.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from logging import Logger
 
 class LogStream(object):
     """
     Reads from a stream in a background thread and loggs the result line by line
     """
-
     def __init__(
         self, logger: Logger, log_level: int, stream: IO[bytes], extra: Dict[str, str]
     ) -> None:
         """
         :param Logger logger: the logger to which the stream content is written
         :param int log_level: the log level (see Python logging)
         :param IOBase stream: the stream that is logged
@@ -26,15 +25,15 @@
         self.extra = extra
         self.thread: Optional[Thread] = None
 
     def _run(self):
         try:
             for line in self.stream:
                 strline = line.decode(sys.getdefaultencoding()).rstrip("\r\n\t ")
-                self.logger.log(self.log_level, strline, extra=self.extra)
+                self.logger.log(self.log_level, strline, extra=self.extra)   
         except ValueError:
             pass  # stream was closed
         except OSError:
             self.logger.exception(
                 "I/O Error while logging: %s", self.name, extra=self.extra  # type: ignore
             )
         except:
@@ -47,16 +46,17 @@
         """starts reading and logging"""
         program = self.extra.get("program", "")
         name = f"{program}:{self.log_level}"
         thread = Thread(target=lambda: self._run(), name=name)
         thread.daemon = True
         self.thread = thread
         thread.start()
-        thread.join(0.01)
         return self
 
     def close(self):
         try:
             self.stream.flush()
+            if self.thread:
+                self.thread.join(0.1)
         except IOError:
             pass
         self.stream.close()
```

### Comparing `encab-0.0.8/src/encab/common/process.py` & `encab-0.0.9/src/encab/common/process.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import pwd
 
 from typing import Dict, Optional, Callable, Any, List, Union
 
 from subprocess import Popen, PIPE
 from signal import SIGKILL, SIGTERM
 
 from logging import Logger, INFO, ERROR
@@ -33,23 +34,45 @@
     :rtype: int 
     :raise: KeyError if the User does not exist
     """
     return getpwnam(name).pw_uid
 
 
 class Process(object):
+    """
+    Wrapper for POpen that supports logging of stdout and stdin
+    """
+    
     @staticmethod
     def update_current(user: Optional[int] = None, 
                        group: Optional[int] = None, 
                        umask: Optional[int] = None):
-        if user:
-            os.setuid(user)
-            
+        """
+        sets the current process user, group and umask
+
+        :param user: the UID, defaults to None
+        :type user: Optional[int], optional
+        :param group: the GID, defaults to None
+        :type group: Optional[int], optional
+        :param umask: the mask, defaults to None
+        :type umask: Optional[int], optional
+        :raises ValueError: _description_
+        """
+        
         if group:
             os.setgid(group)
+            
+        if user and os.getuid() != user:
+            try:
+                user_data = pwd.getpwuid(user)
+            except KeyError as e:
+                raise ValueError(f"No passwd entry for user id: {user}", e)
+                       
+            os.initgroups(user_data.pw_name, user_data.pw_gid)
+            os.setuid(user)
 
         if umask and umask != -1:
             os.umask(umask)
 
     
     def __init__(self, 
                  args:Union[str, List[str]], 
@@ -74,22 +97,32 @@
                 exec: Callable[[Popen], Any], 
                 stdin: Optional[int] = None, 
                 stdout: Optional[int] = None, 
                 stderr: Optional[int] = None) -> int:
         uid = self._user
         gid = self._group
         umask = self._umask
-        
+
+        if uid and os.getuid() != uid:
+            try:
+                user_data = pwd.getpwuid(uid)
+            except KeyError as e:
+                raise ValueError(f"No passwd entry for user id: {uid}", e)
+            
         def preexec_fn():
             if gid:
                 os.setgid(gid)
-            if uid:
+                
+            if uid and user_data:
+                os.initgroups(user_data.pw_name, user_data.pw_gid)
                 os.setuid(uid)
+
             if umask and umask != -1:
                 os.umask(umask)
+
         
         self._process = Popen(
                 self._args,
                 stdin=stdin,
                 stdout=stdout,
                 stderr=stderr,
                 env=self._env,
```

### Comparing `encab-0.0.8/src/encab/config.py` & `encab-0.0.9/src/encab/config.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab/encab.py` & `encab-0.0.9/src/encab/encab.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     try:
         config, location = load_config(encab_stream)
 
         logger = set_up_logger(config)
 
         extra = {"program": ENCAB}
 
-        logger.info("encab 0.0.8", extra=extra)
+        logger.info("encab 0.0.9", extra=extra)
         logger.info("Using configuration %s", location, extra=extra)
 
         logger.debug(
             "Encab config: %s",
             shorten(str(config), width=127, placeholder="..."),
             extra=extra,
         )
```

### Comparing `encab-0.0.8/src/encab/ext/log_sanitizer.py` & `encab-0.0.9/src/encab/ext/log_sanitizer.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab/ext/startup_script.py` & `encab-0.0.9/src/encab/ext/startup_script.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab/ext/validation.py` & `encab-0.0.9/src/encab/ext/validation.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab/extensions.py` & `encab-0.0.9/src/encab/extensions.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab/program.py` & `encab-0.0.9/src/encab/program.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab/program_state.py` & `encab-0.0.9/src/encab/program_state.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab/programs.py` & `encab-0.0.9/src/encab/programs.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.8/src/encab.egg-info/PKG-INFO` & `encab-0.0.9/src/encab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.8
+Version: 0.0.9
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.8
+   INFO  encab: encab 0.0.9
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -104,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.8
+INFO  encab: encab 0.0.9
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -177,15 +177,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.8
+   INFO  encab: encab 0.0.9
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.8/src/encab.egg-info/SOURCES.txt` & `encab-0.0.9/src/encab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

