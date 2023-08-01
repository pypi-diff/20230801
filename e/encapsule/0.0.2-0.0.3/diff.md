# Comparing `tmp/encapsule-0.0.2.tar.gz` & `tmp/encapsule-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.2.tar", last modified: Tue Aug  1 15:32:32 2023, max compression
+gzip compressed data, was "encapsule-0.0.3.tar", last modified: Tue Aug  1 18:54:07 2023, max compression
```

## Comparing `encapsule-0.0.2.tar` & `encapsule-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.158211 encapsule-0.0.2/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 15:32:32.158211 encapsule-0.0.2/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.2/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.126949 encapsule-0.0.2/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:51:10.000000 encapsule-0.0.2/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     3237 2023-08-01 14:58:34.000000 encapsule-0.0.2/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)      579 2023-08-01 14:50:28.000000 encapsule-0.0.2/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.158211 encapsule-0.0.2/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 15:32:31.000000 encapsule-0.0.2/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 15:32:32.158211 encapsule-0.0.2/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 15:31:12.000000 encapsule-0.0.2/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 18:54:07.005564 encapsule-0.0.3/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 18:54:07.005564 encapsule-0.0.3/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.3/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 18:54:06.958588 encapsule-0.0.3/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:51:10.000000 encapsule-0.0.3/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     3239 2023-08-01 18:43:20.000000 encapsule-0.0.3/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     3111 2023-08-01 18:47:40.000000 encapsule-0.0.3/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 18:54:07.005564 encapsule-0.0.3/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 18:54:07.005564 encapsule-0.0.3/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 18:53:13.000000 encapsule-0.0.3/setup.py
```

### Comparing `encapsule-0.0.2/PKG-INFO` & `encapsule-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.2
+Version: 0.0.3
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.2/encapsule/isolate_bin.py` & `encapsule-0.0.3/encapsule/isolate_bin.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 
 	def pipeStringContext(options):
 		# Subject Main.
 		# Perform access check.
 
 		# setuid pipe invocation
 
-		isolate_sys.checkAccess(self)
+		isolate_sys.checkAccess(self.name)
 
-		settings = dict(env = dict(TASK_ID = isolate_sys.generateNewTaskId())) \
+		settings = dict(env = isolate_sys.generateNewTaskId_env()) \
 				   if self.parentOptions.compartmentalize \
 				   else dict()
 
 		# XXX Todo: inside, set system-level 'current frame process id'
 		# for whatever this task is.  Do this in a python context, when
 		# exiting, reset to 'this frame process id.'
 		return self.executable.pipeStringContext \
@@ -103,15 +103,15 @@
 		self.value = value
 
 	def __str__(self):
 		return f'--{name}={value}'
 
 def exeCall(name, *args, **kwd)
 	'''
-	from encapsulate.isolate_bin import exeCallObject
+	from encapsulate.isolate_bin import exeCallObject, keyword
 
 	def run():
 		try: return exeCallObject \
 			('assets/Itham/services/component/query',
 			 keyword('keyword', 'value'),
 			 'arg1', 'arg2', 'arg3',
 			 compartmentalize = True)
```

### Comparing `encapsule-0.0.2/encapsule.egg-info/PKG-INFO` & `encapsule-0.0.3/encapsule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.2
+Version: 0.0.3
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.2/setup.py` & `encapsule-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

