# Comparing `tmp/fkeycapture-1.2.3.tar.gz` & `tmp/fkeycapture-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fkeycapture-1.2.3.tar", last modified: Wed Apr 19 15:40:35 2023, max compression
+gzip compressed data, was "fkeycapture-1.2.4.tar", last modified: Tue Aug  1 03:25:49 2023, max compression
```

## Comparing `fkeycapture-1.2.3.tar` & `fkeycapture-1.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.2.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2649 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1534 2023-04-19 15:40:03.000000 fkeycapture-1.2.3/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      815 2023-04-19 15:40:35.877558 fkeycapture-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/src/fkeycapture/
--rw-r--r--   0 runner    (1000) runner    (1000)     3538 2023-04-19 15:04:10.000000 fkeycapture-1.2.3/src/fkeycapture/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/src/fkeycapture.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2649 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-01 03:25:49.504129 fkeycapture-1.2.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2309 2023-08-01 03:25:49.508129 fkeycapture-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1563 2023-08-01 03:24:30.000000 fkeycapture-1.2.4/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      815 2023-08-01 03:25:49.508129 fkeycapture-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-01 03:25:49.452124 fkeycapture-1.2.4/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-01 03:25:49.456125 fkeycapture-1.2.4/src/fkeycapture/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3920 2023-08-01 03:21:14.000000 fkeycapture-1.2.4/src/fkeycapture/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-01 03:25:49.504129 fkeycapture-1.2.4/src/fkeycapture.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2309 2023-08-01 03:25:49.000000 fkeycapture-1.2.4/src/fkeycapture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-08-01 03:25:49.000000 fkeycapture-1.2.4/src/fkeycapture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-01 03:25:49.000000 fkeycapture-1.2.4/src/fkeycapture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-08-01 03:25:49.000000 fkeycapture-1.2.4/src/fkeycapture.egg-info/top_level.txt
```

### Comparing `fkeycapture-1.2.3/LICENSE` & `fkeycapture-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fkeycapture-1.2.3/PKG-INFO` & `fkeycapture-1.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.2.3
+Version: 1.2.4
 Summary: A way to capture keystrokes
 Home-page: https://github.com/F1repup650/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/fkeycapture/issues
 Project-URL: replit, https://replit.com/@Firepup650/fkeycapture
-Description: # fkeycapture
-        This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
-        #### Forms:
-        1. (Default) Recive key as a string
-        2. Recive key as bytes (get only)
-        3. Recive key as ints  (getnum only)
-        #### How to Use:
-        1. from fkeycapture import get, getnum, getchars
-        2. Use get like this: `get(keycount = any int, bytes = True or False)`
-        3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
-        4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
-        #### Change log:
-        ###### v.1.2.3:
-        Project links updated
-        ###### v.1.2.2:
-        Internal improvements, Changelog improved
-        ###### v.1.2.1:
-        Changelog issue fixed, removed the help command from 1.0.10
-        ###### v.1.2.0
-        Type hinting, docstrings, and int support for getnum!
-        ###### v.1.0.10
-        ~~Now includes a help command! Use fkeycapture.help() to recive help.~~ See v.1.2.1
-        ###### v.1.0.9
-        Fixed README issues in 1.0.8
-        ###### v.1.0.8
-        Added getchars method
-        ###### v.1.0.7
-        Added the getnum method
-        ###### v.1.0.6
-        Finally made the package usable.
-        ###### v.1.0.5
-        Repaired an issue in 1.0.4 which caused the module to cause a recusion error.
-        ###### v.1.0.4
-        Repaired an issue in 1.0.3 which caused the module to be unusable.
-        ###### v.1.0.3
-        Repaired an issue in 1.0.0, 1.0.1, and 1.0.2 which caused the module to be unusable.
-        ###### v.1.0.2 (Missing)
-        Unknown
-        ###### v.1.0.1
-        Corrected incorrect text in certain files
-        ###### v.0.0.6 (v.1.0.0 on PyPI)
-        Removed unnecessary code
-        ###### v.0.0.5
-        Replit support?
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# fkeycapture
+This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
+#### Forms:
+1. (Default) Recive key as a string
+2. Recive key as bytes (get only)
+3. Recive key as ints  (getnum only)
+#### How to Use:
+1. from fkeycapture import get, getnum, getchars
+2. Use get like this: `get(keycount = any int, bytes = True or False)`
+3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
+4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
+#### Change log:
+###### v.1.2.4:
+Mypy support
+###### v.1.2.3:
+Project links updated
+###### v.1.2.2:
+Internal improvements, Changelog improved
+###### v.1.2.1:
+Changelog issue fixed, removed the help command from 1.0.10
+###### v.1.2.0
+Type hinting, docstrings, and int support for getnum!
+###### v.1.0.10
+~~Now includes a help command! Use fkeycapture.help() to recive help.~~ See v.1.2.1
+###### v.1.0.9
+Fixed README issues in 1.0.8
+###### v.1.0.8
+Added getchars method
+###### v.1.0.7
+Added the getnum method
+###### v.1.0.6
+Finally made the package usable.
+###### v.1.0.5
+Repaired an issue in 1.0.4 which caused the module to cause a recusion error.
+###### v.1.0.4
+Repaired an issue in 1.0.3 which caused the module to be unusable.
+###### v.1.0.3
+Repaired an issue in 1.0.0, 1.0.1, and 1.0.2 which caused the module to be unusable.
+###### v.1.0.2 (Missing)
+Unknown
+###### v.1.0.1
+Corrected incorrect text in certain files
+###### v.0.0.6 (v.1.0.0 on PyPI)
+Removed unnecessary code
+###### v.0.0.5
+Replit support?
```

### Comparing `fkeycapture-1.2.3/README.md` & `fkeycapture-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 3. Recive key as ints  (getnum only)
 #### How to Use:
 1. from fkeycapture import get, getnum, getchars
 2. Use get like this: `get(keycount = any int, bytes = True or False)`
 3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
 4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
 #### Change log:
+###### v.1.2.4:
+Mypy support
 ###### v.1.2.3:
 Project links updated
 ###### v.1.2.2:
 Internal improvements, Changelog improved
 ###### v.1.2.1:
 Changelog issue fixed, removed the help command from 1.0.10
 ###### v.1.2.0
```

### Comparing `fkeycapture-1.2.3/setup.cfg` & `fkeycapture-1.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fkeycapture
-version = 1.2.3
+version = 1.2.4
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = A way to capture keystrokes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/F1repup650/fkeycapture
 project_urls =
```

### Comparing `fkeycapture-1.2.3/src/fkeycapture/__init__.py` & `fkeycapture-1.2.4/src/fkeycapture/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,140 @@
 """Firepup650's fkeycapture module"""
 import termios, fcntl, sys
-global fd,flags_save,attrs_save
+from typing import Union
+
+global fd, flags_save, attrs_save
 fd = sys.stdin.fileno()
 flags_save = fcntl.fcntl(fd, fcntl.F_GETFL)
 attrs_save = termios.tcgetattr(fd)
+
+
 def __getp1():
     """Internal Method - Modify terminal settings"""
     import termios, fcntl, sys, os
+
     fd = sys.stdin.fileno()
     # save old state
     flags_save = fcntl.fcntl(fd, fcntl.F_GETFL)
     attrs_save = termios.tcgetattr(fd)
     # make raw - the way to do this comes from the termios(3) man page.
-    attrs = list(attrs_save) # copy the stored version to update
+    attrs = list(attrs_save)  # copy the stored version to update
     # iflag
-    attrs[0] &= ~(termios.IGNBRK | termios.BRKINT | termios.PARMRK
-                  | termios.ISTRIP | termios.INLCR | termios. IGNCR
-                  | termios.ICRNL | termios.IXON )
+    attrs[0] &= ~(
+        termios.IGNBRK
+        | termios.BRKINT
+        | termios.PARMRK
+        | termios.ISTRIP
+        | termios.INLCR
+        | termios.IGNCR
+        | termios.ICRNL
+        | termios.IXON
+    )
     # oflag
     attrs[1] &= ~termios.OPOST
     # cflag
-    attrs[2] &= ~(termios.CSIZE | termios. PARENB)
+    attrs[2] &= ~(termios.CSIZE | termios.PARENB)
     attrs[2] |= termios.CS8
     # lflag
-    attrs[3] &= ~(termios.ECHONL | termios.ECHO | termios.ICANON
-                  | termios.ISIG | termios.IEXTEN)
+    attrs[3] &= ~(
+        termios.ECHONL | termios.ECHO | termios.ICANON | termios.ISIG | termios.IEXTEN
+    )
     termios.tcsetattr(fd, termios.TCSANOW, attrs)
     # turn off non-blocking
     fcntl.fcntl(fd, fcntl.F_SETFL, flags_save & ~os.O_NONBLOCK)
+
+
 def __getp2():
     """Internal Method - Reset terminal settings"""
     termios.tcsetattr(fd, termios.TCSAFLUSH, attrs_save)
     fcntl.fcntl(fd, fcntl.F_SETFL, flags_save)
-def get(keycount: int = 1, bytes: bool = False) -> str or bytes:
-  """# Function: get
 
-# Inputs:
-  keycount: int - Number of keys, defualts to 1
-  bytes: bool   - Wether or not to return the key(s) as bytes, defaults to False
-
-# Returns:
-  str or bytes
-
-# Raises:
-  None"""
-  __getp1()
-  key = sys.stdin.read(keycount)
-  __getp2()
-  if bytes:
-    return key.encode()
-  else:
-    return key
-def getnum(keycount: int = 1, ints: bool = False) -> str or int:
-  """# Function: getnum
-
-# Inputs:
-  keycount: int - Number of keys, defualts to 1
-  ints: bool    - Wether to return the keys as ints, defaults to False
-
-# Returns:
-  str or int
-
-# Raises:
-  None"""
-  internalcounter=0
-  keys = []
-  while internalcounter != keycount:
-    key = get()
-    if key in ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]:
-      keys.append(key)
-      internalcounter += 1
-  key = "".join(keys)
-  if not ints:
-    return key
-  else:
-    return int(key)
-def getchars(keycount: int = 1, chars: list = ["1", "2"], bytes: bool = False) -> str:
-  """# Function: getchars
-
-# Inputs:
-  keycount: int - Number of keys, defualts to 1
-  chars: list   - List of allowed keys, defaults to ["1", "2"]
-  bytes: bool   - Wether or not to return the key(s) as bytes, defaults to False
-
-# Returns:
-  str
-
-# Raises:
-  None"""
-  internalcounter=0
-  keys = []
-  while internalcounter != keycount:
-    key = get()
-    for char in chars:
-      if key == char:
-        keys.append(key)
-        internalcounter += 1
-  key = "".join(keys)
-  if not bytes:
-    return key
-  else:
-    return key.encode()
+
+def get(keycount: int = 1, bytes: bool = False) -> Union[str, bytes]:
+    """# Function: get
+
+    # Inputs:
+      keycount: int - Number of keys, defualts to 1
+      bytes: bool   - Wether or not to return the key(s) as bytes, defaults to False
+
+    # Returns:
+      Union[str, bytes]
+
+    # Raises:
+      None"""
+    __getp1()
+    key = sys.stdin.read(keycount)
+    __getp2()
+    if bytes:
+        return key.encode()
+    else:
+        return key
+
+
+def getnum(keycount: int = 1, ints: bool = False) -> Union[str, int]:
+    """# Function: getnum
+
+    # Inputs:
+      keycount: int - Number of keys, defualts to 1
+      ints: bool    - Wether to return the keys as ints, defaults to False
+
+    # Returns:
+      Union[str, int]
+
+    # Raises:
+      None"""
+    internalcounter = 0
+    keys = []
+    while internalcounter != keycount:
+        key = get()
+        if key in ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]:
+            keys.append(key)
+            internalcounter += 1
+    key = "".join(keys)  # type: ignore[arg-type]
+    if not ints:
+        return key
+    else:
+        return int(key)
+
+
+def getchars(
+    keycount: int = 1, chars: list = ["1", "2"], bytes: bool = False
+) -> Union[str, bytes]:
+    """# Function: getchars
+
+    # Inputs:
+      keycount: int - Number of keys, defualts to 1
+      chars: list   - List of allowed keys, defaults to ["1", "2"]
+      bytes: bool   - Wether or not to return the key(s) as bytes, defaults to False
+
+    # Returns:
+      Union[str, bytes]
+
+    # Raises:
+      None"""
+    internalcounter = 0
+    keys = []
+    while internalcounter != keycount:
+        key = get()
+        for char in chars:
+            if key == char:
+                keys.append(key)
+                internalcounter += 1
+    key = "".join(keys)  # type: ignore[arg-type]
+    if not bytes:
+        return key
+    else:
+        return key.encode()
+
+
 # def help():
 #   """# Function: help
 
 # # Inputs:
 #   None
 
 # # Returns:
 #   None
 
 # # Raises:
 #   None"""
-#   print("FKEYCAPTURE HELP\nThis is a simple and easy to use package that allows you to capture individual keystrokes from the user.\nFORMS:\n1. (Default) Recive key as a string\n2. Recive key as bytes\nHOW TO USE:\n1. from fkeycapture import get, getnum, getchars\n2. Use get like this: get([number of keys to capture],[if you want bytes output, make this 'True'])\n3. Use getnum like this: getnum([number of numbers to capture])\n4. Use getchars like this: get([number of keys to capture],[list of chars to capture])")
+#   print("FKEYCAPTURE HELP\nThis is a simple and easy to use package that allows you to capture individual keystrokes from the user.\nFORMS:\n1. (Default) Recive key as a string\n2. Recive key as bytes\nHOW TO USE:\n1. from fkeycapture import get, getnum, getchars\n2. Use get like this: get([number of keys to capture],[if you want bytes output, make this 'True'])\n3. Use getnum like this: getnum([number of numbers to capture])\n4. Use getchars like this: get([number of keys to capture],[list of chars to capture])")
```

### Comparing `fkeycapture-1.2.3/src/fkeycapture.egg-info/PKG-INFO` & `fkeycapture-1.2.4/src/fkeycapture.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.2.3
+Version: 1.2.4
 Summary: A way to capture keystrokes
 Home-page: https://github.com/F1repup650/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/fkeycapture/issues
 Project-URL: replit, https://replit.com/@Firepup650/fkeycapture
-Description: # fkeycapture
-        This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
-        #### Forms:
-        1. (Default) Recive key as a string
-        2. Recive key as bytes (get only)
-        3. Recive key as ints  (getnum only)
-        #### How to Use:
-        1. from fkeycapture import get, getnum, getchars
-        2. Use get like this: `get(keycount = any int, bytes = True or False)`
-        3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
-        4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
-        #### Change log:
-        ###### v.1.2.3:
-        Project links updated
-        ###### v.1.2.2:
-        Internal improvements, Changelog improved
-        ###### v.1.2.1:
-        Changelog issue fixed, removed the help command from 1.0.10
-        ###### v.1.2.0
-        Type hinting, docstrings, and int support for getnum!
-        ###### v.1.0.10
-        ~~Now includes a help command! Use fkeycapture.help() to recive help.~~ See v.1.2.1
-        ###### v.1.0.9
-        Fixed README issues in 1.0.8
-        ###### v.1.0.8
-        Added getchars method
-        ###### v.1.0.7
-        Added the getnum method
-        ###### v.1.0.6
-        Finally made the package usable.
-        ###### v.1.0.5
-        Repaired an issue in 1.0.4 which caused the module to cause a recusion error.
-        ###### v.1.0.4
-        Repaired an issue in 1.0.3 which caused the module to be unusable.
-        ###### v.1.0.3
-        Repaired an issue in 1.0.0, 1.0.1, and 1.0.2 which caused the module to be unusable.
-        ###### v.1.0.2 (Missing)
-        Unknown
-        ###### v.1.0.1
-        Corrected incorrect text in certain files
-        ###### v.0.0.6 (v.1.0.0 on PyPI)
-        Removed unnecessary code
-        ###### v.0.0.5
-        Replit support?
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# fkeycapture
+This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
+#### Forms:
+1. (Default) Recive key as a string
+2. Recive key as bytes (get only)
+3. Recive key as ints  (getnum only)
+#### How to Use:
+1. from fkeycapture import get, getnum, getchars
+2. Use get like this: `get(keycount = any int, bytes = True or False)`
+3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
+4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
+#### Change log:
+###### v.1.2.4:
+Mypy support
+###### v.1.2.3:
+Project links updated
+###### v.1.2.2:
+Internal improvements, Changelog improved
+###### v.1.2.1:
+Changelog issue fixed, removed the help command from 1.0.10
+###### v.1.2.0
+Type hinting, docstrings, and int support for getnum!
+###### v.1.0.10
+~~Now includes a help command! Use fkeycapture.help() to recive help.~~ See v.1.2.1
+###### v.1.0.9
+Fixed README issues in 1.0.8
+###### v.1.0.8
+Added getchars method
+###### v.1.0.7
+Added the getnum method
+###### v.1.0.6
+Finally made the package usable.
+###### v.1.0.5
+Repaired an issue in 1.0.4 which caused the module to cause a recusion error.
+###### v.1.0.4
+Repaired an issue in 1.0.3 which caused the module to be unusable.
+###### v.1.0.3
+Repaired an issue in 1.0.0, 1.0.1, and 1.0.2 which caused the module to be unusable.
+###### v.1.0.2 (Missing)
+Unknown
+###### v.1.0.1
+Corrected incorrect text in certain files
+###### v.0.0.6 (v.1.0.0 on PyPI)
+Removed unnecessary code
+###### v.0.0.5
+Replit support?
```

