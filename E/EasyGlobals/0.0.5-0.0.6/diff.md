# Comparing `tmp/easyglobals-0.0.5.tar.gz` & `tmp/easyglobals-0.0.6.tar.gz`

## Comparing `easyglobals-0.0.5.tar` & `easyglobals-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/Easy_Globals.iml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0    13306 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 easyglobals-0.0.5/src/EasyGlobals/EasyGlobals.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 easyglobals-0.0.5/src/EasyGlobals/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/attribute_test.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_complex.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_minimal.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_multiprocess_easyglobals.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_multiprocess_easyglobals2.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.5/LICENSE
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 easyglobals-0.0.5/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyglobals-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 easyglobals-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/Easy_Globals.iml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0    13249 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 easyglobals-0.0.6/src/EasyGlobals/EasyGlobals.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 easyglobals-0.0.6/src/EasyGlobals/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 easyglobals-0.0.6/tests/attribute_test.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.6/tests/example_complex.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.6/tests/example_minimal.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 easyglobals-0.0.6/tests/example_multiprocess_easyglobals.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 easyglobals-0.0.6/tests/example_multiprocess_easyglobals2.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 easyglobals-0.0.6/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 easyglobals-0.0.6/README.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 easyglobals-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 easyglobals-0.0.6/PKG-INFO
```

### Comparing `easyglobals-0.0.5/.idea/workspace.xml` & `easyglobals-0.0.6/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `easyglobals-0.0.5/.idea/workspace.xml` & `easyglobals-0.0.6/.idea/workspace.xml`

```diff
@@ -1,21 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="f94c1167-ab5b-4afc-b6d8-c986fd0deda2" name="Changes" comment="typo fix , some documentation and v0.0.3">
-      <change afterPath="$PROJECT_DIR$/build_instructions.txt" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/tests/attribute_test.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/tests/example_multiprocess_easyglobals2.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+    <list default="true" id="f94c1167-ab5b-4afc-b6d8-c986fd0deda2" name="Changes" comment="TCP no delay for more actual">
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/EasyGlobals/EasyGlobals.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/EasyGlobals/EasyGlobals.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/example_multiprocess_easyglobals.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/example_multiprocess_easyglobals.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -36,29 +30,30 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
+    "git-widget-placeholder": "main",
     "last_opened_file_path": "/home/pc/Documents/Easy_Globals/tests",
     "run.code.analysis.last.selected.profile": "pProject Default",
     "settings.editor.selected.configurable": "FeaturesTrainerSettingsPanel"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/Easy_Globals"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python.example_minimal">
+  <component name="RunManager" selected="Python.example_multiprocess_easyglobals">
     <configuration name="attribute_test" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="Easy_Globals"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -72,105 +67,105 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="example_minimal" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="example_complex" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="Easy_Globals"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/example_minimal.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/example_complex.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="example_multiprocess_easyglobals" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="example_minimal" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="Easy_Globals"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/example_multiprocess_easyglobals.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/example_minimal.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="example_multiprocess_easyglobals2" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="example_multiprocess_easyglobals" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="Easy_Globals"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/example_multiprocess_easyglobals2.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/example_multiprocess_easyglobals.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="setattr_testing" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="example_multiprocess_easyglobals2" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="Easy_Globals"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/setattr_testing.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/example_multiprocess_easyglobals2.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
-        <item itemvalue="Python.example_minimal"/>
-        <item itemvalue="Python.example_multiprocess_easyglobals2"/>
         <item itemvalue="Python.example_multiprocess_easyglobals"/>
+        <item itemvalue="Python.example_multiprocess_easyglobals2"/>
+        <item itemvalue="Python.example_complex"/>
+        <item itemvalue="Python.example_minimal"/>
         <item itemvalue="Python.attribute_test"/>
-        <item itemvalue="Python.setattr_testing"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="f94c1167-ab5b-4afc-b6d8-c986fd0deda2" name="Changes" comment=""/>
@@ -245,37 +240,57 @@
     <task id="LOCAL-00010" summary="readme update">
       <created>1685545134632</created>
       <option name="number" value="00010"/>
       <option name="presentableId" value="LOCAL-00010"/>
       <option name="project" value="LOCAL"/>
       <updated>1685545134632</updated>
     </task>
-    <option name="localTasksCounter" value="11"/>
+    <task id="LOCAL-00011" summary="TCP no delay for more actual">
+      <option name="closed" value="true"/>
+      <created>1690894688245</created>
+      <option name="number" value="00011"/>
+      <option name="presentableId" value="LOCAL-00011"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1690894688245</updated>
+    </task>
+    <option name="localTasksCounter" value="12"/>
     <servers/>
   </component>
+  <component name="Vcs.Log.Tabs.Properties">
+    <option name="TAB_STATES">
+      <map>
+        <entry key="MAIN">
+          <value>
+            <State/>
+          </value>
+        </entry>
+      </map>
+    </option>
+  </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="Added project files"/>
     <MESSAGE value="Imports"/>
     <MESSAGE value="for first upload"/>
     <MESSAGE value="Version 0.0.1"/>
     <MESSAGE value="Version 0.0.2 init fix"/>
     <MESSAGE value="typo fix , some documentation and v0.0.3"/>
     <MESSAGE value="readme update"/>
-    <option name="LAST_COMMIT_MESSAGE" value="readme update"/>
+    <MESSAGE value="TCP no delay for more actual"/>
+    <option name="LAST_COMMIT_MESSAGE" value="TCP no delay for more actual"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/attribute_test.py</url>
           <line>18</line>
           <option name="timeStamp" value="1"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/example_multiprocess_easyglobals2.py</url>
-          <line>22</line>
-          <option name="timeStamp" value="4"/>
+          <line>19</line>
+          <option name="timeStamp" value="5"/>
         </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
 </project>
```

### Comparing `easyglobals-0.0.5/.idea/inspectionProfiles/Project_Default.xml` & `easyglobals-0.0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.5/src/EasyGlobals/EasyGlobals.py` & `easyglobals-0.0.6/src/EasyGlobals/EasyGlobals.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,30 +4,37 @@
 from pymemcache.client import base
 from pymemcache import serde
 
 class Globals:
     # Don t put this in init, that will break with setattr
     memcached_ip = 'localhost'
     memcached_port = 11211
-    memcached_globals_client = base.Client((memcached_ip, memcached_port), serde=serde.pickle_serde)
+    memcached_globals_client = base.Client((memcached_ip, memcached_port), serde=serde.pickle_serde, connect_timeout=10, no_delay=True)
+    memcached_globals_client.cache_memlimit(8000)
 
-    def globals_log_error_message(self, Exception):
-        if Exception == ConnectionRefusedError:
+
+    def log_error_message_globals(self, exception):
+        if exception == ConnectionRefusedError:
             exception_info = traceback.format_exc(limit=1)
-            # print(exception_info)
             logging.log(level=40 , msg=exception_info)
             logging.log(level = 40, msg =
                  (f'{30*"*"} Error: EasyGlobals failed to connect to Memcached. {30*"*"}\n'
                   f'-       Is Memcahed installed? https://github.com/YacobBY/Easy_Globals \n'
                   f'-       Is the Memcached server running on port {self.memcached_port}?'))
+
     def __setattr__(self, key, value):
         try:
             self.memcached_globals_client.set(key, value)
         except ConnectionRefusedError:
-            self.globals_log_error_message(ConnectionRefusedError)
-
+            self.log_error_message_globals(ConnectionRefusedError)
 
     def __getattr__(self, key):
         try:
             return self.memcached_globals_client.get(key)
         except ConnectionRefusedError:
-            self.globals_log_error_message(ConnectionRefusedError)
+            self.log_error_message_globals(ConnectionRefusedError)
+
+    def __getitem__(self, key):
+        return getattr(self, key)
+
+    def __setitem__(self, key, value):
+        return setattr(self, key, value)
```

### Comparing `easyglobals-0.0.5/tests/attribute_test.py` & `easyglobals-0.0.6/tests/attribute_test.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.5/tests/example_complex.py` & `easyglobals-0.0.6/tests/example_complex.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.5/.gitignore` & `easyglobals-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.5/LICENSE` & `easyglobals-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.5/README.md` & `easyglobals-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Introduction
- EasyGlobals is an easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory.
+ EasyGlobals is an easy to use variable sharing library for Python that can quickly share almost all types of variables and full Python objects between processes as if they had shared memory.
 
 It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax. No need for Multiprocessing Manager dicts, queues and other complex data pipelines in your program anymore.
 
 # Usage
 After installation following the instructions down below, try running the following example
 ```
 import EasyGlobals
```

### Comparing `easyglobals-0.0.5/pyproject.toml` & `easyglobals-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "EasyGlobals"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
     "pymemcache"
 ]
 authors = [
-  { name="Yacob", email="asnaeb2@gmail.com" },
+  { name="Y", email="asnaeb2@gmail.com" },
 ]
 description = "An easy to use variable sharing library for Python using Memcached to can quickly share complex objects between processes as if they had shared memory."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `easyglobals-0.0.5/PKG-INFO` & `easyglobals-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: EasyGlobals
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy to use variable sharing library for Python using Memcached to can quickly share complex objects between processes as if they had shared memory.
 Project-URL: Homepage, https://github.com/YacobBY/Easy_Globals
 Project-URL: Bug Tracker, https://github.com/YacobBY/Easy_Globals/issues
-Author-email: Yacob <asnaeb2@gmail.com>
+Author-email: Y <asnaeb2@gmail.com>
 License-File: LICENSE
 Keywords: Globals,Python,Shared memory
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pymemcache
 Description-Content-Type: text/markdown
 
 # Introduction
- EasyGlobals is an easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory.
+ EasyGlobals is an easy to use variable sharing library for Python that can quickly share almost all types of variables and full Python objects between processes as if they had shared memory.
 
 It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax. No need for Multiprocessing Manager dicts, queues and other complex data pipelines in your program anymore.
 
 # Usage
 After installation following the instructions down below, try running the following example
 ```
 import EasyGlobals
```

