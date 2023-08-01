# Comparing `tmp/huckle-3.0.1.tar.gz` & `tmp/huckle-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huckle-3.0.1.tar", last modified: Fri Jul  7 03:05:10 2023, max compression
+gzip compressed data, was "huckle-3.0.2.tar", last modified: Tue Aug  1 02:33:51 2023, max compression
```

## Comparing `huckle-3.0.1.tar` & `huckle-3.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.320445 huckle-3.0.1/
--rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.0.1/LICENSE.txt
--rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.0.1/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-07-07 03:05:10.320558 huckle-3.0.1/PKG-INFO
--rwx------   0 jeff       (501) staff       (20)     7575 2023-04-09 22:47:09.000000 huckle-3.0.1/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.319349 huckle-3.0.1/huckle/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.0.1/huckle/__init__.py
--rwxr-x---   0 jeff       (501) staff       (20)      308 2022-03-20 22:23:06.000000 huckle-3.0.1/huckle/__main__.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     4505 2023-07-07 02:58:30.000000 huckle-3.0.1/huckle/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.320226 huckle-3.0.1/huckle/data/
--rwxr-x---   0 jeff       (501) staff       (20)     2352 2023-04-09 22:53:51.000000 huckle-3.0.1/huckle/data/huckle.1
--rwxr-xr-x   0 jeff       (501) staff       (20)    10129 2023-07-07 02:34:29.000000 huckle-3.0.1/huckle/hclinav.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     2842 2023-07-07 02:33:09.000000 huckle-3.0.1/huckle/huckle.py
--rwxr-x---   0 jeff       (501) staff       (20)      858 2022-03-20 22:23:06.000000 huckle-3.0.1/huckle/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      248 2023-07-07 02:55:08.000000 huckle-3.0.1/huckle/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.320123 huckle-3.0.1/huckle.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      381 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       48 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       84 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        7 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/top_level.txt
--rwxr-x---   0 jeff       (501) staff       (20)       67 2023-07-07 03:05:10.320833 huckle-3.0.1/setup.cfg
--rwxr-x---   0 jeff       (501) staff       (20)     3314 2023-07-07 02:52:48.000000 huckle-3.0.1/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-08-01 02:33:51.248382 huckle-3.0.2/
+-rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.0.2/LICENSE.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.0.2/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-08-01 02:33:51.248473 huckle-3.0.2/PKG-INFO
+-rwx------   0 jeff       (501) staff       (20)     7575 2023-04-09 22:47:09.000000 huckle-3.0.2/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-08-01 02:33:51.247434 huckle-3.0.2/huckle/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.0.2/huckle/__init__.py
+-rwxr-x---   0 jeff       (501) staff       (20)      308 2022-03-20 22:23:06.000000 huckle-3.0.2/huckle/__main__.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     4505 2023-07-07 02:58:30.000000 huckle-3.0.2/huckle/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-08-01 02:33:51.248276 huckle-3.0.2/huckle/data/
+-rwxr-x---   0 jeff       (501) staff       (20)     3270 2023-08-01 02:31:29.000000 huckle-3.0.2/huckle/data/huckle.1
+-rwxr-xr-x   0 jeff       (501) staff       (20)    10478 2023-08-01 02:01:59.000000 huckle-3.0.2/huckle/hclinav.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     2782 2023-08-01 01:50:22.000000 huckle-3.0.2/huckle/huckle.py
+-rwxr-x---   0 jeff       (501) staff       (20)      858 2022-03-20 22:23:06.000000 huckle-3.0.2/huckle/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      248 2023-08-01 00:53:13.000000 huckle-3.0.2/huckle/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-08-01 02:33:51.248150 huckle-3.0.2/huckle.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-08-01 02:33:51.000000 huckle-3.0.2/huckle.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      381 2023-08-01 02:33:51.000000 huckle-3.0.2/huckle.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-08-01 02:33:51.000000 huckle-3.0.2/huckle.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       48 2023-08-01 02:33:51.000000 huckle-3.0.2/huckle.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       84 2023-08-01 02:33:51.000000 huckle-3.0.2/huckle.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        7 2023-08-01 02:33:51.000000 huckle-3.0.2/huckle.egg-info/top_level.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       67 2023-08-01 02:33:51.248734 huckle-3.0.2/setup.cfg
+-rwxr-x---   0 jeff       (501) staff       (20)     3314 2023-07-07 02:52:48.000000 huckle-3.0.2/setup.py
```

### Comparing `huckle-3.0.1/LICENSE.txt` & `huckle-3.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `huckle-3.0.1/PKG-INFO` & `huckle-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.0.1
+Version: 3.0.2
 Summary: A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `huckle-3.0.1/README.rst` & `huckle-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `huckle-3.0.1/huckle/config.py` & `huckle-3.0.2/huckle/config.py`

 * *Files identical despite different names*

### Comparing `huckle-3.0.1/huckle/data/huckle.1` & `huckle-3.0.2/huckle/data/huckle.1`

 * *Files 26% similar despite different names*

```diff
@@ -32,14 +32,38 @@
 Note that an existing configuration file is left alone if the command is run multiple times
 for the same CLI.
 .IP "cli rm <cliname>"
 Removes an installed CLI.
 .IP "cli run <cliname>"
 Used to invoke a CLI by name, the details of which are otherwise left to API implementers. This is equivalent to invoking
 <cliname> directly after CLI installation and after exporting the huckle env path (see "huckle env").
+
+Note that in certain exceptional cases where a parameter might be passed on the command line, if the parameter value matches exactly an available command,
+huckle will not be able to distinguish between an intent to pass a command or a parameter and will require additional information; notably escapement via backslash double quote or single quote.
+
+Huckle accept lazy parameters (without quotes), and this works most of the time, however if ambiguity arises, additional information must be provided.
+
+For example, assuming an "hc" HCLI, an hc "connect" command and otherwise valid "-j" option; the following will fail:
+
+echo '$$' | hc -j "connect"
+
+echo '$$' | hc -j 'connect'
+
+The following however would succeed:
+
+echo '$$'| hc -j \\'connect\\'
+
+echo '$$'| hc -j \\"connect\\"
+
+This would also succeed if multiple words must be passed as a parameter:
+
+echo '$$'| hc -j 'connect me'
+
+echo '$$'| hc -j "connect me"
+
 .IP "cli ls"
 Lists all the installed CLIs.
 .IP "cli config <cliname>"
 Lists the configuration options of an installed CLI.
 .IP "<cliname> ..."
 The <cliname> alias created for brevity, via huckle cli install.
 .IP "<cliname> ... help"
```

### Comparing `huckle-3.0.1/huckle/hclinav.py` & `huckle-3.0.2/huckle/hclinav.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,17 @@
             sys.exit(0)
 
         # we give precedence to parameter traversal to help avoid forcing double quoting on the command line
         try:
             for k, l in enumerate(nav.links()["cli"][j]):
                 hcli_type = l.links()["profile"][0].uri.split('#', 1)[1]
                 if hcli_type == config.hcli_parameter_type:
-                    nav = l["cli"][0](hcli_param=quote('\"' + arg + '\"'))
+                    if not (arg.startswith('\"') and arg.endswith('\"')):
+                        arg = '\"' + arg + '\"'
+                    nav = l["cli"][0](hcli_param=quote(arg))
                     return nav
         except:
             pass
 
         tempnav = nav.links()["cli"][j]
         try:
             if tempnav()["name"] == arg:
@@ -81,23 +83,28 @@
 
         if j == ilength - 1:
             hutils.eprint(config.cliname + ": " + arg + ": " + "command not found.")
             sys.exit(2)
 
 # attempts to traverse through an execution. (only attempted when we've run out of command line arguments to parse)
 def traverse_execution(nav):
-    for k, z in enumerate(nav.links()["cli"]):
-        tempnav = nav.links()["cli"][k]
-
-        hcli_type = tempnav.links()["profile"][0].uri.split('#', 1)[1]
-        if hcli_type == config.hcli_execution_type:
-            method = tempnav()["http"]
-            nav = tempnav["cli"][0]
-            flexible_executor(nav.uri, method)
-            sys.exit(0)
+    try:
+        for k, z in enumerate(nav.links()["cli"]):
+            tempnav = nav.links()["cli"][k]
+
+            hcli_type = tempnav.links()["profile"][0].uri.split('#', 1)[1]
+            if hcli_type == config.hcli_execution_type:
+                method = tempnav()["http"]
+                nav = tempnav["cli"][0]
+                flexible_executor(nav.uri, method)
+                sys.exit(0)
+    except KeyError:
+        hutils.eprint(config.cliname + ": " + "command/parameter confusion. try escaping parameter: e.g., \\\"param\\\" or \\\'param\\\'.")
+        for_help()
+        sys.exit(2)
 
     hutils.eprint(config.cliname + ": " + "unable to execute.")
     for_help()
     sys.exit(2)
 
 # attempts to pull at the root of the hcli to auto configure the cli
 def pull(url):
```

### Comparing `huckle-3.0.1/huckle/huckle.py` & `huckle-3.0.2/huckle/huckle.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,25 @@
         if i == length - 1:
             hclinav.traverse_execution(nav)
 
 # huckle's minimal set of commands
 def cli():
 
     if len(sys.argv) > 2:
-    
+
         if sys.argv[1] == "cli" and sys.argv[2] == "install":
-            
+
             if len(sys.argv) > 3:
                 hclinav.pull(sys.argv[3])
-                
+
             else:
                 huckle_help()
-            
+
         elif sys.argv[1] == "cli" and sys.argv[2] == "run":
-                
+
             if len(sys.argv) > 3:
                 config.parse_configuration(sys.argv[3])
                 navigate(sys.argv[3:])
 
             else:
                 huckle_help()
```

### Comparing `huckle-3.0.1/huckle/hutils.py` & `huckle-3.0.2/huckle/hutils.py`

 * *Files identical despite different names*

### Comparing `huckle-3.0.1/huckle.egg-info/PKG-INFO` & `huckle-3.0.2/huckle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.0.1
+Version: 3.0.2
 Summary: A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `huckle-3.0.1/setup.py` & `huckle-3.0.2/setup.py`

 * *Files identical despite different names*

