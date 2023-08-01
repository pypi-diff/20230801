# Comparing `tmp/yvesCMD-0.0.1.4.2.tar.gz` & `tmp/yvesCMD-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.1.4.2.tar", last modified: Tue Aug  1 09:15:11 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.2.tar", last modified: Tue Aug  1 09:22:21 2023, max compression
```

## Comparing `yvesCMD-0.0.1.4.2.tar` & `yvesCMD-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:15:11.628750 yvesCMD-0.0.1.4.2/
--rw-rw-rw-   0        0        0      207 2023-08-01 09:15:11.626752 yvesCMD-0.0.1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 09:15:11.582868 yvesCMD-0.0.1.4.2/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.1.4.2/YvesCMD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:15:11.590848 yvesCMD-0.0.1.4.2/YvesCMD/src/
--rw-rw-rw-   0        0        0       77 2023-08-01 08:32:37.000000 yvesCMD-0.0.1.4.2/YvesCMD/src/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.0.1.4.2/YvesCMD/src/register.py
--rw-rw-rw-   0        0        0     6431 2023-08-01 08:35:27.000000 yvesCMD-0.0.1.4.2/YvesCMD/src/yvescmd.py
--rw-rw-rw-   0        0        0       42 2023-08-01 09:15:11.629746 yvesCMD-0.0.1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      337 2023-08-01 09:15:08.000000 yvesCMD-0.0.1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:15:11.621764 yvesCMD-0.0.1.4.2/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      207 2023-08-01 09:15:11.000000 yvesCMD-0.0.1.4.2/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-01 09:15:11.000000 yvesCMD-0.0.1.4.2/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:15:11.000000 yvesCMD-0.0.1.4.2/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 09:15:11.000000 yvesCMD-0.0.1.4.2/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.240825 yvesCMD-0.0.2/
+-rw-rw-rw-   0        0        0      203 2023-08-01 09:22:21.238828 yvesCMD-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.194944 yvesCMD-0.0.2/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.2/YvesCMD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.208909 yvesCMD-0.0.2/YvesCMD/src/
+-rw-rw-rw-   0        0        0       77 2023-08-01 08:32:37.000000 yvesCMD-0.0.2/YvesCMD/src/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.0.2/YvesCMD/src/register.py
+-rw-rw-rw-   0        0        0     6397 2023-08-01 09:22:01.000000 yvesCMD-0.0.2/YvesCMD/src/yvescmd.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:22:21.240825 yvesCMD-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-08-01 09:22:15.000000 yvesCMD-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.234843 yvesCMD-0.0.2/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-08-01 09:22:20.000000 yvesCMD-0.0.2/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-01 09:22:21.000000 yvesCMD-0.0.2/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:22:20.000000 yvesCMD-0.0.2/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 09:22:20.000000 yvesCMD-0.0.2/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.1.4.2/README.md` & `yvesCMD-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.1.4.2/YvesCMD/src/register.py` & `yvesCMD-0.0.2/YvesCMD/src/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.1.4.2/YvesCMD/src/yvescmd.py` & `yvesCMD-0.0.2/YvesCMD/src/yvescmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 class YveCMD(metaclass=AutoRegisterCommandsMeta):
     identchars = IDENTCHARS
     ruler = '='
     lastcmd = ''
     intro = None
     relative_prompt = '[ cmd ] ' 
+    admin = False
 
     def __init__(self):
         self.cmdqueue = []
 
     @classmethod
     def register_handler(cls, cmd_handler):
         cls.register_handler_method(cmd_handler)  # Call the class method to register the handler
@@ -135,16 +136,19 @@
             except AttributeError:
                 try:
                     func = getattr(self, 'void_' + cmd)
                     func()  # Call the void_ method without arguments
                 except AttributeError:
                     return self.default(line)
             except TypeError as e:
-                print("Error: Invalid number of arguments.")
-                print("Type 'help {}' for more information.".format(cmd))
+                if not self.admin:
+                    print("Error: Invalid number of arguments.")
+                    print("Type 'help {}' for more information.".format(cmd))
+                else:
+                    print(e)
             except Exception as e:
                 print("Error:", e)
 
     def emptyline(self):
         """
         [Goals]
             - Handles an empty input line.
@@ -171,18 +175,14 @@
         [ForExm]
             - parseline line1
         """
         line = line.strip()
         if not line:
             return None, None, line
 
-        if line.startswith("low_"):
-            cmd_name = "low_" + line[4:].strip()
-            return cmd_name, line[4:].strip().split(), line
-
         elif line[0] == '?':
             line = 'help ' + line[1:]
         elif line[0] == '!':
             if hasattr(self, 'do_shell'):
                 line = 'shell ' + line[1:]
             else:
                 return None, None, line
```

