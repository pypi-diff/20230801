# Comparing `tmp/yvesCMD-0.1.1.tar.gz` & `tmp/yvesCMD-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.1.1.tar", last modified: Tue Aug  1 06:43:43 2023, max compression
+gzip compressed data, was "yvesCMD-0.1.2.tar", last modified: Tue Aug  1 07:06:17 2023, max compression
```

## Comparing `yvesCMD-0.1.1.tar` & `yvesCMD-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 06:43:43.970845 yvesCMD-0.1.1/
--rw-rw-rw-   0        0        0      158 2023-08-01 06:43:43.966855 yvesCMD-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 06:43:43.970845 yvesCMD-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      272 2023-08-01 06:42:19.000000 yvesCMD-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 06:43:43.922972 yvesCMD-0.1.1/src/
--rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.1.1/src/register.py
--rw-rw-rw-   0        0        0     6415 2023-08-01 06:39:50.000000 yvesCMD-0.1.1/src/yvescmd.py
-drwxrwxrwx   0        0        0        0 2023-08-01 06:43:43.963863 yvesCMD-0.1.1/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      158 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 07:06:17.092139 yvesCMD-0.1.2/
+-rw-rw-rw-   0        0        0      203 2023-08-01 07:06:17.090142 yvesCMD-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:06:17.092139 yvesCMD-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-08-01 07:05:59.000000 yvesCMD-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:06:17.052244 yvesCMD-0.1.2/src/
+-rw-rw-rw-   0        0        0       77 2023-08-01 07:04:42.000000 yvesCMD-0.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.1.2/src/register.py
+-rw-rw-rw-   0        0        0     5891 2023-08-01 07:01:36.000000 yvesCMD-0.1.2/src/yvescmd.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:06:17.087150 yvesCMD-0.1.2/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.1.1/README.md` & `yvesCMD-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.1.1/src/register.py` & `yvesCMD-0.1.2/src/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.1.1/src/yvescmd.py` & `yvesCMD-0.1.2/src/yvescmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,14 @@
             def do_command(self, a, b, c=None, d=None): . . .
                 [ cmd ] command option_a option_b
                 # Arguments 'a' and 'b' will contain 'option_a' and 'option_b,' respectively. If an option-arg has no value, the parameter is not mandatory.
     )
 """
 
 
-
 import string
 import register as reg
 
 IDENTCHARS = string.ascii_letters + string.digits + '_'
 
 __all__ = ["YveCMD"]
 
@@ -172,24 +171,8 @@
             - parseline line1
         """
         line = line.strip()
         if not line:
             return None, None, line
 
         if line.startswith("low_"):
-            cmd_name = "low_" + line[4:].strip()
-            return cmd_name, line[4:].strip().split(), line
-
-        elif line[0] == '?':
-            line = 'help ' + line[1:]
-        elif line[0] == '!':
-            if hasattr(self, 'do_shell'):
-                line = 'shell ' + line[1:]
-            else:
-                return None, None, line
-
-        i, n = 0, len(line)
-        while i < n and line[i] in self.identchars:
-            i += 1
-        cmd, arg = line[:i], line[i:].strip().split()
-        return cmd, arg, line
-
+            cmd_name = "low
```

