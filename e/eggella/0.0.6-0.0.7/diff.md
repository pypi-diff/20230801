# Comparing `tmp/eggella-0.0.6.tar.gz` & `tmp/eggella-0.0.7.tar.gz`

## Comparing `eggella-0.0.6.tar` & `eggella-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/__init__.py
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/app.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/exceptions.py
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/manager.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/abc.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/arg_caster.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/completer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/handler.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/objects.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/events/abc.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/events/events.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.6/.gitignore
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 eggella-0.0.6/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 eggella-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/__init__.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/app.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/exceptions.py
+-rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/manager.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/abc.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/arg_caster.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/completer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/handler.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/objects.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/command/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/events/abc.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/events/events.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.7/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eggella-0.0.7/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 eggella-0.0.7/PKG-INFO
```

### Comparing `eggella-0.0.6/eggella/app.py` & `eggella-0.0.7/eggella/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 
 from prompt_toolkit import HTML, PromptSession
 from prompt_toolkit.completion.fuzzy_completer import FuzzyCompleter
 from prompt_toolkit.completion.nested import NestedDict
 from prompt_toolkit.formatted_text import FormattedText
 
 from eggella.command.abc import ABCCommandHandler
-from eggella.exceptions import CommandNotFoundError, CommandParseError, CommandTooManyArgumentsError, \
-    CommandArgumentValueError
+from eggella.command.objects import Command
+from eggella.exceptions import (
+    CommandArgumentValueError,
+    CommandNotFoundError,
+    CommandParseError,
+    CommandTooManyArgumentsError,
+)
 from eggella.fsm.fsm import FsmController, IntStateGroup
 from eggella.manager import CommandManager, EventManager
 from eggella.shortcuts.cmd_shortcuts import CmdShortCuts
 
 PromptLikeMsg = Union[str, FormattedText, Callable[..., Union[FormattedText, List[Tuple[str, str]]]]]
 
 _DEFAULT_INTRO_MSG = HTML(
@@ -89,45 +94,44 @@
         key: Optional[str] = None,
         short_description: Optional[str] = None,
         *,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
         nested_completions: Optional[NestedDict] = None,
         nested_meta: Optional[Dict[str, Any]] = None,
+        is_visible: bool = True,
     ):
         return self._command_manager.command(
             key,
             short_description=short_description,
             usage=usage,
             cmd_handler=cmd_handler,
             nested_completions=nested_completions,
             nested_meta=nested_meta,
+            is_visible=is_visible,
         )
 
     def on_state(self, state: IntStateGroup):
         return self.fsm.state(state)
 
     def register_states(self, states: Type[IntStateGroup]):
         self.fsm.attach(states)
 
     def register_command(
         self,
         func: Callable,
         key: Optional[str] = None,
         short_description: Optional[str] = None,
         *,
+        is_visible: bool = True,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
     ):
         self._command_manager.register_command(
-            func,
-            key,
-            short_description=short_description,
-            usage=usage,
-            cmd_handler=cmd_handler,
+            func, key, short_description=short_description, usage=usage, cmd_handler=cmd_handler, is_visible=is_visible
         )
 
     @overload
     def register_event(
         self,
         name: Literal["start", "close", "kb_interrupt", "eof", "command_not_found", "command_complete"],
         func: Callable,
@@ -171,14 +175,17 @@
         for event in self._event_manager.startup_events:
             event()
 
     def _handle_close_events(self):
         for event in self._event_manager.close_events:
             event()
 
+    def get_command(self, key: str) -> Command:
+        return self._command_manager.get(key)
+
     def _handle_commands(self):
         while True:
             try:
                 completer = FuzzyCompleter(completer=self._command_manager.get_completer())
                 result = self.session.prompt(self.prompt_msg, completer=completer)
                 if not result:
                     continue
@@ -189,15 +196,17 @@
                 else:
                     key, args = tokens[0], tokens[1]
 
                 if result := self._command_manager.exec(key, args):
                     self._event_manager.command_complete_event(result)
             except CommandNotFoundError:
                 self._event_manager.command_not_found_event(key, args)
-                self._event_manager.command_suggest_event(key, self._command_manager.commands.keys())
+                self._event_manager.command_suggest_event(
+                    key, [c.key for c in self._command_manager.commands.values() if c.is_visible]
+                )
             except CommandParseError:
                 self._event_manager.command_error_event(key, args)
             except CommandTooManyArgumentsError as exc:
                 self._event_manager.command_many_args_err_event(key, args, exc)
             except CommandArgumentValueError as exc:
                 self._event_manager.command_argument_value_err_event(key, args, exc)
             except KeyboardInterrupt:
```

### Comparing `eggella-0.0.6/eggella/manager.py` & `eggella-0.0.7/eggella/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,28 @@
 from prompt_toolkit.completion.nested import NestedDict
 
 from eggella.command.abc import ABCCommandHandler
 from eggella.command.completer import CommandCompleter
 from eggella.command.handler import CommandHandler
 from eggella.command.objects import Command
 from eggella.events.events import (
+    OnCommandArgumentValueError,
     OnCommandCompleteSuccess,
     OnCommandError,
     OnCommandNotFound,
+    OnCommandTooManyArgumentsError,
     OnEOFError,
     OnKeyboardInterrupt,
-    OnSuggest, OnCommandTooManyArgumentsError, OnCommandArgumentValueError,
+    OnSuggest,
+)
+from eggella.exceptions import (
+    CommandArgumentValueError,
+    CommandNotFoundError,
+    CommandTooManyArgumentsError,
 )
-from eggella.exceptions import CommandNotFoundError, CommandTooManyArgumentsError, CommandArgumentValueError
 from eggella.shortcuts.help_pager import gen_help_pager
 
 if TYPE_CHECKING:
     from eggella.app import Eggella
 
 
 _ErrorEventsMapping = Dict[str, Tuple[Type[BaseException], ...]]
@@ -54,23 +60,27 @@
                 kwargs[key] = value
             else:
                 args.append(token)
         return tuple(args), kwargs
 
     def exec(self, key: str, args: str):
         command = self.get(key)
+
+        if not command.is_visible:
+            raise CommandNotFoundError
+
         try:
             return command.handle(args)
         except TypeError as e:
             if 'too many positional arguments' in e.args[0]:
                 raise CommandTooManyArgumentsError("Too many arguments") from e
             else:
                 raise e
         except ValueError as e:
-            raise CommandArgumentValueError(f"Wrong argument type passed: {e.args}")
+            raise CommandArgumentValueError(f"Wrong argument type passed: {e.args}") from e
         except BaseException as e:
             if err_handler := self.error_events.get(command.fn.__name__):
                 handle_exceptions = self.handled_exceptions.get(command.fn.__name__, None)
                 if handle_exceptions and any(e.__class__ == exc for exc in handle_exceptions):
                     _args, _kwargs = self._simple_parse_arguments(args)
                     return err_handler(key, e, *_args, **_kwargs)
                 else:
@@ -101,15 +111,15 @@
 
             return decorator_wrapper
 
         return decorator
 
     @property
     def all_completions(self) -> List[Tuple[str, str]]:
-        return [com.completion for com in self.commands.values()]
+        return [com.completion for com in self.commands.values() if com.is_visible]
 
     def get(self, key: str) -> Command:
         if command := self.commands.get(key, None):
             return command
         raise CommandNotFoundError(f"Command {key} not founded")
 
     def command(
@@ -117,24 +127,26 @@
         key: Optional[str] = None,
         *,
         short_description: Optional[str] = None,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
         nested_completions: Optional[NestedDict] = None,
         nested_meta: Optional[Dict[str, Any]] = None,
+        is_visible: bool = True,
     ):
         def decorator(func: Callable):
             self.register_command(
                 func,
                 key=key,
                 short_description=short_description,
                 usage=usage,
                 cmd_handler=cmd_handler,
                 nested_completions=nested_completions,
                 nested_meta=nested_meta,
+                is_visible=is_visible,
             )
 
             @wraps(func)
             def wrapper(*args, **kwargs):
                 return func(*args, **kwargs)
 
             return wrapper
@@ -147,14 +159,15 @@
         key: Optional[str] = None,
         *,
         short_description: Optional[str] = None,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
         nested_completions: Optional[NestedDict] = None,
         nested_meta: Optional[Dict[str, Any]] = None,
+        is_visible: bool = True,
     ):
         if not key:
             key = func.__name__
         if self.commands.get(key):
             raise TypeError(f"Command '{key}' already register")
 
         if not cmd_handler:
@@ -162,24 +175,26 @@
                 fn=func,
                 key=key,
                 handler=CommandHandler(),
                 short_description=short_description,
                 usage=usage,
                 nested_completions={key: nested_completions},
                 nested_meta=nested_meta or {},
+                is_visible=is_visible,
             )
         elif cmd_handler:
             self.commands[key] = Command(
                 fn=func,
                 key=key,
                 handler=cmd_handler,
                 short_description=short_description,
                 usage=usage,
                 nested_completions={key: nested_completions},
                 nested_meta=nested_meta or {},
+                is_visible=is_visible,
             )
 
     def _help_command(self, key: Optional[str] = None):
         """show help or show pager documentation for all commands if not argument passed"""
         if not key:
             commands = self.commands.values()
             gen_help_pager(self._app, commands)
```

### Comparing `eggella-0.0.6/eggella/command/arg_caster.py` & `eggella-0.0.7/eggella/command/arg_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/eggella/command/completer.py` & `eggella-0.0.7/eggella/command/completer.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,17 @@
             text_before_cursor = text_before_cursor.lower()
         text_arr = text_before_cursor.split(" ")
         last_words = text_arr[-1]
         completions = self.__get_current_completions(text_arr[:-1])
         if all(isinstance(d, dict) for d in completions):
             try:
                 nested, meta = completions
-                yield from NestedCommandCompleter.from_nested_dict(nested, meta).get_completions(document, complete_event)
+                yield from NestedCommandCompleter.from_nested_dict(nested, meta).get_completions(
+                    document, complete_event
+                )
             except (ValueError, TypeError):  # unpack err
                 yield
         else:
             # echo({'echo': None}, {})
             for completion, meta in completions:
                 if completion not in document.text_before_cursor and "=" not in last_words:
                     yield Completion(completion, -len(last_words), display_meta=meta or "")
```

### Comparing `eggella-0.0.6/eggella/command/handler.py` & `eggella-0.0.7/eggella/command/handler.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/eggella/command/objects.py` & `eggella-0.0.7/eggella/command/objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import inspect
-from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple
+from dataclasses import dataclass, field
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from prompt_toolkit.completion.nested import NestedDict
 
 from eggella.command.abc import ABCCommandHandler
 from eggella.command.handler import CommandHandler
 
 
-class Command(NamedTuple):
+@dataclass
+class Command:
     fn: Callable[..., Any]
     key: str
     handler: ABCCommandHandler = CommandHandler()
     usage: Optional[str] = None
     short_description: Optional[str] = None
     nested_completions: Optional[NestedDict] = None
-    nested_meta: Dict[str, Any] = {}
+    nested_meta: Dict[str, Any] = field(default_factory=dict)
+    is_visible: bool = True
 
     def handle(self, command_text: str) -> Tuple[Tuple[Any, ...], Dict[str, Any]]:
         args, kwargs = self.handler.handle(self.fn, command_text)
         return self.fn(*args, **kwargs)
 
     @property
     def arguments(self) -> List[str]:
```

### Comparing `eggella-0.0.6/eggella/events/events.py` & `eggella-0.0.7/eggella/events/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,18 +66,19 @@
         suggested_command = None
         ratio = 0
         for possible_command in possible_commands:
             possible_ratio = SequenceMatcher(None, command, possible_command).ratio()
             if possible_ratio > ratio:
                 ratio = possible_ratio  # type: ignore
                 suggested_command = possible_command
-        print_ft(
-            HTML(f"Did your mean: <mean>{suggested_command}</mean> ?"),
-            style=self._STYLE,
-        )
+        if suggested_command:
+            print_ft(
+                HTML(f"Did your mean: <mean>{suggested_command}</mean> ?"),
+                style=self._STYLE,
+            )
 
 
 class OnCommandCompleteSuccess(ABCEvent):
     _STYLE = Style.from_dict({"out": "#696969 bold"})
 
     def __call__(self, result: Any):
         if result:
@@ -94,26 +95,30 @@
         {
             "cmd_key": "#7d7c80 italic",
         }
     )
 
     def __call__(self, key: str, args: str, exc: Exception):
         print_ft(
-            HTML(f"<ansired>Error!</ansired> `<cmd_key>{key}</cmd_key>` "
-                 f"accept wrong argument type. ({', '.join(exc.args)})"),
+            HTML(
+                f"<ansired>Error!</ansired> `<cmd_key>{key}</cmd_key>` "
+                f"accept wrong argument type. ({', '.join(exc.args)})"
+            ),
             style=self._STYLE,
         )
 
 
 class OnCommandTooManyArgumentsError(ABCEvent):
     _STYLE = Style.from_dict(
         {
             "cmd_key": "#7d7c80 italic",
         }
     )
 
     def __call__(self, key: str, args: str, exc: Exception):
         print_ft(
-            HTML(f"<ansired>Error!</ansired> `<cmd_key>{key}</cmd_key>` "
-                 f"too many arguments passed ({', '.join(exc.args)})"),
+            HTML(
+                f"<ansired>Error!</ansired> `<cmd_key>{key}</cmd_key>` "
+                f"too many arguments passed ({', '.join(exc.args)})"
+            ),
             style=self._STYLE,
         )
```

### Comparing `eggella-0.0.6/eggella/fsm/fsm.py` & `eggella-0.0.7/eggella/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.7/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/eggella/shortcuts/help_pager.py` & `eggella-0.0.7/eggella/shortcuts/help_pager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/eggella/tools/type_caster.py` & `eggella-0.0.7/eggella/tools/type_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/.gitignore` & `eggella-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/README.md` & `eggella-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,8 +40,10 @@
     return "Hello, world!"
 
 
 if __name__ == '__main__':
     app.loop()
 ```
 
+![quickstart](docs/gifs/quickstart.gif)
+
 See the [documentation](https://eggella.readthedocs.io/en/latest/) and [examples](examples)!
```

### Comparing `eggella-0.0.6/pyproject.toml` & `eggella-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eggella-0.0.6/PKG-INFO` & `eggella-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eggella
-Version: 0.0.6
+Version: 0.0.7
 Summary: Create awesome command line applications with less effort
 Project-URL: Documentation, https://github.com/unknown/eggella#readme
 Project-URL: Issues, https://github.com/unknown/eggella/issues
 Project-URL: Source, https://github.com/unknown/eggella
 Author: georgiy
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -66,8 +66,10 @@
     return "Hello, world!"
 
 
 if __name__ == '__main__':
     app.loop()
 ```
 
+![quickstart](docs/gifs/quickstart.gif)
+
 See the [documentation](https://eggella.readthedocs.io/en/latest/) and [examples](examples)!
```

