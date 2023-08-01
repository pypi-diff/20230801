# Comparing `tmp/eggella-0.0.7.tar.gz` & `tmp/eggella-0.0.8.tar.gz`

## Comparing `eggella-0.0.7.tar` & `eggella-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/__init__.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/app.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/exceptions.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/manager.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/abc.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/arg_caster.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/completer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/handler.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/objects.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/events/abc.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/events/events.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.7/.gitignore
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eggella-0.0.7/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 eggella-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/__init__.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/app.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/exceptions.py
+-rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/manager.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/abc.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/arg_caster.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/completer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/handler.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/objects.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/events/abc.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/events/events.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eggella-0.0.8/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 eggella-0.0.8/PKG-INFO
```

### Comparing `eggella-0.0.7/eggella/app.py` & `eggella-0.0.8/eggella/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     Any,
     Callable,
     Dict,
     Hashable,
     List,
     Literal,
     Optional,
+    Set,
     Tuple,
     Type,
     Union,
     overload,
 )
 
 from prompt_toolkit import HTML, PromptSession
@@ -36,35 +37,40 @@
     "<ansigreen>Press |TAB| or type</ansigreen> help <ansigreen>for get commands information</ansigreen>"
 )
 
 
 class Eggella:
     __app_instances__: Dict[str, "Eggella"] = {}
 
-    def __new__(cls, app_name: str, msg: PromptLikeMsg = "~> ") -> "Eggella":
+    def __new__(cls, app_name: str, msg: PromptLikeMsg = "> ") -> "Eggella":
         if _app := cls.__app_instances__.get(app_name):
             return _app
 
         new_app = super().__new__(cls)
         cls.__app_instances__[app_name] = new_app
         return new_app
 
-    def __init__(self, app_name: str, msg: PromptLikeMsg = "~> "):
+    def __init__(self, app_name: str, msg: PromptLikeMsg = "> "):
         self.app_name = app_name
         self.prompt_msg = msg
         self.session: PromptSession = PromptSession(msg)
         self.cmd = CmdShortCuts()
 
         self.CTX: Dict[Hashable, Any] = {}
         self._intro: Union[HTML, PromptLikeMsg] = _DEFAULT_INTRO_MSG
         self._doc: str = ""
         # managers
         self._command_manager: CommandManager = CommandManager(self)
         self._event_manager = EventManager(self)
 
+        # TODO create blueprints manager
+        self._blueprints: List["Eggella"] = []
+        self._loaded_blueprints: Set[str] = set()
+        self.overwrite_commands_from_blueprints: bool = False
+
         # fsm
         self.fsm = FsmController(self)
 
     @property
     def documentation(self):
         return self._doc
 
@@ -112,14 +118,39 @@
 
     def on_state(self, state: IntStateGroup):
         return self.fsm.state(state)
 
     def register_states(self, states: Type[IntStateGroup]):
         self.fsm.attach(states)
 
+    def register_blueprint(self, *apps: "Eggella"):
+        for app in apps:
+            self._blueprints.append(app)
+
+    def _load_blueprints(self):
+        for blueprint in self._blueprints:
+            if blueprint.app_name in self._loaded_blueprints:
+                continue
+
+            for key, command in blueprint._command_manager.commands.items():
+                if self._command_manager.commands.get(key) and not self.overwrite_commands_from_blueprints:
+                    raise TypeError(f"Command '{key}' already register")
+                self._command_manager.commands[key] = command
+
+            for key, fsm_state in blueprint.fsm.fsm_storage.items():
+                self.fsm.fsm_storage[key] = fsm_state
+
+            for start_ev in blueprint._event_manager.startup_events:
+                self._event_manager.startup_events.append(start_ev)
+
+            for close_ev in blueprint._event_manager.close_events:
+                self._event_manager.close_events.append(close_ev)
+
+            self._loaded_blueprints.add(blueprint.app_name)
+
     def register_command(
         self,
         func: Callable,
         key: Optional[str] = None,
         short_description: Optional[str] = None,
         *,
         is_visible: bool = True,
@@ -162,14 +193,15 @@
         if self.has_command(key):
             self._command_manager.commands.pop(key)
         else:
             raise KeyError
 
     def loop(self):
         self.cmd.print_ft(self.intro)
+        self._load_blueprints()
         self._command_manager.register_buildin_commands()
         self._handle_startup_events()
         self._handle_commands()
         self._handle_close_events()
 
     def _handle_startup_events(self):
         for event in self._event_manager.startup_events:
```

### Comparing `eggella-0.0.7/eggella/manager.py` & `eggella-0.0.8/eggella/manager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/command/arg_caster.py` & `eggella-0.0.8/eggella/command/arg_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/command/completer.py` & `eggella-0.0.8/eggella/command/completer.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/command/handler.py` & `eggella-0.0.8/eggella/command/handler.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/command/objects.py` & `eggella-0.0.8/eggella/command/objects.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/events/events.py` & `eggella-0.0.8/eggella/events/events.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/fsm/fsm.py` & `eggella-0.0.8/eggella/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.8/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/shortcuts/help_pager.py` & `eggella-0.0.8/eggella/shortcuts/help_pager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/eggella/tools/type_caster.py` & `eggella-0.0.8/eggella/tools/type_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/.gitignore` & `eggella-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/README.md` & `eggella-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/pyproject.toml` & `eggella-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eggella-0.0.7/PKG-INFO` & `eggella-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eggella
-Version: 0.0.7
+Version: 0.0.8
 Summary: Create awesome command line applications with less effort
 Project-URL: Documentation, https://github.com/unknown/eggella#readme
 Project-URL: Issues, https://github.com/unknown/eggella/issues
 Project-URL: Source, https://github.com/unknown/eggella
 Author: georgiy
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

