# Comparing `tmp/encapsule-0.0.4.tar.gz` & `tmp/encapsule-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.4.tar", last modified: Tue Aug  1 20:27:22 2023, max compression
+gzip compressed data, was "encapsule-0.0.5.tar", last modified: Tue Aug  1 21:20:08 2023, max compression
```

## Comparing `encapsule-0.0.4.tar` & `encapsule-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 20:27:22.915703 encapsule-0.0.4/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 20:27:22.915703 encapsule-0.0.4/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.4/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 20:27:22.900096 encapsule-0.0.4/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.4/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     3541 2023-08-01 20:26:18.000000 encapsule-0.0.4/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     5660 2023-08-01 20:25:03.000000 encapsule-0.0.4/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 20:27:22.915703 encapsule-0.0.4/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 20:27:22.000000 encapsule-0.0.4/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 20:27:22.931325 encapsule-0.0.4/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 20:27:01.000000 encapsule-0.0.4/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 21:20:08.044753 encapsule-0.0.5/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 21:20:08.044753 encapsule-0.0.5/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.5/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 21:20:08.013504 encapsule-0.0.5/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.5/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     4252 2023-08-01 21:18:49.000000 encapsule-0.0.5/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     5660 2023-08-01 20:25:03.000000 encapsule-0.0.5/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 21:20:08.029128 encapsule-0.0.5/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 21:20:07.000000 encapsule-0.0.5/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 21:20:07.000000 encapsule-0.0.5/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 21:20:07.000000 encapsule-0.0.5/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 21:20:07.000000 encapsule-0.0.5/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 21:20:08.044753 encapsule-0.0.5/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 21:19:23.000000 encapsule-0.0.5/setup.py
```

### Comparing `encapsule-0.0.4/PKG-INFO` & `encapsule-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.4
+Version: 0.0.5
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.4/encapsule/isolate_bin.py` & `encapsule-0.0.5/encapsule/isolate_bin.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,18 +50,30 @@
 	sys.stdout.write(output)
 
 
 def buildOptions_parent(options):
 	return namespace \
 		(component_root = isolate_sys.COMPONENTS_PATH,
 		 compartmentalize = options.get('compartmentalize'),
-		 segments = options.get('segments'))
+		 segments = options.get('segments'),
+		 post_context = options.get('post_context'))
 
 def parseCmdln_subjective(argv):
-	pass
+	# Todo: wrong
+	from optparse import OptionParser
+	parser = OptionParser()
+	parser.add_option('--compartmentalize', action = 'store_true')
+	parser.add_option('--post-context', action = 'store_true')
+
+	(options, args) = parser.parse_args(argv)
+
+	return ((buildOptions_parent \
+				(namespace(compartmentalize = options.compartmentalize,
+						   post_context = options.post_context)),
+			 (args[0],)), args[1:])
 
 
 class Component:
 	@classmethod
 	def Locate(self, options, name):
 		return self(name, options, io.path \
 			(options.component_root) \
@@ -87,21 +99,28 @@
 		# isolate_sys.checkAccessCurrentUser(self.name)
 
 		settings = self.newTaskId()
 
 		# XXX Todo: inside, set system-level 'current frame process id'
 		# for whatever this task is.  Do this in a python context, when
 		# exiting, reset to 'this frame process id.'
-		return self.executable.pipeStringContext \
-			(isolate_sys.effectiveContextId(), args,
-			 # segments = self.parentOptions.segments,
-			 # setTaskFrame_pid = isolate_sys.setTaskFrame_pid,
-			 **settings)
+		# return self.executable.pipeStringContext \
+		# 	(isolate_sys.effectiveContextId(), args,
+		# 	 # segments = self.parentOptions.segments,
+		# 	 # setTaskFrame_pid = isolate_sys.setTaskFrame_pid,
+		# 	 **settings)
+
+		# To work:
+		return self.executable.pipe \
+			(*args, **settings) \
+			.decode() # Why subprocess returns bytes stream,
+					  # but sys.stdout is default opened str.
 
 def main(argv):
+	# import pdb; pdb.set_trace()
 	((parentOptions, parentArgs), isoOptions) = \
 		parseCmdln_subjective(argv)
 
 	return (parentOptions, Component.Locate \
 		(parentOptions, *parentArgs)	\
 			.pipeStringContext(isoOptions))
 
@@ -139,8 +158,9 @@
 def exeCallObject(*args, **kwd):
 	return deserialize(exeCall(*args, **kwd))
 
 exeCallObject.error = CalledProcessError
 
 
 if __name__ == '__main__':
-	invocation(sys.argv)
+	invocation(sys.argv[1:])
+	# invocation(sys.argv)
```

### Comparing `encapsule-0.0.4/encapsule/isolate_sys.py` & `encapsule-0.0.5/encapsule/isolate_sys.py`

 * *Files identical despite different names*

### Comparing `encapsule-0.0.4/encapsule.egg-info/PKG-INFO` & `encapsule-0.0.5/encapsule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.4
+Version: 0.0.5
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.4/setup.py` & `encapsule-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

