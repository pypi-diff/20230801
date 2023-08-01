# Comparing `tmp/encapsule-0.0.3.tar.gz` & `tmp/encapsule-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.3.tar", last modified: Tue Aug  1 18:54:07 2023, max compression
+gzip compressed data, was "encapsule-0.0.4.tar", last modified: Tue Aug  1 20:27:22 2023, max compression
```

## Comparing `encapsule-0.0.3.tar` & `encapsule-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 18:54:07.005564 encapsule-0.0.3/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 18:54:07.005564 encapsule-0.0.3/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.3/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 18:54:06.958588 encapsule-0.0.3/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:51:10.000000 encapsule-0.0.3/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     3239 2023-08-01 18:43:20.000000 encapsule-0.0.3/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     3111 2023-08-01 18:47:40.000000 encapsule-0.0.3/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 18:54:07.005564 encapsule-0.0.3/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 18:54:06.000000 encapsule-0.0.3/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 18:54:07.005564 encapsule-0.0.3/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 18:53:13.000000 encapsule-0.0.3/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 20:27:22.915703 encapsule-0.0.4/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 20:27:22.915703 encapsule-0.0.4/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.4/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 20:27:22.900096 encapsule-0.0.4/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.4/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     3541 2023-08-01 20:26:18.000000 encapsule-0.0.4/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     5660 2023-08-01 20:25:03.000000 encapsule-0.0.4/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 20:27:22.915703 encapsule-0.0.4/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 20:27:22.931325 encapsule-0.0.4/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 20:27:01.000000 encapsule-0.0.4/setup.py
```

### Comparing `encapsule-0.0.3/PKG-INFO` & `encapsule-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.3
+Version: 0.0.4
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.3/encapsule/isolate_bin.py` & `encapsule-0.0.4/encapsule/isolate_bin.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 from json import loads as deserialize, dumps as serialize
 
 from op.platform.path import CalledProcessError
 
 from . import isolate_sys
 
+__all__ = ['exeCall', 'exeCallObject', 'keyword']
+
 publicName = hash
 
 def invocation(argv = None):
 	try: (options, output) = main(argv)
 	except CalledProcessError as e:
 		sys.stderr.write(e.stderrOutput)
 		sys.exit(e.returncode)
@@ -45,15 +47,18 @@
 				(isolate_sys.effectiveContextId()),
 			 content = output))
 
 	sys.stdout.write(output)
 
 
 def buildOptions_parent(options):
-	pass
+	return namespace \
+		(component_root = isolate_sys.COMPONENTS_PATH,
+		 compartmentalize = options.get('compartmentalize'),
+		 segments = options.get('segments'))
 
 def parseCmdln_subjective(argv):
 	pass
 
 
 class Component:
 	@classmethod
@@ -63,33 +68,37 @@
 				(*name.split('/')))
 
 	def __init__(self, name, parentOptions, executable):
 		self.name = name
 		self.parentOptions = parentOptions
 		self.executable = executable
 
-	def pipeStringContext(options):
+	def newTaskId(self):
+		return dict(env = isolate_sys.generateNewTaskId_env()) \
+			   if self.parentOptions.compartmentalize \
+			   else dict()
+
+	def pipeStringContext(self, args):
 		# Subject Main.
 		# Perform access check.
 
 		# setuid pipe invocation
 
-		isolate_sys.checkAccess(self.name)
+		# XXX DISABLED FOR TESTING XXX
+		# isolate_sys.checkAccessCurrentUser(self.name)
 
-		settings = dict(env = isolate_sys.generateNewTaskId_env()) \
-				   if self.parentOptions.compartmentalize \
-				   else dict()
+		settings = self.newTaskId()
 
 		# XXX Todo: inside, set system-level 'current frame process id'
 		# for whatever this task is.  Do this in a python context, when
 		# exiting, reset to 'this frame process id.'
 		return self.executable.pipeStringContext \
-			(isolate_sys.effectiveContextId(), options,
-			 segments = self.parentOptions.segments,
-			 setTaskFrame_pid = isolate_sys.setTaskFrame_pid,
+			(isolate_sys.effectiveContextId(), args,
+			 # segments = self.parentOptions.segments,
+			 # setTaskFrame_pid = isolate_sys.setTaskFrame_pid,
 			 **settings)
 
 def main(argv):
 	((parentOptions, parentArgs), isoOptions) = \
 		parseCmdln_subjective(argv)
 
 	return (parentOptions, Component.Locate \
@@ -101,17 +110,17 @@
 	def __init__(self, name, value):
 		self.name = name
 		self.value = value
 
 	def __str__(self):
 		return f'--{name}={value}'
 
-def exeCall(name, *args, **kwd)
+def exeCall(name, *args, **kwd):
 	'''
-	from encapsulate.isolate_bin import exeCallObject, keyword
+	from encapsulate import exeCallObject, keyword
 
 	def run():
 		try: return exeCallObject \
 			('assets/Itham/services/component/query',
 			 keyword('keyword', 'value'),
 			 'arg1', 'arg2', 'arg3',
 			 compartmentalize = True)
@@ -130,8 +139,8 @@
 def exeCallObject(*args, **kwd):
 	return deserialize(exeCall(*args, **kwd))
 
 exeCallObject.error = CalledProcessError
 
 
 if __name__ == '__main__':
-	return main(sys.argv)
+	invocation(sys.argv)
```

### Comparing `encapsule-0.0.3/encapsule.egg-info/PKG-INFO` & `encapsule-0.0.4/encapsule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.3
+Version: 0.0.4
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.3/setup.py` & `encapsule-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

