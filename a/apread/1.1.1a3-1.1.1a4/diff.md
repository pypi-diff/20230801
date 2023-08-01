# Comparing `tmp/apread-1.1.1a3.tar.gz` & `tmp/apread-1.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apread-1.1.1a3.tar", last modified: Mon Apr 24 22:09:52 2023, max compression
+gzip compressed data, was "apread-1.1.1a4.tar", last modified: Tue Aug  1 19:48:54 2023, max compression
```

## Comparing `apread-1.1.1a3.tar` & `apread-1.1.1a4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:09:52.694482 apread-1.1.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 22:09:41.000000 apread-1.1.1a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-24 22:09:52.694482 apread-1.1.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-04-24 22:09:41.000000 apread-1.1.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:09:52.694482 apread-1.1.1a3/apread/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 22:09:41.000000 apread-1.1.1a3/apread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-04-24 22:09:41.000000 apread-1.1.1a3/apread/apreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-24 22:09:41.000000 apread-1.1.1a3/apread/binaryReader.py
--rw-r--r--   0 runner    (1001) docker     (123)    17564 2023-04-24 22:09:41.000000 apread-1.1.1a3/apread/entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-24 22:09:41.000000 apread-1.1.1a3/apread/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-24 22:09:41.000000 apread-1.1.1a3/apread/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:09:52.694482 apread-1.1.1a3/apread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-24 22:09:52.000000 apread-1.1.1a3/apread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-24 22:09:52.000000 apread-1.1.1a3/apread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:09:52.000000 apread-1.1.1a3/apread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 22:09:52.000000 apread-1.1.1a3/apread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 22:09:52.000000 apread-1.1.1a3/apread.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:09:52.694482 apread-1.1.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-24 22:09:41.000000 apread-1.1.1a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:09:52.694482 apread-1.1.1a3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-24 22:09:41.000000 apread-1.1.1a3/test/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:48:54.044951 apread-1.1.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-01 19:48:45.000000 apread-1.1.1a4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-08-01 19:48:54.044951 apread-1.1.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-08-01 19:48:45.000000 apread-1.1.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:48:54.044951 apread-1.1.1a4/apread/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 19:48:45.000000 apread-1.1.1a4/apread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-08-01 19:48:45.000000 apread-1.1.1a4/apread/apreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-01 19:48:45.000000 apread-1.1.1a4/apread/binaryReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-01 19:48:45.000000 apread-1.1.1a4/apread/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-01 19:48:45.000000 apread-1.1.1a4/apread/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-01 19:48:45.000000 apread-1.1.1a4/apread/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:48:54.044951 apread-1.1.1a4/apread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-08-01 19:48:53.000000 apread-1.1.1a4/apread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-01 19:48:54.000000 apread-1.1.1a4/apread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:48:53.000000 apread-1.1.1a4/apread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 19:48:53.000000 apread-1.1.1a4/apread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 19:48:53.000000 apread-1.1.1a4/apread.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:48:54.044951 apread-1.1.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-01 19:48:45.000000 apread-1.1.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:48:54.044951 apread-1.1.1a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-01 19:48:45.000000 apread-1.1.1a4/test/testing.py
```

### Comparing `apread-1.1.1a3/LICENSE.txt` & `apread-1.1.1a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apread-1.1.1a3/PKG-INFO` & `apread-1.1.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apread
-Version: 1.1.1a3
+Version: 1.1.1a4
 Summary: Import data from CatmanAP binary files.
 Home-page: https://github.com/leonbohmann/apreader
 Author: Leon Bohmann
 Author-email: mail@leonbohmann.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -179,15 +179,15 @@
 ## Release History
 
 ### Version 1.1.1-alpha1
 
 * Added converted timestamp property on channels (`Channel.date`)
   * *Property `Channel.time` will be deleted at some point in the future...*
 * Parallel reading of binary files
-  * Max degree of parallelism is defined with maximum amount of processors
+  * Max degree of parallelism is automatically set to amount of available cores
 * ----------------------------
 * ----------------------------
   
 #### Version 1.1
 
 ##### Breaking changes
```

### Comparing `apread-1.1.1a3/README.md` & `apread-1.1.1a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 ## Release History
 
 ### Version 1.1.1-alpha1
 
 * Added converted timestamp property on channels (`Channel.date`)
   * *Property `Channel.time` will be deleted at some point in the future...*
 * Parallel reading of binary files
-  * Max degree of parallelism is defined with maximum amount of processors
+  * Max degree of parallelism is automatically set to amount of available cores
 * ----------------------------
 * ----------------------------
   
 #### Version 1.1
 
 ##### Breaking changes
```

### Comparing `apread-1.1.1a3/apread/apreader.py` & `apread-1.1.1a4/apread/apreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,18 @@
                 if re.match(r"([T|t]ime)|([Z|z]eit)",channel.Name) is not None:
                     timeChannel = channel
                     # there is only one time-channel
                     break
 
                 # instead of assuming, ask the user if the timechannel is the one with "seconds"
                 if "s" == channel.unit:
+                    # this should be uncommented for the testing timing functions to be usable
+                    # timeChannel = channel
+                    # break
+                
                     if input(f"Is '{channel.Name}' your time/reference channel? [y/n] ") == "y":
                         timeChannel = channel
                         break
 # %%
 
             #%% sdasd
             # set the time-channel on every channel but itself
```

### Comparing `apread-1.1.1a3/apread/binaryReader.py` & `apread-1.1.1a4/apread/binaryReader.py`

 * *Files identical despite different names*

### Comparing `apread-1.1.1a3/apread/entries.py` & `apread-1.1.1a4/apread/entries.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
     """Time channel only."""
     # all other data-channels
     ChannelsY: List[Channel]
     """Data channels only."""
 
     # the data time interval with a fitting unit
     intervalstr: str
-    # the data time interval in milliseconds
+    # the data time interval in seconds
     interval: float
     # frequency of the corresponding time
     frequency: float
 
     # the file this group is located in
     fileName: str
     # fully qualifying name
@@ -415,22 +415,22 @@
         # determine frequency and time delta unit
         unit = 's'
         fac = 1
         if timeC.data[1] < 1:
             unit = 'ms'
             fac = 1e3
         if timeC.data[1] < 1e-3:
-            unit = 'ns'
+            unit = 'μs'
             fac = 1e6
         if timeC.data[1] < 1e-6:
-            unit = 'μs'
+            unit = 'ns'
             fac = 1e9
 
         self.intervalstr = f"{timeC.data[1]*fac:.3f}{unit}"
-        self.interval = timeC[1]/1e3
+        self.interval = timeC[1]
         self.frequency = 1/timeC.data[1]
 
     def __getitem__(self, key):
         """Return the time and all y-channels at index.
 
         Args:
             key (int): index
```

### Comparing `apread-1.1.1a3/apread/loader.py` & `apread-1.1.1a4/apread/loader.py`

 * *Files identical despite different names*

### Comparing `apread-1.1.1a3/apread/tools.py` & `apread-1.1.1a4/apread/tools.py`

 * *Files identical despite different names*

### Comparing `apread-1.1.1a3/apread.egg-info/PKG-INFO` & `apread-1.1.1a4/apread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apread
-Version: 1.1.1a3
+Version: 1.1.1a4
 Summary: Import data from CatmanAP binary files.
 Home-page: https://github.com/leonbohmann/apreader
 Author: Leon Bohmann
 Author-email: mail@leonbohmann.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -179,15 +179,15 @@
 ## Release History
 
 ### Version 1.1.1-alpha1
 
 * Added converted timestamp property on channels (`Channel.date`)
   * *Property `Channel.time` will be deleted at some point in the future...*
 * Parallel reading of binary files
-  * Max degree of parallelism is defined with maximum amount of processors
+  * Max degree of parallelism is automatically set to amount of available cores
 * ----------------------------
 * ----------------------------
   
 #### Version 1.1
 
 ##### Breaking changes
```

### Comparing `apread-1.1.1a3/setup.py` & `apread-1.1.1a4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="apread",
-    version="1.1.1-alpha3",
+    version="1.1.1-alpha4",
     description="Import data from CatmanAP binary files.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/leonbohmann/apreader",
     author="Leon Bohmann",
     author_email="mail@leonbohmann.de",
     license="MIT",
```

