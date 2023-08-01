# Comparing `tmp/yvesCMD-0.1.0.tar.gz` & `tmp/yvesCMD-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.1.0.tar", last modified: Mon Jul 31 17:43:46 2023, max compression
+gzip compressed data, was "yvesCMD-0.1.1.tar", last modified: Tue Aug  1 06:43:43 2023, max compression
```

## Comparing `yvesCMD-0.1.0.tar` & `yvesCMD-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:43:46.377227 yvesCMD-0.1.0/
--rw-rw-rw-   0        0        0      158 2023-07-31 17:43:46.375232 yvesCMD-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 17:43:46.377227 yvesCMD-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      272 2023-07-31 17:43:14.000000 yvesCMD-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:43:46.336339 yvesCMD-0.1.0/src/
--rw-rw-rw-   0        0        0       75 2023-07-31 17:41:47.000000 yvesCMD-0.1.0/src/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.1.0/src/register.py
--rw-rw-rw-   0        0        0     6391 2023-07-31 17:33:06.000000 yvesCMD-0.1.0/src/yvescmd.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:43:46.373237 yvesCMD-0.1.0/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      158 2023-07-31 17:43:45.000000 yvesCMD-0.1.0/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-31 17:43:46.000000 yvesCMD-0.1.0/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:43:45.000000 yvesCMD-0.1.0/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 17:43:45.000000 yvesCMD-0.1.0/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 06:43:43.970845 yvesCMD-0.1.1/
+-rw-rw-rw-   0        0        0      158 2023-08-01 06:43:43.966855 yvesCMD-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 06:43:43.970845 yvesCMD-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      272 2023-08-01 06:42:19.000000 yvesCMD-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:43:43.922972 yvesCMD-0.1.1/src/
+-rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.1.1/src/register.py
+-rw-rw-rw-   0        0        0     6415 2023-08-01 06:39:50.000000 yvesCMD-0.1.1/src/yvescmd.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:43:43.963863 yvesCMD-0.1.1/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      158 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 06:43:43.000000 yvesCMD-0.1.1/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.1.0/src/register.py` & `yvesCMD-0.1.1/src/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.1.0/src/yvescmd.py` & `yvesCMD-0.1.1/src/yvescmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 import string
 import register as reg
 
 IDENTCHARS = string.ascii_letters + string.digits + '_'
 
+__all__ = ["YveCMD"]
 
 class YveCMD(metaclass=reg.AutoRegisterCommandsMeta):
     identchars = IDENTCHARS
     ruler = '='
     lastcmd = ''
     intro = None
     relative_prompt = '[ cmd ] ' 
@@ -187,7 +188,8 @@
                 return None, None, line
 
         i, n = 0, len(line)
         while i < n and line[i] in self.identchars:
             i += 1
         cmd, arg = line[:i], line[i:].strip().split()
         return cmd, arg, line
+
```

