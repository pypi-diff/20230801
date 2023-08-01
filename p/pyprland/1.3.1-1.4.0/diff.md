# Comparing `tmp/pyprland-1.3.1.tar.gz` & `tmp/pyprland-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-1.3.1.tar", max compression
+gzip compressed data, was "pyprland-1.4.0.tar", max compression
```

## Comparing `pyprland-1.3.1.tar` & `pyprland-1.4.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0     8090 2023-05-03 20:05:11.985744 pyprland-1.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 18:41:04.588762 pyprland-1.3.1/pyprland/__init__.py
--rwxr-xr-x   0        0        0     5275 2023-04-30 14:37:56.478027 pyprland-1.3.1/pyprland/command.py
--rw-r--r--   0        0        0      118 2023-04-27 18:41:04.588762 pyprland-1.3.1/pyprland/common.py
--rw-r--r--   0        0        0     2117 2023-04-28 10:09:47.980551 pyprland-1.3.1/pyprland/ipc.py
--rw-r--r--   0        0        0        0 2023-04-27 18:41:04.588762 pyprland-1.3.1/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      148 2023-04-27 18:44:06.597774 pyprland-1.3.1/pyprland/plugins/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      164 2023-05-03 20:54:59.005595 pyprland-1.3.1/pyprland/plugins/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1855 2023-04-29 15:18:14.972474 pyprland-1.3.1/pyprland/plugins/__pycache__/attract_lost_windows.cpython-310.pyc
--rw-r--r--   0        0        0      458 2023-04-27 18:01:47.746725 pyprland-1.3.1/pyprland/plugins/__pycache__/experimental.cpython-310.pyc
--rw-r--r--   0        0        0      936 2023-04-27 18:44:06.597774 pyprland-1.3.1/pyprland/plugins/__pycache__/interface.cpython-310.pyc
--rw-r--r--   0        0        0     1285 2023-05-03 20:54:59.005595 pyprland-1.3.1/pyprland/plugins/__pycache__/interface.cpython-311.pyc
--rw-r--r--   0        0        0     1928 2023-04-29 21:15:35.763119 pyprland-1.3.1/pyprland/plugins/__pycache__/lost_windows.cpython-310.pyc
--rw-r--r--   0        0        0     3460 2023-05-04 18:42:34.460220 pyprland-1.3.1/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc
--rw-r--r--   0        0        0      989 2023-04-29 21:15:35.764119 pyprland-1.3.1/pyprland/plugins/__pycache__/magnify.cpython-310.pyc
--rw-r--r--   0        0        0     1581 2023-05-04 18:42:34.462220 pyprland-1.3.1/pyprland/plugins/__pycache__/magnify.cpython-311.pyc
--rw-r--r--   0        0        0     2229 2023-04-29 08:30:17.349907 pyprland-1.3.1/pyprland/plugins/__pycache__/monitors.cpython-310.pyc
--rw-r--r--   0        0        0     4743 2023-05-05 15:40:31.611716 pyprland-1.3.1/pyprland/plugins/__pycache__/monitors.cpython-311.pyc
--rw-r--r--   0        0        0     9708 2023-05-01 06:55:35.339694 pyprland-1.3.1/pyprland/plugins/__pycache__/scratchpads.cpython-310.pyc
--rw-r--r--   0        0        0    19778 2023-05-04 18:42:34.454220 pyprland-1.3.1/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc
--rw-r--r--   0        0        0     1445 2023-05-03 19:55:35.614143 pyprland-1.3.1/pyprland/plugins/__pycache__/shift_monitors.cpython-310.pyc
--rw-r--r--   0        0        0      891 2023-04-29 21:15:35.763119 pyprland-1.3.1/pyprland/plugins/__pycache__/toggle_dpms.cpython-310.pyc
--rw-r--r--   0        0        0     1333 2023-05-04 18:42:34.461220 pyprland-1.3.1/pyprland/plugins/__pycache__/toggle_dpms.cpython-311.pyc
--rw-r--r--   0        0        0     2709 2023-04-30 21:21:33.453785 pyprland-1.3.1/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-310.pyc
--rw-r--r--   0        0        0     4779 2023-05-04 18:42:34.464220 pyprland-1.3.1/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc
--rw-r--r--   0        0        0      106 2023-04-27 21:50:15.745405 pyprland-1.3.1/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0      350 2023-04-27 18:41:04.588762 pyprland-1.3.1/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     1454 2023-04-29 21:05:54.013318 pyprland-1.3.1/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0      735 2023-04-29 21:05:54.003318 pyprland-1.3.1/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     2969 2023-05-05 15:42:02.149497 pyprland-1.3.1/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0    11860 2023-04-30 21:23:29.432861 pyprland-1.3.1/pyprland/plugins/scratchpads.py
--rw-r--r--   0        0        0      808 2023-05-04 17:40:59.087396 pyprland-1.3.1/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0      411 2023-04-29 21:05:53.999318 pyprland-1.3.1/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     2218 2023-04-30 20:53:43.753682 pyprland-1.3.1/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      452 2023-05-05 15:43:05.613620 pyprland-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     8568 1970-01-01 00:00:00.000000 pyprland-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1244 2023-07-31 18:20:25.972576 pyprland-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 18:41:04.588762 pyprland-1.4.0/pyprland/__init__.py
+-rwxr-xr-x   0        0        0     7931 2023-07-31 18:15:32.657503 pyprland-1.4.0/pyprland/command.py
+-rw-r--r--   0        0        0     2212 2023-07-30 11:17:26.551074 pyprland-1.4.0/pyprland/common.py
+-rw-r--r--   0        0        0     2664 2023-07-30 11:17:26.552074 pyprland-1.4.0/pyprland/ipc.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:41:04.588762 pyprland-1.4.0/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      148 2023-04-27 18:44:06.597774 pyprland-1.4.0/pyprland/plugins/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      164 2023-05-03 20:54:59.005595 pyprland-1.4.0/pyprland/plugins/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1855 2023-04-29 15:18:14.972474 pyprland-1.4.0/pyprland/plugins/__pycache__/attract_lost_windows.cpython-310.pyc
+-rw-r--r--   0        0        0      458 2023-04-27 18:01:47.746725 pyprland-1.4.0/pyprland/plugins/__pycache__/experimental.cpython-310.pyc
+-rw-r--r--   0        0        0     4352 2023-07-31 18:56:13.448320 pyprland-1.4.0/pyprland/plugins/__pycache__/expose.cpython-311.pyc
+-rw-r--r--   0        0        0      936 2023-04-27 18:44:06.597774 pyprland-1.4.0/pyprland/plugins/__pycache__/interface.cpython-310.pyc
+-rw-r--r--   0        0        0     1679 2023-07-29 22:09:46.157367 pyprland-1.4.0/pyprland/plugins/__pycache__/interface.cpython-311.pyc
+-rw-r--r--   0        0        0     1928 2023-04-29 21:15:35.763119 pyprland-1.4.0/pyprland/plugins/__pycache__/lost_windows.cpython-310.pyc
+-rw-r--r--   0        0        0     3758 2023-07-31 18:56:13.417321 pyprland-1.4.0/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc
+-rw-r--r--   0        0        0      989 2023-04-29 21:15:35.764119 pyprland-1.4.0/pyprland/plugins/__pycache__/magnify.cpython-310.pyc
+-rw-r--r--   0        0        0     1458 2023-07-30 11:17:58.311403 pyprland-1.4.0/pyprland/plugins/__pycache__/magnify.cpython-311.pyc
+-rw-r--r--   0        0        0     2229 2023-04-29 08:30:17.349907 pyprland-1.4.0/pyprland/plugins/__pycache__/monitors.cpython-310.pyc
+-rw-r--r--   0        0        0     5578 2023-07-31 18:56:13.338322 pyprland-1.4.0/pyprland/plugins/__pycache__/monitors.cpython-311.pyc
+-rw-r--r--   0        0        0     9708 2023-05-01 06:55:35.339694 pyprland-1.4.0/pyprland/plugins/__pycache__/scratchpads.cpython-310.pyc
+-rw-r--r--   0        0        0    25056 2023-07-31 18:56:13.310322 pyprland-1.4.0/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc
+-rw-r--r--   0        0        0     1445 2023-05-03 19:55:35.614143 pyprland-1.4.0/pyprland/plugins/__pycache__/shift_monitors.cpython-310.pyc
+-rw-r--r--   0        0        0     2711 2023-07-31 18:56:13.419321 pyprland-1.4.0/pyprland/plugins/__pycache__/shift_monitors.cpython-311.pyc
+-rw-r--r--   0        0        0      891 2023-04-29 21:15:35.763119 pyprland-1.4.0/pyprland/plugins/__pycache__/toggle_dpms.cpython-310.pyc
+-rw-r--r--   0        0        0     1604 2023-07-31 18:56:13.446321 pyprland-1.4.0/pyprland/plugins/__pycache__/toggle_dpms.cpython-311.pyc
+-rw-r--r--   0        0        0     2709 2023-04-30 21:21:33.453785 pyprland-1.4.0/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-310.pyc
+-rw-r--r--   0        0        0     5315 2023-07-31 18:56:13.453320 pyprland-1.4.0/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc
+-rw-r--r--   0        0        0      148 2023-07-29 22:06:59.046911 pyprland-1.4.0/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     2419 2023-07-30 17:12:07.923812 pyprland-1.4.0/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0      699 2023-07-29 22:06:59.046911 pyprland-1.4.0/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     1710 2023-07-30 17:08:23.535992 pyprland-1.4.0/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0      760 2023-07-30 11:17:26.552074 pyprland-1.4.0/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     3610 2023-07-30 17:12:07.953812 pyprland-1.4.0/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0    14965 2023-07-30 17:12:08.142814 pyprland-1.4.0/pyprland/plugins/scratchpads.py
+-rw-r--r--   0        0        0     1065 2023-07-30 17:12:07.901811 pyprland-1.4.0/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0      543 2023-07-30 17:12:07.880811 pyprland-1.4.0/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     2598 2023-07-30 17:12:07.934812 pyprland-1.4.0/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      452 2023-08-01 16:24:59.500386 pyprland-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 pyprland-1.4.0/PKG-INFO
```

### Comparing `pyprland-1.3.1/pyprland/command.py` & `pyprland-1.4.0/pyprland/command.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,105 @@
 #!/bin/env python
+" Pyprland - an Hyprland companion app "
 import asyncio
+from typing import cast
 import json
 import sys
 import os
 import importlib
-import traceback
+import itertools
 
 
-from .ipc import get_event_stream
-from .common import DEBUG
+from .ipc import get_event_stream, init as ipc_init
+from .common import init_logger, get_logger, PyprError
 from .plugins.interface import Plugin
 
 CONTROL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.pyprland.sock'
 
 CONFIG_FILE = "~/.config/hypr/pyprland.json"
 
 
 class Pyprland:
+    "Main app object"
     server: asyncio.Server
     event_reader: asyncio.StreamReader
     stopped = False
     name = "builtin"
+    config: None | dict[str, dict] = None
 
     def __init__(self):
         self.plugins: dict[str, Plugin] = {}
+        self.log = get_logger()
 
     async def load_config(self, init=True):
-        self.config = json.loads(
-            open(os.path.expanduser(CONFIG_FILE), encoding="utf-8").read()
-        )
-        for name in self.config["pyprland"]["plugins"]:
+        """Loads the configuration
+
+        if `init` is true, also initializes the plugins"""
+        try:
+            with open(os.path.expanduser(CONFIG_FILE), encoding="utf-8") as f:
+                self.config = json.loads(f.read())
+        except FileNotFoundError as e:
+            self.log.critical(
+                "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
+            )
+            raise PyprError() from e
+
+        assert self.config
+
+        for name in cast(dict, self.config["pyprland"]["plugins"]):
             if name not in self.plugins:
                 modname = name if "." in name else f"pyprland.plugins.{name}"
                 try:
                     plug = importlib.import_module(modname).Extension(name)
                     if init:
                         await plug.init()
                     self.plugins[name] = plug
                 except Exception as e:
-                    print(f"Error loading plugin {name}: {e}")
-                    if DEBUG:
-                        traceback.print_exc()
+                    self.log.error("Error loading plugin %s:", name, exc_info=True)
+                    raise PyprError() from e
             if init:
-                await self.plugins[name].load_config(self.config)
+                try:
+                    await self.plugins[name].load_config(self.config)
+                except PyprError:
+                    raise
+                except Exception as e:
+                    self.log.error("Error initializing plugin %s:", name, exc_info=True)
+                    raise PyprError() from e
 
     async def _callHandler(self, full_name, *params):
+        "Call an event handler with params"
+
         for plugin in [self] + list(self.plugins.values()):
             if hasattr(plugin, full_name):
+                self.log.debug("%s.%s%s", plugin.name, full_name, params)
                 try:
                     await getattr(plugin, full_name)(*params)
-                except Exception as e:
-                    print(f"{plugin.name}::{full_name}({params}) failed:")
-                    traceback.print_exc()
+                except Exception as e:  # pylint: disable=W0718
+                    self.log.warning(
+                        "%s::%s(%s) failed:", plugin.name, full_name, params
+                    )
+                    self.log.exception(e)
 
     async def read_events_loop(self):
+        "Consumes the event loop and calls corresponding handlers"
         while not self.stopped:
             data = (await self.event_reader.readline()).decode()
             if not data:
-                print("Reader starved")
+                self.log.critical("Reader starved")
                 return
             cmd, params = data.split(">>")
             full_name = f"event_{cmd}"
 
-            if DEBUG:
-                print(f"EVT {full_name}({params.strip()})")
             await self._callHandler(full_name, params)
 
     async def read_command(self, reader, writer) -> None:
+        "Receives a socket command"
         data = (await reader.readline()).decode()
         if not data:
-            print("Server starved")
+            self.log.critical("Server starved")
             return
         if data == "exit\n":
             self.stopped = True
             writer.close()
             await writer.wait_closed()
             self.server.close()
             return
@@ -82,66 +108,88 @@
             cmd = args[0]
             args = []
         else:
             cmd = args[0]
             args = args[1:]
 
         full_name = f"run_{cmd}"
+        # Demos:
+        # run mako for notifications & uncomment this
+        # os.system(f"notify-send '{data}'")
 
-        if DEBUG:
-            print(f"CMD: {full_name}({args})")
+        self.log.debug("CMD: %s(%s)", full_name, args)
 
         await self._callHandler(full_name, *args)
 
     async def serve(self):
+        "Runs the server"
         try:
             async with self.server:
                 await self.server.serve_forever()
         finally:
             await asyncio.gather(*(plugin.exit() for plugin in self.plugins.values()))
 
     async def run(self):
+        "Runs the server and the event listener"
         await asyncio.gather(
             asyncio.create_task(self.serve()),
             asyncio.create_task(self.read_events_loop()),
         )
 
     run_reload = load_config
 
 
 async def run_daemon():
+    "Runs the server / daemon"
     manager = Pyprland()
+    err_count = itertools.count()
     manager.server = await asyncio.start_unix_server(manager.read_command, CONTROL)
-    events_reader, events_writer = await get_event_stream()
+    max_retry = 10
+    while True:
+        attempt = next(err_count)
+        try:
+            events_reader, events_writer = await get_event_stream()
+        except Exception as e:  # pylint: disable=W0718
+            if attempt > max_retry:
+                manager.log.critical("Failed to open hyprland event stream: %s.", e)
+                raise PyprError() from e
+            manager.log.warning(
+                "Failed to get event stream: %s}, retry %s/%s...", e, attempt, max_retry
+            )
+            await asyncio.sleep(1)
+        else:
+            break
+
     manager.event_reader = events_reader
 
     try:
         await manager.load_config()  # ensure sockets are connected first
-    except FileNotFoundError:
-        print(
-            f"No config file found, create one at {CONFIG_FILE} with a valid pyprland.plugins list"
-        )
-        raise SystemExit(1)
+    except PyprError as e:
+        raise SystemExit(1) from e
+    except Exception as e:
+        manager.log.critical("Failed to load config.", exc_info=True)
+        raise SystemExit(1) from e
 
     try:
         await manager.run()
     except KeyboardInterrupt:
         print("Interrupted")
     except asyncio.CancelledError:
-        print("Bye!")
+        manager.log.critical("cancelled")
     finally:
         events_writer.close()
         await events_writer.wait_closed()
         manager.server.close()
         await manager.server.wait_closed()
 
 
 async def run_client():
-    if sys.argv[1] in ("--help", "-h"):
-        manager = Pyprland()
+    "Runs the client (CLI)"
+    manager = Pyprland()
+    if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
         print(
             """Syntax: pypr [command]
 
 If command is ommited, runs the daemon which will start every configured command.
 
 Commands:
@@ -155,23 +203,43 @@
                     if callable(fn):
                         print(
                             f" {name[4:]:20} {fn.__doc__.strip() if fn.__doc__ else 'N/A'} (from {plug.name})"
                         )
 
         return
 
-    _, writer = await asyncio.open_unix_connection(CONTROL)
+    try:
+        _, writer = await asyncio.open_unix_connection(CONTROL)
+    except FileNotFoundError as e:
+        manager.log.critical("Failed to open control socket, is pypr daemon running ?")
+        raise PyprError() from e
+
     writer.write((" ".join(sys.argv[1:])).encode())
     await writer.drain()
     writer.close()
     await writer.wait_closed()
 
 
 def main():
+    "runs the command"
+    if "--debug" in sys.argv:
+        i = sys.argv.index("--debug")
+        init_logger(filename=sys.argv[i + 1], force_debug=True)
+        del sys.argv[i : i + 2]
+    else:
+        init_logger()
+    ipc_init()
+    log = get_logger("startup")
     try:
         asyncio.run(run_daemon() if len(sys.argv) <= 1 else run_client())
     except KeyboardInterrupt:
         pass
+    except PyprError:
+        log.critical("Command failed.")
+    except json.decoder.JSONDecodeError as e:
+        log.critical("Invalid JSON syntax in the config file: %s", e.args[0])
+    except Exception:  # pylint: disable=W0718
+        log.critical("Unhandled exception:", exc_info=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyprland-1.3.1/pyprland/ipc.py` & `pyprland-1.4.0/pyprland/ipc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,88 @@
 #!/bin/env python
+""" Interact with hyprland using sockets """
 import asyncio
+from logging import Logger
 from typing import Any
 import json
 import os
 
-from .common import DEBUG
+from .common import get_logger, PyprError
 
+log: Logger | None = None
 
 HYPRCTL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.socket.sock'
 EVENTS = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.socket2.sock'
 
 
 async def get_event_stream():
+    "Returns a new event socket connection"
     return await asyncio.open_unix_connection(EVENTS)
 
 
 async def hyprctlJSON(command) -> list[dict[str, Any]] | dict[str, Any]:
     """Run an IPC command and return the JSON output."""
-    if DEBUG:
-        print("(JS)>>>", command)
-    ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
+    assert log
+    log.debug(command)
+    try:
+        ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
+    except FileNotFoundError as e:
+        log.critical("hyprctl socket not found! is it running ?")
+        raise PyprError() from e
     ctl_writer.write(f"-j/{command}".encode())
     await ctl_writer.drain()
     resp = await ctl_reader.read()
     ctl_writer.close()
     await ctl_writer.wait_closed()
     ret = json.loads(resp)
     assert isinstance(ret, (list, dict))
     return ret
 
 
 def _format_command(command_list, default_base_command):
+    "helper function to format BATCH commands"
     for command in command_list:
         if isinstance(command, str):
             yield f"{default_base_command} {command}"
         else:
             yield f"{command[1]} {command[0]}"
 
 
 async def hyprctl(command, base_command="dispatch") -> bool:
     """Run an IPC command. Returns success value."""
-    if DEBUG:
-        print(">>>", command)
-    ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
+    assert log
+    log.debug(command)
+    try:
+        ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
+    except FileNotFoundError as e:
+        log.critical("hyprctl socket not found! is it running ?")
+        raise PyprError() from e
+
     if isinstance(command, list):
         ctl_writer.write(
             f"[[BATCH]] {' ; '.join(_format_command(command, base_command))}".encode()
         )
     else:
         ctl_writer.write(f"/{base_command} {command}".encode())
     await ctl_writer.drain()
     resp = await ctl_reader.read(100)
     ctl_writer.close()
     await ctl_writer.wait_closed()
-    if DEBUG:
-        print("<<<", resp)
     r: bool = resp == b"ok" * (len(resp) // 2)
-    if DEBUG and not r:
-        print(f"FAILED {resp}")
+    if not r:
+        log.error("FAILED %s", resp)
     return r
 
 
 async def get_focused_monitor_props() -> dict[str, Any]:
+    "Returns focused monitor data"
     for monitor in await hyprctlJSON("monitors"):
         assert isinstance(monitor, dict)
-        if monitor.get("focused") == True:
+        if monitor.get("focused"):
             return monitor
     raise RuntimeError("no focused monitor")
+
+
+def init():
+    "initialize logging"
+    global log
+    log = get_logger("ipc")
```

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/attract_lost_windows.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/attract_lost_windows.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/interface.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/interface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/interface.cpython-311.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/interface.cpython-311.pyc`

 * *Files 26% similar despite different names*

#### Python bytecode

```diff
@@ -1,221 +1,255 @@
 magic:    0xa70d0d0a
-moddate:  0xc0c14a64 (Thu Apr 27 18:41:04 2023 UTC)
-files sz: 350
+moddate:  0x838dc564 (Sat Jul 29 22:06:59 2023 UTC)
+files sz: 699
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c006d015a01010002004700640284006403a6020000ab
-      0200000000000000005a0264045300
+      0x970064005a00640164026c016d025a020100640364046c036d045a0401
+      0002004700640584006406a6020000ab0200000000000000005a05640753
+      00
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Any',))
-                 6 IMPORT_NAME              0 (typing)
-                 8 IMPORT_FROM              1 (Any)
-                10 STORE_NAME               1 (Any)
-                12 POP_TOP
+     1           2 LOAD_CONST               0 (' Common plugin interface ')
+                 4 STORE_NAME               0 (__doc__)
    
-     4          14 PUSH_NULL
-                16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object Plugin, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 4>)
-                20 MAKE_FUNCTION            0
-                22 LOAD_CONST               3 ('Plugin')
-                24 PRECALL                  2
-                28 CALL                     2
-                38 STORE_NAME               2 (Plugin)
-                40 LOAD_CONST               4 (None)
-                42 RETURN_VALUE
+     2           6 LOAD_CONST               1 (0)
+                 8 LOAD_CONST               2 (('Any',))
+                10 IMPORT_NAME              1 (typing)
+                12 IMPORT_FROM              2 (Any)
+                14 STORE_NAME               2 (Any)
+                16 POP_TOP
+   
+     3          18 LOAD_CONST               3 (2)
+                20 LOAD_CONST               4 (('get_logger',))
+                22 IMPORT_NAME              3 (common)
+                24 IMPORT_FROM              4 (get_logger)
+                26 STORE_NAME               4 (get_logger)
+                28 POP_TOP
+   
+     6          30 PUSH_NULL
+                32 LOAD_BUILD_CLASS
+                34 LOAD_CONST               5 (<code object Plugin, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 6>)
+                36 MAKE_FUNCTION            0
+                38 LOAD_CONST               6 ('Plugin')
+                40 PRECALL                  2
+                44 CALL                     2
+                54 STORE_NAME               5 (Plugin)
+                56 LOAD_CONST               7 (None)
+                58 RETURN_VALUE
    consts
+      ' Common plugin interface '
       0
       ('Any',)
+      2
+      ('get_logger',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
-            0x970065005a0164005a02640165036602640284045a04640384005a0564
-            0484005a0664056507650365086602190000000000000000006602640684
-            045a0964075300
-           4           0 RESUME                   0
+            0x970065005a0164005a0264015a03640265046602640384045a05640484
+            005a06640584005a07640665086504650966021900000000000000000066
+            02640784045a0a64085300
+           6           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Plugin')
                        8 STORE_NAME               2 (__qualname__)
          
-           5          10 LOAD_CONST               1 ('name')
-                      12 LOAD_NAME                3 (str)
-                      14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object __init__, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 5>)
-                      18 MAKE_FUNCTION            4 (annotations)
-                      20 STORE_NAME               4 (__init__)
+           7          10 LOAD_CONST               1 ('Base plugin class, handles logger and config')
+                      12 STORE_NAME               3 (__doc__)
          
-           8          22 LOAD_CONST               3 (<code object init, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 8>)
-                      24 MAKE_FUNCTION            0
-                      26 STORE_NAME               5 (init)
+           9          14 LOAD_CONST               2 ('name')
+                      16 LOAD_NAME                4 (str)
+                      18 BUILD_TUPLE              2
+                      20 LOAD_CONST               3 (<code object __init__, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 9>)
+                      22 MAKE_FUNCTION            4 (annotations)
+                      24 STORE_NAME               5 (__init__)
          
-          11          28 LOAD_CONST               4 (<code object exit, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 11>)
-                      30 MAKE_FUNCTION            0
-                      32 STORE_NAME               6 (exit)
+          15          26 LOAD_CONST               4 (<code object init, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 15>)
+                      28 MAKE_FUNCTION            0
+                      30 STORE_NAME               6 (init)
          
-          14          34 LOAD_CONST               5 ('config')
-                      36 LOAD_NAME                7 (dict)
-                      38 LOAD_NAME                3 (str)
-                      40 LOAD_NAME                8 (Any)
-                      42 BUILD_TUPLE              2
-                      44 BINARY_SUBSCR
-                      54 BUILD_TUPLE              2
-                      56 LOAD_CONST               6 (<code object load_config, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 14>)
-                      58 MAKE_FUNCTION            4 (annotations)
-                      60 STORE_NAME               9 (load_config)
-                      62 LOAD_CONST               7 (None)
-                      64 RETURN_VALUE
+          18          32 LOAD_CONST               5 (<code object exit, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 18>)
+                      34 MAKE_FUNCTION            0
+                      36 STORE_NAME               7 (exit)
+         
+          21          38 LOAD_CONST               6 ('config')
+                      40 LOAD_NAME                8 (dict)
+                      42 LOAD_NAME                4 (str)
+                      44 LOAD_NAME                9 (Any)
+                      46 BUILD_TUPLE              2
+                      48 BINARY_SUBSCR
+                      58 BUILD_TUPLE              2
+                      60 LOAD_CONST               7 (<code object load_config, file "/home/fab/dev/std/pyprland/pyprland/plugins/interface.py", line 21>)
+                      62 MAKE_FUNCTION            4 (annotations)
+                      64 STORE_NAME              10 (load_config)
+                      66 LOAD_CONST               8 (None)
+                      68 RETURN_VALUE
          consts
             'Plugin'
+            'Base plugin class, handles logger and config'
             'name'
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 2
+               stacksize : 3
                flags     : 3
-               code 0x97007c017c005f00000000000000000064005300
-                 5           0 RESUME                   0
+               code
+                  0x97007c017c005f0000000000000000007403000000000000000000007c
+                  01a6010000ab0100000000000000007c005f02000000000000000069007c
+                  005f03000000000000000064015300
+                 9           0 RESUME                   0
                
-                 6           2 LOAD_FAST                1 (name)
+                11           2 LOAD_FAST                1 (name)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (name)
-                            16 LOAD_CONST               0 (None)
-                            18 RETURN_VALUE
+               
+                12          16 LOAD_GLOBAL              3 (NULL + get_logger)
+                            28 LOAD_FAST                1 (name)
+                            30 PRECALL                  1
+                            34 CALL                     1
+                            44 LOAD_FAST                0 (self)
+                            46 STORE_ATTR               2 (log)
+               
+                13          56 BUILD_MAP                0
+                            58 LOAD_FAST                0 (self)
+                            60 STORE_ATTR               3 (config)
+                            70 LOAD_CONST               1 (None)
+                            72 RETURN_VALUE
                consts
+                  'create a new plugin `name` and the matching logger'
                   None
-               names      ('name',)
+               names      ('name', 'get_logger', 'log', 'config')
                varnames   ('self', 'name')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/interface.py'
                name       '__init__'
-               firstlineno 5
-               lnotab 0x0201
+               firstlineno 9
+               lnotab 0x02020e012801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 131
-               code 0x4b000100970064005300
-                 8           0 RETURN_GENERATOR
+               code 0x4b000100970064015300
+                15           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
-               
-                 9           6 LOAD_CONST               0 (None)
+                             6 LOAD_CONST               1 (None)
                              8 RETURN_VALUE
                consts
+                  'empty init function'
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/interface.py'
                name       'init'
-               firstlineno 8
-               lnotab 0x0601
+               firstlineno 15
+               lnotab 0x
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 131
-               code 0x4b000100970064005300
-                11           0 RETURN_GENERATOR
+               code 0x4b000100970064015300
+                18           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
-               
-                12           6 LOAD_CONST               0 (None)
+                             6 LOAD_CONST               1 (None)
                              8 RETURN_VALUE
                consts
+                  'empty exit function'
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/interface.py'
                name       'exit'
-               firstlineno 11
-               lnotab 0x0601
+               firstlineno 18
+               lnotab 0x
             'config'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 131
                code
                   0x4b000100970009007c017c006a00000000000000000019000000000000
-                  0000007c005f010000000000000000640053002300740400000000000000
-                  0000002400720b010069007c005f01000000000000000059006400530077
+                  0000007c005f010000000000000000640153002300740400000000000000
+                  0000002400720b010069007c005f01000000000000000059006401530077
                   00780359007701
-                14           0 RETURN_GENERATOR
+                21           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                15           6 NOP
+                23           6 NOP
                
-                16           8 LOAD_FAST                1 (config)
+                24           8 LOAD_FAST                1 (config)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (name)
                             22 BINARY_SUBSCR
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               1 (config)
-                            44 LOAD_CONST               0 (None)
+                            44 LOAD_CONST               1 (None)
                             46 RETURN_VALUE
                        >>   48 PUSH_EXC_INFO
                
-                17          50 LOAD_GLOBAL              4 (KeyError)
+                25          50 LOAD_GLOBAL              4 (KeyError)
                             62 CHECK_EXC_MATCH
                             64 POP_JUMP_FORWARD_IF_FALSE    11 (to 88)
                             66 POP_TOP
                
-                18          68 BUILD_MAP                0
+                26          68 BUILD_MAP                0
                             70 LOAD_FAST                0 (self)
                             72 STORE_ATTR               1 (config)
                             82 POP_EXCEPT
-                            84 LOAD_CONST               0 (None)
+                            84 LOAD_CONST               1 (None)
                             86 RETURN_VALUE
                
-                17     >>   88 RERAISE                  0
+                25     >>   88 RERAISE                  0
                        >>   90 COPY                     3
                             92 POP_EXCEPT
                             94 RERAISE                  1
                ExceptionTable:
                  8 to 42 -> 48 [0]
                  48 to 80 -> 90 [1] lasti
                  88 to 88 -> 90 [1] lasti
                consts
+                  'Loads the configuration section from the passed `config`'
                   None
                names      ('name', 'config', 'KeyError')
                varnames   ('self', 'config')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/interface.py'
                name       'load_config'
-               firstlineno 14
-               lnotab 0x060102012a01120114ff
+               firstlineno 21
+               lnotab 0x060202012a01120114ff
             None
-         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'init', 'exit', 'dict', 'Any', 'load_config')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', 'init', 'exit', 'dict', 'Any', 'load_config')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/interface.py'
          name       'Plugin'
-         firstlineno 4
-         lnotab 0x0a010c0306030603
+         firstlineno 6
+         lnotab 0x0a0104020c0606030603
       'Plugin'
       None
-   names      ('typing', 'Any', 'Plugin')
+   names      ('__doc__', 'typing', 'Any', 'common', 'get_logger', 'Plugin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/fab/dev/std/pyprland/pyprland/plugins/interface.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c03
+   lnotab 0x00ff020104010c010c03
```

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/lost_windows.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/lost_windows.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,53 +1,68 @@
 magic:    0xa70d0d0a
-moddate:  0xb2864d64 (Sat Apr 29 21:05:54 2023 UTC)
-files sz: 1454
+moddate:  0x0799c664 (Sun Jul 30 17:08:23 2023 UTC)
+files sz: 1710
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a010100640264036c026d035a036d045a0401
-      00640484005a05020047006405840064066501a6030000ab030000000000
-      0000005a0664075300
+      0x970064005a00640164026c016d025a026d035a030100640364046c046d
+      055a050100640564066c066d075a076d085a080100640784005a09020047
+      006408840064096505a6030000ab0300000000000000005a0a640a5300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (1)
-                 4 LOAD_CONST               1 (('Plugin',))
-                 6 IMPORT_NAME              0 (interface)
-                 8 IMPORT_FROM              1 (Plugin)
-                10 STORE_NAME               1 (Plugin)
-                12 POP_TOP
+     1           2 LOAD_CONST               0 (' Moves unreachable client windows to the currently focused workspace')
+                 4 STORE_NAME               0 (__doc__)
    
-     3          14 LOAD_CONST               2 (2)
-                16 LOAD_CONST               3 (('hyprctlJSON', 'hyprctl'))
-                18 IMPORT_NAME              2 (ipc)
-                20 IMPORT_FROM              3 (hyprctlJSON)
-                22 STORE_NAME               3 (hyprctlJSON)
-                24 IMPORT_FROM              4 (hyprctl)
-                26 STORE_NAME               4 (hyprctl)
-                28 POP_TOP
+     2           6 LOAD_CONST               1 (0)
+                 8 LOAD_CONST               2 (('Any', 'cast'))
+                10 IMPORT_NAME              1 (typing)
+                12 IMPORT_FROM              2 (Any)
+                14 STORE_NAME               2 (Any)
+                16 IMPORT_FROM              3 (cast)
+                18 STORE_NAME               3 (cast)
+                20 POP_TOP
    
-     6          30 LOAD_CONST               4 (<code object contains, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 6>)
-                32 MAKE_FUNCTION            0
-                34 STORE_NAME               5 (contains)
+     3          22 LOAD_CONST               3 (1)
+                24 LOAD_CONST               4 (('Plugin',))
+                26 IMPORT_NAME              4 (interface)
+                28 IMPORT_FROM              5 (Plugin)
+                30 STORE_NAME               5 (Plugin)
+                32 POP_TOP
    
-    20          36 PUSH_NULL
-                38 LOAD_BUILD_CLASS
-                40 LOAD_CONST               5 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 20>)
-                42 MAKE_FUNCTION            0
-                44 LOAD_CONST               6 ('Extension')
-                46 LOAD_NAME                1 (Plugin)
-                48 PRECALL                  3
-                52 CALL                     3
-                62 STORE_NAME               6 (Extension)
-                64 LOAD_CONST               7 (None)
-                66 RETURN_VALUE
+     5          34 LOAD_CONST               5 (2)
+                36 LOAD_CONST               6 (('hyprctlJSON', 'hyprctl'))
+                38 IMPORT_NAME              6 (ipc)
+                40 IMPORT_FROM              7 (hyprctlJSON)
+                42 STORE_NAME               7 (hyprctlJSON)
+                44 IMPORT_FROM              8 (hyprctl)
+                46 STORE_NAME               8 (hyprctl)
+                48 POP_TOP
+   
+     8          50 LOAD_CONST               7 (<code object contains, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 8>)
+                52 MAKE_FUNCTION            0
+                54 STORE_NAME               9 (contains)
+   
+    23          56 PUSH_NULL
+                58 LOAD_BUILD_CLASS
+                60 LOAD_CONST               8 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 23>)
+                62 MAKE_FUNCTION            0
+                64 LOAD_CONST               9 ('Extension')
+                66 LOAD_NAME                5 (Plugin)
+                68 PRECALL                  3
+                72 CALL                     3
+                82 STORE_NAME              10 (Extension)
+                84 LOAD_CONST              10 (None)
+                86 RETURN_VALUE
    consts
+      ' Moves unreachable client windows to the currently focused workspace'
+      0
+      ('Any', 'cast')
       1
       ('Plugin',)
       2
       ('hyprctlJSON', 'hyprctl')
       code
          argcount  : 2
          nlocals   : 2
@@ -59,78 +74,78 @@
             00000000006402190000000000000000007c006403190000000000000000
             007c006404190000000000000000007a0000006b00000000007302640553
             007c016401190000000000000000006406190000000000000000007c0064
             07190000000000000000006b040000000072217c01640119000000000000
             0000006406190000000000000000007c006407190000000000000000007c
             006408190000000000000000007a0000006b000000000073026405530064
             095300
-           6           0 RESUME                   0
+           8           0 RESUME                   0
          
-           8           2 LOAD_FAST                1 (window)
+          11           2 LOAD_FAST                1 (window)
                        4 LOAD_CONST               1 ('at')
                        6 BINARY_SUBSCR
                       16 LOAD_CONST               2 (0)
                       18 BINARY_SUBSCR
                       28 LOAD_FAST                0 (monitor)
                       30 LOAD_CONST               3 ('x')
                       32 BINARY_SUBSCR
                       42 COMPARE_OP               4 (>)
                       48 POP_JUMP_FORWARD_IF_FALSE    33 (to 116)
          
-           9          50 LOAD_FAST                1 (window)
+          12          50 LOAD_FAST                1 (window)
                       52 LOAD_CONST               1 ('at')
                       54 BINARY_SUBSCR
                       64 LOAD_CONST               2 (0)
                       66 BINARY_SUBSCR
                       76 LOAD_FAST                0 (monitor)
                       78 LOAD_CONST               3 ('x')
                       80 BINARY_SUBSCR
                       90 LOAD_FAST                0 (monitor)
                       92 LOAD_CONST               4 ('width')
                       94 BINARY_SUBSCR
                      104 BINARY_OP                0 (+)
                      108 COMPARE_OP               0 (<)
                      114 POP_JUMP_FORWARD_IF_TRUE     2 (to 120)
          
-          11     >>  116 LOAD_CONST               5 (False)
+          14     >>  116 LOAD_CONST               5 (False)
                      118 RETURN_VALUE
          
-          13     >>  120 LOAD_FAST                1 (window)
+          16     >>  120 LOAD_FAST                1 (window)
                      122 LOAD_CONST               1 ('at')
                      124 BINARY_SUBSCR
                      134 LOAD_CONST               6 (1)
                      136 BINARY_SUBSCR
                      146 LOAD_FAST                0 (monitor)
                      148 LOAD_CONST               7 ('y')
                      150 BINARY_SUBSCR
                      160 COMPARE_OP               4 (>)
                      166 POP_JUMP_FORWARD_IF_FALSE    33 (to 234)
          
-          14         168 LOAD_FAST                1 (window)
+          17         168 LOAD_FAST                1 (window)
                      170 LOAD_CONST               1 ('at')
                      172 BINARY_SUBSCR
                      182 LOAD_CONST               6 (1)
                      184 BINARY_SUBSCR
                      194 LOAD_FAST                0 (monitor)
                      196 LOAD_CONST               7 ('y')
                      198 BINARY_SUBSCR
                      208 LOAD_FAST                0 (monitor)
                      210 LOAD_CONST               8 ('height')
                      212 BINARY_SUBSCR
                      222 BINARY_OP                0 (+)
                      226 COMPARE_OP               0 (<)
                      232 POP_JUMP_FORWARD_IF_TRUE     2 (to 238)
          
-          16     >>  234 LOAD_CONST               5 (False)
+          19     >>  234 LOAD_CONST               5 (False)
                      236 RETURN_VALUE
          
-          17     >>  238 LOAD_CONST               9 (True)
+          20     >>  238 LOAD_CONST               9 (True)
                      240 RETURN_VALUE
          consts
-            None
+            'Tell if a window is visible in a monitor'
             'at'
             0
             'x'
             'width'
             False
             1
             'y'
@@ -138,240 +153,256 @@
             True
          names      ()
          varnames   ('monitor', 'window')
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py'
          name       'contains'
-         firstlineno 6
-         lnotab 0x0202300142020402300142020401
+         firstlineno 8
+         lnotab 0x0203300142020402300142020401
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          20           0 RESUME                   0
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Extension')
                        8 STORE_NAME               2 (__qualname__)
          
-          21          10 LOAD_CONST               1 (<code object run_attract_lost, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 21>)
+          24          10 LOAD_CONST               1 (<code object run_attract_lost, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 24>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (run_attract_lost)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'Extension'
             code
                argcount  : 1
-               nlocals   : 13
-               stacksize : 11
-               flags     : 135
+               nlocals   : 14
+               stacksize : 10
+               flags     : 131
                code
-                  0x870d4b00010097007401000000000000000000006401a6010000ab0100
-                  00000000000000830064027b035600970386048a0d740100000000000000
-                  0000006403a6010000ab010000000000000000830064027b035600970386
-                  047d02880d6601640484087c024400a6000000ab0000000000000000007d
-                  0364058400890d4400a6000000ab00000000000000000064061900000000
-                  00000000007d047c04640719000000000000000000640874030000000000
-                  00000000007c03a6010000ab0100000000000000007a0000007a0b00007d
-                  057c0464091900000000000000000064087403000000000000000000007c
-                  03a6010000ab0100000000000000007a0000007a0b00007d0667007d077c
-                  04640a19000000000000000000640b190000000000000000007d087c0564
-                  0c7a0200007d097c06640c7a0200007d0a7405000000000000000000007c
-                  03a6010000ab01000000000000000044005d825c0200007d0b7d0c7c07a0
-                  030000000000000000000000000000000000000000640d7c089b00640e7c
-                  0c640f190000000000000000009b009d04a6010000ab0100000000000000
-                  0001007c07a0030000000000000000000000000000000000000000641074
-                  09000000000000000000007c097c046411190000000000000000007a0000
-                  007c0b7c057a0500007a000000a6010000ab0100000000000000009b0064
-                  127409000000000000000000007c0a7c046413190000000000000000007a
-                  0000007c0b7c067a0500007a000000a6010000ab0100000000000000009b
-                  00640e7c0c640f190000000000000000009b009d06a6010000ab01000000
-                  000000000001008c83740b000000000000000000007c07a6010000ab0100
-                  00000000000000830064027b03560097038604010064025300
-                             0 MAKE_CELL               13 (monitors)
+                  0x870e4b0001009700740100000000000000000000740200000000000000
+                  0000007405000000000000000000006401a6010000ab0100000000000000
+                  00830064027b03560097038604a6020000ab0200000000000000008a0e74
+                  010000000000000000000074020000000000000000000074050000000000
+                  00000000006403a6010000ab010000000000000000830064027b03560097
+                  038604a6020000ab0200000000000000007d01880e6601640484087c0144
+                  00a6000000ab0000000000000000007d0264058400890e4400a6000000ab
+                  0000000000000000006406190000000000000000007d037c036407190000
+                  0000000000000064087407000000000000000000007c02a6010000ab0100
+                  000000000000007a0000007a0b00007d047c036409190000000000000000
+                  0064087407000000000000000000007c02a6010000ab0100000000000000
+                  007a0000007a0b00007d0567007d067c03640a1900000000000000000064
+                  0b190000000000000000007d077c04640c7a0200007d087c05640c7a0200
+                  007d097409000000000000000000007c02a6010000ab0100000000000000
+                  0044005d875c0200007d0a7d0b740b000000000000000000007c087c0364
+                  0d190000000000000000007a0000007c0a7c047a0500007a000000a60100
+                  00ab0100000000000000007d0c740b000000000000000000007c097c0364
+                  0e190000000000000000007a0000007c0a7c057a0500007a000000a60100
+                  00ab01000000000000000068017d0d7c06a0060000000000000000000000
+                  000000000000000000640f7c079b0064107c0b6411190000000000000000
+                  009b009d04a6010000ab01000000000000000001007c06a0060000000000
+                  00000000000000000000000000000064127c0c9b0064137c0d9b0064107c
+                  0b6411190000000000000000009b009d06a6010000ab0100000000000000
+                  0001008c88740f000000000000000000007c06a6010000ab010000000000
+                  000000830064027b03560097038604010064025300
+                             0 MAKE_CELL               14 (monitors)
                
-                21           2 RETURN_GENERATOR
+                24           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                23           8 LOAD_GLOBAL              1 (NULL + hyprctlJSON)
-                            20 LOAD_CONST               1 ('monitors')
-                            22 PRECALL                  1
-                            26 CALL                     1
-                            36 GET_AWAITABLE            0
-                            38 LOAD_CONST               2 (None)
-                       >>   40 SEND                     3 (to 48)
-                            42 YIELD_VALUE
-                            44 RESUME                   3
-                            46 JUMP_BACKWARD_NO_INTERRUPT     4 (to 40)
-                       >>   48 STORE_DEREF             13 (monitors)
-               
-                24          50 LOAD_GLOBAL              1 (NULL + hyprctlJSON)
-                            62 LOAD_CONST               3 ('clients')
-                            64 PRECALL                  1
-                            68 CALL                     1
-                            78 GET_AWAITABLE            0
-                            80 LOAD_CONST               2 (None)
-                       >>   82 SEND                     3 (to 90)
-                            84 YIELD_VALUE
-                            86 RESUME                   3
-                            88 JUMP_BACKWARD_NO_INTERRUPT     4 (to 82)
-                       >>   90 STORE_FAST               2 (windows)
-               
-                25          92 LOAD_CLOSURE            13 (monitors)
-                            94 BUILD_TUPLE              1
-                            96 LOAD_CONST               4 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 25>)
-                            98 MAKE_FUNCTION            8 (closure)
-               
-                27         100 LOAD_FAST                2 (windows)
-               
-                25         102 GET_ITER
-                           104 PRECALL                  0
-                           108 CALL                     0
-                           118 STORE_FAST               3 (lost)
-               
-                30         120 LOAD_CONST               5 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 30>)
-                           122 MAKE_FUNCTION            0
-                           124 LOAD_DEREF              13 (monitors)
-                           126 GET_ITER
-                           128 PRECALL                  0
-                           132 CALL                     0
-                           142 LOAD_CONST               6 (0)
-                           144 BINARY_SUBSCR
-                           154 STORE_FAST               4 (focused)
-               
-                31         156 LOAD_FAST                4 (focused)
-                           158 LOAD_CONST               7 ('width')
-                           160 BINARY_SUBSCR
-                           170 LOAD_CONST               8 (1)
-                           172 LOAD_GLOBAL              3 (NULL + len)
-                           184 LOAD_FAST                3 (lost)
-                           186 PRECALL                  1
-                           190 CALL                     1
-                           200 BINARY_OP                0 (+)
-                           204 BINARY_OP               11 (/)
-                           208 STORE_FAST               5 (interval)
-               
-                32         210 LOAD_FAST                4 (focused)
-                           212 LOAD_CONST               9 ('height')
-                           214 BINARY_SUBSCR
-                           224 LOAD_CONST               8 (1)
-                           226 LOAD_GLOBAL              3 (NULL + len)
-                           238 LOAD_FAST                3 (lost)
-                           240 PRECALL                  1
-                           244 CALL                     1
-                           254 BINARY_OP                0 (+)
-                           258 BINARY_OP               11 (/)
-                           262 STORE_FAST               6 (intervalY)
-               
-                33         264 BUILD_LIST               0
-                           266 STORE_FAST               7 (batch)
-               
-                34         268 LOAD_FAST                4 (focused)
-                           270 LOAD_CONST              10 ('activeWorkspace')
-                           272 BINARY_SUBSCR
-                           282 LOAD_CONST              11 ('id')
-                           284 BINARY_SUBSCR
-                           294 STORE_FAST               8 (workspace)
-               
-                35         296 LOAD_FAST                5 (interval)
-                           298 LOAD_CONST              12 (2)
-                           300 BINARY_OP                2 (//)
-                           304 STORE_FAST               9 (margin)
-               
-                36         306 LOAD_FAST                6 (intervalY)
-                           308 LOAD_CONST              12 (2)
-                           310 BINARY_OP                2 (//)
-                           314 STORE_FAST              10 (marginY)
-               
-                37         316 LOAD_GLOBAL              5 (NULL + enumerate)
-                           328 LOAD_FAST                3 (lost)
-                           330 PRECALL                  1
-                           334 CALL                     1
-                           344 GET_ITER
-                       >>  346 FOR_ITER               130 (to 608)
-                           348 UNPACK_SEQUENCE          2
-                           352 STORE_FAST              11 (i)
-                           354 STORE_FAST              12 (window)
-               
-                38         356 LOAD_FAST                7 (batch)
-                           358 LOAD_METHOD              3 (append)
-                           380 LOAD_CONST              13 ('movetoworkspacesilent ')
-                           382 LOAD_FAST                8 (workspace)
-                           384 FORMAT_VALUE             0
-                           386 LOAD_CONST              14 (',pid:')
-                           388 LOAD_FAST               12 (window)
-                           390 LOAD_CONST              15 ('pid')
-                           392 BINARY_SUBSCR
-                           402 FORMAT_VALUE             0
-                           404 BUILD_STRING             4
+                26           8 LOAD_GLOBAL              1 (NULL + cast)
+                            20 LOAD_GLOBAL              2 (list)
+                            32 LOAD_GLOBAL              5 (NULL + hyprctlJSON)
+                            44 LOAD_CONST               1 ('monitors')
+                            46 PRECALL                  1
+                            50 CALL                     1
+                            60 GET_AWAITABLE            0
+                            62 LOAD_CONST               2 (None)
+                       >>   64 SEND                     3 (to 72)
+                            66 YIELD_VALUE
+                            68 RESUME                   3
+                            70 JUMP_BACKWARD_NO_INTERRUPT     4 (to 64)
+                       >>   72 PRECALL                  2
+                            76 CALL                     2
+                            86 STORE_DEREF             14 (monitors)
+               
+                27          88 LOAD_GLOBAL              1 (NULL + cast)
+                           100 LOAD_GLOBAL              2 (list)
+                           112 LOAD_GLOBAL              5 (NULL + hyprctlJSON)
+                           124 LOAD_CONST               3 ('clients')
+                           126 PRECALL                  1
+                           130 CALL                     1
+                           140 GET_AWAITABLE            0
+                           142 LOAD_CONST               2 (None)
+                       >>  144 SEND                     3 (to 152)
+                           146 YIELD_VALUE
+                           148 RESUME                   3
+                           150 JUMP_BACKWARD_NO_INTERRUPT     4 (to 144)
+                       >>  152 PRECALL                  2
+                           156 CALL                     2
+                           166 STORE_FAST               1 (windows)
+               
+                28         168 LOAD_CLOSURE            14 (monitors)
+                           170 BUILD_TUPLE              1
+                           172 LOAD_CONST               4 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 28>)
+                           174 MAKE_FUNCTION            8 (closure)
+               
+                30         176 LOAD_FAST                1 (windows)
+               
+                28         178 GET_ITER
+                           180 PRECALL                  0
+                           184 CALL                     0
+                           194 STORE_FAST               2 (lost)
+               
+                33         196 LOAD_CONST               5 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 33>)
+                           198 MAKE_FUNCTION            0
+                           200 LOAD_DEREF              14 (monitors)
+                           202 GET_ITER
+                           204 PRECALL                  0
+                           208 CALL                     0
+                           218 LOAD_CONST               6 (0)
+                           220 BINARY_SUBSCR
+                           230 STORE_FAST               3 (focused)
+               
+                34         232 LOAD_FAST                3 (focused)
+                           234 LOAD_CONST               7 ('width')
+                           236 BINARY_SUBSCR
+                           246 LOAD_CONST               8 (1)
+                           248 LOAD_GLOBAL              7 (NULL + len)
+                           260 LOAD_FAST                2 (lost)
+                           262 PRECALL                  1
+                           266 CALL                     1
+                           276 BINARY_OP                0 (+)
+                           280 BINARY_OP               11 (/)
+                           284 STORE_FAST               4 (interval)
+               
+                35         286 LOAD_FAST                3 (focused)
+                           288 LOAD_CONST               9 ('height')
+                           290 BINARY_SUBSCR
+                           300 LOAD_CONST               8 (1)
+                           302 LOAD_GLOBAL              7 (NULL + len)
+                           314 LOAD_FAST                2 (lost)
+                           316 PRECALL                  1
+                           320 CALL                     1
+                           330 BINARY_OP                0 (+)
+                           334 BINARY_OP               11 (/)
+                           338 STORE_FAST               5 (interval_y)
+               
+                36         340 BUILD_LIST               0
+                           342 STORE_FAST               6 (batch)
+               
+                37         344 LOAD_FAST                3 (focused)
+                           346 LOAD_CONST              10 ('activeWorkspace')
+                           348 BINARY_SUBSCR
+                           358 LOAD_CONST              11 ('id')
+                           360 BINARY_SUBSCR
+                           370 STORE_FAST               7 (workspace)
+               
+                38         372 LOAD_FAST                4 (interval)
+                           374 LOAD_CONST              12 (2)
+                           376 BINARY_OP                2 (//)
+                           380 STORE_FAST               8 (margin)
+               
+                39         382 LOAD_FAST                5 (interval_y)
+                           384 LOAD_CONST              12 (2)
+                           386 BINARY_OP                2 (//)
+                           390 STORE_FAST               9 (margin_y)
+               
+                40         392 LOAD_GLOBAL              9 (NULL + enumerate)
+                           404 LOAD_FAST                2 (lost)
                            406 PRECALL                  1
                            410 CALL                     1
-                           420 POP_TOP
-               
-                39         422 LOAD_FAST                7 (batch)
-                           424 LOAD_METHOD              3 (append)
-               
-                40         446 LOAD_CONST              16 ('movewindowpixel exact ')
-                           448 LOAD_GLOBAL              9 (NULL + int)
-                           460 LOAD_FAST                9 (margin)
-                           462 LOAD_FAST                4 (focused)
-                           464 LOAD_CONST              17 ('x')
-                           466 BINARY_SUBSCR
-                           476 BINARY_OP                0 (+)
-                           480 LOAD_FAST               11 (i)
-                           482 LOAD_FAST                5 (interval)
-                           484 BINARY_OP                5 (*)
-                           488 BINARY_OP                0 (+)
-                           492 PRECALL                  1
-                           496 CALL                     1
-                           506 FORMAT_VALUE             0
-                           508 LOAD_CONST              18 (' ')
-                           510 LOAD_GLOBAL              9 (NULL + int)
-                           522 LOAD_FAST               10 (marginY)
-                           524 LOAD_FAST                4 (focused)
-                           526 LOAD_CONST              19 ('y')
-                           528 BINARY_SUBSCR
-                           538 BINARY_OP                0 (+)
-                           542 LOAD_FAST               11 (i)
-                           544 LOAD_FAST                6 (intervalY)
-                           546 BINARY_OP                5 (*)
-                           550 BINARY_OP                0 (+)
-                           554 PRECALL                  1
-                           558 CALL                     1
-                           568 FORMAT_VALUE             0
-                           570 LOAD_CONST              14 (',pid:')
-                           572 LOAD_FAST               12 (window)
-                           574 LOAD_CONST              15 ('pid')
-                           576 BINARY_SUBSCR
-                           586 FORMAT_VALUE             0
-                           588 BUILD_STRING             6
-               
-                39         590 PRECALL                  1
-                           594 CALL                     1
-                           604 POP_TOP
-                           606 JUMP_BACKWARD          131 (to 346)
-               
-                42     >>  608 LOAD_GLOBAL             11 (NULL + hyprctl)
-                           620 LOAD_FAST                7 (batch)
-                           622 PRECALL                  1
-                           626 CALL                     1
-                           636 GET_AWAITABLE            0
-                           638 LOAD_CONST               2 (None)
-                       >>  640 SEND                     3 (to 648)
-                           642 YIELD_VALUE
-                           644 RESUME                   3
-                           646 JUMP_BACKWARD_NO_INTERRUPT     4 (to 640)
-                       >>  648 POP_TOP
-                           650 LOAD_CONST               2 (None)
-                           652 RETURN_VALUE
+                           420 GET_ITER
+                       >>  422 FOR_ITER               135 (to 694)
+                           424 UNPACK_SEQUENCE          2
+                           428 STORE_FAST              10 (i)
+                           430 STORE_FAST              11 (window)
+               
+                41         432 LOAD_GLOBAL             11 (NULL + int)
+                           444 LOAD_FAST                8 (margin)
+                           446 LOAD_FAST                3 (focused)
+                           448 LOAD_CONST              13 ('x')
+                           450 BINARY_SUBSCR
+                           460 BINARY_OP                0 (+)
+                           464 LOAD_FAST               10 (i)
+                           466 LOAD_FAST                4 (interval)
+                           468 BINARY_OP                5 (*)
+                           472 BINARY_OP                0 (+)
+                           476 PRECALL                  1
+                           480 CALL                     1
+                           490 STORE_FAST              12 (pos_x)
+               
+                42         492 LOAD_GLOBAL             11 (NULL + int)
+                           504 LOAD_FAST                9 (margin_y)
+                           506 LOAD_FAST                3 (focused)
+                           508 LOAD_CONST              14 ('y')
+                           510 BINARY_SUBSCR
+                           520 BINARY_OP                0 (+)
+                           524 LOAD_FAST               10 (i)
+                           526 LOAD_FAST                5 (interval_y)
+                           528 BINARY_OP                5 (*)
+                           532 BINARY_OP                0 (+)
+                           536 PRECALL                  1
+                           540 CALL                     1
+                           550 BUILD_SET                1
+                           552 STORE_FAST              13 (pos_y)
+               
+                43         554 LOAD_FAST                6 (batch)
+                           556 LOAD_METHOD              6 (append)
+                           578 LOAD_CONST              15 ('movetoworkspacesilent ')
+                           580 LOAD_FAST                7 (workspace)
+                           582 FORMAT_VALUE             0
+                           584 LOAD_CONST              16 (',pid:')
+                           586 LOAD_FAST               11 (window)
+                           588 LOAD_CONST              17 ('pid')
+                           590 BINARY_SUBSCR
+                           600 FORMAT_VALUE             0
+                           602 BUILD_STRING             4
+                           604 PRECALL                  1
+                           608 CALL                     1
+                           618 POP_TOP
+               
+                44         620 LOAD_FAST                6 (batch)
+                           622 LOAD_METHOD              6 (append)
+                           644 LOAD_CONST              18 ('movewindowpixel exact ')
+                           646 LOAD_FAST               12 (pos_x)
+                           648 FORMAT_VALUE             0
+                           650 LOAD_CONST              19 (' ')
+                           652 LOAD_FAST               13 (pos_y)
+                           654 FORMAT_VALUE             0
+                           656 LOAD_CONST              16 (',pid:')
+                           658 LOAD_FAST               11 (window)
+                           660 LOAD_CONST              17 ('pid')
+                           662 BINARY_SUBSCR
+                           672 FORMAT_VALUE             0
+                           674 BUILD_STRING             6
+                           676 PRECALL                  1
+                           680 CALL                     1
+                           690 POP_TOP
+                           692 JUMP_BACKWARD          136 (to 422)
+               
+                45     >>  694 LOAD_GLOBAL             15 (NULL + hyprctl)
+                           706 LOAD_FAST                6 (batch)
+                           708 PRECALL                  1
+                           712 CALL                     1
+                           722 GET_AWAITABLE            0
+                           724 LOAD_CONST               2 (None)
+                       >>  726 SEND                     3 (to 734)
+                           728 YIELD_VALUE
+                           730 RESUME                   3
+                           732 JUMP_BACKWARD_NO_INTERRUPT     4 (to 726)
+                       >>  734 POP_TOP
+                           736 LOAD_CONST               2 (None)
+                           738 RETURN_VALUE
                consts
                   'Brings lost floating windows to the current workspace'
                   'monitors'
                   None
                   'clients'
                   code
                      argcount  : 1
@@ -382,59 +413,59 @@
                         0x95018701970067007c005d278a018901640019000000000000000000af
                         0a740100000000000000000000880166016401840889024400a6000000ab
                         000000000000000000a6010000ab010000000000000000b025890191028c
                         285300
                                    0 COPY_FREE_VARS           1
                                    2 MAKE_CELL                1 (win)
                      
-                      25           4 RESUME                   0
+                      28           4 RESUME                   0
                                    6 BUILD_LIST               0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                39 (to 90)
                      
-                      27          12 STORE_DEREF              1 (win)
+                      30          12 STORE_DEREF              1 (win)
                      
-                      28          14 LOAD_DEREF               1 (win)
+                      31          14 LOAD_DEREF               1 (win)
                                   16 LOAD_CONST               0 ('floating')
                                   18 BINARY_SUBSCR
                      
-                      25          28 POP_JUMP_BACKWARD_IF_FALSE    10 (to 10)
+                      28          28 POP_JUMP_BACKWARD_IF_FALSE    10 (to 10)
                      
-                      28          30 LOAD_GLOBAL              1 (NULL + any)
+                      31          30 LOAD_GLOBAL              1 (NULL + any)
                                   42 LOAD_CLOSURE             1 (win)
                                   44 BUILD_TUPLE              1
-                                  46 LOAD_CONST               1 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 28>)
+                                  46 LOAD_CONST               1 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py", line 31>)
                                   48 MAKE_FUNCTION            8 (closure)
                                   50 LOAD_DEREF               2 (monitors)
                                   52 GET_ITER
                                   54 PRECALL                  0
                                   58 CALL                     0
                                   68 PRECALL                  1
                                   72 CALL                     1
                      
-                      25          82 POP_JUMP_BACKWARD_IF_TRUE    37 (to 10)
+                      28          82 POP_JUMP_BACKWARD_IF_TRUE    37 (to 10)
                      
-                      26          84 LOAD_DEREF               1 (win)
+                      29          84 LOAD_DEREF               1 (win)
                      
-                      25          86 LIST_APPEND              2
+                      28          86 LIST_APPEND              2
                                   88 JUMP_BACKWARD           40 (to 10)
                              >>   90 RETURN_VALUE
                      consts
                         'floating'
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 5
                            flags     : 51
                            code
                               0x95014b00010097007c005d147d017401000000000000000000007c0189
                               02a6020000ab0200000000000000005600970101008c1564005300
                                          0 COPY_FREE_VARS           1
                            
-                            28           2 RETURN_GENERATOR
+                            31           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                20 (to 52)
                                         12 STORE_FAST               1 (mon)
                                         14 LOAD_GLOBAL              1 (NULL + contains)
                                         26 LOAD_FAST                1 (mon)
@@ -451,33 +482,33 @@
                               None
                            names      ('contains',)
                            varnames   ('.0', 'mon')
                            freevars   ('win',)
                            cellvars   ()
                            filename   '/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py'
                            name       '<genexpr>'
-                           firstlineno 28
+                           firstlineno 31
                            lnotab 0x
                      names      ('any',)
                      varnames   ('.0',)
                      freevars   ('monitors',)
                      cellvars   ('win',)
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py'
                      name       '<listcomp>'
-                     firstlineno 25
+                     firstlineno 28
                      lnotab 0x0c0202010efd020334fd020102ff
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0c7d017c01640019000000000000000000af0a7c0191
                         028c0d5300
-                      30           0 RESUME                   0
+                      33           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                12 (to 32)
                                    8 STORE_FAST               1 (mon)
                                   10 LOAD_FAST                1 (mon)
                                   12 LOAD_CONST               0 ('focused')
                                   14 BINARY_SUBSCR
@@ -490,52 +521,52 @@
                         'focused'
                      names      ()
                      varnames   ('.0', 'mon')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py'
                      name       '<listcomp>'
-                     firstlineno 30
+                     firstlineno 33
                      lnotab 0x
                   0
                   'width'
                   1
                   'height'
                   'activeWorkspace'
                   'id'
                   2
+                  'x'
+                  'y'
                   'movetoworkspacesilent '
                   ',pid:'
                   'pid'
                   'movewindowpixel exact '
-                  'x'
                   ' '
-                  'y'
-               names      ('hyprctlJSON', 'len', 'enumerate', 'append', 'int', 'hyprctl')
-               varnames   ('self', 'args', 'windows', 'lost', 'focused', 'interval', 'intervalY', 'batch', 'workspace', 'margin', 'marginY', 'i', 'window')
+               names      ('cast', 'list', 'hyprctlJSON', 'len', 'enumerate', 'int', 'append', 'hyprctl')
+               varnames   ('self', 'windows', 'lost', 'focused', 'interval', 'interval_y', 'batch', 'workspace', 'margin', 'margin_y', 'i', 'window', 'pos_x', 'pos_y')
                freevars   ()
                cellvars   ('monitors',)
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py'
                name       'run_attract_lost'
-               firstlineno 21
+               firstlineno 24
                lnotab
-                  0x08022a012a01080202fe120524013601360104011c010a010a01280142
-                  01180190ff1203
+                  0x080250015001080202fe120524013601360104011c010a010a0128013c
+                  013e0142014a01
             None
          names      ('__name__', '__module__', '__qualname__', 'run_attract_lost')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py'
          name       'Extension'
-         firstlineno 20
+         firstlineno 23
          lnotab 0x0a01
       'Extension'
       None
-   names      ('interface', 'Plugin', 'ipc', 'hyprctlJSON', 'hyprctl', 'contains', 'Extension')
+   names      ('__doc__', 'typing', 'Any', 'cast', 'interface', 'Plugin', 'ipc', 'hyprctlJSON', 'hyprctl', 'contains', 'Extension')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/fab/dev/std/pyprland/pyprland/plugins/lost_windows.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c021003060e
+   lnotab 0x00ff0201040110010c021003060f
```

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/magnify.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/magnify.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/magnify.cpython-311.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/magnify.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,102 +1,78 @@
 magic:    0xa70d0d0a
-moddate:  0xb2864d64 (Sat Apr 29 21:05:54 2023 UTC)
-files sz: 735
+moddate:  0xc646c664 (Sun Jul 30 11:17:26 2023 UTC)
+files sz: 760
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a010100640264036c026d035a036d045a0401
-      00020047006404840064056501a6030000ab0300000000000000005a0564
-      065300
+      0x970064005a00640164026c016d025a020100640364046c036d045a0401
+      00020047006405840064066502a6030000ab0300000000000000005a0564
+      075300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (1)
-                 4 LOAD_CONST               1 (('Plugin',))
-                 6 IMPORT_NAME              0 (interface)
-                 8 IMPORT_FROM              1 (Plugin)
-                10 STORE_NAME               1 (Plugin)
-                12 POP_TOP
+     1           2 LOAD_CONST               0 (' Toggles workspace zooming ')
+                 4 STORE_NAME               0 (__doc__)
    
-     3          14 LOAD_CONST               2 (2)
-                16 LOAD_CONST               3 (('hyprctlJSON', 'hyprctl'))
-                18 IMPORT_NAME              2 (ipc)
-                20 IMPORT_FROM              3 (hyprctlJSON)
-                22 STORE_NAME               3 (hyprctlJSON)
+     2           6 LOAD_CONST               1 (1)
+                 8 LOAD_CONST               2 (('Plugin',))
+                10 IMPORT_NAME              1 (interface)
+                12 IMPORT_FROM              2 (Plugin)
+                14 STORE_NAME               2 (Plugin)
+                16 POP_TOP
+   
+     4          18 LOAD_CONST               3 (2)
+                20 LOAD_CONST               4 (('hyprctl',))
+                22 IMPORT_NAME              3 (ipc)
                 24 IMPORT_FROM              4 (hyprctl)
                 26 STORE_NAME               4 (hyprctl)
                 28 POP_TOP
    
-     6          30 PUSH_NULL
+     7          30 PUSH_NULL
                 32 LOAD_BUILD_CLASS
-                34 LOAD_CONST               4 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py", line 6>)
+                34 LOAD_CONST               5 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py", line 7>)
                 36 MAKE_FUNCTION            0
-                38 LOAD_CONST               5 ('Extension')
-                40 LOAD_NAME                1 (Plugin)
+                38 LOAD_CONST               6 ('Extension')
+                40 LOAD_NAME                2 (Plugin)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (Extension)
-                58 LOAD_CONST               6 (None)
+                58 LOAD_CONST               7 (None)
                 60 RETURN_VALUE
    consts
+      ' Toggles workspace zooming '
       1
       ('Plugin',)
       2
-      ('hyprctlJSON', 'hyprctl')
+      ('hyprctl',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
-         code 0x970065005a0164005a02640184005a03640284005a0464035300
-           6           0 RESUME                   0
+         code 0x970065005a0164005a0264015a03640284005a0464035300
+           7           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Extension')
                        8 STORE_NAME               2 (__qualname__)
          
-           7          10 LOAD_CONST               1 (<code object init, file "/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py", line 7>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (init)
+           8          10 LOAD_CONST               1 (False)
+                      12 STORE_NAME               3 (zoomed)
          
-          10          16 LOAD_CONST               2 (<code object run_zoom, file "/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py", line 10>)
-                      18 MAKE_FUNCTION            0
-                      20 STORE_NAME               4 (run_zoom)
-                      22 LOAD_CONST               3 (None)
-                      24 RETURN_VALUE
+          10          14 LOAD_CONST               2 (<code object run_zoom, file "/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py", line 10>)
+                      16 MAKE_FUNCTION            0
+                      18 STORE_NAME               4 (run_zoom)
+                      20 LOAD_CONST               3 (None)
+                      22 RETURN_VALUE
          consts
             'Extension'
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 2
-               flags     : 131
-               code 0x4b000100970064017c005f00000000000000000064005300
-                 7           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-               
-                 8           6 LOAD_CONST               1 (False)
-                             8 LOAD_FAST                0 (self)
-                            10 STORE_ATTR               0 (zoomed)
-                            20 LOAD_CONST               0 (None)
-                            22 RETURN_VALUE
-               consts
-                  None
-                  False
-               names      ('zoomed',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py'
-               name       'init'
-               firstlineno 7
-               lnotab 0x0601
+            False
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 6
                flags     : 135
                code
                   0x4b00010097007c01723b7401000000000000000000007c016401190000
@@ -218,25 +194,25 @@
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py'
                name       'run_zoom'
                firstlineno 10
                lnotab 0x060204012a0132011a020e012e0250013201
             None
-         names      ('__name__', '__module__', '__qualname__', 'init', 'run_zoom')
+         names      ('__name__', '__module__', '__qualname__', 'zoomed', 'run_zoom')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py'
          name       'Extension'
-         firstlineno 6
-         lnotab 0x0a010603
+         firstlineno 7
+         lnotab 0x0a010402
       'Extension'
       None
-   names      ('interface', 'Plugin', 'ipc', 'hyprctlJSON', 'hyprctl', 'Extension')
+   names      ('__doc__', 'interface', 'Plugin', 'ipc', 'hyprctl', 'Extension')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/fab/dev/std/pyprland/pyprland/plugins/magnify.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c021003
+   lnotab 0x00ff020104010c020c03
```

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/monitors.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/monitors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/scratchpads.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/scratchpads.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,1243 +1,1499 @@
 magic:    0xa70d0d0a
-moddate:  0x51dc4e64 (Sun Apr 30 21:23:29 2023 UTC)
-files sz: 11860
+moddate:  0xe899c664 (Sun Jul 30 17:12:08 2023 UTC)
+files sz: 14965
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a020100640064016c035a
-      03640364046c046d055a056d065a066d075a070100640064016c085a0864
-      0564066c096d0a5a0a010064075a0b6408650c6602640984045a0d020047
-      00640a8400640ba6020000ab0200000000000000005a0e02004700640c84
-      00640da6020000ab0200000000000000005a0f02004700640e8400640f65
-      0aa6030000ab0300000000000000005a1064015300
+      0x970064005a00640164026c015a01640164026c025a02640164026c035a
+      03640164036c046d055a056d065a060100640464056c076d085a086d095a
+      096d0a5a0a0100640664076c0b6d0c5a0c010064085a0d6409650e660264
+      0a84045a0f02004700640b8400640ca6020000ab0200000000000000005a
+      1002004700640d8400640ea6020000ab0200000000000000005a11020047
+      00640f84006410650ca6030000ab0300000000000000005a1264025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (subprocess)
-                 8 STORE_NAME               0 (subprocess)
+     1           2 LOAD_CONST               0 (' Scratchpads addon ')
+                 4 STORE_NAME               0 (__doc__)
    
-     2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('Any',))
-                14 IMPORT_NAME              1 (typing)
-                16 IMPORT_FROM              2 (Any)
-                18 STORE_NAME               2 (Any)
-                20 POP_TOP
+     2           6 LOAD_CONST               1 (0)
+                 8 LOAD_CONST               2 (None)
+                10 IMPORT_NAME              1 (os)
+                12 STORE_NAME               1 (os)
    
-     3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               1 (None)
-                26 IMPORT_NAME              3 (asyncio)
-                28 STORE_NAME               3 (asyncio)
+     3          14 LOAD_CONST               1 (0)
+                16 LOAD_CONST               2 (None)
+                18 IMPORT_NAME              2 (asyncio)
+                20 STORE_NAME               2 (asyncio)
    
-     4          30 LOAD_CONST               3 (2)
-                32 LOAD_CONST               4 (('hyprctl', 'hyprctlJSON', 'get_focused_monitor_props'))
-                34 IMPORT_NAME              4 (ipc)
-                36 IMPORT_FROM              5 (hyprctl)
-                38 STORE_NAME               5 (hyprctl)
-                40 IMPORT_FROM              6 (hyprctlJSON)
-                42 STORE_NAME               6 (hyprctlJSON)
-                44 IMPORT_FROM              7 (get_focused_monitor_props)
-                46 STORE_NAME               7 (get_focused_monitor_props)
-                48 POP_TOP
+     4          22 LOAD_CONST               1 (0)
+                24 LOAD_CONST               2 (None)
+                26 IMPORT_NAME              3 (subprocess)
+                28 STORE_NAME               3 (subprocess)
    
-     9          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               1 (None)
-                54 IMPORT_NAME              8 (os)
-                56 STORE_NAME               8 (os)
+     5          30 LOAD_CONST               1 (0)
+                32 LOAD_CONST               3 (('Any', 'cast'))
+                34 IMPORT_NAME              4 (typing)
+                36 IMPORT_FROM              5 (Any)
+                38 STORE_NAME               5 (Any)
+                40 IMPORT_FROM              6 (cast)
+                42 STORE_NAME               6 (cast)
+                44 POP_TOP
    
-    11          58 LOAD_CONST               5 (1)
-                60 LOAD_CONST               6 (('Plugin',))
-                62 IMPORT_NAME              9 (interface)
-                64 IMPORT_FROM             10 (Plugin)
-                66 STORE_NAME              10 (Plugin)
-                68 POP_TOP
+     7          46 LOAD_CONST               4 (2)
+                48 LOAD_CONST               5 (('hyprctl', 'hyprctlJSON', 'get_focused_monitor_props'))
+                50 IMPORT_NAME              7 (ipc)
+                52 IMPORT_FROM              8 (hyprctl)
+                54 STORE_NAME               8 (hyprctl)
+                56 IMPORT_FROM              9 (hyprctlJSON)
+                58 STORE_NAME               9 (hyprctlJSON)
+                60 IMPORT_FROM             10 (get_focused_monitor_props)
+                62 STORE_NAME              10 (get_focused_monitor_props)
+                64 POP_TOP
    
-    13          70 LOAD_CONST               7 (60)
-                72 STORE_NAME              11 (DEFAULT_MARGIN)
+    13          66 LOAD_CONST               6 (1)
+                68 LOAD_CONST               7 (('Plugin',))
+                70 IMPORT_NAME             11 (interface)
+                72 IMPORT_FROM             12 (Plugin)
+                74 STORE_NAME              12 (Plugin)
+                76 POP_TOP
    
-    16          74 LOAD_CONST               8 ('addr')
-                76 LOAD_NAME               12 (str)
-                78 BUILD_TUPLE              2
-                80 LOAD_CONST               9 (<code object get_client_props_by_address, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 16>)
-                82 MAKE_FUNCTION            4 (annotations)
-                84 STORE_NAME              13 (get_client_props_by_address)
+    15          78 LOAD_CONST               8 (60)
+                80 STORE_NAME              13 (DEFAULT_MARGIN)
    
-    23          86 PUSH_NULL
-                88 LOAD_BUILD_CLASS
-                90 LOAD_CONST              10 (<code object Animations, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 23>)
-                92 MAKE_FUNCTION            0
-                94 LOAD_CONST              11 ('Animations')
-                96 PRECALL                  2
-               100 CALL                     2
-               110 STORE_NAME              14 (Animations)
+    18          82 LOAD_CONST               9 ('addr')
+                84 LOAD_NAME               14 (str)
+                86 BUILD_TUPLE              2
+                88 LOAD_CONST              10 (<code object get_client_props_by_address, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 18>)
+                90 MAKE_FUNCTION            4 (annotations)
+                92 STORE_NAME              15 (get_client_props_by_address)
    
-    74         112 PUSH_NULL
-               114 LOAD_BUILD_CLASS
-               116 LOAD_CONST              12 (<code object Scratch, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 74>)
-               118 MAKE_FUNCTION            0
-               120 LOAD_CONST              13 ('Scratch')
-               122 PRECALL                  2
-               126 CALL                     2
-               136 STORE_NAME              15 (Scratch)
+    26          94 PUSH_NULL
+                96 LOAD_BUILD_CLASS
+                98 LOAD_CONST              11 (<code object Animations, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 26>)
+               100 MAKE_FUNCTION            0
+               102 LOAD_CONST              12 ('Animations')
+               104 PRECALL                  2
+               108 CALL                     2
+               118 STORE_NAME              16 (Animations)
    
-   109         138 PUSH_NULL
-               140 LOAD_BUILD_CLASS
-               142 LOAD_CONST              14 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 109>)
-               144 MAKE_FUNCTION            0
-               146 LOAD_CONST              15 ('Extension')
-               148 LOAD_NAME               10 (Plugin)
-               150 PRECALL                  3
-               154 CALL                     3
-               164 STORE_NAME              16 (Extension)
-               166 LOAD_CONST               1 (None)
-               168 RETURN_VALUE
+    88         120 PUSH_NULL
+               122 LOAD_BUILD_CLASS
+               124 LOAD_CONST              13 (<code object Scratch, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 88>)
+               126 MAKE_FUNCTION            0
+               128 LOAD_CONST              14 ('Scratch')
+               130 PRECALL                  2
+               134 CALL                     2
+               144 STORE_NAME              17 (Scratch)
+   
+   133         146 PUSH_NULL
+               148 LOAD_BUILD_CLASS
+               150 LOAD_CONST              15 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 133>)
+               152 MAKE_FUNCTION            0
+               154 LOAD_CONST              16 ('Extension')
+               156 LOAD_NAME               12 (Plugin)
+               158 PRECALL                  3
+               162 CALL                     3
+               172 STORE_NAME              18 (Extension)
+               174 LOAD_CONST               2 (None)
+               176 RETURN_VALUE
    consts
+      ' Scratchpads addon '
       0
       None
-      ('Any',)
+      ('Any', 'cast')
       2
       ('hyprctl', 'hyprctlJSON', 'get_focused_monitor_props')
       1
       ('Plugin',)
       60
       'addr'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 131
          code
             0x4b00010097007401000000000000000000006401a6010000ab01000000
-            0000000000830064007b0356009703860444005d367d0174030000000000
+            0000000000830064027b0356009703860444005d367d0174030000000000
             00000000007c01740400000000000000000000a6020000ab020000000000
             00000073024a0082017c01a0030000000000000000000000000000000000
-            0000006402a6010000ab0100000000000000007c006b020000000072047c
-            016302010053008c3764005300
-          16           0 RETURN_GENERATOR
+            0000006403a6010000ab0100000000000000007c006b020000000072047c
+            016302010053008c3764025300
+          18           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-          17           6 LOAD_GLOBAL              1 (NULL + hyprctlJSON)
+          20           6 LOAD_GLOBAL              1 (NULL + hyprctlJSON)
                       18 LOAD_CONST               1 ('clients')
                       20 PRECALL                  1
                       24 CALL                     1
                       34 GET_AWAITABLE            0
-                      36 LOAD_CONST               0 (None)
+                      36 LOAD_CONST               2 (None)
                  >>   38 SEND                     3 (to 46)
                       40 YIELD_VALUE
                       42 RESUME                   3
                       44 JUMP_BACKWARD_NO_INTERRUPT     4 (to 38)
                  >>   46 GET_ITER
                  >>   48 FOR_ITER                54 (to 158)
                       50 STORE_FAST               1 (client)
          
-          18          52 LOAD_GLOBAL              3 (NULL + isinstance)
+          21          52 LOAD_GLOBAL              3 (NULL + isinstance)
                       64 LOAD_FAST                1 (client)
                       66 LOAD_GLOBAL              4 (dict)
                       78 PRECALL                  2
                       82 CALL                     2
                       92 POP_JUMP_FORWARD_IF_TRUE     2 (to 98)
                       94 LOAD_ASSERTION_ERROR
                       96 RAISE_VARARGS            1
          
-          19     >>   98 LOAD_FAST                1 (client)
+          22     >>   98 LOAD_FAST                1 (client)
                      100 LOAD_METHOD              3 (get)
-                     122 LOAD_CONST               2 ('address')
+                     122 LOAD_CONST               3 ('address')
                      124 PRECALL                  1
                      128 CALL                     1
                      138 LOAD_FAST                0 (addr)
                      140 COMPARE_OP               2 (==)
                      146 POP_JUMP_FORWARD_IF_FALSE     4 (to 156)
          
-          20         148 LOAD_FAST                1 (client)
+          23         148 LOAD_FAST                1 (client)
                      150 SWAP                     2
                      152 POP_TOP
                      154 RETURN_VALUE
          
-          19     >>  156 JUMP_BACKWARD           55 (to 48)
+          22     >>  156 JUMP_BACKWARD           55 (to 48)
          
-          17     >>  158 LOAD_CONST               0 (None)
+          20     >>  158 LOAD_CONST               2 (None)
                      160 RETURN_VALUE
          consts
-            None
+            'Returns client properties given its address'
             'clients'
+            None
             'address'
          names      ('hyprctlJSON', 'isinstance', 'dict', 'get')
          varnames   ('addr', 'client')
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
          name       'get_client_props_by_address'
-         firstlineno 16
-         lnotab 0x06012e012e01320108ff02fe
+         firstlineno 18
+         lnotab 0x06022e012e01320108ff02fe
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
-            0x970065005a0164005a02650364018400a6000000ab0000000000000000
-            005a04650364028400a6000000ab0000000000000000005a056503640384
-            00a6000000ab0000000000000000005a06650364048400a6000000ab0000
-            000000000000005a0764055300
-          23           0 RESUME                   0
+            0x970065005a0164005a0264015a03650464028400a6000000ab00000000
+            00000000005a05650464038400a6000000ab0000000000000000005a0665
+            0464048400a6000000ab0000000000000000005a07650464058400a60000
+            00ab0000000000000000005a0864065300
+          26           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Animations')
                        8 STORE_NAME               2 (__qualname__)
          
-          24          10 LOAD_NAME                3 (classmethod)
+          27          10 LOAD_CONST               1 ('Animation store')
+                      12 STORE_NAME               3 (__doc__)
          
-          25          12 LOAD_CONST               1 (<code object fromtop, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 24>)
-                      14 MAKE_FUNCTION            0
+          29          14 LOAD_NAME                4 (staticmethod)
          
-          24          16 PRECALL                  0
-                      20 CALL                     0
+          30          16 LOAD_CONST               2 (<code object fromtop, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 29>)
+                      18 MAKE_FUNCTION            0
          
-          25          30 STORE_NAME               4 (fromtop)
+          29          20 PRECALL                  0
+                      24 CALL                     0
          
-          34          32 LOAD_NAME                3 (classmethod)
+          30          34 STORE_NAME               5 (fromtop)
          
-          35          34 LOAD_CONST               2 (<code object frombottom, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 34>)
-                      36 MAKE_FUNCTION            0
+          42          36 LOAD_NAME                4 (staticmethod)
          
-          34          38 PRECALL                  0
-                      42 CALL                     0
+          43          38 LOAD_CONST               3 (<code object frombottom, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 42>)
+                      40 MAKE_FUNCTION            0
          
-          35          52 STORE_NAME               5 (frombottom)
+          42          42 PRECALL                  0
+                      46 CALL                     0
          
-          48          54 LOAD_NAME                3 (classmethod)
+          43          56 STORE_NAME               6 (frombottom)
          
-          49          56 LOAD_CONST               3 (<code object fromleft, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 48>)
-                      58 MAKE_FUNCTION            0
+          58          58 LOAD_NAME                4 (staticmethod)
          
-          48          60 PRECALL                  0
-                      64 CALL                     0
+          59          60 LOAD_CONST               4 (<code object fromleft, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 58>)
+                      62 MAKE_FUNCTION            0
          
-          49          74 STORE_NAME               6 (fromleft)
+          58          64 PRECALL                  0
+                      68 CALL                     0
          
-          59          76 LOAD_NAME                3 (classmethod)
+          59          78 STORE_NAME               7 (fromleft)
          
-          60          78 LOAD_CONST               4 (<code object fromright, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 59>)
-                      80 MAKE_FUNCTION            0
+          71          80 LOAD_NAME                4 (staticmethod)
          
-          59          82 PRECALL                  0
-                      86 CALL                     0
+          72          82 LOAD_CONST               5 (<code object fromright, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 71>)
+                      84 MAKE_FUNCTION            0
          
-          60          96 STORE_NAME               7 (fromright)
-                      98 LOAD_CONST               5 (None)
-                     100 RETURN_VALUE
+          71          86 PRECALL                  0
+                      90 CALL                     0
+         
+          72         100 STORE_NAME               8 (fromright)
+                     102 LOAD_CONST               6 (None)
+                     104 RETURN_VALUE
          consts
             'Animations'
+            'Animation store'
             code
-               argcount  : 5
+               argcount  : 4
                nlocals   : 10
                stacksize : 8
                flags     : 131
                code
-                  0x4b00010097007c016401190000000000000000007d057c016402190000
-                  000000000000007d067c016403190000000000000000007d077c02640419
-                  0000000000000000006405190000000000000000007d0874010000000000
-                  00000000007c077c087a0a000064067a0b0000a6010000ab010000000000
-                  0000007c057a0000007d0974030000000000000000000064077c099b0064
-                  087c067c047a0000009b0064097c039b009d06a6010000ab010000000000
-                  000000830064007b03560097038604010064005300
-                24           0 RETURN_GENERATOR
+                  0x4b00010097007401000000000000000000007c00640119000000000000
+                  000000a6010000ab0100000000000000007d047c00640219000000000000
+                  0000007d057c006403190000000000000000007d06740300000000000000
+                  0000007c006404190000000000000000007c047a0b0000a6010000ab0100
+                  000000000000007d077c0164051900000000000000000064061900000000
+                  00000000007d087403000000000000000000007c077c087a0a000064077a
+                  0b0000a6010000ab0100000000000000007c057a0000007d097405000000
+                  0000000000000064087c099b0064097c067c037a0000009b00640a7c029b
+                  009d06a6010000ab0100000000000000008300640b7b0356009703860401
+                  00640b5300
+                29           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                26           6 LOAD_FAST                1 (monitor)
-                             8 LOAD_CONST               1 ('x')
-                            10 BINARY_SUBSCR
-                            20 STORE_FAST               5 (mon_x)
+                32           6 LOAD_GLOBAL              1 (NULL + float)
+                            18 LOAD_FAST                0 (monitor)
+                            20 LOAD_CONST               1 ('scale')
+                            22 BINARY_SUBSCR
+                            32 PRECALL                  1
+                            36 CALL                     1
+                            46 STORE_FAST               4 (scale)
+               
+                33          48 LOAD_FAST                0 (monitor)
+                            50 LOAD_CONST               2 ('x')
+                            52 BINARY_SUBSCR
+                            62 STORE_FAST               5 (mon_x)
+               
+                34          64 LOAD_FAST                0 (monitor)
+                            66 LOAD_CONST               3 ('y')
+                            68 BINARY_SUBSCR
+                            78 STORE_FAST               6 (mon_y)
+               
+                35          80 LOAD_GLOBAL              3 (NULL + int)
+                            92 LOAD_FAST                0 (monitor)
+                            94 LOAD_CONST               4 ('width')
+                            96 BINARY_SUBSCR
+                           106 LOAD_FAST                4 (scale)
+                           108 BINARY_OP               11 (/)
+                           112 PRECALL                  1
+                           116 CALL                     1
+                           126 STORE_FAST               7 (mon_width)
+               
+                37         128 LOAD_FAST                1 (client)
+                           130 LOAD_CONST               5 ('size')
+                           132 BINARY_SUBSCR
+                           142 LOAD_CONST               6 (0)
+                           144 BINARY_SUBSCR
+                           154 STORE_FAST               8 (client_width)
+               
+                38         156 LOAD_GLOBAL              3 (NULL + int)
+                           168 LOAD_FAST                7 (mon_width)
+                           170 LOAD_FAST                8 (client_width)
+                           172 BINARY_OP               10 (-)
+                           176 LOAD_CONST               7 (2)
+                           178 BINARY_OP               11 (/)
+                           182 PRECALL                  1
+                           186 CALL                     1
+                           196 LOAD_FAST                5 (mon_x)
+                           198 BINARY_OP                0 (+)
+                           202 STORE_FAST               9 (margin_x)
                
-                27          22 LOAD_FAST                1 (monitor)
-                            24 LOAD_CONST               2 ('y')
-                            26 BINARY_SUBSCR
-                            36 STORE_FAST               6 (mon_y)
-               
-                28          38 LOAD_FAST                1 (monitor)
-                            40 LOAD_CONST               3 ('width')
-                            42 BINARY_SUBSCR
-                            52 STORE_FAST               7 (mon_width)
-               
-                30          54 LOAD_FAST                2 (client)
-                            56 LOAD_CONST               4 ('size')
-                            58 BINARY_SUBSCR
-                            68 LOAD_CONST               5 (0)
-                            70 BINARY_SUBSCR
-                            80 STORE_FAST               8 (client_width)
-               
-                31          82 LOAD_GLOBAL              1 (NULL + int)
-                            94 LOAD_FAST                7 (mon_width)
-                            96 LOAD_FAST                8 (client_width)
-                            98 BINARY_OP               10 (-)
-                           102 LOAD_CONST               6 (2)
-                           104 BINARY_OP               11 (/)
-                           108 PRECALL                  1
-                           112 CALL                     1
-                           122 LOAD_FAST                5 (mon_x)
-                           124 BINARY_OP                0 (+)
-                           128 STORE_FAST               9 (margin_x)
-               
-                32         130 LOAD_GLOBAL              3 (NULL + hyprctl)
-                           142 LOAD_CONST               7 ('movewindowpixel exact ')
-                           144 LOAD_FAST                9 (margin_x)
-                           146 FORMAT_VALUE             0
-                           148 LOAD_CONST               8 (' ')
-                           150 LOAD_FAST                6 (mon_y)
-                           152 LOAD_FAST                4 (margin)
-                           154 BINARY_OP                0 (+)
-                           158 FORMAT_VALUE             0
-                           160 LOAD_CONST               9 (',')
-                           162 LOAD_FAST                3 (client_uid)
-                           164 FORMAT_VALUE             0
-                           166 BUILD_STRING             6
-                           168 PRECALL                  1
-                           172 CALL                     1
-                           182 GET_AWAITABLE            0
-                           184 LOAD_CONST               0 (None)
-                       >>  186 SEND                     3 (to 194)
-                           188 YIELD_VALUE
-                           190 RESUME                   3
-                           192 JUMP_BACKWARD_NO_INTERRUPT     4 (to 186)
-                       >>  194 POP_TOP
-                           196 LOAD_CONST               0 (None)
-                           198 RETURN_VALUE
+                40         204 LOAD_GLOBAL              5 (NULL + hyprctl)
+                           216 LOAD_CONST               8 ('movewindowpixel exact ')
+                           218 LOAD_FAST                9 (margin_x)
+                           220 FORMAT_VALUE             0
+                           222 LOAD_CONST               9 (' ')
+                           224 LOAD_FAST                6 (mon_y)
+                           226 LOAD_FAST                3 (margin)
+                           228 BINARY_OP                0 (+)
+                           232 FORMAT_VALUE             0
+                           234 LOAD_CONST              10 (',')
+                           236 LOAD_FAST                2 (client_uid)
+                           238 FORMAT_VALUE             0
+                           240 BUILD_STRING             6
+                           242 PRECALL                  1
+                           246 CALL                     1
+                           256 GET_AWAITABLE            0
+                           258 LOAD_CONST              11 (None)
+                       >>  260 SEND                     3 (to 268)
+                           262 YIELD_VALUE
+                           264 RESUME                   3
+                           266 JUMP_BACKWARD_NO_INTERRUPT     4 (to 260)
+                       >>  268 POP_TOP
+                           270 LOAD_CONST              11 (None)
+                           272 RETURN_VALUE
                consts
-                  None
+                  'Slide from/to top'
+                  'scale'
                   'x'
                   'y'
                   'width'
                   'size'
                   0
                   2
                   'movewindowpixel exact '
                   ' '
                   ','
-               names      ('int', 'hyprctl')
-               varnames   ('cls', 'monitor', 'client', 'client_uid', 'margin', 'mon_x', 'mon_y', 'mon_width', 'client_width', 'margin_x')
+                  None
+               names      ('float', 'int', 'hyprctl')
+               varnames   ('monitor', 'client', 'client_uid', 'margin', 'scale', 'mon_x', 'mon_y', 'mon_width', 'client_width', 'margin_x')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'fromtop'
-               firstlineno 24
-               lnotab 0x06021001100110021c013001
+               firstlineno 29
+               lnotab 0x06032a011001100130021c013002
             code
-               argcount  : 5
+               argcount  : 4
                nlocals   : 12
                stacksize : 8
                flags     : 131
                code
-                  0x4b00010097007c016401190000000000000000007d057c016402190000
-                  000000000000007d067c016403190000000000000000007d077c01640419
-                  0000000000000000007d087c026405190000000000000000006406190000
-                  000000000000007d097c0264051900000000000000000064071900000000
-                  00000000007d0a7401000000000000000000007c077c097a0a000064087a
-                  0b0000a6010000ab0100000000000000007c057a0000007d0b7403000000
-                  0000000000000064097c0b9b00640a7c067c087a0000007c0a7a0a00007c
-                  047a0a00009b00640b7c039b009d06a6010000ab01000000000000000083
-                  0064007b03560097038604010064005300
-                34           0 RETURN_GENERATOR
+                  0x4b00010097007401000000000000000000007c00640119000000000000
+                  000000a6010000ab0100000000000000007d047c00640219000000000000
+                  0000007d057c006403190000000000000000007d06740300000000000000
+                  0000007c006404190000000000000000007c047a0b0000a6010000ab0100
+                  000000000000007d077403000000000000000000007c0064051900000000
+                  00000000007c047a0b0000a6010000ab0100000000000000007d087c0164
+                  06190000000000000000006407190000000000000000007d097c01640619
+                  0000000000000000006408190000000000000000007d0a74030000000000
+                  00000000007c077c097a0a000064097a0b0000a6010000ab010000000000
+                  0000007c057a0000007d0b740500000000000000000000640a7c0b9b0064
+                  0b7c067c087a0000007c0a7a0a00007c037a0a00009b00640c7c029b009d
+                  06a6010000ab0100000000000000008300640d7b03560097038604010064
+                  0d5300
+                42           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                36           6 LOAD_FAST                1 (monitor)
-                             8 LOAD_CONST               1 ('x')
-                            10 BINARY_SUBSCR
-                            20 STORE_FAST               5 (mon_x)
+                45           6 LOAD_GLOBAL              1 (NULL + float)
+                            18 LOAD_FAST                0 (monitor)
+                            20 LOAD_CONST               1 ('scale')
+                            22 BINARY_SUBSCR
+                            32 PRECALL                  1
+                            36 CALL                     1
+                            46 STORE_FAST               4 (scale)
+               
+                46          48 LOAD_FAST                0 (monitor)
+                            50 LOAD_CONST               2 ('x')
+                            52 BINARY_SUBSCR
+                            62 STORE_FAST               5 (mon_x)
                
-                37          22 LOAD_FAST                1 (monitor)
-                            24 LOAD_CONST               2 ('y')
-                            26 BINARY_SUBSCR
-                            36 STORE_FAST               6 (mon_y)
-               
-                38          38 LOAD_FAST                1 (monitor)
-                            40 LOAD_CONST               3 ('width')
-                            42 BINARY_SUBSCR
-                            52 STORE_FAST               7 (mon_width)
-               
-                39          54 LOAD_FAST                1 (monitor)
-                            56 LOAD_CONST               4 ('height')
-                            58 BINARY_SUBSCR
-                            68 STORE_FAST               8 (mon_height)
-               
-                41          70 LOAD_FAST                2 (client)
-                            72 LOAD_CONST               5 ('size')
-                            74 BINARY_SUBSCR
-                            84 LOAD_CONST               6 (0)
-                            86 BINARY_SUBSCR
-                            96 STORE_FAST               9 (client_width)
+                47          64 LOAD_FAST                0 (monitor)
+                            66 LOAD_CONST               3 ('y')
+                            68 BINARY_SUBSCR
+                            78 STORE_FAST               6 (mon_y)
                
-                42          98 LOAD_FAST                2 (client)
-                           100 LOAD_CONST               5 ('size')
-                           102 BINARY_SUBSCR
-                           112 LOAD_CONST               7 (1)
-                           114 BINARY_SUBSCR
-                           124 STORE_FAST              10 (client_height)
-               
-                43         126 LOAD_GLOBAL              1 (NULL + int)
-                           138 LOAD_FAST                7 (mon_width)
-                           140 LOAD_FAST                9 (client_width)
-                           142 BINARY_OP               10 (-)
-                           146 LOAD_CONST               8 (2)
-                           148 BINARY_OP               11 (/)
-                           152 PRECALL                  1
-                           156 CALL                     1
-                           166 LOAD_FAST                5 (mon_x)
-                           168 BINARY_OP                0 (+)
-                           172 STORE_FAST              11 (margin_x)
-               
-                44         174 LOAD_GLOBAL              3 (NULL + hyprctl)
-               
-                45         186 LOAD_CONST               9 ('movewindowpixel exact ')
-                           188 LOAD_FAST               11 (margin_x)
-                           190 FORMAT_VALUE             0
-                           192 LOAD_CONST              10 (' ')
-                           194 LOAD_FAST                6 (mon_y)
-                           196 LOAD_FAST                8 (mon_height)
-                           198 BINARY_OP                0 (+)
-                           202 LOAD_FAST               10 (client_height)
-                           204 BINARY_OP               10 (-)
-                           208 LOAD_FAST                4 (margin)
-                           210 BINARY_OP               10 (-)
-                           214 FORMAT_VALUE             0
-                           216 LOAD_CONST              11 (',')
-                           218 LOAD_FAST                3 (client_uid)
-                           220 FORMAT_VALUE             0
-                           222 BUILD_STRING             6
+                48          80 LOAD_GLOBAL              3 (NULL + int)
+                            92 LOAD_FAST                0 (monitor)
+                            94 LOAD_CONST               4 ('width')
+                            96 BINARY_SUBSCR
+                           106 LOAD_FAST                4 (scale)
+                           108 BINARY_OP               11 (/)
+                           112 PRECALL                  1
+                           116 CALL                     1
+                           126 STORE_FAST               7 (mon_width)
                
-                44         224 PRECALL                  1
-                           228 CALL                     1
-                           238 GET_AWAITABLE            0
-                           240 LOAD_CONST               0 (None)
-                       >>  242 SEND                     3 (to 250)
-                           244 YIELD_VALUE
-                           246 RESUME                   3
-                           248 JUMP_BACKWARD_NO_INTERRUPT     4 (to 242)
-                       >>  250 POP_TOP
-                           252 LOAD_CONST               0 (None)
-                           254 RETURN_VALUE
+                49         128 LOAD_GLOBAL              3 (NULL + int)
+                           140 LOAD_FAST                0 (monitor)
+                           142 LOAD_CONST               5 ('height')
+                           144 BINARY_SUBSCR
+                           154 LOAD_FAST                4 (scale)
+                           156 BINARY_OP               11 (/)
+                           160 PRECALL                  1
+                           164 CALL                     1
+                           174 STORE_FAST               8 (mon_height)
+               
+                51         176 LOAD_FAST                1 (client)
+                           178 LOAD_CONST               6 ('size')
+                           180 BINARY_SUBSCR
+                           190 LOAD_CONST               7 (0)
+                           192 BINARY_SUBSCR
+                           202 STORE_FAST               9 (client_width)
+               
+                52         204 LOAD_FAST                1 (client)
+                           206 LOAD_CONST               6 ('size')
+                           208 BINARY_SUBSCR
+                           218 LOAD_CONST               8 (1)
+                           220 BINARY_SUBSCR
+                           230 STORE_FAST              10 (client_height)
+               
+                53         232 LOAD_GLOBAL              3 (NULL + int)
+                           244 LOAD_FAST                7 (mon_width)
+                           246 LOAD_FAST                9 (client_width)
+                           248 BINARY_OP               10 (-)
+                           252 LOAD_CONST               9 (2)
+                           254 BINARY_OP               11 (/)
+                           258 PRECALL                  1
+                           262 CALL                     1
+                           272 LOAD_FAST                5 (mon_x)
+                           274 BINARY_OP                0 (+)
+                           278 STORE_FAST              11 (margin_x)
+               
+                54         280 LOAD_GLOBAL              5 (NULL + hyprctl)
+               
+                55         292 LOAD_CONST              10 ('movewindowpixel exact ')
+                           294 LOAD_FAST               11 (margin_x)
+                           296 FORMAT_VALUE             0
+                           298 LOAD_CONST              11 (' ')
+                           300 LOAD_FAST                6 (mon_y)
+                           302 LOAD_FAST                8 (mon_height)
+                           304 BINARY_OP                0 (+)
+                           308 LOAD_FAST               10 (client_height)
+                           310 BINARY_OP               10 (-)
+                           314 LOAD_FAST                3 (margin)
+                           316 BINARY_OP               10 (-)
+                           320 FORMAT_VALUE             0
+                           322 LOAD_CONST              12 (',')
+                           324 LOAD_FAST                2 (client_uid)
+                           326 FORMAT_VALUE             0
+                           328 BUILD_STRING             6
+               
+                54         330 PRECALL                  1
+                           334 CALL                     1
+                           344 GET_AWAITABLE            0
+                           346 LOAD_CONST              13 (None)
+                       >>  348 SEND                     3 (to 356)
+                           350 YIELD_VALUE
+                           352 RESUME                   3
+                           354 JUMP_BACKWARD_NO_INTERRUPT     4 (to 348)
+                       >>  356 POP_TOP
+                           358 LOAD_CONST              13 (None)
+                           360 RETURN_VALUE
                consts
-                  None
+                  'Slide from/to bottom'
+                  'scale'
                   'x'
                   'y'
                   'width'
                   'height'
                   'size'
                   0
                   1
                   2
                   'movewindowpixel exact '
                   ' '
                   ','
-               names      ('int', 'hyprctl')
-               varnames   ('cls', 'monitor', 'client', 'client_uid', 'margin', 'mon_x', 'mon_y', 'mon_width', 'mon_height', 'client_width', 'client_height', 'margin_x')
+                  None
+               names      ('float', 'int', 'hyprctl')
+               varnames   ('monitor', 'client', 'client_uid', 'margin', 'scale', 'mon_x', 'mon_y', 'mon_width', 'mon_height', 'client_width', 'client_height', 'margin_x')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'frombottom'
-               firstlineno 34
-               lnotab 0x060210011001100110021c011c0130010c0126ff
+               firstlineno 42
+               lnotab 0x06032a0110011001300130021c011c0130010c0126ff
             code
-               argcount  : 5
+               argcount  : 4
                nlocals   : 10
                stacksize : 8
                flags     : 131
                code
-                  0x4b00010097007c016401190000000000000000007d057c016402190000
-                  000000000000007d067c016403190000000000000000007d077c02640419
-                  0000000000000000006405190000000000000000007d0874010000000000
-                  00000000007c077c087a0a000064067a0b0000a6010000ab010000000000
-                  0000007c067a0000007d0974030000000000000000000064077c047c057a
-                  0000009b0064087c099b0064097c039b009d06a6010000ab010000000000
-                  000000830064007b03560097038604010064005300
-                48           0 RETURN_GENERATOR
+                  0x4b00010097007401000000000000000000007c00640119000000000000
+                  000000a6010000ab0100000000000000007d047c00640219000000000000
+                  0000007d057c006403190000000000000000007d06740300000000000000
+                  0000007c006404190000000000000000007c047a0b0000a6010000ab0100
+                  000000000000007d077c0164051900000000000000000064061900000000
+                  00000000007d087403000000000000000000007c077c087a0a000064077a
+                  0b0000a6010000ab0100000000000000007c067a0000007d097405000000
+                  0000000000000064087c037c057a0000009b0064097c099b00640a7c029b
+                  009d06a6010000ab0100000000000000008300640b7b0356009703860401
+                  00640b5300
+                58           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                50           6 LOAD_FAST                1 (monitor)
-                             8 LOAD_CONST               1 ('x')
-                            10 BINARY_SUBSCR
-                            20 STORE_FAST               5 (mon_x)
+                61           6 LOAD_GLOBAL              1 (NULL + float)
+                            18 LOAD_FAST                0 (monitor)
+                            20 LOAD_CONST               1 ('scale')
+                            22 BINARY_SUBSCR
+                            32 PRECALL                  1
+                            36 CALL                     1
+                            46 STORE_FAST               4 (scale)
+               
+                62          48 LOAD_FAST                0 (monitor)
+                            50 LOAD_CONST               2 ('x')
+                            52 BINARY_SUBSCR
+                            62 STORE_FAST               5 (mon_x)
+               
+                63          64 LOAD_FAST                0 (monitor)
+                            66 LOAD_CONST               3 ('y')
+                            68 BINARY_SUBSCR
+                            78 STORE_FAST               6 (mon_y)
+               
+                64          80 LOAD_GLOBAL              3 (NULL + int)
+                            92 LOAD_FAST                0 (monitor)
+                            94 LOAD_CONST               4 ('height')
+                            96 BINARY_SUBSCR
+                           106 LOAD_FAST                4 (scale)
+                           108 BINARY_OP               11 (/)
+                           112 PRECALL                  1
+                           116 CALL                     1
+                           126 STORE_FAST               7 (mon_height)
                
-                51          22 LOAD_FAST                1 (monitor)
-                            24 LOAD_CONST               2 ('y')
-                            26 BINARY_SUBSCR
-                            36 STORE_FAST               6 (mon_y)
-               
-                52          38 LOAD_FAST                1 (monitor)
-                            40 LOAD_CONST               3 ('height')
-                            42 BINARY_SUBSCR
-                            52 STORE_FAST               7 (mon_height)
-               
-                54          54 LOAD_FAST                2 (client)
-                            56 LOAD_CONST               4 ('size')
-                            58 BINARY_SUBSCR
-                            68 LOAD_CONST               5 (1)
-                            70 BINARY_SUBSCR
-                            80 STORE_FAST               8 (client_height)
-               
-                55          82 LOAD_GLOBAL              1 (NULL + int)
-                            94 LOAD_FAST                7 (mon_height)
-                            96 LOAD_FAST                8 (client_height)
-                            98 BINARY_OP               10 (-)
-                           102 LOAD_CONST               6 (2)
-                           104 BINARY_OP               11 (/)
-                           108 PRECALL                  1
-                           112 CALL                     1
-                           122 LOAD_FAST                6 (mon_y)
-                           124 BINARY_OP                0 (+)
-                           128 STORE_FAST               9 (margin_y)
-               
-                57         130 LOAD_GLOBAL              3 (NULL + hyprctl)
-                           142 LOAD_CONST               7 ('movewindowpixel exact ')
-                           144 LOAD_FAST                4 (margin)
-                           146 LOAD_FAST                5 (mon_x)
-                           148 BINARY_OP                0 (+)
-                           152 FORMAT_VALUE             0
-                           154 LOAD_CONST               8 (' ')
-                           156 LOAD_FAST                9 (margin_y)
-                           158 FORMAT_VALUE             0
-                           160 LOAD_CONST               9 (',')
-                           162 LOAD_FAST                3 (client_uid)
-                           164 FORMAT_VALUE             0
-                           166 BUILD_STRING             6
-                           168 PRECALL                  1
-                           172 CALL                     1
-                           182 GET_AWAITABLE            0
-                           184 LOAD_CONST               0 (None)
-                       >>  186 SEND                     3 (to 194)
-                           188 YIELD_VALUE
-                           190 RESUME                   3
-                           192 JUMP_BACKWARD_NO_INTERRUPT     4 (to 186)
-                       >>  194 POP_TOP
-                           196 LOAD_CONST               0 (None)
-                           198 RETURN_VALUE
+                66         128 LOAD_FAST                1 (client)
+                           130 LOAD_CONST               5 ('size')
+                           132 BINARY_SUBSCR
+                           142 LOAD_CONST               6 (1)
+                           144 BINARY_SUBSCR
+                           154 STORE_FAST               8 (client_height)
+               
+                67         156 LOAD_GLOBAL              3 (NULL + int)
+                           168 LOAD_FAST                7 (mon_height)
+                           170 LOAD_FAST                8 (client_height)
+                           172 BINARY_OP               10 (-)
+                           176 LOAD_CONST               7 (2)
+                           178 BINARY_OP               11 (/)
+                           182 PRECALL                  1
+                           186 CALL                     1
+                           196 LOAD_FAST                6 (mon_y)
+                           198 BINARY_OP                0 (+)
+                           202 STORE_FAST               9 (margin_y)
+               
+                69         204 LOAD_GLOBAL              5 (NULL + hyprctl)
+                           216 LOAD_CONST               8 ('movewindowpixel exact ')
+                           218 LOAD_FAST                3 (margin)
+                           220 LOAD_FAST                5 (mon_x)
+                           222 BINARY_OP                0 (+)
+                           226 FORMAT_VALUE             0
+                           228 LOAD_CONST               9 (' ')
+                           230 LOAD_FAST                9 (margin_y)
+                           232 FORMAT_VALUE             0
+                           234 LOAD_CONST              10 (',')
+                           236 LOAD_FAST                2 (client_uid)
+                           238 FORMAT_VALUE             0
+                           240 BUILD_STRING             6
+                           242 PRECALL                  1
+                           246 CALL                     1
+                           256 GET_AWAITABLE            0
+                           258 LOAD_CONST              11 (None)
+                       >>  260 SEND                     3 (to 268)
+                           262 YIELD_VALUE
+                           264 RESUME                   3
+                           266 JUMP_BACKWARD_NO_INTERRUPT     4 (to 260)
+                       >>  268 POP_TOP
+                           270 LOAD_CONST              11 (None)
+                           272 RETURN_VALUE
                consts
-                  None
+                  'Slide from/to left'
+                  'scale'
                   'x'
                   'y'
                   'height'
                   'size'
                   1
                   2
                   'movewindowpixel exact '
                   ' '
                   ','
-               names      ('int', 'hyprctl')
-               varnames   ('cls', 'monitor', 'client', 'client_uid', 'margin', 'mon_x', 'mon_y', 'mon_height', 'client_height', 'margin_y')
+                  None
+               names      ('float', 'int', 'hyprctl')
+               varnames   ('monitor', 'client', 'client_uid', 'margin', 'scale', 'mon_x', 'mon_y', 'mon_height', 'client_height', 'margin_y')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'fromleft'
-               firstlineno 48
-               lnotab 0x06021001100110021c013002
+               firstlineno 58
+               lnotab 0x06032a011001100130021c013002
             code
-               argcount  : 5
+               argcount  : 4
                nlocals   : 12
                stacksize : 8
                flags     : 131
                code
-                  0x4b00010097007c016401190000000000000000007d057c016402190000
-                  000000000000007d067c016403190000000000000000007d077c01640419
-                  0000000000000000007d087c026405190000000000000000006406190000
-                  000000000000007d097c0264051900000000000000000064071900000000
-                  00000000007d0a7401000000000000000000007c087c0a7a0a000064087a
-                  0b0000a6010000ab0100000000000000007c067a0000007d0b7403000000
-                  0000000000000064097c077c097a0a00007c047a0a00007c057a0000009b
-                  00640a7c0b9b00640b7c039b009d06a6010000ab01000000000000000083
-                  0064007b03560097038604010064005300
-                59           0 RETURN_GENERATOR
+                  0x4b00010097007401000000000000000000007c00640119000000000000
+                  000000a6010000ab0100000000000000007d047c00640219000000000000
+                  0000007d057c006403190000000000000000007d06740300000000000000
+                  0000007c006404190000000000000000007c047a0b0000a6010000ab0100
+                  000000000000007d077403000000000000000000007c0064051900000000
+                  00000000007c047a0b0000a6010000ab0100000000000000007d087c0164
+                  06190000000000000000006407190000000000000000007d097c01640619
+                  0000000000000000006408190000000000000000007d0a74030000000000
+                  00000000007c087c0a7a0a000064097a0b0000a6010000ab010000000000
+                  0000007c067a0000007d0b740500000000000000000000640a7c077c097a
+                  0a00007c037a0a00007c057a0000009b00640b7c0b9b00640c7c029b009d
+                  06a6010000ab0100000000000000008300640d7b03560097038604010064
+                  0d5300
+                71           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                61           6 LOAD_FAST                1 (monitor)
-                             8 LOAD_CONST               1 ('x')
-                            10 BINARY_SUBSCR
-                            20 STORE_FAST               5 (mon_x)
+                74           6 LOAD_GLOBAL              1 (NULL + float)
+                            18 LOAD_FAST                0 (monitor)
+                            20 LOAD_CONST               1 ('scale')
+                            22 BINARY_SUBSCR
+                            32 PRECALL                  1
+                            36 CALL                     1
+                            46 STORE_FAST               4 (scale)
+               
+                75          48 LOAD_FAST                0 (monitor)
+                            50 LOAD_CONST               2 ('x')
+                            52 BINARY_SUBSCR
+                            62 STORE_FAST               5 (mon_x)
                
-                62          22 LOAD_FAST                1 (monitor)
-                            24 LOAD_CONST               2 ('y')
-                            26 BINARY_SUBSCR
-                            36 STORE_FAST               6 (mon_y)
-               
-                63          38 LOAD_FAST                1 (monitor)
-                            40 LOAD_CONST               3 ('width')
-                            42 BINARY_SUBSCR
-                            52 STORE_FAST               7 (mon_width)
-               
-                64          54 LOAD_FAST                1 (monitor)
-                            56 LOAD_CONST               4 ('height')
-                            58 BINARY_SUBSCR
-                            68 STORE_FAST               8 (mon_height)
-               
-                66          70 LOAD_FAST                2 (client)
-                            72 LOAD_CONST               5 ('size')
-                            74 BINARY_SUBSCR
-                            84 LOAD_CONST               6 (0)
-                            86 BINARY_SUBSCR
-                            96 STORE_FAST               9 (client_width)
+                76          64 LOAD_FAST                0 (monitor)
+                            66 LOAD_CONST               3 ('y')
+                            68 BINARY_SUBSCR
+                            78 STORE_FAST               6 (mon_y)
                
-                67          98 LOAD_FAST                2 (client)
-                           100 LOAD_CONST               5 ('size')
-                           102 BINARY_SUBSCR
-                           112 LOAD_CONST               7 (1)
-                           114 BINARY_SUBSCR
-                           124 STORE_FAST              10 (client_height)
-               
-                68         126 LOAD_GLOBAL              1 (NULL + int)
-                           138 LOAD_FAST                8 (mon_height)
-                           140 LOAD_FAST               10 (client_height)
-                           142 BINARY_OP               10 (-)
-                           146 LOAD_CONST               8 (2)
-                           148 BINARY_OP               11 (/)
-                           152 PRECALL                  1
-                           156 CALL                     1
-                           166 LOAD_FAST                6 (mon_y)
-                           168 BINARY_OP                0 (+)
-                           172 STORE_FAST              11 (margin_y)
-               
-                69         174 LOAD_GLOBAL              3 (NULL + hyprctl)
-               
-                70         186 LOAD_CONST               9 ('movewindowpixel exact ')
-                           188 LOAD_FAST                7 (mon_width)
-                           190 LOAD_FAST                9 (client_width)
-                           192 BINARY_OP               10 (-)
-                           196 LOAD_FAST                4 (margin)
-                           198 BINARY_OP               10 (-)
-                           202 LOAD_FAST                5 (mon_x)
-                           204 BINARY_OP                0 (+)
-                           208 FORMAT_VALUE             0
-                           210 LOAD_CONST              10 (' ')
-                           212 LOAD_FAST               11 (margin_y)
-                           214 FORMAT_VALUE             0
-                           216 LOAD_CONST              11 (',')
-                           218 LOAD_FAST                3 (client_uid)
-                           220 FORMAT_VALUE             0
-                           222 BUILD_STRING             6
+                77          80 LOAD_GLOBAL              3 (NULL + int)
+                            92 LOAD_FAST                0 (monitor)
+                            94 LOAD_CONST               4 ('width')
+                            96 BINARY_SUBSCR
+                           106 LOAD_FAST                4 (scale)
+                           108 BINARY_OP               11 (/)
+                           112 PRECALL                  1
+                           116 CALL                     1
+                           126 STORE_FAST               7 (mon_width)
                
-                69         224 PRECALL                  1
-                           228 CALL                     1
-                           238 GET_AWAITABLE            0
-                           240 LOAD_CONST               0 (None)
-                       >>  242 SEND                     3 (to 250)
-                           244 YIELD_VALUE
-                           246 RESUME                   3
-                           248 JUMP_BACKWARD_NO_INTERRUPT     4 (to 242)
-                       >>  250 POP_TOP
-                           252 LOAD_CONST               0 (None)
-                           254 RETURN_VALUE
+                78         128 LOAD_GLOBAL              3 (NULL + int)
+                           140 LOAD_FAST                0 (monitor)
+                           142 LOAD_CONST               5 ('height')
+                           144 BINARY_SUBSCR
+                           154 LOAD_FAST                4 (scale)
+                           156 BINARY_OP               11 (/)
+                           160 PRECALL                  1
+                           164 CALL                     1
+                           174 STORE_FAST               8 (mon_height)
+               
+                80         176 LOAD_FAST                1 (client)
+                           178 LOAD_CONST               6 ('size')
+                           180 BINARY_SUBSCR
+                           190 LOAD_CONST               7 (0)
+                           192 BINARY_SUBSCR
+                           202 STORE_FAST               9 (client_width)
+               
+                81         204 LOAD_FAST                1 (client)
+                           206 LOAD_CONST               6 ('size')
+                           208 BINARY_SUBSCR
+                           218 LOAD_CONST               8 (1)
+                           220 BINARY_SUBSCR
+                           230 STORE_FAST              10 (client_height)
+               
+                82         232 LOAD_GLOBAL              3 (NULL + int)
+                           244 LOAD_FAST                8 (mon_height)
+                           246 LOAD_FAST               10 (client_height)
+                           248 BINARY_OP               10 (-)
+                           252 LOAD_CONST               9 (2)
+                           254 BINARY_OP               11 (/)
+                           258 PRECALL                  1
+                           262 CALL                     1
+                           272 LOAD_FAST                6 (mon_y)
+                           274 BINARY_OP                0 (+)
+                           278 STORE_FAST              11 (margin_y)
+               
+                83         280 LOAD_GLOBAL              5 (NULL + hyprctl)
+               
+                84         292 LOAD_CONST              10 ('movewindowpixel exact ')
+                           294 LOAD_FAST                7 (mon_width)
+                           296 LOAD_FAST                9 (client_width)
+                           298 BINARY_OP               10 (-)
+                           302 LOAD_FAST                3 (margin)
+                           304 BINARY_OP               10 (-)
+                           308 LOAD_FAST                5 (mon_x)
+                           310 BINARY_OP                0 (+)
+                           314 FORMAT_VALUE             0
+                           316 LOAD_CONST              11 (' ')
+                           318 LOAD_FAST               11 (margin_y)
+                           320 FORMAT_VALUE             0
+                           322 LOAD_CONST              12 (',')
+                           324 LOAD_FAST                2 (client_uid)
+                           326 FORMAT_VALUE             0
+                           328 BUILD_STRING             6
+               
+                83         330 PRECALL                  1
+                           334 CALL                     1
+                           344 GET_AWAITABLE            0
+                           346 LOAD_CONST              13 (None)
+                       >>  348 SEND                     3 (to 356)
+                           350 YIELD_VALUE
+                           352 RESUME                   3
+                           354 JUMP_BACKWARD_NO_INTERRUPT     4 (to 348)
+                       >>  356 POP_TOP
+                           358 LOAD_CONST              13 (None)
+                           360 RETURN_VALUE
                consts
-                  None
+                  'Slide from/to right'
+                  'scale'
                   'x'
                   'y'
                   'width'
                   'height'
                   'size'
                   0
                   1
                   2
                   'movewindowpixel exact '
                   ' '
                   ','
-               names      ('int', 'hyprctl')
-               varnames   ('cls', 'monitor', 'client', 'client_uid', 'margin', 'mon_x', 'mon_y', 'mon_width', 'mon_height', 'client_width', 'client_height', 'margin_y')
+                  None
+               names      ('float', 'int', 'hyprctl')
+               varnames   ('monitor', 'client', 'client_uid', 'margin', 'scale', 'mon_x', 'mon_y', 'mon_width', 'mon_height', 'client_width', 'client_height', 'margin_y')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'fromright'
-               firstlineno 59
-               lnotab 0x060210011001100110021c011c0130010c0126ff
+               firstlineno 71
+               lnotab 0x06032a0110011001300130021c011c0130010c0126ff
             None
-         names      ('__name__', '__module__', '__qualname__', 'classmethod', 'fromtop', 'frombottom', 'fromleft', 'fromright')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'staticmethod', 'fromtop', 'frombottom', 'fromleft', 'fromright')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
          name       'Animations'
-         firstlineno 23
+         firstlineno 26
          lnotab
-            0x0a01020104ff0e010209020104ff0e01020d020104ff0e01020a020104
-            ff0e01
+            0x0a010402020104ff0e01020c020104ff0e01020f020104ff0e01020c02
+            0104ff0e01
       'Animations'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
-            0x970065005a0164005a02640184005a03640265046602640384045a0564
-            046506640264056604640684045a07650864026509660264078404a60000
-            00ab0000000000000000005a0a6409640a640884055a0b64055300
-          74           0 RESUME                   0
+            0x970065005a0164005a0264015a03640284005a04640365056602640484
+            045a0664056507640364066604640784045a0865096403650a6602640884
+            04a6000000ab0000000000000000005a0b640b640c640984055a0c640a84
+            005a0d64065300
+          88           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Scratch')
                        8 STORE_NAME               2 (__qualname__)
          
-          75          10 LOAD_CONST               1 (<code object __init__, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 75>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (__init__)
-         
-          83          16 LOAD_CONST               2 ('return')
-                      18 LOAD_NAME                4 (bool)
-                      20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object isAlive, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 83>)
-                      24 MAKE_FUNCTION            4 (annotations)
-                      26 STORE_NAME               5 (isAlive)
-         
-          92          28 LOAD_CONST               4 ('pid')
-                      30 LOAD_NAME                6 (int)
-                      32 LOAD_CONST               2 ('return')
-                      34 LOAD_CONST               5 (None)
-                      36 BUILD_TUPLE              4
-                      38 LOAD_CONST               6 (<code object reset, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 92>)
-                      40 MAKE_FUNCTION            4 (annotations)
-                      42 STORE_NAME               7 (reset)
-         
-          98          44 LOAD_NAME                8 (property)
-         
-          99          46 LOAD_CONST               2 ('return')
-                      48 LOAD_NAME                9 (str)
-                      50 BUILD_TUPLE              2
-                      52 LOAD_CONST               7 (<code object address, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 98>)
-                      54 MAKE_FUNCTION            4 (annotations)
-         
-          98          56 PRECALL                  0
-                      60 CALL                     0
-         
-          99          70 STORE_NAME              10 (address)
-         
-         102          72 LOAD_CONST               9 ((None,))
-                      74 LOAD_CONST              10 (('return', None))
-                      76 LOAD_CONST               8 (<code object updateClientInfo, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 102>)
-                      78 MAKE_FUNCTION            5 (defaults, annotations)
-                      80 STORE_NAME              11 (updateClientInfo)
-                      82 LOAD_CONST               5 (None)
-                      84 RETURN_VALUE
+          89          10 LOAD_CONST               1 ('A scratchpad state including configuration & client state')
+                      12 STORE_NAME               3 (__doc__)
+         
+          91          14 LOAD_CONST               2 (<code object __init__, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 91>)
+                      16 MAKE_FUNCTION            0
+                      18 STORE_NAME               4 (__init__)
+         
+          99          20 LOAD_CONST               3 ('return')
+                      22 LOAD_NAME                5 (bool)
+                      24 BUILD_TUPLE              2
+                      26 LOAD_CONST               4 (<code object isAlive, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 99>)
+                      28 MAKE_FUNCTION            4 (annotations)
+                      30 STORE_NAME               6 (isAlive)
+         
+         110          32 LOAD_CONST               5 ('pid')
+                      34 LOAD_NAME                7 (int)
+                      36 LOAD_CONST               3 ('return')
+                      38 LOAD_CONST               6 (None)
+                      40 BUILD_TUPLE              4
+                      42 LOAD_CONST               7 (<code object reset, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 110>)
+                      44 MAKE_FUNCTION            4 (annotations)
+                      46 STORE_NAME               8 (reset)
+         
+         117          48 LOAD_NAME                9 (property)
+         
+         118          50 LOAD_CONST               3 ('return')
+                      52 LOAD_NAME               10 (str)
+                      54 BUILD_TUPLE              2
+                      56 LOAD_CONST               8 (<code object address, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 117>)
+                      58 MAKE_FUNCTION            4 (annotations)
+         
+         117          60 PRECALL                  0
+                      64 CALL                     0
+         
+         118          74 STORE_NAME              11 (address)
+         
+         122          76 LOAD_CONST              11 ((None,))
+                      78 LOAD_CONST              12 (('return', None))
+                      80 LOAD_CONST               9 (<code object updateClientInfo, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 122>)
+                      82 MAKE_FUNCTION            5 (defaults, annotations)
+                      84 STORE_NAME              12 (updateClientInfo)
+         
+         129          86 LOAD_CONST              10 (<code object __str__, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 129>)
+                      88 MAKE_FUNCTION            0
+                      90 STORE_NAME              13 (__str__)
+                      92 LOAD_CONST               6 (None)
+                      94 RETURN_VALUE
          consts
             'Scratch'
+            'A scratchpad state including configuration & client state'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f00000000000000000064017c005f0100000000000000
                   007c027c005f02000000000000000064027c005f03000000000000000064
                   037c005f04000000000000000069007c005f050000000000000000640053
                   00
-                75           0 RESUME                   0
+                91           0 RESUME                   0
                
-                76           2 LOAD_FAST                1 (uid)
+                92           2 LOAD_FAST                1 (uid)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (uid)
                
-                77          16 LOAD_CONST               1 (0)
+                93          16 LOAD_CONST               1 (0)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (pid)
                
-                78          30 LOAD_FAST                2 (opts)
+                94          30 LOAD_FAST                2 (opts)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (conf)
                
-                79          44 LOAD_CONST               2 (False)
+                95          44 LOAD_CONST               2 (False)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (visible)
                
-                80          58 LOAD_CONST               3 (True)
+                96          58 LOAD_CONST               3 (True)
                             60 LOAD_FAST                0 (self)
                             62 STORE_ATTR               4 (just_created)
                
-                81          72 BUILD_MAP                0
+                97          72 BUILD_MAP                0
                             74 LOAD_FAST                0 (self)
-                            76 STORE_ATTR               5 (clientInfo)
+                            76 STORE_ATTR               5 (client_info)
                             86 LOAD_CONST               0 (None)
                             88 RETURN_VALUE
                consts
                   None
                   0
                   False
                   True
-               names      ('uid', 'pid', 'conf', 'visible', 'just_created', 'clientInfo')
+               names      ('uid', 'pid', 'conf', 'visible', 'just_created', 'client_info')
                varnames   ('self', 'uid', 'opts')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '__init__'
-               firstlineno 75
+               firstlineno 91
                lnotab 0x02010e010e010e010e010e01
             'return'
             code
                argcount  : 1
-               nlocals   : 4
+               nlocals   : 5
                stacksize : 6
                flags     : 3
                code
                   0x970064017c006a0000000000000000009b009d027d0174020000000000
                   00000000006a020000000000000000a00300000000000000000000000000
-                  000000000000007c01a6010000ab01000000000000000072787409000000
+                  000000000000007c01a6010000ab01000000000000000072a17409000000
                   000000000000007402000000000000000000006a020000000000000000a0
                   0500000000000000000000000000000000000000007c016402a6020000ab
-                  0200000000000000006403a6020000ab020000000000000000a006000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  0044005d377d027c02a00700000000000000000000000000000000000000
-                  006404a6010000ab01000000000000000072207c02a00800000000000000
-                  00000000000000000000000000a6000000ab000000000000000000640519
-                  0000000000000000007d037c03640676006302010053008c3864075300
-                83           0 RESUME                   0
+                  02000000000000000064036404ac05a6030000ab03000000000000000035
+                  007d027c02a0060000000000000000000000000000000000000000a60000
+                  00ab00000000000000000044005d437d037c03a007000000000000000000
+                  00000000000000000000006406a6010000ab010000000000000000722c7c
+                  03a0080000000000000000000000000000000000000000a6000000ab0000
+                  000000000000006407190000000000000000007d047c0464087600630201
+                  006302640964096409a6020000ab020000000000000000010053008c4409
+                  00640964096409a6020000ab02000000000000000001006e0b2300310073
+                  0477027803590077010100590001000100640a5300
+                99           0 RESUME                   0
                
-                84           2 LOAD_CONST               1 ('/proc/')
+               101           2 LOAD_CONST               1 ('/proc/')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (pid)
                             16 FORMAT_VALUE             0
                             18 BUILD_STRING             2
                             20 STORE_FAST               1 (path)
                
-                85          22 LOAD_GLOBAL              2 (os)
+               102          22 LOAD_GLOBAL              2 (os)
                             34 LOAD_ATTR                2 (path)
                             44 LOAD_METHOD              3 (exists)
                             66 LOAD_FAST                1 (path)
                             68 PRECALL                  1
                             72 CALL                     1
-                            82 POP_JUMP_FORWARD_IF_FALSE   120 (to 324)
+                            82 POP_JUMP_FORWARD_IF_FALSE   161 (to 406)
                
-                86          84 LOAD_GLOBAL              9 (NULL + open)
+               103          84 LOAD_GLOBAL              9 (NULL + open)
                             96 LOAD_GLOBAL              2 (os)
                            108 LOAD_ATTR                2 (path)
                            118 LOAD_METHOD              5 (join)
                            140 LOAD_FAST                1 (path)
                            142 LOAD_CONST               2 ('status')
                            144 PRECALL                  2
                            148 CALL                     2
                            158 LOAD_CONST               3 ('r')
-                           160 PRECALL                  2
-                           164 CALL                     2
-                           174 LOAD_METHOD              6 (readlines)
-                           196 PRECALL                  0
-                           200 CALL                     0
-                           210 GET_ITER
-                       >>  212 FOR_ITER                55 (to 324)
-                           214 STORE_FAST               2 (line)
-               
-                87         216 LOAD_FAST                2 (line)
-                           218 LOAD_METHOD              7 (startswith)
-                           240 LOAD_CONST               4 ('State')
-                           242 PRECALL                  1
-                           246 CALL                     1
-                           256 POP_JUMP_FORWARD_IF_FALSE    32 (to 322)
-               
-                88         258 LOAD_FAST                2 (line)
-                           260 LOAD_METHOD              8 (split)
-                           282 PRECALL                  0
-                           286 CALL                     0
-                           296 LOAD_CONST               5 (1)
-                           298 BINARY_SUBSCR
-                           308 STORE_FAST               3 (state)
-               
-                89         310 LOAD_FAST                3 (state)
-                           312 LOAD_CONST               6 ('RSDTt')
-                           314 CONTAINS_OP              0
-                           316 SWAP                     2
-                           318 POP_TOP
-                           320 RETURN_VALUE
-               
-                87     >>  322 JUMP_BACKWARD           56 (to 212)
-               
-                90     >>  324 LOAD_CONST               7 (False)
-                           326 RETURN_VALUE
+                           160 LOAD_CONST               4 ('utf-8')
+                           162 KW_NAMES                 5
+                           164 PRECALL                  3
+                           168 CALL                     3
+                           178 BEFORE_WITH
+                           180 STORE_FAST               2 (f)
+               
+               104         182 LOAD_FAST                2 (f)
+                           184 LOAD_METHOD              6 (readlines)
+                           206 PRECALL                  0
+                           210 CALL                     0
+                           220 GET_ITER
+                       >>  222 FOR_ITER                67 (to 358)
+                           224 STORE_FAST               3 (line)
+               
+               105         226 LOAD_FAST                3 (line)
+                           228 LOAD_METHOD              7 (startswith)
+                           250 LOAD_CONST               6 ('State')
+                           252 PRECALL                  1
+                           256 CALL                     1
+                           266 POP_JUMP_FORWARD_IF_FALSE    44 (to 356)
+               
+               106         268 LOAD_FAST                3 (line)
+                           270 LOAD_METHOD              8 (split)
+                           292 PRECALL                  0
+                           296 CALL                     0
+                           306 LOAD_CONST               7 (1)
+                           308 BINARY_SUBSCR
+                           318 STORE_FAST               4 (state)
+               
+               107         320 LOAD_FAST                4 (state)
+                           322 LOAD_CONST               8 ('RSDTt')
+                           324 CONTAINS_OP              0
+                           326 SWAP                     2
+                           328 POP_TOP
+               
+               103         330 SWAP                     2
+                           332 LOAD_CONST               9 (None)
+                           334 LOAD_CONST               9 (None)
+                           336 LOAD_CONST               9 (None)
+                           338 PRECALL                  2
+                           342 CALL                     2
+                           352 POP_TOP
+                           354 RETURN_VALUE
+               
+               105     >>  356 JUMP_BACKWARD           68 (to 222)
+               
+               104     >>  358 NOP
+               
+               103         360 LOAD_CONST               9 (None)
+                           362 LOAD_CONST               9 (None)
+                           364 LOAD_CONST               9 (None)
+                           366 PRECALL                  2
+                           370 CALL                     2
+                           380 POP_TOP
+                           382 JUMP_FORWARD            11 (to 406)
+                       >>  384 PUSH_EXC_INFO
+                           386 WITH_EXCEPT_START
+                           388 POP_JUMP_FORWARD_IF_TRUE     4 (to 398)
+                           390 RERAISE                  2
+                       >>  392 COPY                     3
+                           394 POP_EXCEPT
+                           396 RERAISE                  1
+                       >>  398 POP_TOP
+                           400 POP_EXCEPT
+                           402 POP_TOP
+                           404 POP_TOP
+               
+               108     >>  406 LOAD_CONST              10 (False)
+                           408 RETURN_VALUE
+               ExceptionTable:
+                 180 to 328 -> 384 [1] lasti
+                 356 to 356 -> 384 [1] lasti
+                 384 to 390 -> 392 [3] lasti
+                 398 to 398 -> 392 [3] lasti
                consts
-                  None
+                  'is the process running ?'
                   '/proc/'
                   'status'
                   'r'
+                  'utf-8'
+                  ('encoding',)
                   'State'
                   1
                   'RSDTt'
+                  None
                   False
                names      ('pid', 'os', 'path', 'exists', 'open', 'join', 'readlines', 'startswith', 'split')
-               varnames   ('self', 'path', 'line', 'state')
+               varnames   ('self', 'path', 'f', 'line', 'state')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'isAlive'
-               firstlineno 83
-               lnotab 0x020114013e0184012a0134010cfe0203
+               firstlineno 99
+               lnotab 0x020214013e0162012c012a0134010afc1a0202ff02ff2e05
             'pid'
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f00000000000000000064017c005f0100000000000000
                   0064027c005f02000000000000000069007c005f03000000000000000064
-                  005300
-                92           0 RESUME                   0
+                  035300
+               110           0 RESUME                   0
                
-                93           2 LOAD_FAST                1 (pid)
+               112           2 LOAD_FAST                1 (pid)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (pid)
                
-                94          16 LOAD_CONST               1 (False)
+               113          16 LOAD_CONST               1 (False)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (visible)
                
-                95          30 LOAD_CONST               2 (True)
+               114          30 LOAD_CONST               2 (True)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (just_created)
                
-                96          44 BUILD_MAP                0
+               115          44 BUILD_MAP                0
                             46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               3 (clientInfo)
-                            58 LOAD_CONST               0 (None)
+                            48 STORE_ATTR               3 (client_info)
+                            58 LOAD_CONST               3 (None)
                             60 RETURN_VALUE
                consts
-                  None
+                  'clear the object'
                   False
                   True
-               names      ('pid', 'visible', 'just_created', 'clientInfo')
+                  None
+               names      ('pid', 'visible', 'just_created', 'client_info')
                varnames   ('self', 'pid')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'reset'
-               firstlineno 92
-               lnotab 0x02010e010e010e01
+               firstlineno 110
+               lnotab 0x02020e010e010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a00200
                   0000000000000000000000000000000000000064016402a6020000ab0200
-                  00000000000000a6010000ab010000000000000000640364008502190000
+                  00000000000000a6010000ab010000000000000000640364048502190000
                   000000000000005300
-                98           0 RESUME                   0
+               117           0 RESUME                   0
                
-               100           2 LOAD_GLOBAL              1 (NULL + str)
+               120           2 LOAD_GLOBAL              1 (NULL + str)
                             14 LOAD_FAST                0 (self)
-                            16 LOAD_ATTR                1 (clientInfo)
+                            16 LOAD_ATTR                1 (client_info)
                             26 LOAD_METHOD              2 (get)
                             48 LOAD_CONST               1 ('address')
                             50 LOAD_CONST               2 ('')
                             52 PRECALL                  2
                             56 CALL                     2
                             66 PRECALL                  1
                             70 CALL                     1
                             80 LOAD_CONST               3 (2)
-                            82 LOAD_CONST               0 (None)
+                            82 LOAD_CONST               4 (None)
                             84 BUILD_SLICE              2
                             86 BINARY_SUBSCR
                             96 RETURN_VALUE
                consts
-                  None
+                  'Returns the client address'
                   'address'
                   ''
                   2
-               names      ('str', 'clientInfo', 'get')
+                  None
+               names      ('str', 'client_info', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'address'
-               firstlineno 98
-               lnotab 0x0202
+               firstlineno 117
+               lnotab 0x0203
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 131
                code
-                  0x4b00010097007c01801d74010000000000000000000064017c006a0100
-                  000000000000007a000000a6010000ab010000000000000000830064007b
+                  0x4b00010097007c01801d74010000000000000000000064027c006a0100
+                  000000000000007a000000a6010000ab010000000000000000830064017b
                   035600970386047d017405000000000000000000007c0174060000000000
                   0000000000a6020000ab02000000000000000073024a0082017c006a0400
                   00000000000000a00500000000000000000000000000000000000000007c
-                  01a6010000ab010000000000000000010064005300
-               102           0 RETURN_GENERATOR
+                  01a6010000ab010000000000000000010064015300
+               122           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               103           6 LOAD_FAST                1 (clientInfo)
+               124           6 LOAD_FAST                1 (client_info)
                              8 POP_JUMP_FORWARD_IF_NOT_NONE    29 (to 68)
                
-               104          10 LOAD_GLOBAL              1 (NULL + get_client_props_by_address)
-                            22 LOAD_CONST               1 ('0x')
+               125          10 LOAD_GLOBAL              1 (NULL + get_client_props_by_address)
+                            22 LOAD_CONST               2 ('0x')
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                1 (address)
                             36 BINARY_OP                0 (+)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 GET_AWAITABLE            0
-                            56 LOAD_CONST               0 (None)
+                            56 LOAD_CONST               1 (None)
                        >>   58 SEND                     3 (to 66)
                             60 YIELD_VALUE
                             62 RESUME                   3
                             64 JUMP_BACKWARD_NO_INTERRUPT     4 (to 58)
-                       >>   66 STORE_FAST               1 (clientInfo)
+                       >>   66 STORE_FAST               1 (client_info)
                
-               105     >>   68 LOAD_GLOBAL              5 (NULL + isinstance)
-                            80 LOAD_FAST                1 (clientInfo)
+               126     >>   68 LOAD_GLOBAL              5 (NULL + isinstance)
+                            80 LOAD_FAST                1 (client_info)
                             82 LOAD_GLOBAL              6 (dict)
                             94 PRECALL                  2
                             98 CALL                     2
                            108 POP_JUMP_FORWARD_IF_TRUE     2 (to 114)
                            110 LOAD_ASSERTION_ERROR
                            112 RAISE_VARARGS            1
                
-               106     >>  114 LOAD_FAST                0 (self)
-                           116 LOAD_ATTR                4 (clientInfo)
+               127     >>  114 LOAD_FAST                0 (self)
+                           116 LOAD_ATTR                4 (client_info)
                            126 LOAD_METHOD              5 (update)
-                           148 LOAD_FAST                1 (clientInfo)
+                           148 LOAD_FAST                1 (client_info)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 POP_TOP
-                           166 LOAD_CONST               0 (None)
+                           166 LOAD_CONST               1 (None)
                            168 RETURN_VALUE
                consts
+                  'update the internal client info property, if not provided, refresh based on the current address'
                   None
                   '0x'
-               names      ('get_client_props_by_address', 'address', 'isinstance', 'dict', 'clientInfo', 'update')
-               varnames   ('self', 'clientInfo')
+               names      ('get_client_props_by_address', 'address', 'isinstance', 'dict', 'client_info', 'update')
+               varnames   ('self', 'client_info')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'updateClientInfo'
-               firstlineno 102
-               lnotab 0x060104013a012e01
+               firstlineno 122
+               lnotab 0x060204013a012e01
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 7
+               flags     : 3
+               code
+                  0x97007c006a0000000000000000009b0064017c006a0100000000000000
+                  009b0064027c006a0200000000000000009b0064037c006a030000000000
+                  0000009b009d075300
+               129           0 RESUME                   0
+               
+               130           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (uid)
+                            14 FORMAT_VALUE             0
+                            16 LOAD_CONST               1 (' ')
+                            18 LOAD_FAST                0 (self)
+                            20 LOAD_ATTR                1 (address)
+                            30 FORMAT_VALUE             0
+                            32 LOAD_CONST               2 (' : ')
+                            34 LOAD_FAST                0 (self)
+                            36 LOAD_ATTR                2 (client_info)
+                            46 FORMAT_VALUE             0
+                            48 LOAD_CONST               3 (' / ')
+                            50 LOAD_FAST                0 (self)
+                            52 LOAD_ATTR                3 (conf)
+                            62 FORMAT_VALUE             0
+                            64 BUILD_STRING             7
+                            66 RETURN_VALUE
+               consts
+                  None
+                  ' '
+                  ' : '
+                  ' / '
+               names      ('uid', 'address', 'client_info', 'conf')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
+               name       '__str__'
+               firstlineno 129
+               lnotab 0x0201
             (None,)
             ('return', None)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'bool', 'isAlive', 'int', 'reset', 'property', 'str', 'address', 'updateClientInfo')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'bool', 'isAlive', 'int', 'reset', 'property', 'str', 'address', 'updateClientInfo', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
          name       'Scratch'
-         firstlineno 74
-         lnotab 0x0a0106080c09100602010aff0e010203
+         firstlineno 88
+         lnotab 0x0a01040206080c0b100702010aff0e0102040a07
       'Scratch'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
-            0x970065005a0164005a026411640384045a036411640484045a04641164
-            0584045a0564066506640164026604640784045a076411640884045a0864
-            11640984045a09640a6506640164026604640b84045a0a6412640c650b64
-            027a070000640164026604640d84055a0c6413640a650664016402660464
-            0f84055a0d64146411641084055a0e64025300
-         109           0 RESUME                   0
+            0x970065005a0164005a02550069005a036504650565066a070000000000
+            000000660219000000000000000000650864013c00000069005a09650465
+            05650a660219000000000000000000650864023c0000000200650ba60000
+            00ab0000000000000000005a0c650b650519000000000000000000650864
+            033c0000000200650ba6000000ab0000000000000000005a0d650b650519
+            000000000000000000650864043c0000000200650ba6000000ab00000000
+            00000000005a0e650b650519000000000000000000650864053c00000069
+            005a0f65046505650a660219000000000000000000650864063c00000069
+            005a1065046511650a660219000000000000000000650864073c00000069
+            005a12650465056504660219000000000000000000650864083c00000064
+            1b640b84045a13640c650465056514660219000000000000000000640964
+            0a6604640d84045a15641c640f65056409640a6604641084055a16641b64
+            1184045a17641284005a18641b641384045a19641465056409640a660464
+            1584045a1a641684005a1b641d6417650a640a7a0700006409640a660464
+            1884055a1c641e641465056409640a6604641984055a1d641c641b641a84
+            055a1e640a5300
+         133           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Extension')
                        8 STORE_NAME               2 (__qualname__)
+                      10 SETUP_ANNOTATIONS
          
-         110          10 LOAD_CONST              17 (('return', None))
-                      12 LOAD_CONST               3 (<code object init, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 110>)
-                      14 MAKE_FUNCTION            4 (annotations)
-                      16 STORE_NAME               3 (init)
-         
-         119          18 LOAD_CONST              17 (('return', None))
-                      20 LOAD_CONST               4 (<code object exit, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 119>)
-                      22 MAKE_FUNCTION            4 (annotations)
-                      24 STORE_NAME               4 (exit)
-         
-         135          26 LOAD_CONST              17 (('return', None))
-                      28 LOAD_CONST               5 (<code object load_config, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 135>)
-                      30 MAKE_FUNCTION            4 (annotations)
-                      32 STORE_NAME               5 (load_config)
-         
-         152          34 LOAD_CONST               6 ('name')
-                      36 LOAD_NAME                6 (str)
-                      38 LOAD_CONST               1 ('return')
-                      40 LOAD_CONST               2 (None)
-                      42 BUILD_TUPLE              4
-                      44 LOAD_CONST               7 (<code object start_scratch_command, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 152>)
-                      46 MAKE_FUNCTION            4 (annotations)
-                      48 STORE_NAME               7 (start_scratch_command)
-         
-         170          50 LOAD_CONST              17 (('return', None))
-                      52 LOAD_CONST               8 (<code object event_activewindowv2, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 170>)
-                      54 MAKE_FUNCTION            4 (annotations)
-                      56 STORE_NAME               8 (event_activewindowv2)
-         
-         187          58 LOAD_CONST              17 (('return', None))
-                      60 LOAD_CONST               9 (<code object event_openwindow, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 187>)
-                      62 MAKE_FUNCTION            4 (annotations)
-                      64 STORE_NAME               9 (event_openwindow)
-         
-         199          66 LOAD_CONST              10 ('uid')
-                      68 LOAD_NAME                6 (str)
-                      70 LOAD_CONST               1 ('return')
-                      72 LOAD_CONST               2 (None)
-                      74 BUILD_TUPLE              4
-                      76 LOAD_CONST              11 (<code object run_toggle, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 199>)
-                      78 MAKE_FUNCTION            4 (annotations)
-                      80 STORE_NAME              10 (run_toggle)
-         
-         211          82 LOAD_CONST              18 ((None,))
-                      84 LOAD_CONST              12 ('scratch')
-                      86 LOAD_NAME               11 (Scratch)
-                      88 LOAD_CONST               2 (None)
-                      90 BINARY_OP                7 (|)
-                      94 LOAD_CONST               1 ('return')
-                      96 LOAD_CONST               2 (None)
-                      98 BUILD_TUPLE              4
-                     100 LOAD_CONST              13 (<code object updateScratchInfo, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 211>)
-                     102 MAKE_FUNCTION            5 (defaults, annotations)
-                     104 STORE_NAME              12 (updateScratchInfo)
-         
-         230         106 LOAD_CONST              19 ((False, False))
-                     108 LOAD_CONST              10 ('uid')
-                     110 LOAD_NAME                6 (str)
-                     112 LOAD_CONST               1 ('return')
-                     114 LOAD_CONST               2 (None)
-                     116 BUILD_TUPLE              4
-                     118 LOAD_CONST              15 (<code object run_hide, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 230>)
-                     120 MAKE_FUNCTION            5 (defaults, annotations)
-                     122 STORE_NAME              13 (run_hide)
-         
-         276         124 LOAD_CONST              20 ((False,))
-                     126 LOAD_CONST              17 (('return', None))
-                     128 LOAD_CONST              16 (<code object run_show, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 276>)
-                     130 MAKE_FUNCTION            5 (defaults, annotations)
-                     132 STORE_NAME              14 (run_show)
-                     134 LOAD_CONST               2 (None)
-                     136 RETURN_VALUE
+         134          12 BUILD_MAP                0
+                      14 STORE_NAME               3 (procs)
+                      16 LOAD_NAME                4 (dict)
+                      18 LOAD_NAME                5 (str)
+                      20 LOAD_NAME                6 (subprocess)
+                      22 LOAD_ATTR                7 (Popen)
+                      32 BUILD_TUPLE              2
+                      34 BINARY_SUBSCR
+                      44 LOAD_NAME                8 (__annotations__)
+                      46 LOAD_CONST               1 ('procs')
+                      48 STORE_SUBSCR
+         
+         135          52 BUILD_MAP                0
+                      54 STORE_NAME               9 (scratches)
+                      56 LOAD_NAME                4 (dict)
+                      58 LOAD_NAME                5 (str)
+                      60 LOAD_NAME               10 (Scratch)
+                      62 BUILD_TUPLE              2
+                      64 BINARY_SUBSCR
+                      74 LOAD_NAME                8 (__annotations__)
+                      76 LOAD_CONST               2 ('scratches')
+                      78 STORE_SUBSCR
+         
+         136          82 PUSH_NULL
+                      84 LOAD_NAME               11 (set)
+                      86 PRECALL                  0
+                      90 CALL                     0
+                     100 STORE_NAME              12 (transitioning_scratches)
+                     102 LOAD_NAME               11 (set)
+                     104 LOAD_NAME                5 (str)
+                     106 BINARY_SUBSCR
+                     116 LOAD_NAME                8 (__annotations__)
+                     118 LOAD_CONST               3 ('transitioning_scratches')
+                     120 STORE_SUBSCR
+         
+         137         124 PUSH_NULL
+                     126 LOAD_NAME               11 (set)
+                     128 PRECALL                  0
+                     132 CALL                     0
+                     142 STORE_NAME              13 (_new_scratches)
+                     144 LOAD_NAME               11 (set)
+                     146 LOAD_NAME                5 (str)
+                     148 BINARY_SUBSCR
+                     158 LOAD_NAME                8 (__annotations__)
+                     160 LOAD_CONST               4 ('_new_scratches')
+                     162 STORE_SUBSCR
+         
+         138         166 PUSH_NULL
+                     168 LOAD_NAME               11 (set)
+                     170 PRECALL                  0
+                     174 CALL                     0
+                     184 STORE_NAME              14 (_respawned_scratches)
+                     186 LOAD_NAME               11 (set)
+                     188 LOAD_NAME                5 (str)
+                     190 BINARY_SUBSCR
+                     200 LOAD_NAME                8 (__annotations__)
+                     202 LOAD_CONST               5 ('_respawned_scratches')
+                     204 STORE_SUBSCR
+         
+         139         208 BUILD_MAP                0
+                     210 STORE_NAME              15 (scratches_by_address)
+                     212 LOAD_NAME                4 (dict)
+                     214 LOAD_NAME                5 (str)
+                     216 LOAD_NAME               10 (Scratch)
+                     218 BUILD_TUPLE              2
+                     220 BINARY_SUBSCR
+                     230 LOAD_NAME                8 (__annotations__)
+                     232 LOAD_CONST               6 ('scratches_by_address')
+                     234 STORE_SUBSCR
+         
+         140         238 BUILD_MAP                0
+                     240 STORE_NAME              16 (scratches_by_pid)
+                     242 LOAD_NAME                4 (dict)
+                     244 LOAD_NAME               17 (int)
+                     246 LOAD_NAME               10 (Scratch)
+                     248 BUILD_TUPLE              2
+                     250 BINARY_SUBSCR
+                     260 LOAD_NAME                8 (__annotations__)
+                     262 LOAD_CONST               7 ('scratches_by_pid')
+                     264 STORE_SUBSCR
+         
+         141         268 BUILD_MAP                0
+                     270 STORE_NAME              18 (focused_window_tracking)
+                     272 LOAD_NAME                4 (dict)
+                     274 LOAD_NAME                5 (str)
+                     276 LOAD_NAME                4 (dict)
+                     278 BUILD_TUPLE              2
+                     280 BINARY_SUBSCR
+                     290 LOAD_NAME                8 (__annotations__)
+                     292 LOAD_CONST               8 ('focused_window_tracking')
+                     294 STORE_SUBSCR
+         
+         143         298 LOAD_CONST              27 (('return', None))
+                     300 LOAD_CONST              11 (<code object exit, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 143>)
+                     302 MAKE_FUNCTION            4 (annotations)
+                     304 STORE_NAME              19 (exit)
+         
+         161         306 LOAD_CONST              12 ('config')
+                     308 LOAD_NAME                4 (dict)
+                     310 LOAD_NAME                5 (str)
+                     312 LOAD_NAME               20 (Any)
+                     314 BUILD_TUPLE              2
+                     316 BINARY_SUBSCR
+                     326 LOAD_CONST               9 ('return')
+                     328 LOAD_CONST              10 (None)
+                     330 BUILD_TUPLE              4
+                     332 LOAD_CONST              13 (<code object load_config, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 161>)
+                     334 MAKE_FUNCTION            4 (annotations)
+                     336 STORE_NAME              21 (load_config)
+         
+         180         338 LOAD_CONST              28 ((False,))
+                     340 LOAD_CONST              15 ('name')
+                     342 LOAD_NAME                5 (str)
+                     344 LOAD_CONST               9 ('return')
+                     346 LOAD_CONST              10 (None)
+                     348 BUILD_TUPLE              4
+                     350 LOAD_CONST              16 (<code object start_scratch_command, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 180>)
+                     352 MAKE_FUNCTION            5 (defaults, annotations)
+                     354 STORE_NAME              22 (start_scratch_command)
+         
+         203         356 LOAD_CONST              27 (('return', None))
+                     358 LOAD_CONST              17 (<code object event_activewindowv2, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 203>)
+                     360 MAKE_FUNCTION            4 (annotations)
+                     362 STORE_NAME              23 (event_activewindowv2)
+         
+         223         364 LOAD_CONST              18 (<code object _alternative_lookup, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 223>)
+                     366 MAKE_FUNCTION            0
+                     368 STORE_NAME              24 (_alternative_lookup)
+         
+         242         370 LOAD_CONST              27 (('return', None))
+                     372 LOAD_CONST              19 (<code object event_openwindow, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 242>)
+                     374 MAKE_FUNCTION            4 (annotations)
+                     376 STORE_NAME              25 (event_openwindow)
+         
+         259         378 LOAD_CONST              20 ('uid')
+                     380 LOAD_NAME                5 (str)
+                     382 LOAD_CONST               9 ('return')
+                     384 LOAD_CONST              10 (None)
+                     386 BUILD_TUPLE              4
+                     388 LOAD_CONST              21 (<code object run_toggle, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 259>)
+                     390 MAKE_FUNCTION            4 (annotations)
+                     392 STORE_NAME              26 (run_toggle)
+         
+         272         394 LOAD_CONST              22 (<code object _anim_hide, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 272>)
+                     396 MAKE_FUNCTION            0
+                     398 STORE_NAME              27 (_anim_hide)
+         
+         295         400 LOAD_CONST              29 ((None,))
+                     402 LOAD_CONST              23 ('scratch')
+                     404 LOAD_NAME               10 (Scratch)
+                     406 LOAD_CONST              10 (None)
+                     408 BINARY_OP                7 (|)
+                     412 LOAD_CONST               9 ('return')
+                     414 LOAD_CONST              10 (None)
+                     416 BUILD_TUPLE              4
+                     418 LOAD_CONST              24 (<code object updateScratchInfo, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 295>)
+                     420 MAKE_FUNCTION            5 (defaults, annotations)
+                     422 STORE_NAME              28 (updateScratchInfo)
+         
+         316         424 LOAD_CONST              30 ((False, False))
+                     426 LOAD_CONST              20 ('uid')
+                     428 LOAD_NAME                5 (str)
+                     430 LOAD_CONST               9 ('return')
+                     432 LOAD_CONST              10 (None)
+                     434 BUILD_TUPLE              4
+                     436 LOAD_CONST              25 (<code object run_hide, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 316>)
+                     438 MAKE_FUNCTION            5 (defaults, annotations)
+                     440 STORE_NAME              29 (run_hide)
+         
+         345         442 LOAD_CONST              28 ((False,))
+                     444 LOAD_CONST              27 (('return', None))
+                     446 LOAD_CONST              26 (<code object run_show, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 345>)
+                     448 MAKE_FUNCTION            5 (defaults, annotations)
+                     450 STORE_NAME              30 (run_show)
+                     452 LOAD_CONST              10 (None)
+                     454 RETURN_VALUE
          consts
             'Extension'
+            'procs'
+            'scratches'
+            'transitioning_scratches'
+            '_new_scratches'
+            '_respawned_scratches'
+            'scratches_by_address'
+            'scratches_by_pid'
+            'focused_window_tracking'
             'return'
             None
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 2
-               flags     : 131
-               code
-                  0x4b000100970069007c005f00000000000000000069007c005f01000000
-                  0000000000740500000000000000000000a6000000ab0000000000000000
-                  007c005f030000000000000000740500000000000000000000a6000000ab
-                  0000000000000000007c005f04000000000000000069007c005f05000000
-                  000000000069007c005f060000000000000000740f000000000000000000
-                  00a6000000ab0000000000000000007c005f080000000000000000640053
-                  00
-               110           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-               
-               111           6 BUILD_MAP                0
-                             8 LOAD_FAST                0 (self)
-                            10 STORE_ATTR               0 (procs)
-               
-               112          20 BUILD_MAP                0
-                            22 LOAD_FAST                0 (self)
-                            24 STORE_ATTR               1 (scratches)
-               
-               113          34 LOAD_GLOBAL              5 (NULL + set)
-                            46 PRECALL                  0
-                            50 CALL                     0
-                            60 LOAD_FAST                0 (self)
-                            62 STORE_ATTR               3 (transitioning_scratches)
-               
-               114          72 LOAD_GLOBAL              5 (NULL + set)
-                            84 PRECALL                  0
-                            88 CALL                     0
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               4 (_respawned_scratches)
-               
-               115         110 BUILD_MAP                0
-                           112 LOAD_FAST                0 (self)
-                           114 STORE_ATTR               5 (scratches_by_address)
-               
-               116         124 BUILD_MAP                0
-                           126 LOAD_FAST                0 (self)
-                           128 STORE_ATTR               6 (scratches_by_pid)
-               
-               117         138 LOAD_GLOBAL             15 (NULL + dict)
-                           150 PRECALL                  0
-                           154 CALL                     0
-                           164 LOAD_FAST                0 (self)
-                           166 STORE_ATTR               8 (focused_window_tracking)
-                           176 LOAD_CONST               0 (None)
-                           178 RETURN_VALUE
-               consts
-                  None
-               names      ('procs', 'scratches', 'set', 'transitioning_scratches', '_respawned_scratches', 'scratches_by_address', 'scratches_by_pid', 'dict', 'focused_window_tracking')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
-               name       'init'
-               firstlineno 110
-               lnotab 0x06010e010e01260126010e010e01
-            code
-               argcount  : 1
-               nlocals   : 1
                stacksize : 5
                flags     : 131
                code
                   0x870087014b000100970064017400000000000000000000006602880066
                   016402840c8a017403000000000000000000006a02000000000000000088
                   0166016403840889006a030000000000000000a004000000000000000000
                   0000000000000000000000a6000000ab0000000000000000004400a60000
-                  00ab0000000000000000008e00830064007b035600970386040100640053
+                  00ab0000000000000000008e00830064047b035600970386040100640453
                   00
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (die_in_piece)
                
-               119           4 RETURN_GENERATOR
+               143           4 RETURN_GENERATOR
                              6 POP_TOP
                              8 RESUME                   0
                
-               120          10 LOAD_CONST               1 ('scratch')
+               146          10 LOAD_CONST               1 ('scratch')
                             12 LOAD_GLOBAL              0 (Scratch)
                             24 BUILD_TUPLE              2
                             26 LOAD_CLOSURE             0 (self)
                             28 BUILD_TUPLE              1
-                            30 LOAD_CONST               2 (<code object die_in_piece, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 120>)
+                            30 LOAD_CONST               2 (<code object die_in_piece, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 146>)
                             32 MAKE_FUNCTION           12 (annotations, closure)
                             34 STORE_DEREF              1 (die_in_piece)
                
-               131          36 LOAD_GLOBAL              3 (NULL + asyncio)
+               157          36 LOAD_GLOBAL              3 (NULL + asyncio)
                             48 LOAD_ATTR                2 (gather)
                
-               132          58 LOAD_CLOSURE             1 (die_in_piece)
+               158          58 LOAD_CLOSURE             1 (die_in_piece)
                             60 BUILD_TUPLE              1
-                            62 LOAD_CONST               3 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 132>)
+                            62 LOAD_CONST               3 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 158>)
                             64 MAKE_FUNCTION            8 (closure)
                             66 LOAD_DEREF               0 (self)
                             68 LOAD_ATTR                3 (scratches)
                             78 LOAD_METHOD              4 (values)
                            100 PRECALL                  0
                            104 CALL                     0
                            114 GET_ITER
                            116 PRECALL                  0
                            120 CALL                     0
                
-               131         130 CALL_FUNCTION_EX         0
+               157         130 CALL_FUNCTION_EX         0
                            132 GET_AWAITABLE            0
-                           134 LOAD_CONST               0 (None)
+                           134 LOAD_CONST               4 (None)
                        >>  136 SEND                     3 (to 144)
                            138 YIELD_VALUE
                            140 RESUME                   3
                            142 JUMP_BACKWARD_NO_INTERRUPT     4 (to 136)
                        >>  144 POP_TOP
-                           146 LOAD_CONST               0 (None)
+                           146 LOAD_CONST               4 (None)
                            148 RETURN_VALUE
                consts
-                  None
+                  'exit hook'
                   'scratch'
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 147
                      code
@@ -1251,104 +1507,104 @@
                         03860401008c337c00a00400000000000000000000000000000000000000
                         00a6000000ab00000000000000000072147c01a007000000000000000000
                         0000000000000000000000a6000000ab00000000000000000001007c01a0
                         080000000000000000000000000000000000000000a6000000ab00000000
                         0000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     120           2 RETURN_GENERATOR
+                     146           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                     121           8 LOAD_DEREF               3 (self)
+                     147           8 LOAD_DEREF               3 (self)
                                   10 LOAD_ATTR                0 (procs)
                                   20 LOAD_FAST                0 (scratch)
                                   22 LOAD_ATTR                1 (uid)
                                   32 BINARY_SUBSCR
                                   42 STORE_FAST               1 (proc)
                      
-                     122          44 LOAD_FAST                1 (proc)
+                     148          44 LOAD_FAST                1 (proc)
                                   46 LOAD_METHOD              2 (terminate)
                                   68 PRECALL                  0
                                   72 CALL                     0
                                   82 POP_TOP
                      
-                     123          84 LOAD_GLOBAL              7 (NULL + range)
+                     149          84 LOAD_GLOBAL              7 (NULL + range)
                                   96 LOAD_CONST               1 (10)
                                   98 PRECALL                  1
                                  102 CALL                     1
                                  112 GET_ITER
                              >>  114 FOR_ITER                50 (to 216)
-                                 116 STORE_FAST               2 (n)
+                                 116 STORE_FAST               2 (_)
                      
-                     124         118 LOAD_FAST                0 (scratch)
+                     150         118 LOAD_FAST                0 (scratch)
                                  120 LOAD_METHOD              4 (isAlive)
                                  142 PRECALL                  0
                                  146 CALL                     0
                                  156 POP_JUMP_FORWARD_IF_TRUE     2 (to 162)
                      
-                     125         158 POP_TOP
+                     151         158 POP_TOP
                                  160 JUMP_FORWARD            27 (to 216)
                      
-                     126     >>  162 LOAD_GLOBAL             11 (NULL + asyncio)
+                     152     >>  162 LOAD_GLOBAL             11 (NULL + asyncio)
                                  174 LOAD_ATTR                6 (sleep)
                                  184 LOAD_CONST               2 (0.1)
                                  186 PRECALL                  1
                                  190 CALL                     1
                                  200 GET_AWAITABLE            0
                                  202 LOAD_CONST               0 (None)
                              >>  204 SEND                     3 (to 212)
                                  206 YIELD_VALUE
                                  208 RESUME                   3
                                  210 JUMP_BACKWARD_NO_INTERRUPT     4 (to 204)
                              >>  212 POP_TOP
                                  214 JUMP_BACKWARD           51 (to 114)
                      
-                     127     >>  216 LOAD_FAST                0 (scratch)
+                     153     >>  216 LOAD_FAST                0 (scratch)
                                  218 LOAD_METHOD              4 (isAlive)
                                  240 PRECALL                  0
                                  244 CALL                     0
                                  254 POP_JUMP_FORWARD_IF_FALSE    20 (to 296)
                      
-                     128         256 LOAD_FAST                1 (proc)
+                     154         256 LOAD_FAST                1 (proc)
                                  258 LOAD_METHOD              7 (kill)
                                  280 PRECALL                  0
                                  284 CALL                     0
                                  294 POP_TOP
                      
-                     129     >>  296 LOAD_FAST                1 (proc)
+                     155     >>  296 LOAD_FAST                1 (proc)
                                  298 LOAD_METHOD              8 (wait)
                                  320 PRECALL                  0
                                  324 CALL                     0
                                  334 POP_TOP
                                  336 LOAD_CONST               0 (None)
                                  338 RETURN_VALUE
                      consts
                         None
                         10
                         0.1
                      names      ('procs', 'uid', 'terminate', 'range', 'isAlive', 'asyncio', 'sleep', 'kill', 'wait')
-                     varnames   ('scratch', 'proc', 'n')
+                     varnames   ('scratch', 'proc', '_')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                      name       'die_in_piece'
-                     firstlineno 120
+                     firstlineno 146
                      lnotab 0x080124012801220128010401360128012801
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 51
                      code
                         0x95014b00010097007c005d0f7d01020089027c01a6010000ab01000000
                         00000000005600970101008c1064005300
                                    0 COPY_FREE_VARS           1
                      
-                     132           2 RETURN_GENERATOR
+                     158           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                15 (to 42)
                                   12 STORE_FAST               1 (scratch)
                                   14 PUSH_NULL
                                   16 LOAD_DEREF               2 (die_in_piece)
@@ -1365,131 +1621,157 @@
                         None
                      names      ()
                      varnames   ('.0', 'scratch')
                      freevars   ('die_in_piece',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                      name       '<genexpr>'
-                     firstlineno 132
+                     firstlineno 158
                      lnotab 0x
+                  None
                names      ('Scratch', 'asyncio', 'gather', 'scratches', 'values')
                varnames   ('self',)
                freevars   ()
                cellvars   ('self', 'die_in_piece')
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'exit'
-               firstlineno 119
-               lnotab 0x0a011a0b160148ff
+               firstlineno 143
+               lnotab 0x0a031a0b160148ff
+            'config'
             code
                argcount  : 2
-               nlocals   : 5
-               stacksize : 4
+               nlocals   : 6
+               stacksize : 5
                flags     : 131
                code
-                  0x4b00010097007c016401190000000000000000007d01640284007c01a0
+                  0x4b00010097007c016401190000000000000000007d02640284007c02a0
                   000000000000000000000000000000000000000000a6000000ab00000000
-                  00000000004400a6000000ab0000000000000000007d0274030000000000
-                  0000000000a6000000ab0000000000000000007d037c0244005d4e7d047c
-                  047c006a020000000000000000760172267c027c04190000000000000000
-                  007c006a0200000000000000007c043c0000007c03a00300000000000000
-                  000000000000000000000000007c04a6010000ab01000000000000000001
-                  008c317c027c04190000000000000000006a0400000000000000007c006a
-                  0200000000000000007c04190000000000000000005f0400000000000000
-                  008c4f7c0344005d177d047c00a005000000000000000000000000000000
-                  00000000007c04a6010000ab01000000000000000001008c1864005300
-               135           0 RETURN_GENERATOR
+                  00000000004400a6000000ab0000000000000000007d0374030000000000
+                  0000000000a6000000ab0000000000000000007d047c0344005d4e7d057c
+                  057c006a020000000000000000760172267c037c05190000000000000000
+                  007c006a0200000000000000007c053c0000007c04a00300000000000000
+                  000000000000000000000000007c05a6010000ab01000000000000000001
+                  008c317c037c05190000000000000000006a0400000000000000007c006a
+                  0200000000000000007c05190000000000000000005f0400000000000000
+                  008c4f7c0444005d457d057c006a0200000000000000007c051900000000
+                  00000000006a040000000000000000a00500000000000000000000000000
+                  0000000000000064036404a6020000ab020000000000000000731d7c00a0
+                  0600000000000000000000000000000000000000007c056405ac06a60200
+                  00ab020000000000000000830064077b0356009703860401008c46640753
+                  00
+               161           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               136           6 LOAD_FAST                1 (config)
+               163           6 LOAD_FAST                1 (config)
                              8 LOAD_CONST               1 ('scratchpads')
                             10 BINARY_SUBSCR
-                            20 STORE_FAST               1 (config)
+                            20 STORE_FAST               2 (my_config)
                
-               137          22 LOAD_CONST               2 (<code object <dictcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 137>)
+               164          22 LOAD_CONST               2 (<code object <dictcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 164>)
                             24 MAKE_FUNCTION            0
-                            26 LOAD_FAST                1 (config)
+                            26 LOAD_FAST                2 (my_config)
                             28 LOAD_METHOD              0 (items)
                             50 PRECALL                  0
                             54 CALL                     0
                             64 GET_ITER
                             66 PRECALL                  0
                             70 CALL                     0
-                            80 STORE_FAST               2 (scratches)
+                            80 STORE_FAST               3 (scratches)
                
-               139          82 LOAD_GLOBAL              3 (NULL + set)
+               166          82 LOAD_GLOBAL              3 (NULL + set)
                             94 PRECALL                  0
                             98 CALL                     0
-                           108 STORE_FAST               3 (new_scratches)
+                           108 STORE_FAST               4 (new_scratches)
                
-               141         110 LOAD_FAST                2 (scratches)
+               168         110 LOAD_FAST                3 (scratches)
                            112 GET_ITER
                        >>  114 FOR_ITER                78 (to 272)
-                           116 STORE_FAST               4 (name)
+                           116 STORE_FAST               5 (name)
                
-               142         118 LOAD_FAST                4 (name)
+               169         118 LOAD_FAST                5 (name)
                            120 LOAD_FAST                0 (self)
                            122 LOAD_ATTR                2 (scratches)
                            132 CONTAINS_OP              1
                            134 POP_JUMP_FORWARD_IF_FALSE    38 (to 212)
                
-               143         136 LOAD_FAST                2 (scratches)
-                           138 LOAD_FAST                4 (name)
+               170         136 LOAD_FAST                3 (scratches)
+                           138 LOAD_FAST                5 (name)
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 LOAD_ATTR                2 (scratches)
-                           162 LOAD_FAST                4 (name)
+                           162 LOAD_FAST                5 (name)
                            164 STORE_SUBSCR
                
-               144         168 LOAD_FAST                3 (new_scratches)
+               171         168 LOAD_FAST                4 (new_scratches)
                            170 LOAD_METHOD              3 (add)
-                           192 LOAD_FAST                4 (name)
+                           192 LOAD_FAST                5 (name)
                            194 PRECALL                  1
                            198 CALL                     1
                            208 POP_TOP
                            210 JUMP_BACKWARD           49 (to 114)
                
-               146     >>  212 LOAD_FAST                2 (scratches)
-                           214 LOAD_FAST                4 (name)
+               173     >>  212 LOAD_FAST                3 (scratches)
+                           214 LOAD_FAST                5 (name)
                            216 BINARY_SUBSCR
                            226 LOAD_ATTR                4 (conf)
                            236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                2 (scratches)
-                           248 LOAD_FAST                4 (name)
+                           248 LOAD_FAST                5 (name)
                            250 BINARY_SUBSCR
                            260 STORE_ATTR               4 (conf)
                            270 JUMP_BACKWARD           79 (to 114)
                
-               149     >>  272 LOAD_FAST                3 (new_scratches)
+               176     >>  272 LOAD_FAST                4 (new_scratches)
                            274 GET_ITER
-                       >>  276 FOR_ITER                23 (to 324)
-                           278 STORE_FAST               4 (name)
+                       >>  276 FOR_ITER                69 (to 416)
+                           278 STORE_FAST               5 (name)
                
-               150         280 LOAD_FAST                0 (self)
-                           282 LOAD_METHOD              5 (start_scratch_command)
-                           304 LOAD_FAST                4 (name)
-                           306 PRECALL                  1
-                           310 CALL                     1
-                           320 POP_TOP
-                           322 JUMP_BACKWARD           24 (to 276)
+               177         280 LOAD_FAST                0 (self)
+                           282 LOAD_ATTR                2 (scratches)
+                           292 LOAD_FAST                5 (name)
+                           294 BINARY_SUBSCR
+                           304 LOAD_ATTR                4 (conf)
+                           314 LOAD_METHOD              5 (get)
+                           336 LOAD_CONST               3 ('lazy')
+                           338 LOAD_CONST               4 (False)
+                           340 PRECALL                  2
+                           344 CALL                     2
+                           354 POP_JUMP_FORWARD_IF_TRUE    29 (to 414)
+               
+               178         356 LOAD_FAST                0 (self)
+                           358 LOAD_METHOD              6 (start_scratch_command)
+                           380 LOAD_FAST                5 (name)
+                           382 LOAD_CONST               5 (True)
+                           384 KW_NAMES                 6
+                           386 PRECALL                  2
+                           390 CALL                     2
+                           400 GET_AWAITABLE            0
+                           402 LOAD_CONST               7 (None)
+                       >>  404 SEND                     3 (to 412)
+                           406 YIELD_VALUE
+                           408 RESUME                   3
+                           410 JUMP_BACKWARD_NO_INTERRUPT     4 (to 404)
+                       >>  412 POP_TOP
+                       >>  414 JUMP_BACKWARD           70 (to 276)
                
-               149     >>  324 LOAD_CONST               0 (None)
-                           326 RETURN_VALUE
+               176     >>  416 LOAD_CONST               7 (None)
+                           418 RETURN_VALUE
                consts
-                  None
+                  'config loader'
                   'scratchpads'
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 7
                      flags     : 19
                      code
                         0x970069007c005d165c0200007d017d027c017401000000000000000000
                         007c017c02a6020000ab02000000000000000093028c175300
-                     137           0 RESUME                   0
+                     164           0 RESUME                   0
                                    2 BUILD_MAP                0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                22 (to 52)
                                    8 UNPACK_SEQUENCE          2
                                   12 STORE_FAST               1 (k)
                                   14 STORE_FAST               2 (v)
                                   16 LOAD_FAST                1 (k)
@@ -1504,1517 +1786,1910 @@
                      consts
                      names      ('Scratch',)
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                      name       '<dictcomp>'
-                     firstlineno 137
+                     firstlineno 164
                      lnotab 0x
-               names      ('items', 'set', 'scratches', 'add', 'conf', 'start_scratch_command')
-               varnames   ('self', 'config', 'scratches', 'new_scratches', 'name')
+                  'lazy'
+                  False
+                  True
+                  ('is_new',)
+                  None
+               names      ('items', 'set', 'scratches', 'add', 'conf', 'get', 'start_scratch_command')
+               varnames   ('self', 'config', 'my_config', 'scratches', 'new_scratches', 'name')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'load_config'
-               firstlineno 135
-               lnotab 0x060110013c021c020801120120012c023c0308012cff
+               firstlineno 161
+               lnotab 0x060210013c021c020801120120012c023c0308014c013cfe
+            False
             'name'
             code
-               argcount  : 2
-               nlocals   : 5
+               argcount  : 3
+               nlocals   : 7
                stacksize : 7
-               flags     : 3
+               flags     : 131
                code
-                  0x97007c006a000000000000000000a00100000000000000000000000000
-                  000000000000007c01a6010000ab01000000000000000001007c006a0200
-                  000000000000007c01190000000000000000007d027c017c006a03000000
-                  0000000000760072127c006a0300000000000000007c0119000000000000
-                  0000006a0400000000000000006e0164017d03740b000000000000000000
-                  006a0600000000000000007c026a07000000000000000064021900000000
-                  0000000000740a000000000000000000006a080000000000000000740a00
-                  0000000000000000006a080000000000000000740a000000000000000000
-                  006a0800000000000000006403ac04a6050000ab0500000000000000007c
-                  006a0300000000000000007c013c0000007c006a0300000000000000007c
-                  01190000000000000000006a0400000000000000007d047c006a02000000
-                  00000000007c0119000000000000000000a0090000000000000000000000
-                  0000000000000000007c04a6010000ab01000000000000000001007c027c
-                  006a0a00000000000000007c006a0300000000000000007c011900000000
-                  00000000006a0400000000000000003c0000007c0372137c037c006a0a00
-                  000000000000007600720c7c006a0a00000000000000007c033d00640053
-                  006400530064005300
-               152           0 RESUME                   0
-               
-               153           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (_respawned_scratches)
-                            14 LOAD_METHOD              1 (add)
-                            36 LOAD_FAST                1 (name)
-                            38 PRECALL                  1
-                            42 CALL                     1
-                            52 POP_TOP
-               
-               154          54 LOAD_FAST                0 (self)
-                            56 LOAD_ATTR                2 (scratches)
-                            66 LOAD_FAST                1 (name)
-                            68 BINARY_SUBSCR
-                            78 STORE_FAST               2 (scratch)
+                  0x4b00010097007c02721a7c006a000000000000000000a0010000000000
+                  0000000000000000000000000000007c01a6010000ab0100000000000000
+                  0001007c006a020000000000000000a00100000000000000000000000000
+                  000000000000007c01a6010000ab01000000000000000001007c006a0300
+                  000000000000007c01190000000000000000007d037c017c006a04000000
+                  0000000000760072127c006a0400000000000000007c0119000000000000
+                  0000006a0500000000000000006e0164017d04740d000000000000000000
+                  006a0700000000000000007c036a08000000000000000064021900000000
+                  0000000000740c000000000000000000006a090000000000000000740c00
+                  0000000000000000006a090000000000000000740c000000000000000000
+                  006a0900000000000000006403ac04a6050000ab0500000000000000007d
+                  057c057c006a0400000000000000007c013c0000007c056a050000000000
+                  0000007d067c006a0300000000000000007c0119000000000000000000a0
+                  0a00000000000000000000000000000000000000007c06a6010000ab0100
+                  0000000000000001007c037c006a0b00000000000000007c056a05000000
+                  00000000003c0000007c0472137c047c006a0b0000000000000000760072
+                  0c7c006a0b00000000000000007c043d00640553006405530064055300
+               180           0 RETURN_GENERATOR
+                             2 POP_TOP
+                             4 RESUME                   0
+               
+               182           6 LOAD_FAST                2 (is_new)
+                             8 POP_JUMP_FORWARD_IF_FALSE    26 (to 62)
                
-               155          80 LOAD_FAST                1 (name)
-                            82 LOAD_FAST                0 (self)
-                            84 LOAD_ATTR                3 (procs)
-                            94 CONTAINS_OP              0
-                            96 POP_JUMP_FORWARD_IF_FALSE    18 (to 134)
-                            98 LOAD_FAST                0 (self)
-                           100 LOAD_ATTR                3 (procs)
-                           110 LOAD_FAST                1 (name)
-                           112 BINARY_SUBSCR
-                           122 LOAD_ATTR                4 (pid)
-                           132 JUMP_FORWARD             1 (to 136)
-                       >>  134 LOAD_CONST               1 (0)
-                       >>  136 STORE_FAST               3 (old_pid)
-               
-               156         138 LOAD_GLOBAL             11 (NULL + subprocess)
-                           150 LOAD_ATTR                6 (Popen)
-               
-               157         160 LOAD_FAST                2 (scratch)
-                           162 LOAD_ATTR                7 (conf)
-                           172 LOAD_CONST               2 ('command')
-                           174 BINARY_SUBSCR
-               
-               158         184 LOAD_GLOBAL             10 (subprocess)
-                           196 LOAD_ATTR                8 (DEVNULL)
-               
-               159         206 LOAD_GLOBAL             10 (subprocess)
-                           218 LOAD_ATTR                8 (DEVNULL)
-               
-               160         228 LOAD_GLOBAL             10 (subprocess)
-                           240 LOAD_ATTR                8 (DEVNULL)
-               
-               161         250 LOAD_CONST               3 (True)
-               
-               156         252 KW_NAMES                 4
-                           254 PRECALL                  5
-                           258 CALL                     5
-                           268 LOAD_FAST                0 (self)
-                           270 LOAD_ATTR                3 (procs)
-                           280 LOAD_FAST                1 (name)
-                           282 STORE_SUBSCR
-               
-               163         286 LOAD_FAST                0 (self)
-                           288 LOAD_ATTR                3 (procs)
-                           298 LOAD_FAST                1 (name)
-                           300 BINARY_SUBSCR
-                           310 LOAD_ATTR                4 (pid)
-                           320 STORE_FAST               4 (pid)
-               
-               164         322 LOAD_FAST                0 (self)
-                           324 LOAD_ATTR                2 (scratches)
-                           334 LOAD_FAST                1 (name)
-                           336 BINARY_SUBSCR
-                           346 LOAD_METHOD              9 (reset)
-                           368 LOAD_FAST                4 (pid)
-                           370 PRECALL                  1
-                           374 CALL                     1
-                           384 POP_TOP
-               
-               165         386 LOAD_FAST                2 (scratch)
-                           388 LOAD_FAST                0 (self)
-                           390 LOAD_ATTR               10 (scratches_by_pid)
-                           400 LOAD_FAST                0 (self)
-                           402 LOAD_ATTR                3 (procs)
-                           412 LOAD_FAST                1 (name)
-                           414 BINARY_SUBSCR
-                           424 LOAD_ATTR                4 (pid)
-                           434 STORE_SUBSCR
-               
-               166         438 LOAD_FAST                3 (old_pid)
-                           440 POP_JUMP_FORWARD_IF_FALSE    19 (to 480)
-                           442 LOAD_FAST                3 (old_pid)
-                           444 LOAD_FAST                0 (self)
-                           446 LOAD_ATTR               10 (scratches_by_pid)
-                           456 CONTAINS_OP              0
-                           458 POP_JUMP_FORWARD_IF_FALSE    12 (to 484)
-               
-               167         460 LOAD_FAST                0 (self)
-                           462 LOAD_ATTR               10 (scratches_by_pid)
-                           472 LOAD_FAST                3 (old_pid)
-                           474 DELETE_SUBSCR
-                           476 LOAD_CONST               0 (None)
-                           478 RETURN_VALUE
-               
-               166     >>  480 LOAD_CONST               0 (None)
-                           482 RETURN_VALUE
-                       >>  484 LOAD_CONST               0 (None)
-                           486 RETURN_VALUE
+               183          10 LOAD_FAST                0 (self)
+                            12 LOAD_ATTR                0 (_new_scratches)
+                            22 LOAD_METHOD              1 (add)
+                            44 LOAD_FAST                1 (name)
+                            46 PRECALL                  1
+                            50 CALL                     1
+                            60 POP_TOP
+               
+               184     >>   62 LOAD_FAST                0 (self)
+                            64 LOAD_ATTR                2 (_respawned_scratches)
+                            74 LOAD_METHOD              1 (add)
+                            96 LOAD_FAST                1 (name)
+                            98 PRECALL                  1
+                           102 CALL                     1
+                           112 POP_TOP
+               
+               185         114 LOAD_FAST                0 (self)
+                           116 LOAD_ATTR                3 (scratches)
+                           126 LOAD_FAST                1 (name)
+                           128 BINARY_SUBSCR
+                           138 STORE_FAST               3 (scratch)
+               
+               186         140 LOAD_FAST                1 (name)
+                           142 LOAD_FAST                0 (self)
+                           144 LOAD_ATTR                4 (procs)
+                           154 CONTAINS_OP              0
+                           156 POP_JUMP_FORWARD_IF_FALSE    18 (to 194)
+                           158 LOAD_FAST                0 (self)
+                           160 LOAD_ATTR                4 (procs)
+                           170 LOAD_FAST                1 (name)
+                           172 BINARY_SUBSCR
+                           182 LOAD_ATTR                5 (pid)
+                           192 JUMP_FORWARD             1 (to 196)
+                       >>  194 LOAD_CONST               1 (0)
+                       >>  196 STORE_FAST               4 (old_pid)
+               
+               187         198 LOAD_GLOBAL             13 (NULL + subprocess)
+                           210 LOAD_ATTR                7 (Popen)
+               
+               188         220 LOAD_FAST                3 (scratch)
+                           222 LOAD_ATTR                8 (conf)
+                           232 LOAD_CONST               2 ('command')
+                           234 BINARY_SUBSCR
+               
+               189         244 LOAD_GLOBAL             12 (subprocess)
+                           256 LOAD_ATTR                9 (DEVNULL)
+               
+               190         266 LOAD_GLOBAL             12 (subprocess)
+                           278 LOAD_ATTR                9 (DEVNULL)
+               
+               191         288 LOAD_GLOBAL             12 (subprocess)
+                           300 LOAD_ATTR                9 (DEVNULL)
+               
+               192         310 LOAD_CONST               3 (True)
+               
+               187         312 KW_NAMES                 4
+                           314 PRECALL                  5
+                           318 CALL                     5
+                           328 STORE_FAST               5 (proc)
+               
+               194         330 LOAD_FAST                5 (proc)
+                           332 LOAD_FAST                0 (self)
+                           334 LOAD_ATTR                4 (procs)
+                           344 LOAD_FAST                1 (name)
+                           346 STORE_SUBSCR
+               
+               195         350 LOAD_FAST                5 (proc)
+                           352 LOAD_ATTR                5 (pid)
+                           362 STORE_FAST               6 (pid)
+               
+               196         364 LOAD_FAST                0 (self)
+                           366 LOAD_ATTR                3 (scratches)
+                           376 LOAD_FAST                1 (name)
+                           378 BINARY_SUBSCR
+                           388 LOAD_METHOD             10 (reset)
+                           410 LOAD_FAST                6 (pid)
+                           412 PRECALL                  1
+                           416 CALL                     1
+                           426 POP_TOP
+               
+               197         428 LOAD_FAST                3 (scratch)
+                           430 LOAD_FAST                0 (self)
+                           432 LOAD_ATTR               11 (scratches_by_pid)
+                           442 LOAD_FAST                5 (proc)
+                           444 LOAD_ATTR                5 (pid)
+                           454 STORE_SUBSCR
+               
+               199         458 LOAD_FAST                4 (old_pid)
+                           460 POP_JUMP_FORWARD_IF_FALSE    19 (to 500)
+                           462 LOAD_FAST                4 (old_pid)
+                           464 LOAD_FAST                0 (self)
+                           466 LOAD_ATTR               11 (scratches_by_pid)
+                           476 CONTAINS_OP              0
+                           478 POP_JUMP_FORWARD_IF_FALSE    12 (to 504)
+               
+               200         480 LOAD_FAST                0 (self)
+                           482 LOAD_ATTR               11 (scratches_by_pid)
+                           492 LOAD_FAST                4 (old_pid)
+                           494 DELETE_SUBSCR
+                           496 LOAD_CONST               5 (None)
+                           498 RETURN_VALUE
+               
+               199     >>  500 LOAD_CONST               5 (None)
+                           502 RETURN_VALUE
+                       >>  504 LOAD_CONST               5 (None)
+                           506 RETURN_VALUE
                consts
-                  None
+                  "spawns a given scratchpad's process"
                   0
                   'command'
                   True
                   ('stdin', 'stdout', 'stderr', 'shell')
-               names      ('_respawned_scratches', 'add', 'scratches', 'procs', 'pid', 'subprocess', 'Popen', 'conf', 'DEVNULL', 'reset', 'scratches_by_pid')
-               varnames   ('self', 'name', 'scratch', 'old_pid', 'pid')
+                  None
+               names      ('_new_scratches', 'add', '_respawned_scratches', 'scratches', 'procs', 'pid', 'subprocess', 'Popen', 'conf', 'DEVNULL', 'reset', 'scratches_by_pid')
+               varnames   ('self', 'name', 'is_new', 'scratch', 'old_pid', 'proc', 'pid')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'start_scratch_command'
-               firstlineno 152
+               firstlineno 180
                lnotab
-                  0x020134011a013a011601180116011601160102fb220724014001340116
-                  0114ff
+                  0x06020401340134011a013a011601180116011601160102fb120714010e
+                  0140011e02160114ff
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c01a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d017c006a010000000000000000a0
                   0200000000000000000000000000000000000000007c01a6010000ab0100
-                  000000000000007d027c0272347c026a030000000000000000722b7c00a0
-                  0400000000000000000000000000000000000000007c026a050000000000
-                  0000006401ac02a6020000ab020000000000000000830064007b03560097
-                  038604010064037c025f03000000000000000064005300640053007c006a
-                  060000000000000000a00700000000000000000000000000000000000000
-                  00a6000000ab00000000000000000044005d675c0200007d037d027c026a
-                  080000000000000000725b7c026a0900000000000000007c016b03000000
-                  0072507c026a0a000000000000000072497c026a0b0000000000000000a0
-                  0200000000000000000000000000000000000000006404a6010000ab0100
-                  0000000000000064056b0200000000722b7c026a0500000000000000007c
-                  006a0c00000000000000007601721d7c00a0040000000000000000000000
-                  0000000000000000007c036401ac06a6020000ab02000000000000000083
-                  0064007b0356009703860401008c6864005300
-               170           0 RETURN_GENERATOR
+                  000000000000007d027c0272547c026a030000000000000000724b7c006a
+                  040000000000000000a00500000000000000000000000000000000000000
+                  0064017c026a060000000000000000a6020000ab02000000000000000001
+                  007c00a00700000000000000000000000000000000000000007c026a0600
+                  000000000000006402ac03a6020000ab020000000000000000830064047b
+                  03560097038604010064057c025f03000000000000000064045300640453
+                  007c006a080000000000000000a009000000000000000000000000000000
+                  0000000000a6000000ab00000000000000000044005d825c0200007d037d
+                  027c026a0a000000000000000072767c026a0b00000000000000007c016b
+                  0300000000726b7c026a0c000000000000000072647c026a0d0000000000
+                  000000a00200000000000000000000000000000000000000006406a60100
+                  00ab01000000000000000064076b020000000072467c026a060000000000
+                  0000007c006a0e0000000000000000760172387c006a0400000000000000
+                  00a005000000000000000000000000000000000000000064087c03a60200
+                  00ab02000000000000000001007c00a00700000000000000000000000000
+                  000000000000007c036402ac09a6020000ab020000000000000000830064
+                  047b0356009703860401008c8364045300
+               203           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               171           6 LOAD_FAST                1 (addr)
+               205           6 LOAD_FAST                1 (addr)
                              8 LOAD_METHOD              0 (strip)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 STORE_FAST               1 (addr)
                
-               172          46 LOAD_FAST                0 (self)
+               206          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                1 (scratches_by_address)
                             58 LOAD_METHOD              2 (get)
                             80 LOAD_FAST                1 (addr)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               2 (scratch)
                
-               173          98 LOAD_FAST                2 (scratch)
-                           100 POP_JUMP_FORWARD_IF_FALSE    52 (to 206)
+               207          98 LOAD_FAST                2 (scratch)
+                           100 POP_JUMP_FORWARD_IF_FALSE    84 (to 270)
                
-               174         102 LOAD_FAST                2 (scratch)
+               208         102 LOAD_FAST                2 (scratch)
                            104 LOAD_ATTR                3 (just_created)
-                           114 POP_JUMP_FORWARD_IF_FALSE    43 (to 202)
+                           114 POP_JUMP_FORWARD_IF_FALSE    75 (to 266)
                
-               175         116 LOAD_FAST                0 (self)
-                           118 LOAD_METHOD              4 (run_hide)
-                           140 LOAD_FAST                2 (scratch)
-                           142 LOAD_ATTR                5 (uid)
-                           152 LOAD_CONST               1 (True)
-                           154 KW_NAMES                 2
-                           156 PRECALL                  2
-                           160 CALL                     2
-                           170 GET_AWAITABLE            0
-                           172 LOAD_CONST               0 (None)
-                       >>  174 SEND                     3 (to 182)
-                           176 YIELD_VALUE
-                           178 RESUME                   3
-                           180 JUMP_BACKWARD_NO_INTERRUPT     4 (to 174)
-                       >>  182 POP_TOP
-               
-               176         184 LOAD_CONST               3 (False)
-                           186 LOAD_FAST                2 (scratch)
-                           188 STORE_ATTR               3 (just_created)
-                           198 LOAD_CONST               0 (None)
-                           200 RETURN_VALUE
-               
-               174     >>  202 LOAD_CONST               0 (None)
-                           204 RETURN_VALUE
-               
-               178     >>  206 LOAD_FAST                0 (self)
-                           208 LOAD_ATTR                6 (scratches)
-                           218 LOAD_METHOD              7 (items)
-                           240 PRECALL                  0
-                           244 CALL                     0
-                           254 GET_ITER
-                       >>  256 FOR_ITER               103 (to 464)
-                           258 UNPACK_SEQUENCE          2
-                           262 STORE_FAST               3 (uid)
-                           264 STORE_FAST               2 (scratch)
-               
-               179         266 LOAD_FAST                2 (scratch)
-                           268 LOAD_ATTR                8 (clientInfo)
-                           278 POP_JUMP_FORWARD_IF_FALSE    91 (to 462)
-                           280 LOAD_FAST                2 (scratch)
-                           282 LOAD_ATTR                9 (address)
-                           292 LOAD_FAST                1 (addr)
-                           294 COMPARE_OP               3 (!=)
-                           300 POP_JUMP_FORWARD_IF_FALSE    80 (to 462)
-               
-               181         302 LOAD_FAST                2 (scratch)
-                           304 LOAD_ATTR               10 (visible)
-               
-               180         314 POP_JUMP_FORWARD_IF_FALSE    73 (to 462)
-               
-               182         316 LOAD_FAST                2 (scratch)
-                           318 LOAD_ATTR               11 (conf)
-                           328 LOAD_METHOD              2 (get)
-                           350 LOAD_CONST               4 ('unfocus')
-                           352 PRECALL                  1
-                           356 CALL                     1
-                           366 LOAD_CONST               5 ('hide')
-                           368 COMPARE_OP               2 (==)
-                           374 POP_JUMP_FORWARD_IF_FALSE    43 (to 462)
-               
-               183         376 LOAD_FAST                2 (scratch)
-                           378 LOAD_ATTR                5 (uid)
-                           388 LOAD_FAST                0 (self)
-                           390 LOAD_ATTR               12 (transitioning_scratches)
-                           400 CONTAINS_OP              1
-                           402 POP_JUMP_FORWARD_IF_FALSE    29 (to 462)
-               
-               185         404 LOAD_FAST                0 (self)
-                           406 LOAD_METHOD              4 (run_hide)
-                           428 LOAD_FAST                3 (uid)
-                           430 LOAD_CONST               1 (True)
-                           432 KW_NAMES                 6
-                           434 PRECALL                  2
-                           438 CALL                     2
-                           448 GET_AWAITABLE            0
-                           450 LOAD_CONST               0 (None)
-                       >>  452 SEND                     3 (to 460)
-                           454 YIELD_VALUE
-                           456 RESUME                   3
-                           458 JUMP_BACKWARD_NO_INTERRUPT     4 (to 452)
-                       >>  460 POP_TOP
-                       >>  462 JUMP_BACKWARD          104 (to 256)
+               209         116 LOAD_FAST                0 (self)
+                           118 LOAD_ATTR                4 (log)
+                           128 LOAD_METHOD              5 (debug)
+                           150 LOAD_CONST               1 ('Hiding just created scratch %s')
+                           152 LOAD_FAST                2 (scratch)
+                           154 LOAD_ATTR                6 (uid)
+                           164 PRECALL                  2
+                           168 CALL                     2
+                           178 POP_TOP
+               
+               210         180 LOAD_FAST                0 (self)
+                           182 LOAD_METHOD              7 (run_hide)
+                           204 LOAD_FAST                2 (scratch)
+                           206 LOAD_ATTR                6 (uid)
+                           216 LOAD_CONST               2 (True)
+                           218 KW_NAMES                 3
+                           220 PRECALL                  2
+                           224 CALL                     2
+                           234 GET_AWAITABLE            0
+                           236 LOAD_CONST               4 (None)
+                       >>  238 SEND                     3 (to 246)
+                           240 YIELD_VALUE
+                           242 RESUME                   3
+                           244 JUMP_BACKWARD_NO_INTERRUPT     4 (to 238)
+                       >>  246 POP_TOP
+               
+               211         248 LOAD_CONST               5 (False)
+                           250 LOAD_FAST                2 (scratch)
+                           252 STORE_ATTR               3 (just_created)
+                           262 LOAD_CONST               4 (None)
+                           264 RETURN_VALUE
+               
+               208     >>  266 LOAD_CONST               4 (None)
+                           268 RETURN_VALUE
+               
+               213     >>  270 LOAD_FAST                0 (self)
+                           272 LOAD_ATTR                8 (scratches)
+                           282 LOAD_METHOD              9 (items)
+                           304 PRECALL                  0
+                           308 CALL                     0
+                           318 GET_ITER
+                       >>  320 FOR_ITER               130 (to 582)
+                           322 UNPACK_SEQUENCE          2
+                           326 STORE_FAST               3 (uid)
+                           328 STORE_FAST               2 (scratch)
+               
+               214         330 LOAD_FAST                2 (scratch)
+                           332 LOAD_ATTR               10 (client_info)
+                           342 POP_JUMP_FORWARD_IF_FALSE   118 (to 580)
+                           344 LOAD_FAST                2 (scratch)
+                           346 LOAD_ATTR               11 (address)
+                           356 LOAD_FAST                1 (addr)
+                           358 COMPARE_OP               3 (!=)
+                           364 POP_JUMP_FORWARD_IF_FALSE   107 (to 580)
+               
+               216         366 LOAD_FAST                2 (scratch)
+                           368 LOAD_ATTR               12 (visible)
+               
+               215         378 POP_JUMP_FORWARD_IF_FALSE   100 (to 580)
+               
+               217         380 LOAD_FAST                2 (scratch)
+                           382 LOAD_ATTR               13 (conf)
+                           392 LOAD_METHOD              2 (get)
+                           414 LOAD_CONST               6 ('unfocus')
+                           416 PRECALL                  1
+                           420 CALL                     1
+                           430 LOAD_CONST               7 ('hide')
+                           432 COMPARE_OP               2 (==)
+                           438 POP_JUMP_FORWARD_IF_FALSE    70 (to 580)
+               
+               218         440 LOAD_FAST                2 (scratch)
+                           442 LOAD_ATTR                6 (uid)
+                           452 LOAD_FAST                0 (self)
+                           454 LOAD_ATTR               14 (transitioning_scratches)
+                           464 CONTAINS_OP              1
+                           466 POP_JUMP_FORWARD_IF_FALSE    56 (to 580)
+               
+               220         468 LOAD_FAST                0 (self)
+                           470 LOAD_ATTR                4 (log)
+                           480 LOAD_METHOD              5 (debug)
+                           502 LOAD_CONST               8 ('hide %s because another client is active')
+                           504 LOAD_FAST                3 (uid)
+                           506 PRECALL                  2
+                           510 CALL                     2
+                           520 POP_TOP
+               
+               221         522 LOAD_FAST                0 (self)
+                           524 LOAD_METHOD              7 (run_hide)
+                           546 LOAD_FAST                3 (uid)
+                           548 LOAD_CONST               2 (True)
+                           550 KW_NAMES                 9
+                           552 PRECALL                  2
+                           556 CALL                     2
+                           566 GET_AWAITABLE            0
+                           568 LOAD_CONST               4 (None)
+                       >>  570 SEND                     3 (to 578)
+                           572 YIELD_VALUE
+                           574 RESUME                   3
+                           576 JUMP_BACKWARD_NO_INTERRUPT     4 (to 570)
+                       >>  578 POP_TOP
+                       >>  580 JUMP_BACKWARD          131 (to 320)
                
-               178     >>  464 LOAD_CONST               0 (None)
-                           466 RETURN_VALUE
+               213     >>  582 LOAD_CONST               4 (None)
+                           584 RETURN_VALUE
                consts
-                  None
+                  'active windows hook'
+                  'Hiding just created scratch %s'
                   True
                   ('force',)
+                  None
                   False
                   'unfocus'
                   'hide'
+                  'hide %s because another client is active'
                   ('autohide',)
-               names      ('strip', 'scratches_by_address', 'get', 'just_created', 'run_hide', 'uid', 'scratches', 'items', 'clientInfo', 'address', 'visible', 'conf', 'transitioning_scratches')
+               names      ('strip', 'scratches_by_address', 'get', 'just_created', 'log', 'debug', 'uid', 'run_hide', 'scratches', 'items', 'client_info', 'address', 'visible', 'conf', 'transitioning_scratches')
                varnames   ('self', 'addr', 'scratch', 'uid')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'event_activewindowv2'
-               firstlineno 170
+               firstlineno 203
+               lnotab
+                  0x06022801340104010e014001440112fd04053c0124020cff02023c011c
+                  0236013cf8
+            code
+               argcount  : 1
+               nlocals   : 4
+               stacksize : 7
+               flags     : 131
+               code
+                  0x87004b0001009700880066016401840889006a00000000000000000044
+                  00a6000000ab0000000000000000007d017c0173026402530089006a0100
+                  00000000000000a002000000000000000000000000000000000000000064
+                  03a6010000ab010000000000000000010074070000000000000000000064
+                  04a6010000ab010000000000000000830064057b0356009703860444005d
+                  837d027409000000000000000000007c02740a00000000000000000000a6
+                  020000ab02000000000000000073024a0082017c0144005d677d037c036a
+                  0600000000000000006406190000000000000000007c0264061900000000
+                  00000000006b0200000000724e7c0389006a0700000000000000007c0264
+                  0719000000000000000000640864058502190000000000000000003c0000
+                  0089006a010000000000000000a002000000000000000000000000000000
+                  000000000064097c02a6020000ab02000000000000000001007c03a00800
+                  000000000000000000000000000000000000007c02a6010000ab01000000
+                  0000000000830064057b0356009703860401008c688c84640a5300
+                             0 MAKE_CELL                0 (self)
+               
+               223           2 RETURN_GENERATOR
+                             4 POP_TOP
+                             6 RESUME                   0
+               
+               225           8 LOAD_CLOSURE             0 (self)
+                            10 BUILD_TUPLE              1
+                            12 LOAD_CONST               1 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 225>)
+                            14 MAKE_FUNCTION            8 (closure)
+               
+               227          16 LOAD_DEREF               0 (self)
+                            18 LOAD_ATTR                0 (_respawned_scratches)
+               
+               225          28 GET_ITER
+                            30 PRECALL                  0
+                            34 CALL                     0
+                            44 STORE_FAST               1 (class_lookup_hack)
+               
+               230          46 LOAD_FAST                1 (class_lookup_hack)
+                            48 POP_JUMP_FORWARD_IF_TRUE     2 (to 54)
+               
+               231          50 LOAD_CONST               2 (False)
+                            52 RETURN_VALUE
+               
+               232     >>   54 LOAD_DEREF               0 (self)
+                            56 LOAD_ATTR                1 (log)
+                            66 LOAD_METHOD              2 (debug)
+                            88 LOAD_CONST               3 ('Lookup hack triggered')
+                            90 PRECALL                  1
+                            94 CALL                     1
+                           104 POP_TOP
+               
+               233         106 LOAD_GLOBAL              7 (NULL + hyprctlJSON)
+                           118 LOAD_CONST               4 ('clients')
+                           120 PRECALL                  1
+                           124 CALL                     1
+                           134 GET_AWAITABLE            0
+                           136 LOAD_CONST               5 (None)
+                       >>  138 SEND                     3 (to 146)
+                           140 YIELD_VALUE
+                           142 RESUME                   3
+                           144 JUMP_BACKWARD_NO_INTERRUPT     4 (to 138)
+                       >>  146 GET_ITER
+                       >>  148 FOR_ITER               131 (to 412)
+                           150 STORE_FAST               2 (client)
+               
+               234         152 LOAD_GLOBAL              9 (NULL + isinstance)
+                           164 LOAD_FAST                2 (client)
+                           166 LOAD_GLOBAL             10 (dict)
+                           178 PRECALL                  2
+                           182 CALL                     2
+                           192 POP_JUMP_FORWARD_IF_TRUE     2 (to 198)
+                           194 LOAD_ASSERTION_ERROR
+                           196 RAISE_VARARGS            1
+               
+               235     >>  198 LOAD_FAST                1 (class_lookup_hack)
+                           200 GET_ITER
+                       >>  202 FOR_ITER               103 (to 410)
+                           204 STORE_FAST               3 (pending_scratch)
+               
+               236         206 LOAD_FAST                3 (pending_scratch)
+                           208 LOAD_ATTR                6 (conf)
+                           218 LOAD_CONST               6 ('class')
+                           220 BINARY_SUBSCR
+                           230 LOAD_FAST                2 (client)
+                           232 LOAD_CONST               6 ('class')
+                           234 BINARY_SUBSCR
+                           244 COMPARE_OP               2 (==)
+                           250 POP_JUMP_FORWARD_IF_FALSE    78 (to 408)
+               
+               237         252 LOAD_FAST                3 (pending_scratch)
+                           254 LOAD_DEREF               0 (self)
+                           256 LOAD_ATTR                7 (scratches_by_address)
+                           266 LOAD_FAST                2 (client)
+                           268 LOAD_CONST               7 ('address')
+                           270 BINARY_SUBSCR
+                           280 LOAD_CONST               8 (2)
+                           282 LOAD_CONST               5 (None)
+                           284 BUILD_SLICE              2
+                           286 BINARY_SUBSCR
+                           296 STORE_SUBSCR
+               
+               238         300 LOAD_DEREF               0 (self)
+                           302 LOAD_ATTR                1 (log)
+                           312 LOAD_METHOD              2 (debug)
+                           334 LOAD_CONST               9 ('client class found: %s')
+                           336 LOAD_FAST                2 (client)
+                           338 PRECALL                  2
+                           342 CALL                     2
+                           352 POP_TOP
+               
+               239         354 LOAD_FAST                3 (pending_scratch)
+                           356 LOAD_METHOD              8 (updateClientInfo)
+                           378 LOAD_FAST                2 (client)
+                           380 PRECALL                  1
+                           384 CALL                     1
+                           394 GET_AWAITABLE            0
+                           396 LOAD_CONST               5 (None)
+                       >>  398 SEND                     3 (to 406)
+                           400 YIELD_VALUE
+                           402 RESUME                   3
+                           404 JUMP_BACKWARD_NO_INTERRUPT     4 (to 398)
+                       >>  406 POP_TOP
+                       >>  408 JUMP_BACKWARD          104 (to 202)
+               
+               235     >>  410 JUMP_BACKWARD          132 (to 148)
+               
+               240     >>  412 LOAD_CONST              10 (True)
+                           414 RETURN_VALUE
+               consts
+                  'if class attribute is defined, use class matching and return True'
+                  code
+                     argcount  : 1
+                     nlocals   : 2
+                     stacksize : 5
+                     flags     : 19
+                     code
+                        0x9501970067007c005d347d0189026a0000000000000000007c01190000
+                        000000000000006a010000000000000000a0020000000000000000000000
+                        0000000000000000006400a6010000ab010000000000000000af2789026a
+                        0000000000000000007c011900000000000000000091028c355300
+                                   0 COPY_FREE_VARS           1
+                     
+                     225           2 RESUME                   0
+                                   4 BUILD_LIST               0
+                                   6 LOAD_FAST                0 (.0)
+                             >>    8 FOR_ITER                52 (to 114)
+                     
+                     227          10 STORE_FAST               1 (name)
+                     
+                     228          12 LOAD_DEREF               2 (self)
+                                  14 LOAD_ATTR                0 (scratches)
+                                  24 LOAD_FAST                1 (name)
+                                  26 BINARY_SUBSCR
+                                  36 LOAD_ATTR                1 (conf)
+                                  46 LOAD_METHOD              2 (get)
+                                  68 LOAD_CONST               0 ('class')
+                                  70 PRECALL                  1
+                                  74 CALL                     1
+                     
+                     225          84 POP_JUMP_BACKWARD_IF_FALSE    39 (to 8)
+                     
+                     226          86 LOAD_DEREF               2 (self)
+                                  88 LOAD_ATTR                0 (scratches)
+                                  98 LOAD_FAST                1 (name)
+                                 100 BINARY_SUBSCR
+                     
+                     225         110 LIST_APPEND              2
+                                 112 JUMP_BACKWARD           53 (to 8)
+                             >>  114 RETURN_VALUE
+                     consts
+                        'class'
+                     names      ('scratches', 'conf', 'get')
+                     varnames   ('.0', 'name')
+                     freevars   ('self',)
+                     cellvars   ()
+                     filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
+                     name       '<listcomp>'
+                     firstlineno 225
+                     lnotab 0x0a02020148fd020118ff
+                  False
+                  'Lookup hack triggered'
+                  'clients'
+                  None
+                  'class'
+                  'address'
+                  2
+                  'client class found: %s'
+                  True
+               names      ('_respawned_scratches', 'log', 'debug', 'hyprctlJSON', 'isinstance', 'dict', 'conf', 'scratches_by_address', 'updateClientInfo')
+               varnames   ('self', 'class_lookup_hack', 'client', 'pending_scratch')
+               freevars   ()
+               cellvars   ('self',)
+               filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
+               name       '_alternative_lookup'
+               firstlineno 223
                lnotab
-                  0x06012801340104010e01440112fe04043c0124020cff02023c011c023c
-                  f9
+                  0x080208020cfe12050401040134012e012e0108012e013001360138fc02
+                  05
             code
                argcount  : 2
                nlocals   : 7
                stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c01a00000000000000000000000000000000000000000
                   0064016402a6020000ab0200000000000000005c0400007d027d037d047d
                   057c03a00100000000000000000000000000000000000000006403a60100
-                  00ab01000000000000000072aa7c006a020000000000000000a003000000
+                  00ab01000000000000000072f17c006a020000000000000000a003000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
-                  0000007d067c06733b7c006a04000000000000000072347c00a005000000
+                  0000007d067c0673557c006a040000000000000000724e7c00a005000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
-                  00830064007b0356009703860401007c006a020000000000000000a00300
-                  000000000000000000000000000000000000007c02a6010000ab01000000
-                  00000000007d067c0672537c066a060000000000000000724e7c006a0400
-                  00000000000000a00700000000000000000000000000000000000000007c
-                  066a080000000000000000a6010000ab01000000000000000001007c00a0
-                  0900000000000000000000000000000000000000007c066a080000000000
-                  0000006404ac05a6020000ab020000000000000000830064007b03560097
-                  038604010064067c065f0600000000000000006400530064005300640053
-                  0064005300
-               187           0 RETURN_GENERATOR
+                  00830064047b03560097038604731a7c00a0060000000000000000000000
+                  000000000000000000a6000000ab000000000000000000830064047b0356
+                  009703860401007c006a020000000000000000a003000000000000000000
+                  00000000000000000000007c02a6010000ab0100000000000000007d067c
+                  0672807c066a070000000000000000727b7c066a0800000000000000007c
+                  006a090000000000000000760072227c00a00a0000000000000000000000
+                  0000000000000000007c066a0800000000000000006405ac06a6020000ab
+                  020000000000000000830064047b0356009703860401007c006a09000000
+                  0000000000a00b00000000000000000000000000000000000000007c066a
+                  080000000000000000a6010000ab01000000000000000001007c006a0400
+                  00000000000000a00b00000000000000000000000000000000000000007c
+                  066a080000000000000000a6010000ab010000000000000000010064077c
+                  065f07000000000000000064045300640453006404530064045300
+               242           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               188           6 LOAD_FAST                1 (params)
+               244           6 LOAD_FAST                1 (params)
                              8 LOAD_METHOD              0 (split)
                             30 LOAD_CONST               1 (',')
                             32 LOAD_CONST               2 (3)
                             34 PRECALL                  2
                             38 CALL                     2
                             48 UNPACK_SEQUENCE          4
                             52 STORE_FAST               2 (addr)
                             54 STORE_FAST               3 (wrkspc)
-                            56 STORE_FAST               4 (kls)
-                            58 STORE_FAST               5 (title)
+                            56 STORE_FAST               4 (_kls)
+                            58 STORE_FAST               5 (_title)
                
-               189          60 LOAD_FAST                3 (wrkspc)
+               245          60 LOAD_FAST                3 (wrkspc)
                             62 LOAD_METHOD              1 (startswith)
                             84 LOAD_CONST               3 ('special')
                             86 PRECALL                  1
                             90 CALL                     1
-                           100 POP_JUMP_FORWARD_IF_FALSE   170 (to 442)
+                           100 POP_JUMP_FORWARD_IF_FALSE   241 (to 584)
                
-               190         102 LOAD_FAST                0 (self)
+               246         102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                2 (scratches_by_address)
                            114 LOAD_METHOD              3 (get)
                            136 LOAD_FAST                2 (addr)
                            138 PRECALL                  1
                            142 CALL                     1
                            152 STORE_FAST               6 (item)
                
-               191         154 LOAD_FAST                6 (item)
-                           156 POP_JUMP_FORWARD_IF_TRUE    59 (to 276)
+               247         154 LOAD_FAST                6 (item)
+                           156 POP_JUMP_FORWARD_IF_TRUE    85 (to 328)
                            158 LOAD_FAST                0 (self)
                            160 LOAD_ATTR                4 (_respawned_scratches)
-                           170 POP_JUMP_FORWARD_IF_FALSE    52 (to 276)
+                           170 POP_JUMP_FORWARD_IF_FALSE    78 (to 328)
                
-               192         172 LOAD_FAST                0 (self)
-                           174 LOAD_METHOD              5 (updateScratchInfo)
+               249         172 LOAD_FAST                0 (self)
+                           174 LOAD_METHOD              5 (_alternative_lookup)
                            196 PRECALL                  0
                            200 CALL                     0
                            210 GET_AWAITABLE            0
-                           212 LOAD_CONST               0 (None)
+                           212 LOAD_CONST               4 (None)
                        >>  214 SEND                     3 (to 222)
                            216 YIELD_VALUE
                            218 RESUME                   3
                            220 JUMP_BACKWARD_NO_INTERRUPT     4 (to 214)
-                       >>  222 POP_TOP
+                       >>  222 POP_JUMP_FORWARD_IF_TRUE    26 (to 276)
                
-               193         224 LOAD_FAST                0 (self)
-                           226 LOAD_ATTR                2 (scratches_by_address)
-                           236 LOAD_METHOD              3 (get)
-                           258 LOAD_FAST                2 (addr)
-                           260 PRECALL                  1
-                           264 CALL                     1
-                           274 STORE_FAST               6 (item)
-               
-               194     >>  276 LOAD_FAST                6 (item)
-                           278 POP_JUMP_FORWARD_IF_FALSE    83 (to 446)
-                           280 LOAD_FAST                6 (item)
-                           282 LOAD_ATTR                6 (just_created)
-                           292 POP_JUMP_FORWARD_IF_FALSE    78 (to 450)
-               
-               195         294 LOAD_FAST                0 (self)
-                           296 LOAD_ATTR                4 (_respawned_scratches)
-                           306 LOAD_METHOD              7 (discard)
-                           328 LOAD_FAST                6 (item)
-                           330 LOAD_ATTR                8 (uid)
-                           340 PRECALL                  1
-                           344 CALL                     1
-                           354 POP_TOP
-               
-               196         356 LOAD_FAST                0 (self)
-                           358 LOAD_METHOD              9 (run_hide)
-                           380 LOAD_FAST                6 (item)
-                           382 LOAD_ATTR                8 (uid)
-                           392 LOAD_CONST               4 (True)
-                           394 KW_NAMES                 5
-                           396 PRECALL                  2
-                           400 CALL                     2
-                           410 GET_AWAITABLE            0
-                           412 LOAD_CONST               0 (None)
-                       >>  414 SEND                     3 (to 422)
-                           416 YIELD_VALUE
-                           418 RESUME                   3
-                           420 JUMP_BACKWARD_NO_INTERRUPT     4 (to 414)
-                       >>  422 POP_TOP
-               
-               197         424 LOAD_CONST               6 (False)
-                           426 LOAD_FAST                6 (item)
-                           428 STORE_ATTR               6 (just_created)
-                           438 LOAD_CONST               0 (None)
-                           440 RETURN_VALUE
-               
-               189     >>  442 LOAD_CONST               0 (None)
-                           444 RETURN_VALUE
-               
-               194     >>  446 LOAD_CONST               0 (None)
-                           448 RETURN_VALUE
-                       >>  450 LOAD_CONST               0 (None)
-                           452 RETURN_VALUE
+               250         224 LOAD_FAST                0 (self)
+                           226 LOAD_METHOD              6 (updateScratchInfo)
+                           248 PRECALL                  0
+                           252 CALL                     0
+                           262 GET_AWAITABLE            0
+                           264 LOAD_CONST               4 (None)
+                       >>  266 SEND                     3 (to 274)
+                           268 YIELD_VALUE
+                           270 RESUME                   3
+                           272 JUMP_BACKWARD_NO_INTERRUPT     4 (to 266)
+                       >>  274 POP_TOP
+               
+               251     >>  276 LOAD_FAST                0 (self)
+                           278 LOAD_ATTR                2 (scratches_by_address)
+                           288 LOAD_METHOD              3 (get)
+                           310 LOAD_FAST                2 (addr)
+                           312 PRECALL                  1
+                           316 CALL                     1
+                           326 STORE_FAST               6 (item)
+               
+               252     >>  328 LOAD_FAST                6 (item)
+                           330 POP_JUMP_FORWARD_IF_FALSE   128 (to 588)
+                           332 LOAD_FAST                6 (item)
+                           334 LOAD_ATTR                7 (just_created)
+                           344 POP_JUMP_FORWARD_IF_FALSE   123 (to 592)
+               
+               253         346 LOAD_FAST                6 (item)
+                           348 LOAD_ATTR                8 (uid)
+                           358 LOAD_FAST                0 (self)
+                           360 LOAD_ATTR                9 (_new_scratches)
+                           370 CONTAINS_OP              0
+                           372 POP_JUMP_FORWARD_IF_FALSE    34 (to 442)
+               
+               254         374 LOAD_FAST                0 (self)
+                           376 LOAD_METHOD             10 (run_hide)
+                           398 LOAD_FAST                6 (item)
+                           400 LOAD_ATTR                8 (uid)
+                           410 LOAD_CONST               5 (True)
+                           412 KW_NAMES                 6
+                           414 PRECALL                  2
+                           418 CALL                     2
+                           428 GET_AWAITABLE            0
+                           430 LOAD_CONST               4 (None)
+                       >>  432 SEND                     3 (to 440)
+                           434 YIELD_VALUE
+                           436 RESUME                   3
+                           438 JUMP_BACKWARD_NO_INTERRUPT     4 (to 432)
+                       >>  440 POP_TOP
+               
+               255     >>  442 LOAD_FAST                0 (self)
+                           444 LOAD_ATTR                9 (_new_scratches)
+                           454 LOAD_METHOD             11 (discard)
+                           476 LOAD_FAST                6 (item)
+                           478 LOAD_ATTR                8 (uid)
+                           488 PRECALL                  1
+                           492 CALL                     1
+                           502 POP_TOP
+               
+               256         504 LOAD_FAST                0 (self)
+                           506 LOAD_ATTR                4 (_respawned_scratches)
+                           516 LOAD_METHOD             11 (discard)
+                           538 LOAD_FAST                6 (item)
+                           540 LOAD_ATTR                8 (uid)
+                           550 PRECALL                  1
+                           554 CALL                     1
+                           564 POP_TOP
+               
+               257         566 LOAD_CONST               7 (False)
+                           568 LOAD_FAST                6 (item)
+                           570 STORE_ATTR               7 (just_created)
+                           580 LOAD_CONST               4 (None)
+                           582 RETURN_VALUE
+               
+               245     >>  584 LOAD_CONST               4 (None)
+                           586 RETURN_VALUE
+               
+               252     >>  588 LOAD_CONST               4 (None)
+                           590 RETURN_VALUE
+                       >>  592 LOAD_CONST               4 (None)
+                           594 RETURN_VALUE
                consts
-                  None
+                  'open windows hook'
                   ','
                   3
                   'special'
+                  None
                   True
                   ('force',)
                   False
-               names      ('split', 'startswith', 'scratches_by_address', 'get', '_respawned_scratches', 'updateScratchInfo', 'just_created', 'discard', 'uid', 'run_hide')
-               varnames   ('self', 'params', 'addr', 'wrkspc', 'kls', 'title', 'item')
+               names      ('split', 'startswith', 'scratches_by_address', 'get', '_respawned_scratches', '_alternative_lookup', 'updateScratchInfo', 'just_created', 'uid', '_new_scratches', 'run_hide', 'discard')
+               varnames   ('self', 'params', 'addr', 'wrkspc', '_kls', '_title', 'item')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'event_openwindow'
-               firstlineno 187
-               lnotab 0x060136012a01340112013401340112013e01440112f80405
+               firstlineno 242
+               lnotab
+                  0x060236012a013401120234013401340112011c0144013e013e0112f404
+                  07
             'uid'
             code
                argcount  : 2
                nlocals   : 3
-               stacksize : 4
+               stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c01a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d017c006a010000000000000000a0
                   0200000000000000000000000000000000000000007c01a6010000ab0100
-                  000000000000007d027c0273147407000000000000000000007c019b0064
-                  019d02a6010000ab0100000000000000000100640253007c026a04000000
-                  0000000000721d7c00a00500000000000000000000000000000000000000
-                  007c01a6010000ab010000000000000000830064027b0356009703860401
-                  00640253007c00a00600000000000000000000000000000000000000007c
-                  01a6010000ab010000000000000000830064027b03560097038604010064
-                  025300
-               199           0 RETURN_GENERATOR
+                  000000000000007d027c02731d7c006a030000000000000000a004000000
+                  000000000000000000000000000000000064017c01a6020000ab02000000
+                  00000000000100640253007c006a030000000000000000a0050000000000
+                  00000000000000000000000000000064037c017c026a0600000000000000
+                  00a6030000ab03000000000000000001007c026a06000000000000000072
+                  1d7c00a00700000000000000000000000000000000000000007c01a60100
+                  00ab010000000000000000830064027b035600970386040100640253007c
+                  00a00800000000000000000000000000000000000000007c01a6010000ab
+                  010000000000000000830064027b03560097038604010064025300
+               259           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               201           6 LOAD_FAST                1 (uid)
+               261           6 LOAD_FAST                1 (uid)
                              8 LOAD_METHOD              0 (strip)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 STORE_FAST               1 (uid)
                
-               202          46 LOAD_FAST                0 (self)
+               262          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                1 (scratches)
                             58 LOAD_METHOD              2 (get)
                             80 LOAD_FAST                1 (uid)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               2 (item)
                
-               203          98 LOAD_FAST                2 (item)
-                           100 POP_JUMP_FORWARD_IF_TRUE    20 (to 142)
+               263          98 LOAD_FAST                2 (item)
+                           100 POP_JUMP_FORWARD_IF_TRUE    29 (to 160)
                
-               204         102 LOAD_GLOBAL              7 (NULL + print)
-                           114 LOAD_FAST                1 (uid)
-                           116 FORMAT_VALUE             0
-                           118 LOAD_CONST               1 (' is not configured')
-                           120 BUILD_STRING             2
-                           122 PRECALL                  1
-                           126 CALL                     1
-                           136 POP_TOP
-               
-               205         138 LOAD_CONST               2 (None)
-                           140 RETURN_VALUE
-               
-               206     >>  142 LOAD_FAST                2 (item)
-                           144 LOAD_ATTR                4 (visible)
-                           154 POP_JUMP_FORWARD_IF_FALSE    29 (to 214)
-               
-               207         156 LOAD_FAST                0 (self)
-                           158 LOAD_METHOD              5 (run_hide)
-                           180 LOAD_FAST                1 (uid)
-                           182 PRECALL                  1
-                           186 CALL                     1
-                           196 GET_AWAITABLE            0
-                           198 LOAD_CONST               2 (None)
-                       >>  200 SEND                     3 (to 208)
-                           202 YIELD_VALUE
-                           204 RESUME                   3
-                           206 JUMP_BACKWARD_NO_INTERRUPT     4 (to 200)
-                       >>  208 POP_TOP
-                           210 LOAD_CONST               2 (None)
-                           212 RETURN_VALUE
-               
-               209     >>  214 LOAD_FAST                0 (self)
-                           216 LOAD_METHOD              6 (run_show)
-                           238 LOAD_FAST                1 (uid)
-                           240 PRECALL                  1
-                           244 CALL                     1
-                           254 GET_AWAITABLE            0
-                           256 LOAD_CONST               2 (None)
-                       >>  258 SEND                     3 (to 266)
-                           260 YIELD_VALUE
-                           262 RESUME                   3
-                           264 JUMP_BACKWARD_NO_INTERRUPT     4 (to 258)
-                       >>  266 POP_TOP
-                           268 LOAD_CONST               2 (None)
-                           270 RETURN_VALUE
+               264         102 LOAD_FAST                0 (self)
+                           104 LOAD_ATTR                3 (log)
+                           114 LOAD_METHOD              4 (warning)
+                           136 LOAD_CONST               1 ('%s is not configured')
+                           138 LOAD_FAST                1 (uid)
+                           140 PRECALL                  2
+                           144 CALL                     2
+                           154 POP_TOP
+               
+               265         156 LOAD_CONST               2 (None)
+                           158 RETURN_VALUE
+               
+               266     >>  160 LOAD_FAST                0 (self)
+                           162 LOAD_ATTR                3 (log)
+                           172 LOAD_METHOD              5 (debug)
+                           194 LOAD_CONST               3 ('%s is visible = %s')
+                           196 LOAD_FAST                1 (uid)
+                           198 LOAD_FAST                2 (item)
+                           200 LOAD_ATTR                6 (visible)
+                           210 PRECALL                  3
+                           214 CALL                     3
+                           224 POP_TOP
+               
+               267         226 LOAD_FAST                2 (item)
+                           228 LOAD_ATTR                6 (visible)
+                           238 POP_JUMP_FORWARD_IF_FALSE    29 (to 298)
+               
+               268         240 LOAD_FAST                0 (self)
+                           242 LOAD_METHOD              7 (run_hide)
+                           264 LOAD_FAST                1 (uid)
+                           266 PRECALL                  1
+                           270 CALL                     1
+                           280 GET_AWAITABLE            0
+                           282 LOAD_CONST               2 (None)
+                       >>  284 SEND                     3 (to 292)
+                           286 YIELD_VALUE
+                           288 RESUME                   3
+                           290 JUMP_BACKWARD_NO_INTERRUPT     4 (to 284)
+                       >>  292 POP_TOP
+                           294 LOAD_CONST               2 (None)
+                           296 RETURN_VALUE
+               
+               270     >>  298 LOAD_FAST                0 (self)
+                           300 LOAD_METHOD              8 (run_show)
+                           322 LOAD_FAST                1 (uid)
+                           324 PRECALL                  1
+                           328 CALL                     1
+                           338 GET_AWAITABLE            0
+                           340 LOAD_CONST               2 (None)
+                       >>  342 SEND                     3 (to 350)
+                           344 YIELD_VALUE
+                           346 RESUME                   3
+                           348 JUMP_BACKWARD_NO_INTERRUPT     4 (to 342)
+                       >>  350 POP_TOP
+                           352 LOAD_CONST               2 (None)
+                           354 RETURN_VALUE
                consts
                   '<name> toggles visibility of scratchpad "name" '
-                  ' is not configured'
+                  '%s is not configured'
                   None
-               names      ('strip', 'scratches', 'get', 'print', 'visible', 'run_hide', 'run_show')
+                  '%s is visible = %s'
+               names      ('strip', 'scratches', 'get', 'log', 'warning', 'debug', 'visible', 'run_hide', 'run_show')
                varnames   ('self', 'uid', 'item')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'run_toggle'
-               firstlineno 199
-               lnotab 0x0602280134010401240104010e013a02
+               firstlineno 259
+               lnotab 0x06022801340104013601040142010e013a02
+            code
+               argcount  : 3
+               nlocals   : 5
+               stacksize : 6
+               flags     : 131
+               code
+                  0x4b000100970064017c026a0000000000000000007a0000007d037c026a
+                  010000000000000000a00200000000000000000000000000000000000000
+                  006402a6010000ab0100000000000000007d047c04804764047c026a0300
+                  000000000000007601721b7c00a004000000000000000000000000000000
+                  00000000007c02a6010000ab010000000000000000830064037b03560097
+                  0386040100740b0000000000000000000064057c026a0300000000000000
+                  006404190000000000000000006406190000000000000000007a050000a6
+                  010000ab0100000000000000007d047c0164076b0200000000721c740d00
+                  00000000000000000064087c049b0064097c039b009d04a6010000ab0100
+                  00000000000000830064037b0356009703860401006e657c01640a6b0200
+                  000000721c740d00000000000000000000640b7c049b0064097c039b009d
+                  04a6010000ab010000000000000000830064037b0356009703860401006e
+                  437c01640c6b0200000000721c740d00000000000000000000640d7c049b
+                  00640e7c039b009d04a6010000ab010000000000000000830064037b0356
+                  009703860401006e217c01640f6b0200000000721b740d00000000000000
+                  00000064107c049b00640e7c039b009d04a6010000ab0100000000000000
+                  00830064037b0356009703860401007c026a0700000000000000007c006a
+                  08000000000000000076007202640353007413000000000000000000006a
+                  0a00000000000000006411a6010000ab010000000000000000830064037b
+                  03560097038604010064035300
+               272           0 RETURN_GENERATOR
+                             2 POP_TOP
+                             4 RESUME                   0
+               
+               274           6 LOAD_CONST               1 ('address:0x')
+                             8 LOAD_FAST                2 (scratch)
+                            10 LOAD_ATTR                0 (address)
+                            20 BINARY_OP                0 (+)
+                            24 STORE_FAST               3 (addr)
+               
+               275          26 LOAD_FAST                2 (scratch)
+                            28 LOAD_ATTR                1 (conf)
+                            38 LOAD_METHOD              2 (get)
+                            60 LOAD_CONST               2 ('offset')
+                            62 PRECALL                  1
+                            66 CALL                     1
+                            76 STORE_FAST               4 (offset)
+               
+               276          78 LOAD_FAST                4 (offset)
+                            80 POP_JUMP_FORWARD_IF_NOT_NONE    71 (to 224)
+               
+               277          82 LOAD_CONST               4 ('size')
+                            84 LOAD_FAST                2 (scratch)
+                            86 LOAD_ATTR                3 (client_info)
+                            96 CONTAINS_OP              1
+                            98 POP_JUMP_FORWARD_IF_FALSE    27 (to 154)
+               
+               278         100 LOAD_FAST                0 (self)
+                           102 LOAD_METHOD              4 (updateScratchInfo)
+                           124 LOAD_FAST                2 (scratch)
+                           126 PRECALL                  1
+                           130 CALL                     1
+                           140 GET_AWAITABLE            0
+                           142 LOAD_CONST               3 (None)
+                       >>  144 SEND                     3 (to 152)
+                           146 YIELD_VALUE
+                           148 RESUME                   3
+                           150 JUMP_BACKWARD_NO_INTERRUPT     4 (to 144)
+                       >>  152 POP_TOP
+               
+               280     >>  154 LOAD_GLOBAL             11 (NULL + int)
+                           166 LOAD_CONST               5 (1.3)
+                           168 LOAD_FAST                2 (scratch)
+                           170 LOAD_ATTR                3 (client_info)
+                           180 LOAD_CONST               4 ('size')
+                           182 BINARY_SUBSCR
+                           192 LOAD_CONST               6 (1)
+                           194 BINARY_SUBSCR
+                           204 BINARY_OP                5 (*)
+                           208 PRECALL                  1
+                           212 CALL                     1
+                           222 STORE_FAST               4 (offset)
+               
+               282     >>  224 LOAD_FAST                1 (animation_type)
+                           226 LOAD_CONST               7 ('fromtop')
+                           228 COMPARE_OP               2 (==)
+                           234 POP_JUMP_FORWARD_IF_FALSE    28 (to 292)
+               
+               283         236 LOAD_GLOBAL             13 (NULL + hyprctl)
+                           248 LOAD_CONST               8 ('movewindowpixel 0 -')
+                           250 LOAD_FAST                4 (offset)
+                           252 FORMAT_VALUE             0
+                           254 LOAD_CONST               9 (',')
+                           256 LOAD_FAST                3 (addr)
+                           258 FORMAT_VALUE             0
+                           260 BUILD_STRING             4
+                           262 PRECALL                  1
+                           266 CALL                     1
+                           276 GET_AWAITABLE            0
+                           278 LOAD_CONST               3 (None)
+                       >>  280 SEND                     3 (to 288)
+                           282 YIELD_VALUE
+                           284 RESUME                   3
+                           286 JUMP_BACKWARD_NO_INTERRUPT     4 (to 280)
+                       >>  288 POP_TOP
+                           290 JUMP_FORWARD           101 (to 494)
+               
+               284     >>  292 LOAD_FAST                1 (animation_type)
+                           294 LOAD_CONST              10 ('frombottom')
+                           296 COMPARE_OP               2 (==)
+                           302 POP_JUMP_FORWARD_IF_FALSE    28 (to 360)
+               
+               285         304 LOAD_GLOBAL             13 (NULL + hyprctl)
+                           316 LOAD_CONST              11 ('movewindowpixel 0 ')
+                           318 LOAD_FAST                4 (offset)
+                           320 FORMAT_VALUE             0
+                           322 LOAD_CONST               9 (',')
+                           324 LOAD_FAST                3 (addr)
+                           326 FORMAT_VALUE             0
+                           328 BUILD_STRING             4
+                           330 PRECALL                  1
+                           334 CALL                     1
+                           344 GET_AWAITABLE            0
+                           346 LOAD_CONST               3 (None)
+                       >>  348 SEND                     3 (to 356)
+                           350 YIELD_VALUE
+                           352 RESUME                   3
+                           354 JUMP_BACKWARD_NO_INTERRUPT     4 (to 348)
+                       >>  356 POP_TOP
+                           358 JUMP_FORWARD            67 (to 494)
+               
+               286     >>  360 LOAD_FAST                1 (animation_type)
+                           362 LOAD_CONST              12 ('fromleft')
+                           364 COMPARE_OP               2 (==)
+                           370 POP_JUMP_FORWARD_IF_FALSE    28 (to 428)
+               
+               287         372 LOAD_GLOBAL             13 (NULL + hyprctl)
+                           384 LOAD_CONST              13 ('movewindowpixel -')
+                           386 LOAD_FAST                4 (offset)
+                           388 FORMAT_VALUE             0
+                           390 LOAD_CONST              14 (' 0,')
+                           392 LOAD_FAST                3 (addr)
+                           394 FORMAT_VALUE             0
+                           396 BUILD_STRING             4
+                           398 PRECALL                  1
+                           402 CALL                     1
+                           412 GET_AWAITABLE            0
+                           414 LOAD_CONST               3 (None)
+                       >>  416 SEND                     3 (to 424)
+                           418 YIELD_VALUE
+                           420 RESUME                   3
+                           422 JUMP_BACKWARD_NO_INTERRUPT     4 (to 416)
+                       >>  424 POP_TOP
+                           426 JUMP_FORWARD            33 (to 494)
+               
+               288     >>  428 LOAD_FAST                1 (animation_type)
+                           430 LOAD_CONST              15 ('fromright')
+                           432 COMPARE_OP               2 (==)
+                           438 POP_JUMP_FORWARD_IF_FALSE    27 (to 494)
+               
+               289         440 LOAD_GLOBAL             13 (NULL + hyprctl)
+                           452 LOAD_CONST              16 ('movewindowpixel ')
+                           454 LOAD_FAST                4 (offset)
+                           456 FORMAT_VALUE             0
+                           458 LOAD_CONST              14 (' 0,')
+                           460 LOAD_FAST                3 (addr)
+                           462 FORMAT_VALUE             0
+                           464 BUILD_STRING             4
+                           466 PRECALL                  1
+                           470 CALL                     1
+                           480 GET_AWAITABLE            0
+                           482 LOAD_CONST               3 (None)
+                       >>  484 SEND                     3 (to 492)
+                           486 YIELD_VALUE
+                           488 RESUME                   3
+                           490 JUMP_BACKWARD_NO_INTERRUPT     4 (to 484)
+                       >>  492 POP_TOP
+               
+               291     >>  494 LOAD_FAST                2 (scratch)
+                           496 LOAD_ATTR                7 (uid)
+                           506 LOAD_FAST                0 (self)
+                           508 LOAD_ATTR                8 (transitioning_scratches)
+                           518 CONTAINS_OP              0
+                           520 POP_JUMP_FORWARD_IF_FALSE     2 (to 526)
+               
+               292         522 LOAD_CONST               3 (None)
+                           524 RETURN_VALUE
+               
+               293     >>  526 LOAD_GLOBAL             19 (NULL + asyncio)
+                           538 LOAD_ATTR               10 (sleep)
+                           548 LOAD_CONST              17 (0.2)
+                           550 PRECALL                  1
+                           554 CALL                     1
+                           564 GET_AWAITABLE            0
+                           566 LOAD_CONST               3 (None)
+                       >>  568 SEND                     3 (to 576)
+                           570 YIELD_VALUE
+                           572 RESUME                   3
+                           574 JUMP_BACKWARD_NO_INTERRUPT     4 (to 568)
+                       >>  576 POP_TOP
+                           578 LOAD_CONST               3 (None)
+                           580 RETURN_VALUE
+               consts
+                  'animate hiding a scratchpad'
+                  'address:0x'
+                  'offset'
+                  None
+                  'size'
+                  1.3
+                  1
+                  'fromtop'
+                  'movewindowpixel 0 -'
+                  ','
+                  'frombottom'
+                  'movewindowpixel 0 '
+                  'fromleft'
+                  'movewindowpixel -'
+                  ' 0,'
+                  'fromright'
+                  'movewindowpixel '
+                  0.2
+               names      ('address', 'conf', 'get', 'client_info', 'updateScratchInfo', 'int', 'hyprctl', 'uid', 'transitioning_scratches', 'asyncio', 'sleep')
+               varnames   ('self', 'animation_type', 'scratch', 'addr', 'offset')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
+               name       '_anim_hide'
+               firstlineno 272
+               lnotab
+                  0x06021401340104011201360246020c0138010c0138010c0138010c0136
+                  021c010401
             'scratch'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
                flags     : 131
                code
-                  0x4b00010097007c0180b27401000000000000000000006401a6010000ab
-                  010000000000000000830064007b0356009703860444005d9a7d02740300
+                  0x4b00010097007c0180b27401000000000000000000006402a6010000ab
+                  010000000000000000830064017b0356009703860444005d9a7d02740300
                   0000000000000000007c02740400000000000000000000a6020000ab0200
                   0000000000000073024a0082017c006a030000000000000000a004000000
-                  00000000000000000000000000000000007c026402190000000000000000
-                  0064036400850219000000000000000000a6010000ab0100000000000000
+                  00000000000000000000000000000000007c026403190000000000000000
+                  0064046401850219000000000000000000a6010000ab0100000000000000
                   007d017c01733a7c006a050000000000000000a004000000000000000000
-                  00000000000000000000007c02640419000000000000000000a6010000ab
+                  00000000000000000000007c02640519000000000000000000a6010000ab
                   0100000000000000007d017c0172187c017c006a0300000000000000007c
-                  02640219000000000000000000640364008502190000000000000000003c
+                  02640319000000000000000000640464018502190000000000000000003c
                   0000007c01721b7c01a00600000000000000000000000000000000000000
-                  007c02a6010000ab010000000000000000830064007b0356009703860401
-                  008c9b6400530064027c016a0700000000000000007601700d7c016a0800
+                  007c02a6010000ab010000000000000000830064017b0356009703860401
+                  008c9b6401530064037c016a0700000000000000007601700d7c016a0800
                   000000000000007c006a03000000000000000076017d037c01a006000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
-                  00830064007b0356009703860401007c03721f7c017c006a030000000000
-                  0000007c016a070000000000000000640219000000000000000000640364
-                  008502190000000000000000003c0000006400530064005300
-               211           0 RETURN_GENERATOR
+                  00830064017b0356009703860401007c03721f7c017c006a030000000000
+                  0000007c016a070000000000000000640319000000000000000000640464
+                  018502190000000000000000003c0000006401530064015300
+               295           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               212           6 LOAD_FAST                1 (scratch)
+               298           6 LOAD_FAST                1 (scratch)
                              8 POP_JUMP_FORWARD_IF_NOT_NONE   178 (to 366)
                
-               213          10 LOAD_GLOBAL              1 (NULL + hyprctlJSON)
-                            22 LOAD_CONST               1 ('clients')
+               299          10 LOAD_GLOBAL              1 (NULL + hyprctlJSON)
+                            22 LOAD_CONST               2 ('clients')
                             24 PRECALL                  1
                             28 CALL                     1
                             38 GET_AWAITABLE            0
-                            40 LOAD_CONST               0 (None)
+                            40 LOAD_CONST               1 (None)
                        >>   42 SEND                     3 (to 50)
                             44 YIELD_VALUE
                             46 RESUME                   3
                             48 JUMP_BACKWARD_NO_INTERRUPT     4 (to 42)
                        >>   50 GET_ITER
                        >>   52 FOR_ITER               154 (to 362)
                             54 STORE_FAST               2 (client)
                
-               214          56 LOAD_GLOBAL              3 (NULL + isinstance)
+               300          56 LOAD_GLOBAL              3 (NULL + isinstance)
                             68 LOAD_FAST                2 (client)
                             70 LOAD_GLOBAL              4 (dict)
                             82 PRECALL                  2
                             86 CALL                     2
                             96 POP_JUMP_FORWARD_IF_TRUE     2 (to 102)
                             98 LOAD_ASSERTION_ERROR
                            100 RAISE_VARARGS            1
                
-               215     >>  102 LOAD_FAST                0 (self)
+               301     >>  102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                3 (scratches_by_address)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_FAST                2 (client)
-                           138 LOAD_CONST               2 ('address')
+                           138 LOAD_CONST               3 ('address')
                            140 BINARY_SUBSCR
-                           150 LOAD_CONST               3 (2)
-                           152 LOAD_CONST               0 (None)
+                           150 LOAD_CONST               4 (2)
+                           152 LOAD_CONST               1 (None)
                            154 BUILD_SLICE              2
                            156 BINARY_SUBSCR
                            166 PRECALL                  1
                            170 CALL                     1
                            180 STORE_FAST               1 (scratch)
                
-               216         182 LOAD_FAST                1 (scratch)
+               302         182 LOAD_FAST                1 (scratch)
                            184 POP_JUMP_FORWARD_IF_TRUE    58 (to 302)
                
-               217         186 LOAD_FAST                0 (self)
+               303         186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                5 (scratches_by_pid)
                            198 LOAD_METHOD              4 (get)
                            220 LOAD_FAST                2 (client)
-                           222 LOAD_CONST               4 ('pid')
+                           222 LOAD_CONST               5 ('pid')
                            224 BINARY_SUBSCR
                            234 PRECALL                  1
                            238 CALL                     1
                            248 STORE_FAST               1 (scratch)
                
-               218         250 LOAD_FAST                1 (scratch)
+               304         250 LOAD_FAST                1 (scratch)
                            252 POP_JUMP_FORWARD_IF_FALSE    24 (to 302)
                
-               219         254 LOAD_FAST                1 (scratch)
+               305         254 LOAD_FAST                1 (scratch)
                            256 LOAD_FAST                0 (self)
                            258 LOAD_ATTR                3 (scratches_by_address)
                            268 LOAD_FAST                2 (client)
-                           270 LOAD_CONST               2 ('address')
+                           270 LOAD_CONST               3 ('address')
                            272 BINARY_SUBSCR
-                           282 LOAD_CONST               3 (2)
-                           284 LOAD_CONST               0 (None)
+                           282 LOAD_CONST               4 (2)
+                           284 LOAD_CONST               1 (None)
                            286 BUILD_SLICE              2
                            288 BINARY_SUBSCR
                            298 STORE_SUBSCR
                
-               220     >>  302 LOAD_FAST                1 (scratch)
+               306     >>  302 LOAD_FAST                1 (scratch)
                            304 POP_JUMP_FORWARD_IF_FALSE    27 (to 360)
                
-               221         306 LOAD_FAST                1 (scratch)
+               307         306 LOAD_FAST                1 (scratch)
                            308 LOAD_METHOD              6 (updateClientInfo)
                            330 LOAD_FAST                2 (client)
                            332 PRECALL                  1
                            336 CALL                     1
                            346 GET_AWAITABLE            0
-                           348 LOAD_CONST               0 (None)
+                           348 LOAD_CONST               1 (None)
                        >>  350 SEND                     3 (to 358)
                            352 YIELD_VALUE
                            354 RESUME                   3
                            356 JUMP_BACKWARD_NO_INTERRUPT     4 (to 350)
                        >>  358 POP_TOP
                        >>  360 JUMP_BACKWARD          155 (to 52)
                
-               213     >>  362 LOAD_CONST               0 (None)
+               299     >>  362 LOAD_CONST               1 (None)
                            364 RETURN_VALUE
                
-               223     >>  366 LOAD_CONST               2 ('address')
+               309     >>  366 LOAD_CONST               3 ('address')
                            368 LOAD_FAST                1 (scratch)
-                           370 LOAD_ATTR                7 (clientInfo)
+                           370 LOAD_ATTR                7 (client_info)
                            380 CONTAINS_OP              1
                            382 JUMP_IF_TRUE_OR_POP     13 (to 410)
                
-               224         384 LOAD_FAST                1 (scratch)
+               310         384 LOAD_FAST                1 (scratch)
                            386 LOAD_ATTR                8 (address)
                            396 LOAD_FAST                0 (self)
                            398 LOAD_ATTR                3 (scratches_by_address)
                            408 CONTAINS_OP              1
                
-               223     >>  410 STORE_FAST               3 (add_to_address_book)
+               309     >>  410 STORE_FAST               3 (add_to_address_book)
                
-               226         412 LOAD_FAST                1 (scratch)
+               312         412 LOAD_FAST                1 (scratch)
                            414 LOAD_METHOD              6 (updateClientInfo)
                            436 PRECALL                  0
                            440 CALL                     0
                            450 GET_AWAITABLE            0
-                           452 LOAD_CONST               0 (None)
+                           452 LOAD_CONST               1 (None)
                        >>  454 SEND                     3 (to 462)
                            456 YIELD_VALUE
                            458 RESUME                   3
                            460 JUMP_BACKWARD_NO_INTERRUPT     4 (to 454)
                        >>  462 POP_TOP
                
-               227         464 LOAD_FAST                3 (add_to_address_book)
+               313         464 LOAD_FAST                3 (add_to_address_book)
                            466 POP_JUMP_FORWARD_IF_FALSE    31 (to 530)
                
-               228         468 LOAD_FAST                1 (scratch)
+               314         468 LOAD_FAST                1 (scratch)
                            470 LOAD_FAST                0 (self)
                            472 LOAD_ATTR                3 (scratches_by_address)
                            482 LOAD_FAST                1 (scratch)
-                           484 LOAD_ATTR                7 (clientInfo)
-                           494 LOAD_CONST               2 ('address')
+                           484 LOAD_ATTR                7 (client_info)
+                           494 LOAD_CONST               3 ('address')
                            496 BINARY_SUBSCR
-                           506 LOAD_CONST               3 (2)
-                           508 LOAD_CONST               0 (None)
+                           506 LOAD_CONST               4 (2)
+                           508 LOAD_CONST               1 (None)
                            510 BUILD_SLICE              2
                            512 BINARY_SUBSCR
                            522 STORE_SUBSCR
-                           526 LOAD_CONST               0 (None)
+                           526 LOAD_CONST               1 (None)
                            528 RETURN_VALUE
                
-               227     >>  530 LOAD_CONST               0 (None)
+               313     >>  530 LOAD_CONST               1 (None)
                            532 RETURN_VALUE
                consts
+                  'Update every scratchpads information if no `scratch` given,\n        else update a specific scratchpad info'
                   None
                   'clients'
                   'address'
                   2
                   'pid'
-               names      ('hyprctlJSON', 'isinstance', 'dict', 'scratches_by_address', 'get', 'scratches_by_pid', 'updateClientInfo', 'clientInfo', 'address')
+               names      ('hyprctlJSON', 'isinstance', 'dict', 'scratches_by_address', 'get', 'scratches_by_pid', 'updateClientInfo', 'client_info', 'address')
                varnames   ('self', 'scratch', 'client', 'add_to_address_book')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'updateScratchInfo'
-               firstlineno 211
+               firstlineno 295
                lnotab
-                  0x060104012e012e0150010401400104013001040138f8040a12011aff02
+                  0x060304012e012e0150010401400104013001040138f8040a12011aff02
                   03340104013eff
-            False
             code
                argcount  : 4
-               nlocals   : 8
+               nlocals   : 7
                stacksize : 6
                flags     : 131
                code
                   0x4b00010097007c01a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d017c006a010000000000000000a0
                   0200000000000000000000000000000000000000007c01a6010000ab0100
-                  000000000000007d047c0473147407000000000000000000007c019b0064
-                  019d02a6010000ab0100000000000000000100640253007c046a04000000
-                  000000000073167c0273147407000000000000000000007c019b0064039d
-                  02a6010000ab01000000000000000001006402530064047c045f04000000
-                  000000000064057c046a0500000000000000007a0000007d057c046a0600
+                  000000000000007d047c04731d7c006a030000000000000000a004000000
+                  000000000000000000000000000000000064017c01a6020000ab02000000
+                  00000000000100640253007c046a050000000000000000731f7c02731d7c
+                  006a030000000000000000a0040000000000000000000000000000000000
+                  00000064037c01a6020000ab0200000000000000000100640253007c006a
+                  030000000000000000a00600000000000000000000000000000000000000
+                  0064047c01a6020000ab020000000000000000010064057c045f05000000
+                  000000000064067c046a0700000000000000007a0000007d057c046a0800
                   00000000000000a002000000000000000000000000000000000000000064
-                  066407a6020000ab020000000000000000a0070000000000000000000000
-                  000000000000000000a6000000ab0000000000000000007d067c06900172
-                  0f7c046a060000000000000000a002000000000000000000000000000000
-                  00000000006408a6010000ab0100000000000000007d077c07804764097c
-                  046a0800000000000000007601721b7c00a0090000000000000000000000
-                  0000000000000000007c04a6010000ab010000000000000000830064027b
-                  035600970386040100741500000000000000000000640a7c046a08000000
-                  0000000000640919000000000000000000640b190000000000000000007a
-                  050000a6010000ab0100000000000000007d077c06640c6b020000000072
-                  1c741700000000000000000000640d7c079b00640e7c059b009d04a60100
-                  00ab010000000000000000830064027b0356009703860401006e657c0664
-                  0f6b0200000000721c74170000000000000000000064107c079b00640e7c
-                  059b009d04a6010000ab010000000000000000830064027b035600970386
-                  0401006e437c0664116b0200000000721c74170000000000000000000064
-                  127c079b0064137c059b009d04a6010000ab010000000000000000830064
-                  027b0356009703860401006e217c0664146b0200000000721b7417000000
-                  0000000000000064157c079b0064137c059b009d04a6010000ab01000000
-                  0000000000830064027b0356009703860401007c017c006a0c0000000000
-                  0000007600720264025300741b000000000000000000006a0e0000000000
-                  0000006416a6010000ab010000000000000000830064027b035600970386
-                  0401007c017c006a0c00000000000000007601721b741700000000000000
-                  00000064177c019b00640e7c059b009d04a6010000ab0100000000000000
-                  00830064027b0356009703860401007c06724d7c017c006a0f0000000000
-                  000000760072467c03734664187c006a0f00000000000000007c01190000
-                  000000000000007600723974170000000000000000000064197c006a0f00
-                  000000000000007c01190000000000000000006418190000000000000000
-                  009b009d02a6010000ab010000000000000000830064027b035600970386
-                  0401007c006a0f00000000000000007c013d006402530064025300640253
-                  006402530064025300
-               230           0 RETURN_GENERATOR
+                  076408a6020000ab020000000000000000a0090000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007d067c06721c7c
+                  00a00a00000000000000000000000000000000000000007c067c04a60200
+                  00ab020000000000000000830064027b0356009703860401007c017c006a
+                  0b00000000000000007601721b74190000000000000000000064097c019b
+                  00640a7c059b009d04a6010000ab010000000000000000830064027b0356
+                  009703860401007c06724d7c017c006a0d0000000000000000760072467c
+                  037346640b7c006a0d00000000000000007c011900000000000000000076
+                  007239741900000000000000000000640c7c006a0d00000000000000007c
+                  0119000000000000000000640b190000000000000000009b009d02a60100
+                  00ab010000000000000000830064027b0356009703860401007c006a0d00
+                  000000000000007c013d0064025300640253006402530064025300640253
+                  00
+               316           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               232           6 LOAD_FAST                1 (uid)
+               318           6 LOAD_FAST                1 (uid)
                              8 LOAD_METHOD              0 (strip)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 STORE_FAST               1 (uid)
                
-               233          46 LOAD_FAST                0 (self)
+               319          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                1 (scratches)
                             58 LOAD_METHOD              2 (get)
                             80 LOAD_FAST                1 (uid)
                             82 PRECALL                  1
                             86 CALL                     1
-                            96 STORE_FAST               4 (item)
+                            96 STORE_FAST               4 (scratch)
                
-               234          98 LOAD_FAST                4 (item)
-                           100 POP_JUMP_FORWARD_IF_TRUE    20 (to 142)
-               
-               235         102 LOAD_GLOBAL              7 (NULL + print)
-                           114 LOAD_FAST                1 (uid)
-                           116 FORMAT_VALUE             0
-                           118 LOAD_CONST               1 (' is not configured')
-                           120 BUILD_STRING             2
-                           122 PRECALL                  1
-                           126 CALL                     1
-                           136 POP_TOP
-               
-               236         138 LOAD_CONST               2 (None)
-                           140 RETURN_VALUE
-               
-               237     >>  142 LOAD_FAST                4 (item)
-                           144 LOAD_ATTR                4 (visible)
-                           154 POP_JUMP_FORWARD_IF_TRUE    22 (to 200)
-                           156 LOAD_FAST                2 (force)
-                           158 POP_JUMP_FORWARD_IF_TRUE    20 (to 200)
-               
-               238         160 LOAD_GLOBAL              7 (NULL + print)
-                           172 LOAD_FAST                1 (uid)
-                           174 FORMAT_VALUE             0
-                           176 LOAD_CONST               3 (' is already hidden')
-                           178 BUILD_STRING             2
-                           180 PRECALL                  1
-                           184 CALL                     1
-                           194 POP_TOP
-               
-               239         196 LOAD_CONST               2 (None)
-                           198 RETURN_VALUE
-               
-               240     >>  200 LOAD_CONST               4 (False)
-                           202 LOAD_FAST                4 (item)
-                           204 STORE_ATTR               4 (visible)
-               
-               241         214 LOAD_CONST               5 ('address:0x')
-                           216 LOAD_FAST                4 (item)
-                           218 LOAD_ATTR                5 (address)
-                           228 BINARY_OP                0 (+)
-                           232 STORE_FAST               5 (addr)
+               320          98 LOAD_FAST                4 (scratch)
+                           100 POP_JUMP_FORWARD_IF_TRUE    29 (to 160)
                
-               242         234 LOAD_FAST                4 (item)
-                           236 LOAD_ATTR                6 (conf)
-                           246 LOAD_METHOD              2 (get)
-                           268 LOAD_CONST               6 ('animation')
-                           270 LOAD_CONST               7 ('')
-                           272 PRECALL                  2
-                           276 CALL                     2
-                           286 LOAD_METHOD              7 (lower)
-                           308 PRECALL                  0
-                           312 CALL                     0
-                           322 STORE_FAST               6 (animation_type)
-               
-               243         324 LOAD_FAST                6 (animation_type)
-                           326 EXTENDED_ARG             1
-                           328 POP_JUMP_FORWARD_IF_FALSE   271 (to 872)
-               
-               244         330 LOAD_FAST                4 (item)
-                           332 LOAD_ATTR                6 (conf)
-                           342 LOAD_METHOD              2 (get)
-                           364 LOAD_CONST               8 ('offset')
-                           366 PRECALL                  1
-                           370 CALL                     1
-                           380 STORE_FAST               7 (offset)
-               
-               245         382 LOAD_FAST                7 (offset)
-                           384 POP_JUMP_FORWARD_IF_NOT_NONE    71 (to 528)
-               
-               246         386 LOAD_CONST               9 ('size')
-                           388 LOAD_FAST                4 (item)
-                           390 LOAD_ATTR                8 (clientInfo)
-                           400 CONTAINS_OP              1
-                           402 POP_JUMP_FORWARD_IF_FALSE    27 (to 458)
-               
-               247         404 LOAD_FAST                0 (self)
-                           406 LOAD_METHOD              9 (updateScratchInfo)
-                           428 LOAD_FAST                4 (item)
-                           430 PRECALL                  1
-                           434 CALL                     1
-                           444 GET_AWAITABLE            0
-                           446 LOAD_CONST               2 (None)
-                       >>  448 SEND                     3 (to 456)
-                           450 YIELD_VALUE
-                           452 RESUME                   3
-                           454 JUMP_BACKWARD_NO_INTERRUPT     4 (to 448)
-                       >>  456 POP_TOP
-               
-               249     >>  458 LOAD_GLOBAL             21 (NULL + int)
-                           470 LOAD_CONST              10 (1.3)
-                           472 LOAD_FAST                4 (item)
-                           474 LOAD_ATTR                8 (clientInfo)
-                           484 LOAD_CONST               9 ('size')
-                           486 BINARY_SUBSCR
-                           496 LOAD_CONST              11 (1)
-                           498 BINARY_SUBSCR
-                           508 BINARY_OP                5 (*)
-                           512 PRECALL                  1
-                           516 CALL                     1
-                           526 STORE_FAST               7 (offset)
-               
-               251     >>  528 LOAD_FAST                6 (animation_type)
-                           530 LOAD_CONST              12 ('fromtop')
-                           532 COMPARE_OP               2 (==)
-                           538 POP_JUMP_FORWARD_IF_FALSE    28 (to 596)
-               
-               252         540 LOAD_GLOBAL             23 (NULL + hyprctl)
-                           552 LOAD_CONST              13 ('movewindowpixel 0 -')
-                           554 LOAD_FAST                7 (offset)
-                           556 FORMAT_VALUE             0
-                           558 LOAD_CONST              14 (',')
-                           560 LOAD_FAST                5 (addr)
-                           562 FORMAT_VALUE             0
-                           564 BUILD_STRING             4
-                           566 PRECALL                  1
-                           570 CALL                     1
-                           580 GET_AWAITABLE            0
-                           582 LOAD_CONST               2 (None)
-                       >>  584 SEND                     3 (to 592)
-                           586 YIELD_VALUE
-                           588 RESUME                   3
-                           590 JUMP_BACKWARD_NO_INTERRUPT     4 (to 584)
-                       >>  592 POP_TOP
-                           594 JUMP_FORWARD           101 (to 798)
-               
-               253     >>  596 LOAD_FAST                6 (animation_type)
-                           598 LOAD_CONST              15 ('frombottom')
-                           600 COMPARE_OP               2 (==)
-                           606 POP_JUMP_FORWARD_IF_FALSE    28 (to 664)
-               
-               254         608 LOAD_GLOBAL             23 (NULL + hyprctl)
-                           620 LOAD_CONST              16 ('movewindowpixel 0 ')
-                           622 LOAD_FAST                7 (offset)
-                           624 FORMAT_VALUE             0
-                           626 LOAD_CONST              14 (',')
-                           628 LOAD_FAST                5 (addr)
-                           630 FORMAT_VALUE             0
-                           632 BUILD_STRING             4
-                           634 PRECALL                  1
-                           638 CALL                     1
-                           648 GET_AWAITABLE            0
-                           650 LOAD_CONST               2 (None)
-                       >>  652 SEND                     3 (to 660)
-                           654 YIELD_VALUE
-                           656 RESUME                   3
-                           658 JUMP_BACKWARD_NO_INTERRUPT     4 (to 652)
-                       >>  660 POP_TOP
-                           662 JUMP_FORWARD            67 (to 798)
-               
-               255     >>  664 LOAD_FAST                6 (animation_type)
-                           666 LOAD_CONST              17 ('fromleft')
-                           668 COMPARE_OP               2 (==)
-                           674 POP_JUMP_FORWARD_IF_FALSE    28 (to 732)
-               
-               256         676 LOAD_GLOBAL             23 (NULL + hyprctl)
-                           688 LOAD_CONST              18 ('movewindowpixel -')
-                           690 LOAD_FAST                7 (offset)
-                           692 FORMAT_VALUE             0
-                           694 LOAD_CONST              19 (' 0,')
-                           696 LOAD_FAST                5 (addr)
-                           698 FORMAT_VALUE             0
-                           700 BUILD_STRING             4
-                           702 PRECALL                  1
-                           706 CALL                     1
-                           716 GET_AWAITABLE            0
-                           718 LOAD_CONST               2 (None)
-                       >>  720 SEND                     3 (to 728)
-                           722 YIELD_VALUE
-                           724 RESUME                   3
-                           726 JUMP_BACKWARD_NO_INTERRUPT     4 (to 720)
-                       >>  728 POP_TOP
-                           730 JUMP_FORWARD            33 (to 798)
-               
-               257     >>  732 LOAD_FAST                6 (animation_type)
-                           734 LOAD_CONST              20 ('fromright')
-                           736 COMPARE_OP               2 (==)
-                           742 POP_JUMP_FORWARD_IF_FALSE    27 (to 798)
-               
-               258         744 LOAD_GLOBAL             23 (NULL + hyprctl)
-                           756 LOAD_CONST              21 ('movewindowpixel ')
-                           758 LOAD_FAST                7 (offset)
-                           760 FORMAT_VALUE             0
-                           762 LOAD_CONST              19 (' 0,')
-                           764 LOAD_FAST                5 (addr)
-                           766 FORMAT_VALUE             0
-                           768 BUILD_STRING             4
-                           770 PRECALL                  1
-                           774 CALL                     1
-                           784 GET_AWAITABLE            0
-                           786 LOAD_CONST               2 (None)
-                       >>  788 SEND                     3 (to 796)
-                           790 YIELD_VALUE
-                           792 RESUME                   3
-                           794 JUMP_BACKWARD_NO_INTERRUPT     4 (to 788)
-                       >>  796 POP_TOP
-               
-               260     >>  798 LOAD_FAST                1 (uid)
-                           800 LOAD_FAST                0 (self)
-                           802 LOAD_ATTR               12 (transitioning_scratches)
-                           812 CONTAINS_OP              0
-                           814 POP_JUMP_FORWARD_IF_FALSE     2 (to 820)
-               
-               261         816 LOAD_CONST               2 (None)
-                           818 RETURN_VALUE
-               
-               262     >>  820 LOAD_GLOBAL             27 (NULL + asyncio)
-                           832 LOAD_ATTR               14 (sleep)
-                           842 LOAD_CONST              22 (0.2)
-                           844 PRECALL                  1
-                           848 CALL                     1
-                           858 GET_AWAITABLE            0
-                           860 LOAD_CONST               2 (None)
-                       >>  862 SEND                     3 (to 870)
-                           864 YIELD_VALUE
-                           866 RESUME                   3
-                           868 JUMP_BACKWARD_NO_INTERRUPT     4 (to 862)
-                       >>  870 POP_TOP
-               
-               264     >>  872 LOAD_FAST                1 (uid)
-                           874 LOAD_FAST                0 (self)
-                           876 LOAD_ATTR               12 (transitioning_scratches)
-                           886 CONTAINS_OP              1
-                           888 POP_JUMP_FORWARD_IF_FALSE    27 (to 944)
-               
-               265         890 LOAD_GLOBAL             23 (NULL + hyprctl)
-                           902 LOAD_CONST              23 ('movetoworkspacesilent special:scratch_')
-                           904 LOAD_FAST                1 (uid)
-                           906 FORMAT_VALUE             0
-                           908 LOAD_CONST              14 (',')
-                           910 LOAD_FAST                5 (addr)
-                           912 FORMAT_VALUE             0
-                           914 BUILD_STRING             4
-                           916 PRECALL                  1
-                           920 CALL                     1
-                           930 GET_AWAITABLE            0
-                           932 LOAD_CONST               2 (None)
-                       >>  934 SEND                     3 (to 942)
-                           936 YIELD_VALUE
-                           938 RESUME                   3
-                           940 JUMP_BACKWARD_NO_INTERRUPT     4 (to 934)
-                       >>  942 POP_TOP
-               
-               268     >>  944 LOAD_FAST                6 (animation_type)
-               
-               267         946 POP_JUMP_FORWARD_IF_FALSE    77 (to 1102)
-               
-               268         948 LOAD_FAST                1 (uid)
-                           950 LOAD_FAST                0 (self)
-                           952 LOAD_ATTR               15 (focused_window_tracking)
-                           962 CONTAINS_OP              0
-                           964 POP_JUMP_FORWARD_IF_FALSE    70 (to 1106)
-               
-               270         966 LOAD_FAST                3 (autohide)
-                           968 POP_JUMP_FORWARD_IF_TRUE    70 (to 1110)
-                           970 LOAD_CONST              24 ('address')
-                           972 LOAD_FAST                0 (self)
-                           974 LOAD_ATTR               15 (focused_window_tracking)
-                           984 LOAD_FAST                1 (uid)
-                           986 BINARY_SUBSCR
-                           996 CONTAINS_OP              0
-                           998 POP_JUMP_FORWARD_IF_FALSE    57 (to 1114)
-               
-               271        1000 LOAD_GLOBAL             23 (NULL + hyprctl)
-               
-               272        1012 LOAD_CONST              25 ('focuswindow address:')
-                          1014 LOAD_FAST                0 (self)
-                          1016 LOAD_ATTR               15 (focused_window_tracking)
-                          1026 LOAD_FAST                1 (uid)
-                          1028 BINARY_SUBSCR
-                          1038 LOAD_CONST              24 ('address')
-                          1040 BINARY_SUBSCR
-                          1050 FORMAT_VALUE             0
-                          1052 BUILD_STRING             2
-               
-               271        1054 PRECALL                  1
-                          1058 CALL                     1
-                          1068 GET_AWAITABLE            0
-                          1070 LOAD_CONST               2 (None)
-                       >> 1072 SEND                     3 (to 1080)
-                          1074 YIELD_VALUE
-                          1076 RESUME                   3
-                          1078 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1072)
-                       >> 1080 POP_TOP
-               
-               274        1082 LOAD_FAST                0 (self)
-                          1084 LOAD_ATTR               15 (focused_window_tracking)
-                          1094 LOAD_FAST                1 (uid)
-                          1096 DELETE_SUBSCR
-                          1098 LOAD_CONST               2 (None)
-                          1100 RETURN_VALUE
-               
-               267     >> 1102 LOAD_CONST               2 (None)
-                          1104 RETURN_VALUE
-               
-               268     >> 1106 LOAD_CONST               2 (None)
-                          1108 RETURN_VALUE
-               
-               270     >> 1110 LOAD_CONST               2 (None)
-                          1112 RETURN_VALUE
-                       >> 1114 LOAD_CONST               2 (None)
-                          1116 RETURN_VALUE
+               321         102 LOAD_FAST                0 (self)
+                           104 LOAD_ATTR                3 (log)
+                           114 LOAD_METHOD              4 (warning)
+                           136 LOAD_CONST               1 ('%s is not configured')
+                           138 LOAD_FAST                1 (uid)
+                           140 PRECALL                  2
+                           144 CALL                     2
+                           154 POP_TOP
+               
+               322         156 LOAD_CONST               2 (None)
+                           158 RETURN_VALUE
+               
+               323     >>  160 LOAD_FAST                4 (scratch)
+                           162 LOAD_ATTR                5 (visible)
+                           172 POP_JUMP_FORWARD_IF_TRUE    31 (to 236)
+                           174 LOAD_FAST                2 (force)
+                           176 POP_JUMP_FORWARD_IF_TRUE    29 (to 236)
+               
+               324         178 LOAD_FAST                0 (self)
+                           180 LOAD_ATTR                3 (log)
+                           190 LOAD_METHOD              4 (warning)
+                           212 LOAD_CONST               3 ('%s is already hidden')
+                           214 LOAD_FAST                1 (uid)
+                           216 PRECALL                  2
+                           220 CALL                     2
+                           230 POP_TOP
+               
+               325         232 LOAD_CONST               2 (None)
+                           234 RETURN_VALUE
+               
+               326     >>  236 LOAD_FAST                0 (self)
+                           238 LOAD_ATTR                3 (log)
+                           248 LOAD_METHOD              6 (info)
+                           270 LOAD_CONST               4 ('Hiding %s')
+                           272 LOAD_FAST                1 (uid)
+                           274 PRECALL                  2
+                           278 CALL                     2
+                           288 POP_TOP
+               
+               327         290 LOAD_CONST               5 (False)
+                           292 LOAD_FAST                4 (scratch)
+                           294 STORE_ATTR               5 (visible)
+               
+               328         304 LOAD_CONST               6 ('address:0x')
+                           306 LOAD_FAST                4 (scratch)
+                           308 LOAD_ATTR                7 (address)
+                           318 BINARY_OP                0 (+)
+                           322 STORE_FAST               5 (addr)
+               
+               329         324 LOAD_FAST                4 (scratch)
+                           326 LOAD_ATTR                8 (conf)
+                           336 LOAD_METHOD              2 (get)
+                           358 LOAD_CONST               7 ('animation')
+                           360 LOAD_CONST               8 ('')
+                           362 PRECALL                  2
+                           366 CALL                     2
+                           376 LOAD_METHOD              9 (lower)
+                           398 PRECALL                  0
+                           402 CALL                     0
+                           412 STORE_FAST               6 (animation_type)
+               
+               330         414 LOAD_FAST                6 (animation_type)
+                           416 POP_JUMP_FORWARD_IF_FALSE    28 (to 474)
+               
+               331         418 LOAD_FAST                0 (self)
+                           420 LOAD_METHOD             10 (_anim_hide)
+                           442 LOAD_FAST                6 (animation_type)
+                           444 LOAD_FAST                4 (scratch)
+                           446 PRECALL                  2
+                           450 CALL                     2
+                           460 GET_AWAITABLE            0
+                           462 LOAD_CONST               2 (None)
+                       >>  464 SEND                     3 (to 472)
+                           466 YIELD_VALUE
+                           468 RESUME                   3
+                           470 JUMP_BACKWARD_NO_INTERRUPT     4 (to 464)
+                       >>  472 POP_TOP
+               
+               333     >>  474 LOAD_FAST                1 (uid)
+                           476 LOAD_FAST                0 (self)
+                           478 LOAD_ATTR               11 (transitioning_scratches)
+                           488 CONTAINS_OP              1
+                           490 POP_JUMP_FORWARD_IF_FALSE    27 (to 546)
+               
+               334         492 LOAD_GLOBAL             25 (NULL + hyprctl)
+                           504 LOAD_CONST               9 ('movetoworkspacesilent special:scratch_')
+                           506 LOAD_FAST                1 (uid)
+                           508 FORMAT_VALUE             0
+                           510 LOAD_CONST              10 (',')
+                           512 LOAD_FAST                5 (addr)
+                           514 FORMAT_VALUE             0
+                           516 BUILD_STRING             4
+                           518 PRECALL                  1
+                           522 CALL                     1
+                           532 GET_AWAITABLE            0
+                           534 LOAD_CONST               2 (None)
+                       >>  536 SEND                     3 (to 544)
+                           538 YIELD_VALUE
+                           540 RESUME                   3
+                           542 JUMP_BACKWARD_NO_INTERRUPT     4 (to 536)
+                       >>  544 POP_TOP
+               
+               337     >>  546 LOAD_FAST                6 (animation_type)
+               
+               336         548 POP_JUMP_FORWARD_IF_FALSE    77 (to 704)
+               
+               337         550 LOAD_FAST                1 (uid)
+                           552 LOAD_FAST                0 (self)
+                           554 LOAD_ATTR               13 (focused_window_tracking)
+                           564 CONTAINS_OP              0
+                           566 POP_JUMP_FORWARD_IF_FALSE    70 (to 708)
+               
+               339         568 LOAD_FAST                3 (autohide)
+                           570 POP_JUMP_FORWARD_IF_TRUE    70 (to 712)
+                           572 LOAD_CONST              11 ('address')
+                           574 LOAD_FAST                0 (self)
+                           576 LOAD_ATTR               13 (focused_window_tracking)
+                           586 LOAD_FAST                1 (uid)
+                           588 BINARY_SUBSCR
+                           598 CONTAINS_OP              0
+                           600 POP_JUMP_FORWARD_IF_FALSE    57 (to 716)
+               
+               340         602 LOAD_GLOBAL             25 (NULL + hyprctl)
+               
+               341         614 LOAD_CONST              12 ('focuswindow address:')
+                           616 LOAD_FAST                0 (self)
+                           618 LOAD_ATTR               13 (focused_window_tracking)
+                           628 LOAD_FAST                1 (uid)
+                           630 BINARY_SUBSCR
+                           640 LOAD_CONST              11 ('address')
+                           642 BINARY_SUBSCR
+                           652 FORMAT_VALUE             0
+                           654 BUILD_STRING             2
+               
+               340         656 PRECALL                  1
+                           660 CALL                     1
+                           670 GET_AWAITABLE            0
+                           672 LOAD_CONST               2 (None)
+                       >>  674 SEND                     3 (to 682)
+                           676 YIELD_VALUE
+                           678 RESUME                   3
+                           680 JUMP_BACKWARD_NO_INTERRUPT     4 (to 674)
+                       >>  682 POP_TOP
+               
+               343         684 LOAD_FAST                0 (self)
+                           686 LOAD_ATTR               13 (focused_window_tracking)
+                           696 LOAD_FAST                1 (uid)
+                           698 DELETE_SUBSCR
+                           700 LOAD_CONST               2 (None)
+                           702 RETURN_VALUE
+               
+               336     >>  704 LOAD_CONST               2 (None)
+                           706 RETURN_VALUE
+               
+               337     >>  708 LOAD_CONST               2 (None)
+                           710 RETURN_VALUE
+               
+               339     >>  712 LOAD_CONST               2 (None)
+                           714 RETURN_VALUE
+                       >>  716 LOAD_CONST               2 (None)
+                           718 RETURN_VALUE
                consts
                   '<name> hides scratchpad "name" '
-                  ' is not configured'
+                  '%s is not configured'
                   None
-                  ' is already hidden'
+                  '%s is already hidden'
+                  'Hiding %s'
                   False
                   'address:0x'
                   'animation'
                   ''
-                  'offset'
-                  'size'
-                  1.3
-                  1
-                  'fromtop'
-                  'movewindowpixel 0 -'
-                  ','
-                  'frombottom'
-                  'movewindowpixel 0 '
-                  'fromleft'
-                  'movewindowpixel -'
-                  ' 0,'
-                  'fromright'
-                  'movewindowpixel '
-                  0.2
                   'movetoworkspacesilent special:scratch_'
+                  ','
                   'address'
                   'focuswindow address:'
-               names      ('strip', 'scratches', 'get', 'print', 'visible', 'address', 'conf', 'lower', 'clientInfo', 'updateScratchInfo', 'int', 'hyprctl', 'transitioning_scratches', 'asyncio', 'sleep', 'focused_window_tracking')
-               varnames   ('self', 'uid', 'force', 'autohide', 'item', 'addr', 'animation_type', 'offset')
+               names      ('strip', 'scratches', 'get', 'log', 'warning', 'visible', 'info', 'address', 'conf', 'lower', '_anim_hide', 'transitioning_scratches', 'hyprctl', 'focused_window_tracking')
+               varnames   ('self', 'uid', 'force', 'autohide', 'scratch', 'addr', 'animation_type')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'run_hide'
-               firstlineno 230
+               firstlineno 316
                lnotab
-                  0x0602280134010401240104011201240104010e0114015a010601340104
-                  011201360246020c0138010c0138010c0138010c01360212010401340212
-                  01360302ff0201120222010c012aff1c0314f904010402
+                  0x06022801340104013601040112013601040136010e0114015a01040138
+                  021201360302ff0201120222010c012aff1c0314f904010402
             code
                argcount  : 3
                nlocals   : 10
                stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c01a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d017c006a010000000000000000a0
                   0200000000000000000000000000000000000000007c01a6010000ab0100
-                  000000000000007d037407000000000000000000006401a6010000ab0100
-                  00000000000000830064027b035600970386047c006a0400000000000000
-                  007c013c0000007c037314740b000000000000000000007c019b0064039d
-                  02a6010000ab0100000000000000000100640253007c036a060000000000
-                  00000072167c027314740b000000000000000000007c019b0064049d02a6
-                  010000ab0100000000000000000100640253007c03a00700000000000000
-                  00000000000000000000000000a6000000ab00000000000000000073a874
-                  0b000000000000000000007c019b0064059d02a6010000ab010000000000
-                  00000001007c006a0800000000000000007c0119000000000000000000a0
-                  090000000000000000000000000000000000000000a6000000ab00000000
-                  000000000001007c036a0a00000000000000007c006a0b00000000000000
-                  007600720d7c006a0b00000000000000007c036a0a00000000000000003d
-                  007c036a0c00000000000000007c006a0d00000000000000007600720d7c
-                  006a0d00000000000000007c036a0c00000000000000003d007c00a00e00
-                  000000000000000000000000000000000000007c01a6010000ab01000000
-                  000000000001007c017c006a0f0000000000000000760072237421000000
-                  000000000000006a1100000000000000006406a6010000ab010000000000
-                  000000830064027b0356009703860401007c017c006a0f00000000000000
-                  007600b02364077c035f0600000000000000007425000000000000000000
-                  00a6000000ab000000000000000000830064027b035600970386047d047c
-                  0473024a0082017c00a01300000000000000000000000000000000000000
-                  007c03a6010000ab010000000000000000830064027b0356009703860401
-                  0064087c036a0c00000000000000007a0000007d057c036a140000000000
-                  000000a00200000000000000000000000000000000000000006409640aa6
-                  020000ab020000000000000000a015000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007d067c04640b1900000000
-                  0000000000640c190000000000000000007d077c006a1600000000000000
-                  00a01700000000000000000000000000000000000000007c01a6010000ab
-                  0100000000000000000100743100000000000000000000640d7c019b0064
-                  0e7c04640f190000000000000000009b009d04a6010000ab010000000000
-                  000000830064027b03560097038604010074310000000000000000000064
-                  107c079b0064117c059b009d04a6010000ab010000000000000000830064
-                  027b0356009703860401007c06724e7c036a140000000000000000a00200
-                  000000000000000000000000000000000000006412743200000000000000
-                  000000a6020000ab0200000000000000007d087435000000000000000000
-                  007436000000000000000000007c06a6020000ab0200000000000000007d
-                  0902007c097c047c036a1c00000000000000007c057c08a6040000ab0400
-                  00000000000000830064027b035600970386040100743100000000000000
-                  00000064137c059b009d02a6010000ab010000000000000000830064027b
-                  0356009703860401007421000000000000000000006a1100000000000000
-                  006414a6010000ab010000000000000000830064027b0356009703860401
-                  007c006a160000000000000000a01d000000000000000000000000000000
-                  00000000007c01a6010000ab010000000000000000010064025300
-               276           0 RETURN_GENERATOR
+                  000000000000007d03740700000000000000000000740800000000000000
+                  000000740a00000000000000000000740c00000000000000000000660219
+                  000000000000000000740f000000000000000000006401a6010000ab0100
+                  00000000000000830064027b03560097038604a6020000ab020000000000
+                  0000007c006a0800000000000000007c013c0000007c03731d7c006a0900
+                  00000000000000a00a000000000000000000000000000000000000000064
+                  037c01a6020000ab0200000000000000000100640253007c036a0b000000
+                  0000000000721f7c02731d7c006a090000000000000000a00a0000000000
+                  00000000000000000000000000000064047c01a6020000ab020000000000
+                  0000000100640253007c006a090000000000000000a00c00000000000000
+                  0000000000000000000000000064057c01a6020000ab0200000000000000
+                  0001007c03a00d0000000000000000000000000000000000000000a60000
+                  00ab00000000000000000073c07c006a090000000000000000a00c000000
+                  000000000000000000000000000000000064067c01a6020000ab02000000
+                  000000000001007c017c006a0e00000000000000007600721f7c006a0e00
+                  000000000000007c0119000000000000000000a00f000000000000000000
+                  0000000000000000000000a6000000ab00000000000000000001007c036a
+                  1000000000000000007c006a1100000000000000007600720d7c006a1100
+                  000000000000007c036a1000000000000000003d007c036a120000000000
+                  0000007c006a1300000000000000007600720d7c006a1300000000000000
+                  007c036a1200000000000000003d007c00a0140000000000000000000000
+                  0000000000000000007c01a6010000ab010000000000000000830064027b
+                  0356009703860401007c017c006a15000000000000000076007223742d00
+                  0000000000000000006a1700000000000000006407a6010000ab01000000
+                  0000000000830064027b0356009703860401007c017c006a150000000000
+                  0000007600b02364087c035f0b0000000000000000743100000000000000
+                  000000a6000000ab000000000000000000830064027b035600970386047d
+                  047c0473024a0082017c00a0190000000000000000000000000000000000
+                  0000007c03a6010000ab010000000000000000830064027b035600970386
+                  04010064097c036a1200000000000000007a0000007d057c036a1a000000
+                  0000000000a0020000000000000000000000000000000000000000640a64
+                  0ba6020000ab020000000000000000a01b00000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007d067c04640c190000
+                  00000000000000640d190000000000000000007d077c006a1c0000000000
+                  000000a01d00000000000000000000000000000000000000007c01a60100
+                  00ab0100000000000000000100743d00000000000000000000640e7c019b
+                  00640f7c046410190000000000000000009b009d04a6010000ab01000000
+                  0000000000830064027b035600970386040100743d000000000000000000
+                  0064117c079b0064127c059b009d04a6010000ab01000000000000000083
+                  0064027b0356009703860401007c06724e7c036a1a0000000000000000a0
+                  0200000000000000000000000000000000000000006413743e0000000000
+                  0000000000a6020000ab0200000000000000007d08744100000000000000
+                  0000007442000000000000000000007c06a6020000ab0200000000000000
+                  007d0902007c097c047c036a2200000000000000007c057c08a6040000ab
+                  040000000000000000830064027b035600970386040100743d0000000000
+                  000000000064147c059b009d02a6010000ab010000000000000000830064
+                  027b035600970386040100742d000000000000000000006a170000000000
+                  0000006415a6010000ab010000000000000000830064027b035600970386
+                  0401007c006a1c0000000000000000a02300000000000000000000000000
+                  000000000000007c01a6010000ab010000000000000000010064025300
+               345           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               278           6 LOAD_FAST                1 (uid)
+               347           6 LOAD_FAST                1 (uid)
                              8 LOAD_METHOD              0 (strip)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 STORE_FAST               1 (uid)
                
-               279          46 LOAD_FAST                0 (self)
+               348          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                1 (scratches)
                             58 LOAD_METHOD              2 (get)
                             80 LOAD_FAST                1 (uid)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               3 (item)
                
-               281          98 LOAD_GLOBAL              7 (NULL + hyprctlJSON)
-                           110 LOAD_CONST               1 ('activewindow')
-                           112 PRECALL                  1
-                           116 CALL                     1
-                           126 GET_AWAITABLE            0
-                           128 LOAD_CONST               2 (None)
-                       >>  130 SEND                     3 (to 138)
-                           132 YIELD_VALUE
-                           134 RESUME                   3
-                           136 JUMP_BACKWARD_NO_INTERRUPT     4 (to 130)
-                       >>  138 LOAD_FAST                0 (self)
-                           140 LOAD_ATTR                4 (focused_window_tracking)
-                           150 LOAD_FAST                1 (uid)
-                           152 STORE_SUBSCR
-               
-               283         156 LOAD_FAST                3 (item)
-                           158 POP_JUMP_FORWARD_IF_TRUE    20 (to 200)
-               
-               284         160 LOAD_GLOBAL             11 (NULL + print)
-                           172 LOAD_FAST                1 (uid)
-                           174 FORMAT_VALUE             0
-                           176 LOAD_CONST               3 (' is not configured')
-                           178 BUILD_STRING             2
-                           180 PRECALL                  1
-                           184 CALL                     1
-                           194 POP_TOP
-               
-               285         196 LOAD_CONST               2 (None)
-                           198 RETURN_VALUE
-               
-               287     >>  200 LOAD_FAST                3 (item)
-                           202 LOAD_ATTR                6 (visible)
-                           212 POP_JUMP_FORWARD_IF_FALSE    22 (to 258)
-                           214 LOAD_FAST                2 (force)
-                           216 POP_JUMP_FORWARD_IF_TRUE    20 (to 258)
+               350          98 LOAD_GLOBAL              7 (NULL + cast)
                
-               288         218 LOAD_GLOBAL             11 (NULL + print)
-                           230 LOAD_FAST                1 (uid)
-                           232 FORMAT_VALUE             0
-                           234 LOAD_CONST               4 (' is already visible')
-                           236 BUILD_STRING             2
-                           238 PRECALL                  1
-                           242 CALL                     1
-                           252 POP_TOP
-               
-               289         254 LOAD_CONST               2 (None)
-                           256 RETURN_VALUE
-               
-               291     >>  258 LOAD_FAST                3 (item)
-                           260 LOAD_METHOD              7 (isAlive)
-                           282 PRECALL                  0
-                           286 CALL                     0
-                           296 POP_JUMP_FORWARD_IF_TRUE   168 (to 634)
-               
-               292         298 LOAD_GLOBAL             11 (NULL + print)
-                           310 LOAD_FAST                1 (uid)
-                           312 FORMAT_VALUE             0
-                           314 LOAD_CONST               5 (' is not running, restarting...')
-                           316 BUILD_STRING             2
-                           318 PRECALL                  1
-                           322 CALL                     1
-                           332 POP_TOP
+               351         110 LOAD_GLOBAL              8 (dict)
+                           122 LOAD_GLOBAL             10 (str)
+                           134 LOAD_GLOBAL             12 (Any)
+                           146 BUILD_TUPLE              2
+                           148 BINARY_SUBSCR
+                           158 LOAD_GLOBAL             15 (NULL + hyprctlJSON)
+                           170 LOAD_CONST               1 ('activewindow')
+                           172 PRECALL                  1
+                           176 CALL                     1
+                           186 GET_AWAITABLE            0
+                           188 LOAD_CONST               2 (None)
+                       >>  190 SEND                     3 (to 198)
+                           192 YIELD_VALUE
+                           194 RESUME                   3
+                           196 JUMP_BACKWARD_NO_INTERRUPT     4 (to 190)
+               
+               350     >>  198 PRECALL                  2
+                           202 CALL                     2
+                           212 LOAD_FAST                0 (self)
+                           214 LOAD_ATTR                8 (focused_window_tracking)
+                           224 LOAD_FAST                1 (uid)
+                           226 STORE_SUBSCR
+               
+               354         230 LOAD_FAST                3 (item)
+                           232 POP_JUMP_FORWARD_IF_TRUE    29 (to 292)
+               
+               355         234 LOAD_FAST                0 (self)
+                           236 LOAD_ATTR                9 (log)
+                           246 LOAD_METHOD             10 (warning)
+                           268 LOAD_CONST               3 ('%s is not configured')
+                           270 LOAD_FAST                1 (uid)
+                           272 PRECALL                  2
+                           276 CALL                     2
+                           286 POP_TOP
+               
+               356         288 LOAD_CONST               2 (None)
+                           290 RETURN_VALUE
                
-               293         334 LOAD_FAST                0 (self)
-                           336 LOAD_ATTR                8 (procs)
+               358     >>  292 LOAD_FAST                3 (item)
+                           294 LOAD_ATTR               11 (visible)
+                           304 POP_JUMP_FORWARD_IF_FALSE    31 (to 368)
+                           306 LOAD_FAST                2 (force)
+                           308 POP_JUMP_FORWARD_IF_TRUE    29 (to 368)
+               
+               359         310 LOAD_FAST                0 (self)
+                           312 LOAD_ATTR                9 (log)
+                           322 LOAD_METHOD             10 (warning)
+                           344 LOAD_CONST               4 ('%s is already visible')
                            346 LOAD_FAST                1 (uid)
-                           348 BINARY_SUBSCR
-                           358 LOAD_METHOD              9 (kill)
-                           380 PRECALL                  0
-                           384 CALL                     0
-                           394 POP_TOP
-               
-               294         396 LOAD_FAST                3 (item)
-                           398 LOAD_ATTR               10 (pid)
-                           408 LOAD_FAST                0 (self)
-                           410 LOAD_ATTR               11 (scratches_by_pid)
-                           420 CONTAINS_OP              0
-                           422 POP_JUMP_FORWARD_IF_FALSE    13 (to 450)
-               
-               295         424 LOAD_FAST                0 (self)
-                           426 LOAD_ATTR               11 (scratches_by_pid)
-                           436 LOAD_FAST                3 (item)
-                           438 LOAD_ATTR               10 (pid)
-                           448 DELETE_SUBSCR
-               
-               296     >>  450 LOAD_FAST                3 (item)
-                           452 LOAD_ATTR               12 (address)
-                           462 LOAD_FAST                0 (self)
-                           464 LOAD_ATTR               13 (scratches_by_address)
-                           474 CONTAINS_OP              0
-                           476 POP_JUMP_FORWARD_IF_FALSE    13 (to 504)
-               
-               297         478 LOAD_FAST                0 (self)
-                           480 LOAD_ATTR               13 (scratches_by_address)
-                           490 LOAD_FAST                3 (item)
-                           492 LOAD_ATTR               12 (address)
-                           502 DELETE_SUBSCR
-               
-               298     >>  504 LOAD_FAST                0 (self)
-                           506 LOAD_METHOD             14 (start_scratch_command)
-                           528 LOAD_FAST                1 (uid)
-                           530 PRECALL                  1
-                           534 CALL                     1
-                           544 POP_TOP
-               
-               299         546 LOAD_FAST                1 (uid)
-                           548 LOAD_FAST                0 (self)
-                           550 LOAD_ATTR               15 (_respawned_scratches)
-                           560 CONTAINS_OP              0
-                           562 POP_JUMP_FORWARD_IF_FALSE    35 (to 634)
-               
-               300     >>  564 LOAD_GLOBAL             33 (NULL + asyncio)
-                           576 LOAD_ATTR               17 (sleep)
-                           586 LOAD_CONST               6 (0.05)
-                           588 PRECALL                  1
-                           592 CALL                     1
-                           602 GET_AWAITABLE            0
-                           604 LOAD_CONST               2 (None)
-                       >>  606 SEND                     3 (to 614)
-                           608 YIELD_VALUE
-                           610 RESUME                   3
-                           612 JUMP_BACKWARD_NO_INTERRUPT     4 (to 606)
-                       >>  614 POP_TOP
-               
-               299         616 LOAD_FAST                1 (uid)
-                           618 LOAD_FAST                0 (self)
-                           620 LOAD_ATTR               15 (_respawned_scratches)
-                           630 CONTAINS_OP              0
-                           632 POP_JUMP_BACKWARD_IF_TRUE    35 (to 564)
+                           348 PRECALL                  2
+                           352 CALL                     2
+                           362 POP_TOP
+               
+               360         364 LOAD_CONST               2 (None)
+                           366 RETURN_VALUE
+               
+               362     >>  368 LOAD_FAST                0 (self)
+                           370 LOAD_ATTR                9 (log)
+                           380 LOAD_METHOD             12 (info)
+                           402 LOAD_CONST               5 ('Showing %s')
+                           404 LOAD_FAST                1 (uid)
+                           406 PRECALL                  2
+                           410 CALL                     2
+                           420 POP_TOP
+               
+               364         422 LOAD_FAST                3 (item)
+                           424 LOAD_METHOD             13 (isAlive)
+                           446 PRECALL                  0
+                           450 CALL                     0
+                           460 POP_JUMP_FORWARD_IF_TRUE   192 (to 846)
+               
+               365         462 LOAD_FAST                0 (self)
+                           464 LOAD_ATTR                9 (log)
+                           474 LOAD_METHOD             12 (info)
+                           496 LOAD_CONST               6 ('%s is not running, restarting...')
+                           498 LOAD_FAST                1 (uid)
+                           500 PRECALL                  2
+                           504 CALL                     2
+                           514 POP_TOP
+               
+               366         516 LOAD_FAST                1 (uid)
+                           518 LOAD_FAST                0 (self)
+                           520 LOAD_ATTR               14 (procs)
+                           530 CONTAINS_OP              0
+                           532 POP_JUMP_FORWARD_IF_FALSE    31 (to 596)
+               
+               367         534 LOAD_FAST                0 (self)
+                           536 LOAD_ATTR               14 (procs)
+                           546 LOAD_FAST                1 (uid)
+                           548 BINARY_SUBSCR
+                           558 LOAD_METHOD             15 (kill)
+                           580 PRECALL                  0
+                           584 CALL                     0
+                           594 POP_TOP
+               
+               368     >>  596 LOAD_FAST                3 (item)
+                           598 LOAD_ATTR               16 (pid)
+                           608 LOAD_FAST                0 (self)
+                           610 LOAD_ATTR               17 (scratches_by_pid)
+                           620 CONTAINS_OP              0
+                           622 POP_JUMP_FORWARD_IF_FALSE    13 (to 650)
                
-               302     >>  634 LOAD_CONST               7 (True)
+               369         624 LOAD_FAST                0 (self)
+                           626 LOAD_ATTR               17 (scratches_by_pid)
                            636 LOAD_FAST                3 (item)
-                           638 STORE_ATTR               6 (visible)
+                           638 LOAD_ATTR               16 (pid)
+                           648 DELETE_SUBSCR
                
-               303         648 LOAD_GLOBAL             37 (NULL + get_focused_monitor_props)
-                           660 PRECALL                  0
-                           664 CALL                     0
-                           674 GET_AWAITABLE            0
-                           676 LOAD_CONST               2 (None)
-                       >>  678 SEND                     3 (to 686)
-                           680 YIELD_VALUE
-                           682 RESUME                   3
-                           684 JUMP_BACKWARD_NO_INTERRUPT     4 (to 678)
-                       >>  686 STORE_FAST               4 (monitor)
-               
-               304         688 LOAD_FAST                4 (monitor)
-                           690 POP_JUMP_FORWARD_IF_TRUE     2 (to 696)
-                           692 LOAD_ASSERTION_ERROR
-                           694 RAISE_VARARGS            1
-               
-               306     >>  696 LOAD_FAST                0 (self)
-                           698 LOAD_METHOD             19 (updateScratchInfo)
-                           720 LOAD_FAST                3 (item)
-                           722 PRECALL                  1
-                           726 CALL                     1
-                           736 GET_AWAITABLE            0
-                           738 LOAD_CONST               2 (None)
-                       >>  740 SEND                     3 (to 748)
-                           742 YIELD_VALUE
-                           744 RESUME                   3
-                           746 JUMP_BACKWARD_NO_INTERRUPT     4 (to 740)
-                       >>  748 POP_TOP
-               
-               308         750 LOAD_CONST               8 ('address:0x')
-                           752 LOAD_FAST                3 (item)
-                           754 LOAD_ATTR               12 (address)
-                           764 BINARY_OP                0 (+)
-                           768 STORE_FAST               5 (addr)
-               
-               310         770 LOAD_FAST                3 (item)
-                           772 LOAD_ATTR               20 (conf)
-                           782 LOAD_METHOD              2 (get)
-                           804 LOAD_CONST               9 ('animation')
-                           806 LOAD_CONST              10 ('')
-                           808 PRECALL                  2
-                           812 CALL                     2
-                           822 LOAD_METHOD             21 (lower)
-                           844 PRECALL                  0
-                           848 CALL                     0
-                           858 STORE_FAST               6 (animation_type)
-               
-               312         860 LOAD_FAST                4 (monitor)
-                           862 LOAD_CONST              11 ('activeWorkspace')
-                           864 BINARY_SUBSCR
-                           874 LOAD_CONST              12 ('id')
-                           876 BINARY_SUBSCR
-                           886 STORE_FAST               7 (wrkspc)
-               
-               314         888 LOAD_FAST                0 (self)
-                           890 LOAD_ATTR               22 (transitioning_scratches)
-                           900 LOAD_METHOD             23 (add)
-                           922 LOAD_FAST                1 (uid)
-                           924 PRECALL                  1
-                           928 CALL                     1
-                           938 POP_TOP
-               
-               315         940 LOAD_GLOBAL             49 (NULL + hyprctl)
-                           952 LOAD_CONST              13 ('moveworkspacetomonitor special:scratch_')
-                           954 LOAD_FAST                1 (uid)
-                           956 FORMAT_VALUE             0
-                           958 LOAD_CONST              14 (' ')
-                           960 LOAD_FAST                4 (monitor)
-                           962 LOAD_CONST              15 ('name')
-                           964 BINARY_SUBSCR
-                           974 FORMAT_VALUE             0
-                           976 BUILD_STRING             4
-                           978 PRECALL                  1
-                           982 CALL                     1
-                           992 GET_AWAITABLE            0
-                           994 LOAD_CONST               2 (None)
-                       >>  996 SEND                     3 (to 1004)
-                           998 YIELD_VALUE
-                          1000 RESUME                   3
-                          1002 JUMP_BACKWARD_NO_INTERRUPT     4 (to 996)
-                       >> 1004 POP_TOP
-               
-               316        1006 LOAD_GLOBAL             49 (NULL + hyprctl)
-                          1018 LOAD_CONST              16 ('movetoworkspacesilent ')
-                          1020 LOAD_FAST                7 (wrkspc)
-                          1022 FORMAT_VALUE             0
-                          1024 LOAD_CONST              17 (',')
-                          1026 LOAD_FAST                5 (addr)
-                          1028 FORMAT_VALUE             0
-                          1030 BUILD_STRING             4
-                          1032 PRECALL                  1
-                          1036 CALL                     1
-                          1046 GET_AWAITABLE            0
-                          1048 LOAD_CONST               2 (None)
-                       >> 1050 SEND                     3 (to 1058)
-                          1052 YIELD_VALUE
-                          1054 RESUME                   3
-                          1056 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1050)
-                       >> 1058 POP_TOP
-               
-               317        1060 LOAD_FAST                6 (animation_type)
-                          1062 POP_JUMP_FORWARD_IF_FALSE    78 (to 1220)
-               
-               318        1064 LOAD_FAST                3 (item)
-                          1066 LOAD_ATTR               20 (conf)
-                          1076 LOAD_METHOD              2 (get)
-                          1098 LOAD_CONST              18 ('margin')
-                          1100 LOAD_GLOBAL             50 (DEFAULT_MARGIN)
-                          1112 PRECALL                  2
-                          1116 CALL                     2
-                          1126 STORE_FAST               8 (margin)
-               
-               319        1128 LOAD_GLOBAL             53 (NULL + getattr)
-                          1140 LOAD_GLOBAL             54 (Animations)
-                          1152 LOAD_FAST                6 (animation_type)
-                          1154 PRECALL                  2
-                          1158 CALL                     2
-                          1168 STORE_FAST               9 (fn)
-               
-               320        1170 PUSH_NULL
-                          1172 LOAD_FAST                9 (fn)
-                          1174 LOAD_FAST                4 (monitor)
-                          1176 LOAD_FAST                3 (item)
-                          1178 LOAD_ATTR               28 (clientInfo)
-                          1188 LOAD_FAST                5 (addr)
-                          1190 LOAD_FAST                8 (margin)
-                          1192 PRECALL                  4
-                          1196 CALL                     4
-                          1206 GET_AWAITABLE            0
-                          1208 LOAD_CONST               2 (None)
-                       >> 1210 SEND                     3 (to 1218)
-                          1212 YIELD_VALUE
-                          1214 RESUME                   3
-                          1216 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1210)
-                       >> 1218 POP_TOP
-               
-               322     >> 1220 LOAD_GLOBAL             49 (NULL + hyprctl)
-                          1232 LOAD_CONST              19 ('focuswindow ')
-                          1234 LOAD_FAST                5 (addr)
-                          1236 FORMAT_VALUE             0
-                          1238 BUILD_STRING             2
-                          1240 PRECALL                  1
-                          1244 CALL                     1
-                          1254 GET_AWAITABLE            0
-                          1256 LOAD_CONST               2 (None)
-                       >> 1258 SEND                     3 (to 1266)
-                          1260 YIELD_VALUE
-                          1262 RESUME                   3
-                          1264 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1258)
-                       >> 1266 POP_TOP
-               
-               323        1268 LOAD_GLOBAL             33 (NULL + asyncio)
-                          1280 LOAD_ATTR               17 (sleep)
-                          1290 LOAD_CONST              20 (0.2)
-                          1292 PRECALL                  1
-                          1296 CALL                     1
-                          1306 GET_AWAITABLE            0
-                          1308 LOAD_CONST               2 (None)
-                       >> 1310 SEND                     3 (to 1318)
-                          1312 YIELD_VALUE
-                          1314 RESUME                   3
-                          1316 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1310)
-                       >> 1318 POP_TOP
-               
-               324        1320 LOAD_FAST                0 (self)
-                          1322 LOAD_ATTR               22 (transitioning_scratches)
-                          1332 LOAD_METHOD             29 (discard)
-                          1354 LOAD_FAST                1 (uid)
-                          1356 PRECALL                  1
-                          1360 CALL                     1
-                          1370 POP_TOP
-                          1372 LOAD_CONST               2 (None)
-                          1374 RETURN_VALUE
+               370     >>  650 LOAD_FAST                3 (item)
+                           652 LOAD_ATTR               18 (address)
+                           662 LOAD_FAST                0 (self)
+                           664 LOAD_ATTR               19 (scratches_by_address)
+                           674 CONTAINS_OP              0
+                           676 POP_JUMP_FORWARD_IF_FALSE    13 (to 704)
+               
+               371         678 LOAD_FAST                0 (self)
+                           680 LOAD_ATTR               19 (scratches_by_address)
+                           690 LOAD_FAST                3 (item)
+                           692 LOAD_ATTR               18 (address)
+                           702 DELETE_SUBSCR
+               
+               372     >>  704 LOAD_FAST                0 (self)
+                           706 LOAD_METHOD             20 (start_scratch_command)
+                           728 LOAD_FAST                1 (uid)
+                           730 PRECALL                  1
+                           734 CALL                     1
+                           744 GET_AWAITABLE            0
+                           746 LOAD_CONST               2 (None)
+                       >>  748 SEND                     3 (to 756)
+                           750 YIELD_VALUE
+                           752 RESUME                   3
+                           754 JUMP_BACKWARD_NO_INTERRUPT     4 (to 748)
+                       >>  756 POP_TOP
+               
+               373         758 LOAD_FAST                1 (uid)
+                           760 LOAD_FAST                0 (self)
+                           762 LOAD_ATTR               21 (_respawned_scratches)
+                           772 CONTAINS_OP              0
+                           774 POP_JUMP_FORWARD_IF_FALSE    35 (to 846)
+               
+               374     >>  776 LOAD_GLOBAL             45 (NULL + asyncio)
+                           788 LOAD_ATTR               23 (sleep)
+                           798 LOAD_CONST               7 (0.05)
+                           800 PRECALL                  1
+                           804 CALL                     1
+                           814 GET_AWAITABLE            0
+                           816 LOAD_CONST               2 (None)
+                       >>  818 SEND                     3 (to 826)
+                           820 YIELD_VALUE
+                           822 RESUME                   3
+                           824 JUMP_BACKWARD_NO_INTERRUPT     4 (to 818)
+                       >>  826 POP_TOP
+               
+               373         828 LOAD_FAST                1 (uid)
+                           830 LOAD_FAST                0 (self)
+                           832 LOAD_ATTR               21 (_respawned_scratches)
+                           842 CONTAINS_OP              0
+                           844 POP_JUMP_BACKWARD_IF_TRUE    35 (to 776)
+               
+               376     >>  846 LOAD_CONST               8 (True)
+                           848 LOAD_FAST                3 (item)
+                           850 STORE_ATTR              11 (visible)
+               
+               377         860 LOAD_GLOBAL             49 (NULL + get_focused_monitor_props)
+                           872 PRECALL                  0
+                           876 CALL                     0
+                           886 GET_AWAITABLE            0
+                           888 LOAD_CONST               2 (None)
+                       >>  890 SEND                     3 (to 898)
+                           892 YIELD_VALUE
+                           894 RESUME                   3
+                           896 JUMP_BACKWARD_NO_INTERRUPT     4 (to 890)
+                       >>  898 STORE_FAST               4 (monitor)
+               
+               378         900 LOAD_FAST                4 (monitor)
+                           902 POP_JUMP_FORWARD_IF_TRUE     2 (to 908)
+                           904 LOAD_ASSERTION_ERROR
+                           906 RAISE_VARARGS            1
+               
+               380     >>  908 LOAD_FAST                0 (self)
+                           910 LOAD_METHOD             25 (updateScratchInfo)
+                           932 LOAD_FAST                3 (item)
+                           934 PRECALL                  1
+                           938 CALL                     1
+                           948 GET_AWAITABLE            0
+                           950 LOAD_CONST               2 (None)
+                       >>  952 SEND                     3 (to 960)
+                           954 YIELD_VALUE
+                           956 RESUME                   3
+                           958 JUMP_BACKWARD_NO_INTERRUPT     4 (to 952)
+                       >>  960 POP_TOP
+               
+               382         962 LOAD_CONST               9 ('address:0x')
+                           964 LOAD_FAST                3 (item)
+                           966 LOAD_ATTR               18 (address)
+                           976 BINARY_OP                0 (+)
+                           980 STORE_FAST               5 (addr)
+               
+               384         982 LOAD_FAST                3 (item)
+                           984 LOAD_ATTR               26 (conf)
+                           994 LOAD_METHOD              2 (get)
+                          1016 LOAD_CONST              10 ('animation')
+                          1018 LOAD_CONST              11 ('')
+                          1020 PRECALL                  2
+                          1024 CALL                     2
+                          1034 LOAD_METHOD             27 (lower)
+                          1056 PRECALL                  0
+                          1060 CALL                     0
+                          1070 STORE_FAST               6 (animation_type)
+               
+               386        1072 LOAD_FAST                4 (monitor)
+                          1074 LOAD_CONST              12 ('activeWorkspace')
+                          1076 BINARY_SUBSCR
+                          1086 LOAD_CONST              13 ('id')
+                          1088 BINARY_SUBSCR
+                          1098 STORE_FAST               7 (wrkspc)
+               
+               388        1100 LOAD_FAST                0 (self)
+                          1102 LOAD_ATTR               28 (transitioning_scratches)
+                          1112 LOAD_METHOD             29 (add)
+                          1134 LOAD_FAST                1 (uid)
+                          1136 PRECALL                  1
+                          1140 CALL                     1
+                          1150 POP_TOP
+               
+               389        1152 LOAD_GLOBAL             61 (NULL + hyprctl)
+                          1164 LOAD_CONST              14 ('moveworkspacetomonitor special:scratch_')
+                          1166 LOAD_FAST                1 (uid)
+                          1168 FORMAT_VALUE             0
+                          1170 LOAD_CONST              15 (' ')
+                          1172 LOAD_FAST                4 (monitor)
+                          1174 LOAD_CONST              16 ('name')
+                          1176 BINARY_SUBSCR
+                          1186 FORMAT_VALUE             0
+                          1188 BUILD_STRING             4
+                          1190 PRECALL                  1
+                          1194 CALL                     1
+                          1204 GET_AWAITABLE            0
+                          1206 LOAD_CONST               2 (None)
+                       >> 1208 SEND                     3 (to 1216)
+                          1210 YIELD_VALUE
+                          1212 RESUME                   3
+                          1214 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1208)
+                       >> 1216 POP_TOP
+               
+               390        1218 LOAD_GLOBAL             61 (NULL + hyprctl)
+                          1230 LOAD_CONST              17 ('movetoworkspacesilent ')
+                          1232 LOAD_FAST                7 (wrkspc)
+                          1234 FORMAT_VALUE             0
+                          1236 LOAD_CONST              18 (',')
+                          1238 LOAD_FAST                5 (addr)
+                          1240 FORMAT_VALUE             0
+                          1242 BUILD_STRING             4
+                          1244 PRECALL                  1
+                          1248 CALL                     1
+                          1258 GET_AWAITABLE            0
+                          1260 LOAD_CONST               2 (None)
+                       >> 1262 SEND                     3 (to 1270)
+                          1264 YIELD_VALUE
+                          1266 RESUME                   3
+                          1268 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1262)
+                       >> 1270 POP_TOP
+               
+               391        1272 LOAD_FAST                6 (animation_type)
+                          1274 POP_JUMP_FORWARD_IF_FALSE    78 (to 1432)
+               
+               392        1276 LOAD_FAST                3 (item)
+                          1278 LOAD_ATTR               26 (conf)
+                          1288 LOAD_METHOD              2 (get)
+                          1310 LOAD_CONST              19 ('margin')
+                          1312 LOAD_GLOBAL             62 (DEFAULT_MARGIN)
+                          1324 PRECALL                  2
+                          1328 CALL                     2
+                          1338 STORE_FAST               8 (margin)
+               
+               393        1340 LOAD_GLOBAL             65 (NULL + getattr)
+                          1352 LOAD_GLOBAL             66 (Animations)
+                          1364 LOAD_FAST                6 (animation_type)
+                          1366 PRECALL                  2
+                          1370 CALL                     2
+                          1380 STORE_FAST               9 (fn)
+               
+               394        1382 PUSH_NULL
+                          1384 LOAD_FAST                9 (fn)
+                          1386 LOAD_FAST                4 (monitor)
+                          1388 LOAD_FAST                3 (item)
+                          1390 LOAD_ATTR               34 (client_info)
+                          1400 LOAD_FAST                5 (addr)
+                          1402 LOAD_FAST                8 (margin)
+                          1404 PRECALL                  4
+                          1408 CALL                     4
+                          1418 GET_AWAITABLE            0
+                          1420 LOAD_CONST               2 (None)
+                       >> 1422 SEND                     3 (to 1430)
+                          1424 YIELD_VALUE
+                          1426 RESUME                   3
+                          1428 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1422)
+                       >> 1430 POP_TOP
+               
+               396     >> 1432 LOAD_GLOBAL             61 (NULL + hyprctl)
+                          1444 LOAD_CONST              20 ('focuswindow ')
+                          1446 LOAD_FAST                5 (addr)
+                          1448 FORMAT_VALUE             0
+                          1450 BUILD_STRING             2
+                          1452 PRECALL                  1
+                          1456 CALL                     1
+                          1466 GET_AWAITABLE            0
+                          1468 LOAD_CONST               2 (None)
+                       >> 1470 SEND                     3 (to 1478)
+                          1472 YIELD_VALUE
+                          1474 RESUME                   3
+                          1476 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1470)
+                       >> 1478 POP_TOP
+               
+               397        1480 LOAD_GLOBAL             45 (NULL + asyncio)
+                          1492 LOAD_ATTR               23 (sleep)
+                          1502 LOAD_CONST              21 (0.2)
+                          1504 PRECALL                  1
+                          1508 CALL                     1
+                          1518 GET_AWAITABLE            0
+                          1520 LOAD_CONST               2 (None)
+                       >> 1522 SEND                     3 (to 1530)
+                          1524 YIELD_VALUE
+                          1526 RESUME                   3
+                          1528 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1522)
+                       >> 1530 POP_TOP
+               
+               398        1532 LOAD_FAST                0 (self)
+                          1534 LOAD_ATTR               28 (transitioning_scratches)
+                          1544 LOAD_METHOD             35 (discard)
+                          1566 LOAD_FAST                1 (uid)
+                          1568 PRECALL                  1
+                          1572 CALL                     1
+                          1582 POP_TOP
+                          1584 LOAD_CONST               2 (None)
+                          1586 RETURN_VALUE
                consts
                   '<name> shows scratchpad "name" '
                   'activewindow'
                   None
-                  ' is not configured'
-                  ' is already visible'
-                  ' is not running, restarting...'
+                  '%s is not configured'
+                  '%s is already visible'
+                  'Showing %s'
+                  '%s is not running, restarting...'
                   0.05
                   True
                   'address:0x'
                   'animation'
                   ''
                   'activeWorkspace'
                   'id'
@@ -3022,39 +3697,41 @@
                   ' '
                   'name'
                   'movetoworkspacesilent '
                   ','
                   'margin'
                   'focuswindow '
                   0.2
-               names      ('strip', 'scratches', 'get', 'hyprctlJSON', 'focused_window_tracking', 'print', 'visible', 'isAlive', 'procs', 'kill', 'pid', 'scratches_by_pid', 'address', 'scratches_by_address', 'start_scratch_command', '_respawned_scratches', 'asyncio', 'sleep', 'get_focused_monitor_props', 'updateScratchInfo', 'conf', 'lower', 'transitioning_scratches', 'add', 'hyprctl', 'DEFAULT_MARGIN', 'getattr', 'Animations', 'clientInfo', 'discard')
+               names      ('strip', 'scratches', 'get', 'cast', 'dict', 'str', 'Any', 'hyprctlJSON', 'focused_window_tracking', 'log', 'warning', 'visible', 'info', 'isAlive', 'procs', 'kill', 'pid', 'scratches_by_pid', 'address', 'scratches_by_address', 'start_scratch_command', '_respawned_scratches', 'asyncio', 'sleep', 'get_focused_monitor_props', 'updateScratchInfo', 'conf', 'lower', 'transitioning_scratches', 'add', 'hyprctl', 'DEFAULT_MARGIN', 'getattr', 'Animations', 'client_info', 'discard')
                varnames   ('self', 'uid', 'force', 'item', 'monitor', 'addr', 'animation_type', 'wrkspc', 'margin', 'fn')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'run_show'
-               firstlineno 276
+               firstlineno 345
                lnotab
-                  0x0602280134023a02040124010402120124010402280124013e011c011a
-                  011c011a012a01120134ff12030e0128010802360214025a021c02340142
-                  013601040140012a01320230013401
+                  0x0602280134020c0158ff20040401360104021201360104023602280136
+                  0112013e011c011a011c011a013601120134ff12030e0128010802360214
+                  025a021c02340142013601040140012a01320230013401
             ('return', None)
+            (False,)
             (None,)
             (False, False)
-            (False,)
-         names      ('__name__', '__module__', '__qualname__', 'init', 'exit', 'load_config', 'str', 'start_scratch_command', 'event_activewindowv2', 'event_openwindow', 'run_toggle', 'Scratch', 'updateScratchInfo', 'run_hide', 'run_show')
+         names      ('__name__', '__module__', '__qualname__', 'procs', 'dict', 'str', 'subprocess', 'Popen', '__annotations__', 'scratches', 'Scratch', 'set', 'transitioning_scratches', '_new_scratches', '_respawned_scratches', 'scratches_by_address', 'scratches_by_pid', 'int', 'focused_window_tracking', 'exit', 'Any', 'load_config', 'start_scratch_command', 'event_activewindowv2', '_alternative_lookup', 'event_openwindow', 'run_toggle', '_anim_hide', 'updateScratchInfo', 'run_hide', 'run_show')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
          name       'Extension'
-         firstlineno 109
-         lnotab 0x0a0108090810081110120811080c100c1813122e
+         firstlineno 133
+         lnotab
+            0x0c0128011e012a012a012a011e011e011e020812201312170814061308
+            11100d06171815121d
       'Extension'
-   names      ('subprocess', 'typing', 'Any', 'asyncio', 'ipc', 'hyprctl', 'hyprctlJSON', 'get_focused_monitor_props', 'os', 'interface', 'Plugin', 'DEFAULT_MARGIN', 'str', 'get_client_props_by_address', 'Animations', 'Scratch', 'Extension')
+   names      ('__doc__', 'os', 'asyncio', 'subprocess', 'typing', 'Any', 'cast', 'ipc', 'hyprctl', 'hyprctlJSON', 'get_focused_monitor_props', 'interface', 'Plugin', 'DEFAULT_MARGIN', 'str', 'get_client_props_by_address', 'Animations', 'Scratch', 'Extension')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c010801140508020c0204030c071a331a23
+   lnotab 0x00ff02010401080108010801100214060c0204030c081a3e1a2d
```

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/shift_monitors.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/shift_monitors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/toggle_dpms.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/toggle_dpms.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-310.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-1.3.1/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc` & `pyprland-1.4.0/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,628 +1,684 @@
 magic:    0xa70d0d0a
-moddate:  0x57d54e64 (Sun Apr 30 20:53:43 2023 UTC)
-files sz: 2218
+moddate:  0xe799c664 (Sun Jul 30 17:12:07 2023 UTC)
+files sz: 2598
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640264036c016d025a020100640464056c036d
-      045a046d055a050100020047006406840064076502a6030000ab03000000
-      00000000005a0664015300
+      0x970064005a00640164026c016d025a020100640364046c036d045a0401
+      00640564066c056d065a066d075a070100020047006407840064086504a6
+      030000ab0300000000000000005a0864095300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (asyncio)
-                 8 STORE_NAME               0 (asyncio)
+     1           2 LOAD_CONST               0 (' Force workspaces to follow the focus / mouse ')
+                 4 STORE_NAME               0 (__doc__)
    
-     2          10 LOAD_CONST               2 (1)
-                12 LOAD_CONST               3 (('Plugin',))
-                14 IMPORT_NAME              1 (interface)
-                16 IMPORT_FROM              2 (Plugin)
-                18 STORE_NAME               2 (Plugin)
-                20 POP_TOP
+     2           6 LOAD_CONST               1 (0)
+                 8 LOAD_CONST               2 (('cast',))
+                10 IMPORT_NAME              1 (typing)
+                12 IMPORT_FROM              2 (cast)
+                14 STORE_NAME               2 (cast)
+                16 POP_TOP
    
-     4          22 LOAD_CONST               4 (2)
-                24 LOAD_CONST               5 (('hyprctlJSON', 'hyprctl'))
-                26 IMPORT_NAME              3 (ipc)
-                28 IMPORT_FROM              4 (hyprctlJSON)
-                30 STORE_NAME               4 (hyprctlJSON)
-                32 IMPORT_FROM              5 (hyprctl)
-                34 STORE_NAME               5 (hyprctl)
-                36 POP_TOP
+     3          18 LOAD_CONST               3 (1)
+                20 LOAD_CONST               4 (('Plugin',))
+                22 IMPORT_NAME              3 (interface)
+                24 IMPORT_FROM              4 (Plugin)
+                26 STORE_NAME               4 (Plugin)
+                28 POP_TOP
    
-     7          38 PUSH_NULL
-                40 LOAD_BUILD_CLASS
-                42 LOAD_CONST               6 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 7>)
-                44 MAKE_FUNCTION            0
-                46 LOAD_CONST               7 ('Extension')
-                48 LOAD_NAME                2 (Plugin)
-                50 PRECALL                  3
-                54 CALL                     3
-                64 STORE_NAME               6 (Extension)
-                66 LOAD_CONST               1 (None)
-                68 RETURN_VALUE
+     5          30 LOAD_CONST               5 (2)
+                32 LOAD_CONST               6 (('hyprctlJSON', 'hyprctl'))
+                34 IMPORT_NAME              5 (ipc)
+                36 IMPORT_FROM              6 (hyprctlJSON)
+                38 STORE_NAME               6 (hyprctlJSON)
+                40 IMPORT_FROM              7 (hyprctl)
+                42 STORE_NAME               7 (hyprctl)
+                44 POP_TOP
+   
+     8          46 PUSH_NULL
+                48 LOAD_BUILD_CLASS
+                50 LOAD_CONST               7 (<code object Extension, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 8>)
+                52 MAKE_FUNCTION            0
+                54 LOAD_CONST               8 ('Extension')
+                56 LOAD_NAME                4 (Plugin)
+                58 PRECALL                  3
+                62 CALL                     3
+                72 STORE_NAME               8 (Extension)
+                74 LOAD_CONST               9 (None)
+                76 RETURN_VALUE
    consts
+      ' Force workspaces to follow the focus / mouse '
       0
-      None
+      ('cast',)
       1
       ('Plugin',)
       2
       ('hyprctlJSON', 'hyprctl')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 2
+         stacksize : 3
          flags     : 0
          code
-            0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            0365056602640484045a06880078015a075300
+            0x8700970065005a0164005a02550067005a036504650519000000000000
+            000000650664013c00000088006601640284085a07640384005a08640465
+            096602640584045a0a880078015a0b5300
                        0 MAKE_CELL                0 (__class__)
          
-           7           2 RESUME                   0
+           8           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Extension')
                       10 STORE_NAME               2 (__qualname__)
+                      12 SETUP_ANNOTATIONS
+         
+           9          14 BUILD_LIST               0
+                      16 STORE_NAME               3 (workspace_list)
+                      18 LOAD_NAME                4 (list)
+                      20 LOAD_NAME                5 (int)
+                      22 BINARY_SUBSCR
+                      32 LOAD_NAME                6 (__annotations__)
+                      34 LOAD_CONST               1 ('workspace_list')
+                      36 STORE_SUBSCR
          
-           8          12 LOAD_CLOSURE             0 (__class__)
-                      14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object load_config, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 8>)
-                      18 MAKE_FUNCTION            8 (closure)
-                      20 STORE_NAME               3 (load_config)
+          11          40 LOAD_CLOSURE             0 (__class__)
+                      42 BUILD_TUPLE              1
+                      44 LOAD_CONST               2 (<code object load_config, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 11>)
+                      46 MAKE_FUNCTION            8 (closure)
+                      48 STORE_NAME               7 (load_config)
          
-          12          22 LOAD_CONST               2 (<code object event_focusedmon, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 12>)
-                      24 MAKE_FUNCTION            0
-                      26 STORE_NAME               4 (event_focusedmon)
+          16          50 LOAD_CONST               3 (<code object event_focusedmon, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 16>)
+                      52 MAKE_FUNCTION            0
+                      54 STORE_NAME               8 (event_focusedmon)
          
-          30          28 LOAD_CONST               3 ('direction')
-                      30 LOAD_NAME                5 (str)
-                      32 BUILD_TUPLE              2
-                      34 LOAD_CONST               4 (<code object run_change_workspace, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 30>)
-                      36 MAKE_FUNCTION            4 (annotations)
-                      38 STORE_NAME               6 (run_change_workspace)
-                      40 LOAD_CLOSURE             0 (__class__)
-                      42 COPY                     1
-                      44 STORE_NAME               7 (__classcell__)
-                      46 RETURN_VALUE
+          39          56 LOAD_CONST               4 ('direction')
+                      58 LOAD_NAME                9 (str)
+                      60 BUILD_TUPLE              2
+                      62 LOAD_CONST               5 (<code object run_change_workspace, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 39>)
+                      64 MAKE_FUNCTION            4 (annotations)
+                      66 STORE_NAME              10 (run_change_workspace)
+                      68 LOAD_CLOSURE             0 (__class__)
+                      70 COPY                     1
+                      72 STORE_NAME              11 (__classcell__)
+                      74 RETURN_VALUE
          consts
             'Extension'
+            'workspace_list'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 131
                code
                   0x95014b0001009700740100000000000000000000a6000000ab00000000
                   0000000000a00100000000000000000000000000000000000000007c01a6
-                  010000ab010000000000000000830064007b035600970386040100740500
-                  00000000000000000074070000000000000000000064017c006a04000000
-                  0000000000a0050000000000000000000000000000000000000000640264
-                  03a6020000ab02000000000000000064017a000000a6020000ab02000000
+                  010000ab010000000000000000830064017b035600970386040100740500
+                  00000000000000000074070000000000000000000064027c006a04000000
+                  0000000000a0050000000000000000000000000000000000000000640364
+                  04a6020000ab02000000000000000064027a000000a6020000ab02000000
                   0000000000a6010000ab0100000000000000007c005f0600000000000000
-                  0064005300
+                  0064015300
                              0 COPY_FREE_VARS           1
                
-                 8           2 RETURN_GENERATOR
+                11           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                 9           8 LOAD_GLOBAL              1 (NULL + super)
+                13           8 LOAD_GLOBAL              1 (NULL + super)
                             20 PRECALL                  0
                             24 CALL                     0
                             34 LOAD_METHOD              1 (load_config)
                             56 LOAD_FAST                1 (config)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 GET_AWAITABLE            0
-                            74 LOAD_CONST               0 (None)
+                            74 LOAD_CONST               1 (None)
                        >>   76 SEND                     3 (to 84)
                             78 YIELD_VALUE
                             80 RESUME                   3
                             82 JUMP_BACKWARD_NO_INTERRUPT     4 (to 76)
                        >>   84 POP_TOP
                
-                10          86 LOAD_GLOBAL              5 (NULL + list)
+                14          86 LOAD_GLOBAL              5 (NULL + list)
                             98 LOAD_GLOBAL              7 (NULL + range)
-                           110 LOAD_CONST               1 (1)
+                           110 LOAD_CONST               2 (1)
                            112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                4 (config)
                            124 LOAD_METHOD              5 (get)
-                           146 LOAD_CONST               2 ('max_workspaces')
-                           148 LOAD_CONST               3 (10)
+                           146 LOAD_CONST               3 ('max_workspaces')
+                           148 LOAD_CONST               4 (10)
                            150 PRECALL                  2
                            154 CALL                     2
-                           164 LOAD_CONST               1 (1)
+                           164 LOAD_CONST               2 (1)
                            166 BINARY_OP                0 (+)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 PRECALL                  1
                            188 CALL                     1
                            198 LOAD_FAST                0 (self)
                            200 STORE_ATTR               6 (workspace_list)
-                           210 LOAD_CONST               0 (None)
+                           210 LOAD_CONST               1 (None)
                            212 RETURN_VALUE
                consts
+                  'loads the config'
                   None
                   1
                   'max_workspaces'
                   10
                names      ('super', 'load_config', 'list', 'range', 'config', 'get', 'workspace_list')
                varnames   ('self', 'config')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
                name       'load_config'
-               firstlineno 8
-               lnotab 0x08014e01
+               firstlineno 11
+               lnotab 0x08024e01
             code
                argcount  : 2
                nlocals   : 7
-               stacksize : 7
+               stacksize : 9
                flags     : 131
                code
                   0x87074b00010097007c01a0000000000000000000000000000000000000
                   0000006401a6010000ab0100000000000000005c0200008a077d02740300
                   0000000000000000007c02a6010000ab0100000000000000007d02740500
-                  000000000000000000880766016402840874070000000000000000000064
-                  03a6010000ab010000000000000000830064007b035600970386044400a6
+                  000000000000000000880766016402840874070000000000000000000074
+                  0800000000000000000000740a0000000000000000000019000000000000
+                  000000740d000000000000000000006403a6010000ab0100000000000000
+                  00830064047b03560097038604a6020000ab0200000000000000004400a6
                   000000ab000000000000000000a6010000ab0100000000000000007d0364
-                  0484007407000000000000000000006405a6010000ab0100000000000000
-                  00830064007b035600970386044400a6000000ab0000000000000000007d
+                  058400740700000000000000000000740800000000000000000000740a00
+                  00000000000000000019000000000000000000740d000000000000000000
+                  006406a6010000ab010000000000000000830064047b03560097038604a6
+                  020000ab0200000000000000004400a6000000ab0000000000000000007d
                   0467007d057c0444005d287d067c067c03760073067c067c026b02000000
-                  0072018c0d7c05a004000000000000000000000000000000000000000064
-                  067c069b00640789079b009d04a6010000ab01000000000000000001008c
-                  29740b000000000000000000007c05a6010000ab01000000000000000083
-                  0064007b03560097038604010064005300
+                  0072018c0d7c05a007000000000000000000000000000000000000000064
+                  077c069b00640889079b009d04a6010000ab01000000000000000001008c
+                  297411000000000000000000007c05a6010000ab01000000000000000083
+                  0064047b03560097038604010064045300
                              0 MAKE_CELL                7 (monitor_id)
                
-                12           2 RETURN_GENERATOR
+                16           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                13           8 LOAD_FAST                1 (screenid_index)
+                18           8 LOAD_FAST                1 (screenid_index)
                             10 LOAD_METHOD              0 (split)
                             32 LOAD_CONST               1 (',')
                             34 PRECALL                  1
                             38 CALL                     1
                             48 UNPACK_SEQUENCE          2
                             52 STORE_DEREF              7 (monitor_id)
                             54 STORE_FAST               2 (workspace_id)
                
-                14          56 LOAD_GLOBAL              3 (NULL + int)
+                19          56 LOAD_GLOBAL              3 (NULL + int)
                             68 LOAD_FAST                2 (workspace_id)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               2 (workspace_id)
                
-                16          86 LOAD_GLOBAL              5 (NULL + set)
+                21          86 LOAD_GLOBAL              5 (NULL + set)
                             98 LOAD_CLOSURE             7 (monitor_id)
                            100 BUILD_TUPLE              1
-                           102 LOAD_CONST               2 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 16>)
+                           102 LOAD_CONST               2 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 21>)
                            104 MAKE_FUNCTION            8 (closure)
                
-                18         106 LOAD_GLOBAL              7 (NULL + hyprctlJSON)
-                           118 LOAD_CONST               3 ('monitors')
-                           120 PRECALL                  1
-                           124 CALL                     1
-                           134 GET_AWAITABLE            0
-                           136 LOAD_CONST               0 (None)
-                       >>  138 SEND                     3 (to 146)
-                           140 YIELD_VALUE
-                           142 RESUME                   3
-                           144 JUMP_BACKWARD_NO_INTERRUPT     4 (to 138)
-               
-                16     >>  146 GET_ITER
-                           148 PRECALL                  0
-                           152 CALL                     0
-                           162 PRECALL                  1
-                           166 CALL                     1
-                           176 STORE_FAST               3 (busy_workspaces)
-               
-                21         178 LOAD_CONST               4 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 21>)
-                           180 MAKE_FUNCTION            0
-                           182 LOAD_GLOBAL              7 (NULL + hyprctlJSON)
-                           194 LOAD_CONST               5 ('workspaces')
-                           196 PRECALL                  1
-                           200 CALL                     1
-                           210 GET_AWAITABLE            0
-                           212 LOAD_CONST               0 (None)
-                       >>  214 SEND                     3 (to 222)
-                           216 YIELD_VALUE
-                           218 RESUME                   3
-                           220 JUMP_BACKWARD_NO_INTERRUPT     4 (to 214)
-                       >>  222 GET_ITER
-                           224 PRECALL                  0
-                           228 CALL                     0
-                           238 STORE_FAST               4 (workspaces)
-               
-                23         240 BUILD_LIST               0
-                           242 STORE_FAST               5 (batch)
-               
-                24         244 LOAD_FAST                4 (workspaces)
-                           246 GET_ITER
-                       >>  248 FOR_ITER                40 (to 330)
-                           250 STORE_FAST               6 (n)
-               
-                25         252 LOAD_FAST                6 (n)
-                           254 LOAD_FAST                3 (busy_workspaces)
-                           256 CONTAINS_OP              0
-                           258 POP_JUMP_FORWARD_IF_TRUE     6 (to 272)
-                           260 LOAD_FAST                6 (n)
-                           262 LOAD_FAST                2 (workspace_id)
-                           264 COMPARE_OP               2 (==)
-                           270 POP_JUMP_FORWARD_IF_FALSE     1 (to 274)
-               
-                26     >>  272 JUMP_BACKWARD           13 (to 248)
-               
-                27     >>  274 LOAD_FAST                5 (batch)
-                           276 LOAD_METHOD              4 (append)
-                           298 LOAD_CONST               6 ('moveworkspacetomonitor ')
-                           300 LOAD_FAST                6 (n)
-                           302 FORMAT_VALUE             0
-                           304 LOAD_CONST               7 (' ')
-                           306 LOAD_DEREF               7 (monitor_id)
-                           308 FORMAT_VALUE             0
-                           310 BUILD_STRING             4
-                           312 PRECALL                  1
-                           316 CALL                     1
-                           326 POP_TOP
-                           328 JUMP_BACKWARD           41 (to 248)
-               
-                28     >>  330 LOAD_GLOBAL             11 (NULL + hyprctl)
-                           342 LOAD_FAST                5 (batch)
-                           344 PRECALL                  1
-                           348 CALL                     1
-                           358 GET_AWAITABLE            0
-                           360 LOAD_CONST               0 (None)
-                       >>  362 SEND                     3 (to 370)
-                           364 YIELD_VALUE
-                           366 RESUME                   3
-                           368 JUMP_BACKWARD_NO_INTERRUPT     4 (to 362)
-                       >>  370 POP_TOP
-                           372 LOAD_CONST               0 (None)
-                           374 RETURN_VALUE
+                23         106 LOAD_GLOBAL              7 (NULL + cast)
+                           118 LOAD_GLOBAL              8 (list)
+                           130 LOAD_GLOBAL             10 (dict)
+                           142 BINARY_SUBSCR
+                           152 LOAD_GLOBAL             13 (NULL + hyprctlJSON)
+                           164 LOAD_CONST               3 ('monitors')
+                           166 PRECALL                  1
+                           170 CALL                     1
+                           180 GET_AWAITABLE            0
+                           182 LOAD_CONST               4 (None)
+                       >>  184 SEND                     3 (to 192)
+                           186 YIELD_VALUE
+                           188 RESUME                   3
+                           190 JUMP_BACKWARD_NO_INTERRUPT     4 (to 184)
+                       >>  192 PRECALL                  2
+                           196 CALL                     2
+               
+                21         206 GET_ITER
+                           208 PRECALL                  0
+                           212 CALL                     0
+                           222 PRECALL                  1
+                           226 CALL                     1
+                           236 STORE_FAST               3 (busy_workspaces)
+               
+                26         238 LOAD_CONST               5 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 26>)
+                           240 MAKE_FUNCTION            0
+               
+                28         242 LOAD_GLOBAL              7 (NULL + cast)
+                           254 LOAD_GLOBAL              8 (list)
+                           266 LOAD_GLOBAL             10 (dict)
+                           278 BINARY_SUBSCR
+                           288 LOAD_GLOBAL             13 (NULL + hyprctlJSON)
+                           300 LOAD_CONST               6 ('workspaces')
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 GET_AWAITABLE            0
+                           318 LOAD_CONST               4 (None)
+                       >>  320 SEND                     3 (to 328)
+                           322 YIELD_VALUE
+                           324 RESUME                   3
+                           326 JUMP_BACKWARD_NO_INTERRUPT     4 (to 320)
+                       >>  328 PRECALL                  2
+                           332 CALL                     2
+               
+                26         342 GET_ITER
+                           344 PRECALL                  0
+                           348 CALL                     0
+                           358 STORE_FAST               4 (workspaces)
+               
+                32         360 BUILD_LIST               0
+                           362 STORE_FAST               5 (batch)
+               
+                33         364 LOAD_FAST                4 (workspaces)
+                           366 GET_ITER
+                       >>  368 FOR_ITER                40 (to 450)
+                           370 STORE_FAST               6 (n)
+               
+                34         372 LOAD_FAST                6 (n)
+                           374 LOAD_FAST                3 (busy_workspaces)
+                           376 CONTAINS_OP              0
+                           378 POP_JUMP_FORWARD_IF_TRUE     6 (to 392)
+                           380 LOAD_FAST                6 (n)
+                           382 LOAD_FAST                2 (workspace_id)
+                           384 COMPARE_OP               2 (==)
+                           390 POP_JUMP_FORWARD_IF_FALSE     1 (to 394)
+               
+                35     >>  392 JUMP_BACKWARD           13 (to 368)
+               
+                36     >>  394 LOAD_FAST                5 (batch)
+                           396 LOAD_METHOD              7 (append)
+                           418 LOAD_CONST               7 ('moveworkspacetomonitor ')
+                           420 LOAD_FAST                6 (n)
+                           422 FORMAT_VALUE             0
+                           424 LOAD_CONST               8 (' ')
+                           426 LOAD_DEREF               7 (monitor_id)
+                           428 FORMAT_VALUE             0
+                           430 BUILD_STRING             4
+                           432 PRECALL                  1
+                           436 CALL                     1
+                           446 POP_TOP
+                           448 JUMP_BACKWARD           41 (to 368)
+               
+                37     >>  450 LOAD_GLOBAL             17 (NULL + hyprctl)
+                           462 LOAD_FAST                5 (batch)
+                           464 PRECALL                  1
+                           468 CALL                     1
+                           478 GET_AWAITABLE            0
+                           480 LOAD_CONST               4 (None)
+                       >>  482 SEND                     3 (to 490)
+                           484 YIELD_VALUE
+                           486 RESUME                   3
+                           488 JUMP_BACKWARD_NO_INTERRUPT     4 (to 482)
+                       >>  490 POP_TOP
+                           492 LOAD_CONST               4 (None)
+                           494 RETURN_VALUE
                consts
-                  None
+                  'reacts to monitor changes'
                   ','
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 51
                      code
                         0x95014b00010097007c005d1e7d017c0164001900000000000000000089
                         026b0300000000af0e7c0164011900000000000000000064021900000000
                         00000000005600970101008c1f64035300
                                    0 COPY_FREE_VARS           1
                      
-                      16           2 RETURN_GENERATOR
+                      21           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                30 (to 72)
                      
-                      18          12 STORE_FAST               1 (mon)
+                      23          12 STORE_FAST               1 (mon)
                      
-                      19          14 LOAD_FAST                1 (mon)
+                      24          14 LOAD_FAST                1 (mon)
                                   16 LOAD_CONST               0 ('name')
                                   18 BINARY_SUBSCR
                                   28 LOAD_DEREF               2 (monitor_id)
                                   30 COMPARE_OP               3 (!=)
                                   36 POP_JUMP_BACKWARD_IF_FALSE    14 (to 10)
                      
-                      17          38 LOAD_FAST                1 (mon)
+                      22          38 LOAD_FAST                1 (mon)
                                   40 LOAD_CONST               1 ('activeWorkspace')
                                   42 BINARY_SUBSCR
                                   52 LOAD_CONST               2 ('id')
                                   54 BINARY_SUBSCR
                      
-                      19          64 YIELD_VALUE
+                      24          64 YIELD_VALUE
                                   66 RESUME                   1
                                   68 POP_TOP
                                   70 JUMP_BACKWARD           31 (to 10)
                      
-                      16     >>   72 LOAD_CONST               3 (None)
+                      21     >>   72 LOAD_CONST               3 (None)
                                   74 RETURN_VALUE
                      consts
                         'name'
                         'activeWorkspace'
                         'id'
                         None
                      names      ()
                      varnames   ('.0', 'mon')
                      freevars   ('monitor_id',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
                      name       '<genexpr>'
-                     firstlineno 16
+                     firstlineno 21
                      lnotab 0x0c02020118fe1a0208fd
                   'monitors'
+                  None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d167d017c0164001900000000000000000064016b0400
                         000000af0e7c0164001900000000000000000091028c175300
-                      21           0 RESUME                   0
+                      26           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                22 (to 52)
-                                   8 STORE_FAST               1 (w)
-                                  10 LOAD_FAST                1 (w)
+                     
+                      28           8 STORE_FAST               1 (w)
+                     
+                      29          10 LOAD_FAST                1 (w)
                                   12 LOAD_CONST               0 ('id')
                                   14 BINARY_SUBSCR
                                   24 LOAD_CONST               1 (0)
                                   26 COMPARE_OP               4 (>)
                                   32 POP_JUMP_BACKWARD_IF_FALSE    14 (to 6)
-                                  34 LOAD_FAST                1 (w)
+                     
+                      27          34 LOAD_FAST                1 (w)
                                   36 LOAD_CONST               0 ('id')
                                   38 BINARY_SUBSCR
-                                  48 LIST_APPEND              2
+                     
+                      29          48 LIST_APPEND              2
                                   50 JUMP_BACKWARD           23 (to 6)
                              >>   52 RETURN_VALUE
                      consts
                         'id'
                         0
                      names      ()
                      varnames   ('.0', 'w')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
                      name       '<listcomp>'
-                     firstlineno 21
-                     lnotab 0x
+                     firstlineno 26
+                     lnotab 0x0802020118fe0e02
                   'workspaces'
                   'moveworkspacetomonitor '
                   ' '
-               names      ('split', 'int', 'set', 'hyprctlJSON', 'append', 'hyprctl')
+               names      ('split', 'int', 'set', 'cast', 'list', 'dict', 'hyprctlJSON', 'append', 'hyprctl')
                varnames   ('self', 'screenid_index', 'workspace_id', 'busy_workspaces', 'workspaces', 'batch', 'n')
                freevars   ()
                cellvars   ('monitor_id',)
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
                name       'event_focusedmon'
-               firstlineno 12
-               lnotab 0x080130011e02140228fe20053e0204010801140102013801
+               firstlineno 16
+               lnotab 0x080230011e02140264fe2005040264fe120604010801140102013801
             'direction'
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 7
                flags     : 131
                code
                   0x870887094b00010097007401000000000000000000007c01a6010000ab
                   0100000000000000007d027403000000000000000000006401a6010000ab
                   010000000000000000830064027b035600970386047d0374050000000000
                   00000000007c03740600000000000000000000a6020000ab020000000000
                   00000073024a0082017c0344005d0c8a0989096403190000000000000000
-                  00720201006e018c0d740500000000000000000000890974080000000000
-                  0000000000a6020000ab02000000000000000073024a008201740b000000
-                  0000000000000088096601640484087c034400a6000000ab000000000000
-                  000000a6010000ab0100000000000000008a088909640519000000000000
-                  0000006406190000000000000000007d0488086601640784087c006a0600
-                  000000000000004400a6000000ab0000000000000000007d0509007c05a0
-                  0700000000000000000000000000000000000000007c04a6010000ab0100
-                  000000000000007d067c057c067c027a0000007411000000000000000000
-                  007c05a6010000ab0100000000000000007a060000190000000000000000
-                  007d076e2023007412000000000000000000002400721301007c057c0264
-                  086b0400000000720264086e016409190000000000000000007d0759006e
-                  047700780359007701741500000000000000000000640a7c079b00640b89
-                  09640c190000000000000000009b009d04a6010000ab0100000000000000
-                  00830064027b035600970386040100741500000000000000000000640d7c
-                  079b009d02a6010000ab010000000000000000830064027b035600970386
-                  04010064025300
+                  00720201006e1d8c0d7c006a040000000000000000a00500000000000000
+                  000000000000000000000000006404a6010000ab01000000000000000001
+                  00640253007405000000000000000000008909740c000000000000000000
+                  00a6020000ab02000000000000000073024a008201740f00000000000000
+                  00000088096601640584087c034400a6000000ab000000000000000000a6
+                  010000ab0100000000000000008a08890964061900000000000000000064
+                  07190000000000000000007d0488086601640884087c006a080000000000
+                  0000004400a6000000ab0000000000000000007d0509007c05a009000000
+                  00000000000000000000000000000000007c04a6010000ab010000000000
+                  0000007d067c057c067c027a0000007415000000000000000000007c05a6
+                  010000ab0100000000000000007a060000190000000000000000007d076e
+                  2023007416000000000000000000002400721301007c057c0264096b0400
+                  000000720264096e01640a190000000000000000007d0759006e04770078
+                  0359007701741900000000000000000000640b7c079b00640c8909640d19
+                  0000000000000000009b009d04a6010000ab010000000000000000830064
+                  027b035600970386040100741900000000000000000000640e7c079b009d
+                  02a6010000ab010000000000000000830064027b03560097038604010064
+                  025300
                              0 MAKE_CELL                8 (busy_workspaces)
                              2 MAKE_CELL                9 (monitor)
                
-                30           4 RETURN_GENERATOR
+                39           4 RETURN_GENERATOR
                              6 POP_TOP
                              8 RESUME                   0
                
-                32          10 LOAD_GLOBAL              1 (NULL + int)
+                41          10 LOAD_GLOBAL              1 (NULL + int)
                             22 LOAD_FAST                1 (direction)
                             24 PRECALL                  1
                             28 CALL                     1
                             38 STORE_FAST               2 (increment)
                
-                34          40 LOAD_GLOBAL              3 (NULL + hyprctlJSON)
+                43          40 LOAD_GLOBAL              3 (NULL + hyprctlJSON)
                             52 LOAD_CONST               1 ('monitors')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 GET_AWAITABLE            0
                             70 LOAD_CONST               2 (None)
                        >>   72 SEND                     3 (to 80)
                             74 YIELD_VALUE
                             76 RESUME                   3
                             78 JUMP_BACKWARD_NO_INTERRUPT     4 (to 72)
                        >>   80 STORE_FAST               3 (monitors)
                
-                35          82 LOAD_GLOBAL              5 (NULL + isinstance)
+                44          82 LOAD_GLOBAL              5 (NULL + isinstance)
                             94 LOAD_FAST                3 (monitors)
                             96 LOAD_GLOBAL              6 (list)
                            108 PRECALL                  2
                            112 CALL                     2
                            122 POP_JUMP_FORWARD_IF_TRUE     2 (to 128)
                            124 LOAD_ASSERTION_ERROR
                            126 RAISE_VARARGS            1
                
-                36     >>  128 LOAD_FAST                3 (monitors)
+                45     >>  128 LOAD_FAST                3 (monitors)
                            130 GET_ITER
                        >>  132 FOR_ITER                12 (to 158)
                            134 STORE_DEREF              9 (monitor)
                
-                37         136 LOAD_DEREF               9 (monitor)
+                46         136 LOAD_DEREF               9 (monitor)
                            138 LOAD_CONST               3 ('focused')
                            140 BINARY_SUBSCR
                            150 POP_JUMP_FORWARD_IF_FALSE     2 (to 156)
                
-                38         152 POP_TOP
-                           154 JUMP_FORWARD             1 (to 158)
+                47         152 POP_TOP
+                           154 JUMP_FORWARD            29 (to 214)
                
-                37     >>  156 JUMP_BACKWARD           13 (to 132)
+                46     >>  156 JUMP_BACKWARD           13 (to 132)
                
-                39     >>  158 LOAD_GLOBAL              5 (NULL + isinstance)
-                           170 LOAD_DEREF               9 (monitor)
-                           172 LOAD_GLOBAL              8 (dict)
-                           184 PRECALL                  2
-                           188 CALL                     2
-                           198 POP_JUMP_FORWARD_IF_TRUE     2 (to 204)
-                           200 LOAD_ASSERTION_ERROR
-                           202 RAISE_VARARGS            1
-               
-                40     >>  204 LOAD_GLOBAL             11 (NULL + set)
-                           216 LOAD_CLOSURE             9 (monitor)
-                           218 BUILD_TUPLE              1
-                           220 LOAD_CONST               4 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 40>)
-                           222 MAKE_FUNCTION            8 (closure)
-               
-                41         224 LOAD_FAST                3 (monitors)
-               
-                40         226 GET_ITER
-                           228 PRECALL                  0
-                           232 CALL                     0
-                           242 PRECALL                  1
-                           246 CALL                     1
-                           256 STORE_DEREF              8 (busy_workspaces)
-               
-                43         258 LOAD_DEREF               9 (monitor)
-                           260 LOAD_CONST               5 ('activeWorkspace')
-                           262 BINARY_SUBSCR
-                           272 LOAD_CONST               6 ('id')
-                           274 BINARY_SUBSCR
-                           284 STORE_FAST               4 (cur_workspace)
-               
-                44         286 LOAD_CLOSURE             8 (busy_workspaces)
-                           288 BUILD_TUPLE              1
-                           290 LOAD_CONST               7 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 44>)
-                           292 MAKE_FUNCTION            8 (closure)
-               
-                45         294 LOAD_FAST                0 (self)
-                           296 LOAD_ATTR                6 (workspace_list)
-               
-                44         306 GET_ITER
-                           308 PRECALL                  0
-                           312 CALL                     0
-                           322 STORE_FAST               5 (available_workspaces)
-               
-                47         324 NOP
-               
-                48         326 LOAD_FAST                5 (available_workspaces)
-                           328 LOAD_METHOD              7 (index)
-                           350 LOAD_FAST                4 (cur_workspace)
-                           352 PRECALL                  1
-                           356 CALL                     1
-                           366 STORE_FAST               6 (idx)
-               
-                52         368 LOAD_FAST                5 (available_workspaces)
-               
-                53         370 LOAD_FAST                6 (idx)
-                           372 LOAD_FAST                2 (increment)
-                           374 BINARY_OP                0 (+)
-                           378 LOAD_GLOBAL             17 (NULL + len)
-                           390 LOAD_FAST                5 (available_workspaces)
-                           392 PRECALL                  1
-                           396 CALL                     1
-                           406 BINARY_OP                6 (%)
-               
-                52         410 BINARY_SUBSCR
-                           420 STORE_FAST               7 (next_workspace)
-                           422 JUMP_FORWARD            32 (to 488)
-                       >>  424 PUSH_EXC_INFO
-               
-                49         426 LOAD_GLOBAL             18 (ValueError)
-                           438 CHECK_EXC_MATCH
-                           440 POP_JUMP_FORWARD_IF_FALSE    19 (to 480)
-                           442 POP_TOP
-               
-                50         444 LOAD_FAST                5 (available_workspaces)
-                           446 LOAD_FAST                2 (increment)
-                           448 LOAD_CONST               8 (0)
-                           450 COMPARE_OP               4 (>)
-                           456 POP_JUMP_FORWARD_IF_FALSE     2 (to 462)
-                           458 LOAD_CONST               8 (0)
-                           460 JUMP_FORWARD             1 (to 464)
-                       >>  462 LOAD_CONST               9 (-1)
-                       >>  464 BINARY_SUBSCR
-                           474 STORE_FAST               7 (next_workspace)
-                           476 POP_EXCEPT
-                           478 JUMP_FORWARD             4 (to 488)
-               
-                49     >>  480 RERAISE                  0
-                       >>  482 COPY                     3
-                           484 POP_EXCEPT
-                           486 RERAISE                  1
-               
-                55     >>  488 LOAD_GLOBAL             21 (NULL + hyprctl)
-                           500 LOAD_CONST              10 ('moveworkspacetomonitor ')
-                           502 LOAD_FAST                7 (next_workspace)
-                           504 FORMAT_VALUE             0
-                           506 LOAD_CONST              11 (',')
-                           508 LOAD_DEREF               9 (monitor)
-                           510 LOAD_CONST              12 ('name')
-                           512 BINARY_SUBSCR
-                           522 FORMAT_VALUE             0
-                           524 BUILD_STRING             4
-                           526 PRECALL                  1
-                           530 CALL                     1
-                           540 GET_AWAITABLE            0
-                           542 LOAD_CONST               2 (None)
-                       >>  544 SEND                     3 (to 552)
-                           546 YIELD_VALUE
-                           548 RESUME                   3
-                           550 JUMP_BACKWARD_NO_INTERRUPT     4 (to 544)
-                       >>  552 POP_TOP
-               
-                56         554 LOAD_GLOBAL             21 (NULL + hyprctl)
-                           566 LOAD_CONST              13 ('workspace ')
-                           568 LOAD_FAST                7 (next_workspace)
-                           570 FORMAT_VALUE             0
-                           572 BUILD_STRING             2
-                           574 PRECALL                  1
-                           578 CALL                     1
-                           588 GET_AWAITABLE            0
-                           590 LOAD_CONST               2 (None)
-                       >>  592 SEND                     3 (to 600)
-                           594 YIELD_VALUE
-                           596 RESUME                   3
-                           598 JUMP_BACKWARD_NO_INTERRUPT     4 (to 592)
-                       >>  600 POP_TOP
-                           602 LOAD_CONST               2 (None)
-                           604 RETURN_VALUE
+                49     >>  158 LOAD_FAST                0 (self)
+                           160 LOAD_ATTR                4 (log)
+                           170 LOAD_METHOD              5 (error)
+                           192 LOAD_CONST               4 ('Can not find a focused monitor')
+                           194 PRECALL                  1
+                           198 CALL                     1
+                           208 POP_TOP
+               
+                50         210 LOAD_CONST               2 (None)
+                           212 RETURN_VALUE
+               
+                51     >>  214 LOAD_GLOBAL              5 (NULL + isinstance)
+                           226 LOAD_DEREF               9 (monitor)
+                           228 LOAD_GLOBAL             12 (dict)
+                           240 PRECALL                  2
+                           244 CALL                     2
+                           254 POP_JUMP_FORWARD_IF_TRUE     2 (to 260)
+                           256 LOAD_ASSERTION_ERROR
+                           258 RAISE_VARARGS            1
+               
+                52     >>  260 LOAD_GLOBAL             15 (NULL + set)
+                           272 LOAD_CLOSURE             9 (monitor)
+                           274 BUILD_TUPLE              1
+                           276 LOAD_CONST               5 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 52>)
+                           278 MAKE_FUNCTION            8 (closure)
+               
+                53         280 LOAD_FAST                3 (monitors)
+               
+                52         282 GET_ITER
+                           284 PRECALL                  0
+                           288 CALL                     0
+                           298 PRECALL                  1
+                           302 CALL                     1
+                           312 STORE_DEREF              8 (busy_workspaces)
+               
+                55         314 LOAD_DEREF               9 (monitor)
+                           316 LOAD_CONST               6 ('activeWorkspace')
+                           318 BINARY_SUBSCR
+                           328 LOAD_CONST               7 ('id')
+                           330 BINARY_SUBSCR
+                           340 STORE_FAST               4 (cur_workspace)
+               
+                56         342 LOAD_CLOSURE             8 (busy_workspaces)
+                           344 BUILD_TUPLE              1
+                           346 LOAD_CONST               8 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py", line 56>)
+                           348 MAKE_FUNCTION            8 (closure)
+               
+                57         350 LOAD_FAST                0 (self)
+                           352 LOAD_ATTR                8 (workspace_list)
+               
+                56         362 GET_ITER
+                           364 PRECALL                  0
+                           368 CALL                     0
+                           378 STORE_FAST               5 (available_workspaces)
+               
+                59         380 NOP
+               
+                60         382 LOAD_FAST                5 (available_workspaces)
+                           384 LOAD_METHOD              9 (index)
+                           406 LOAD_FAST                4 (cur_workspace)
+                           408 PRECALL                  1
+                           412 CALL                     1
+                           422 STORE_FAST               6 (idx)
+               
+                64         424 LOAD_FAST                5 (available_workspaces)
+               
+                65         426 LOAD_FAST                6 (idx)
+                           428 LOAD_FAST                2 (increment)
+                           430 BINARY_OP                0 (+)
+                           434 LOAD_GLOBAL             21 (NULL + len)
+                           446 LOAD_FAST                5 (available_workspaces)
+                           448 PRECALL                  1
+                           452 CALL                     1
+                           462 BINARY_OP                6 (%)
+               
+                64         466 BINARY_SUBSCR
+                           476 STORE_FAST               7 (next_workspace)
+                           478 JUMP_FORWARD            32 (to 544)
+                       >>  480 PUSH_EXC_INFO
+               
+                61         482 LOAD_GLOBAL             22 (ValueError)
+                           494 CHECK_EXC_MATCH
+                           496 POP_JUMP_FORWARD_IF_FALSE    19 (to 536)
+                           498 POP_TOP
+               
+                62         500 LOAD_FAST                5 (available_workspaces)
+                           502 LOAD_FAST                2 (increment)
+                           504 LOAD_CONST               9 (0)
+                           506 COMPARE_OP               4 (>)
+                           512 POP_JUMP_FORWARD_IF_FALSE     2 (to 518)
+                           514 LOAD_CONST               9 (0)
+                           516 JUMP_FORWARD             1 (to 520)
+                       >>  518 LOAD_CONST              10 (-1)
+                       >>  520 BINARY_SUBSCR
+                           530 STORE_FAST               7 (next_workspace)
+                           532 POP_EXCEPT
+                           534 JUMP_FORWARD             4 (to 544)
+               
+                61     >>  536 RERAISE                  0
+                       >>  538 COPY                     3
+                           540 POP_EXCEPT
+                           542 RERAISE                  1
+               
+                67     >>  544 LOAD_GLOBAL             25 (NULL + hyprctl)
+                           556 LOAD_CONST              11 ('moveworkspacetomonitor ')
+                           558 LOAD_FAST                7 (next_workspace)
+                           560 FORMAT_VALUE             0
+                           562 LOAD_CONST              12 (',')
+                           564 LOAD_DEREF               9 (monitor)
+                           566 LOAD_CONST              13 ('name')
+                           568 BINARY_SUBSCR
+                           578 FORMAT_VALUE             0
+                           580 BUILD_STRING             4
+                           582 PRECALL                  1
+                           586 CALL                     1
+                           596 GET_AWAITABLE            0
+                           598 LOAD_CONST               2 (None)
+                       >>  600 SEND                     3 (to 608)
+                           602 YIELD_VALUE
+                           604 RESUME                   3
+                           606 JUMP_BACKWARD_NO_INTERRUPT     4 (to 600)
+                       >>  608 POP_TOP
+               
+                68         610 LOAD_GLOBAL             25 (NULL + hyprctl)
+                           622 LOAD_CONST              14 ('workspace ')
+                           624 LOAD_FAST                7 (next_workspace)
+                           626 FORMAT_VALUE             0
+                           628 BUILD_STRING             2
+                           630 PRECALL                  1
+                           634 CALL                     1
+                           644 GET_AWAITABLE            0
+                           646 LOAD_CONST               2 (None)
+                       >>  648 SEND                     3 (to 656)
+                           650 YIELD_VALUE
+                           652 RESUME                   3
+                           654 JUMP_BACKWARD_NO_INTERRUPT     4 (to 648)
+                       >>  656 POP_TOP
+                           658 LOAD_CONST               2 (None)
+                           660 RETURN_VALUE
                ExceptionTable:
-                 326 to 366 -> 424 [0]
-                 424 to 474 -> 482 [1] lasti
-                 480 to 480 -> 482 [1] lasti
+                 382 to 422 -> 480 [0]
+                 480 to 530 -> 538 [1] lasti
+                 536 to 536 -> 538 [1] lasti
                consts
                   '<+1/-1> Switch workspaces of current monitor, avoiding displayed workspaces'
                   'monitors'
                   None
                   'focused'
+                  'Can not find a focused monitor'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 51
                      code
                         0x95014b00010097007c005d247d017c0164001900000000000000000089
                         026400190000000000000000006b0300000000af147c0164011900000000
                         00000000006400190000000000000000005600970101008c2564025300
                                    0 COPY_FREE_VARS           1
                      
-                      40           2 RETURN_GENERATOR
+                      52           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                36 (to 84)
                      
-                      41          12 STORE_FAST               1 (m)
+                      53          12 STORE_FAST               1 (m)
                                   14 LOAD_FAST                1 (m)
                                   16 LOAD_CONST               0 ('id')
                                   18 BINARY_SUBSCR
                                   28 LOAD_DEREF               2 (monitor)
                                   30 LOAD_CONST               0 ('id')
                                   32 BINARY_SUBSCR
                                   42 COMPARE_OP               3 (!=)
@@ -633,44 +689,44 @@
                                   64 LOAD_CONST               0 ('id')
                                   66 BINARY_SUBSCR
                                   76 YIELD_VALUE
                                   78 RESUME                   1
                                   80 POP_TOP
                                   82 JUMP_BACKWARD           37 (to 10)
                      
-                      40     >>   84 LOAD_CONST               2 (None)
+                      52     >>   84 LOAD_CONST               2 (None)
                                   86 RETURN_VALUE
                      consts
                         'id'
                         'activeWorkspace'
                         None
                      names      ()
                      varnames   ('.0', 'm')
                      freevars   ('monitor',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
                      name       '<genexpr>'
-                     firstlineno 40
+                     firstlineno 52
                      lnotab 0x0c0148ff
                   'activeWorkspace'
                   'id'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code 0x9501970067007c005d087d017c0189027601af067c0191028c095300
                                    0 COPY_FREE_VARS           1
                      
-                      44           2 RESUME                   0
+                      56           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                 8 (to 26)
                      
-                      45          10 STORE_FAST               1 (i)
+                      57          10 STORE_FAST               1 (i)
                                   12 LOAD_FAST                1 (i)
                                   14 LOAD_DEREF               2 (busy_workspaces)
                                   16 CONTAINS_OP              1
                                   18 POP_JUMP_BACKWARD_IF_FALSE     6 (to 8)
                                   20 LOAD_FAST                1 (i)
                                   22 LIST_APPEND              2
                                   24 JUMP_BACKWARD            9 (to 8)
@@ -678,42 +734,43 @@
                      consts
                      names      ()
                      varnames   ('.0', 'i')
                      freevars   ('busy_workspaces',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
                      name       '<listcomp>'
-                     firstlineno 44
+                     firstlineno 56
                      lnotab 0x0a01
                   0
                   -1
                   'moveworkspacetomonitor '
                   ','
                   'name'
                   'workspace '
-               names      ('int', 'hyprctlJSON', 'isinstance', 'list', 'dict', 'set', 'workspace_list', 'index', 'len', 'ValueError', 'hyprctl')
+               names      ('int', 'hyprctlJSON', 'isinstance', 'list', 'log', 'error', 'dict', 'set', 'workspace_list', 'index', 'len', 'ValueError', 'hyprctl')
                varnames   ('self', 'direction', 'increment', 'monitors', 'cur_workspace', 'available_workspaces', 'idx', 'next_workspace')
                freevars   ()
                cellvars   ('busy_workspaces', 'monitor')
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
                name       'run_change_workspace'
-               firstlineno 30
+               firstlineno 39
                lnotab
-                  0x0a021e022a012e010801100104ff02022e01140102ff20031c0108010c
-                  ff120302012a04020128ff10fd120124ff08064201
-         names      ('__name__', '__module__', '__qualname__', 'load_config', 'event_focusedmon', 'str', 'run_change_workspace', '__classcell__')
+                  0x0a021e022a012e010801100104ff0203340104012e01140102ff20031c
+                  0108010cff120302012a04020128ff10fd120124ff08064201
+         names      ('__name__', '__module__', '__qualname__', 'workspace_list', 'list', 'int', '__annotations__', 'load_config', 'event_focusedmon', 'str', 'run_change_workspace', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
          name       'Extension'
-         firstlineno 7
-         lnotab 0x0c010a040612
+         firstlineno 8
+         lnotab 0x0e011a020a050617
       'Extension'
-   names      ('asyncio', 'interface', 'Plugin', 'ipc', 'hyprctlJSON', 'hyprctl', 'Extension')
+      None
+   names      ('__doc__', 'typing', 'cast', 'interface', 'Plugin', 'ipc', 'hyprctlJSON', 'hyprctl', 'Extension')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/fab/dev/std/pyprland/pyprland/plugins/workspaces_follow_focus.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c021003
+   lnotab 0x00ff020104010c010c021003
```

### Comparing `pyprland-1.3.1/pyprland/plugins/lost_windows.py` & `pyprland-1.4.0/pyprland/plugins/lost_windows.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,45 @@
+" Moves unreachable client windows to the currently focused workspace"
+from typing import Any, cast
 from .interface import Plugin
 
 from ..ipc import hyprctlJSON, hyprctl
 
 
 def contains(monitor, window):
+    "Tell if a window is visible in a monitor"
     if not (
         window["at"][0] > monitor["x"]
         and window["at"][0] < monitor["x"] + monitor["width"]
     ):
         return False
     if not (
         window["at"][1] > monitor["y"]
         and window["at"][1] < monitor["y"] + monitor["height"]
     ):
         return False
     return True
 
 
-class Extension(Plugin):
-    async def run_attract_lost(self, *args):
+class Extension(Plugin):  # pylint: disable=missing-class-docstring
+    async def run_attract_lost(self):
         """Brings lost floating windows to the current workspace"""
-        monitors = await hyprctlJSON("monitors")
-        windows = await hyprctlJSON("clients")
+        monitors = cast(list, await hyprctlJSON("monitors"))
+        windows = cast(list, await hyprctlJSON("clients"))
         lost = [
             win
             for win in windows
             if win["floating"] and not any(contains(mon, win) for mon in monitors)
         ]
-        focused = [mon for mon in monitors if mon["focused"]][0]
+        focused: dict[str, Any] = [mon for mon in monitors if mon["focused"]][0]
         interval = focused["width"] / (1 + len(lost))
-        intervalY = focused["height"] / (1 + len(lost))
+        interval_y = focused["height"] / (1 + len(lost))
         batch = []
         workspace: int = focused["activeWorkspace"]["id"]
         margin = interval // 2
-        marginY = intervalY // 2
+        margin_y = interval_y // 2
         for i, window in enumerate(lost):
+            pos_x = int(margin + focused["x"] + i * interval)
+            pos_y = {int(margin_y + focused["y"] + i * interval_y)}
             batch.append(f'movetoworkspacesilent {workspace},pid:{window["pid"]}')
-            batch.append(
-                f'movewindowpixel exact {int(margin + focused["x"] + i*interval)} {int(marginY + focused["y"] + i*intervalY)},pid:{window["pid"]}'
-            )
+            batch.append(f'movewindowpixel exact {pos_x} {pos_y},pid:{window["pid"]}')
         await hyprctl(batch)
```

### Comparing `pyprland-1.3.1/pyprland/plugins/magnify.py` & `pyprland-1.4.0/pyprland/plugins/magnify.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+" Toggles workspace zooming "
 from .interface import Plugin
 
-from ..ipc import hyprctlJSON, hyprctl
+from ..ipc import hyprctl
 
 
-class Extension(Plugin):
-    async def init(self):
-        self.zoomed = False
+class Extension(Plugin):  # pylint: disable=missing-class-docstring
+    zoomed = False
 
     async def run_zoom(self, *args):
         """[factor] zooms to "factor" or toggles zoom level ommited"""
         if args:
             value = int(args[0])
             await hyprctl(f"misc:cursor_zoom_factor {value}", "keyword")
             self.zoomed = value != 1
```

### Comparing `pyprland-1.3.1/pyprland/plugins/monitors.py` & `pyprland-1.4.0/pyprland/plugins/monitors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Any
-from .interface import Plugin
+" The monitors plugin "
 import subprocess
+from typing import Any, cast
+from .interface import Plugin
 
 from ..ipc import hyprctlJSON
 
 
-def configure_monitors(monitors, screenid: str, x: int, y: int) -> None:
-    x_offset = -x if x < 0 else 0
-    y_offset = -y if y < 0 else 0
+def configure_monitors(monitors, screenid: str, pos_x: int, pos_y: int) -> None:
+    "Apply the configuration change"
+    x_offset = -pos_x if pos_x < 0 else 0
+    y_offset = -pos_y if pos_y < 0 else 0
 
-    min_x = x
-    min_y = y
+    min_x = pos_x
+    min_y = pos_y
 
     command = ["wlr-randr"]
     other_monitors = [mon for mon in monitors if mon["name"] != screenid]
     for mon in other_monitors:
         min_x = min(min_x, mon["x"])
         min_y = min(min_y, mon["y"])
     x_offset = -min_x
@@ -25,65 +27,79 @@
                 "--output",
                 mon["name"],
                 "--pos",
                 f"{mon['x']+x_offset},{mon['y']+y_offset}",
             ]
         )
 
-    command.extend(["--output", screenid, "--pos", f"{x+x_offset},{y+y_offset}"])
+    command.extend(
+        ["--output", screenid, "--pos", f"{pos_x+x_offset},{pos_y+y_offset}"]
+    )
     subprocess.call(command)
 
 
-class Extension(Plugin):
+class Extension(Plugin):  # pylint: disable=missing-class-docstring
     async def load_config(self, config) -> None:
         await super().load_config(config)
-        monitors = await hyprctlJSON("monitors")
+        monitors = cast(list[dict], await hyprctlJSON("monitors"))
         for monitor in monitors:
             await self.event_monitoradded(
-                monitor["name"], noDefault=True, monitors=monitors
+                monitor["name"], no_default=True, monitors=monitors
             )
 
     async def event_monitoradded(
-        self, screenid, noDefault=False, monitors: list | None = None
+        self, monitor_name, no_default=False, monitors: list | None = None
     ) -> None:
-        screenid = screenid.strip()
+        "Triggers when a monitor is plugged"
+        monitor_name = monitor_name.strip()
 
         if not monitors:
-            monitors: list[dict[str, Any]] = await hyprctlJSON("monitors")
+            monitors = cast(list, await hyprctlJSON("monitors"))
+
+        assert monitors
 
         for mon in monitors:
-            if mon["name"].startswith(screenid):
-                mon_name = mon["description"]
+            if mon["name"].startswith(monitor_name):
+                mon_description = mon["description"]
                 break
         else:
-            print(f"Monitor {screenid} not found")
+            self.log.info("Monitor %s not found", monitor_name)
             return
 
-        mon_by_name = {m["name"]: m for m in monitors}
+        if self._place_monitors(monitor_name, mon_description, monitors):
+            return
 
-        newmon = mon_by_name[screenid]
+        if not no_default:
+            default_command = self.config.get("unknown")
+            if default_command:
+                subprocess.call(default_command, shell=True)
 
+    def _place_monitors(
+        self, monitor_name: str, mon_description: str, monitors: list[dict[str, Any]]
+    ):
+        "place a given monitor according to config"
+        mon_by_name = {m["name"]: m for m in monitors}
+        newmon = mon_by_name[monitor_name]
         for mon_pattern, conf in self.config["placement"].items():
-            if mon_pattern in mon_name:
-                for placement, mon_name in conf.items():
-                    ref = mon_by_name[mon_name]
+            if mon_pattern in mon_description:
+                for placement, other_mon_description in conf.items():
+                    ref = mon_by_name[other_mon_description]
                     if ref:
                         place = placement.lower()
+                        x: int = 0
+                        y: int = 0
                         if place == "topof":
-                            x: int = ref["x"]
-                            y: int = ref["y"] - newmon["height"]
+                            x = ref["x"]
+                            y = ref["y"] - newmon["height"]
                         elif place == "bottomof":
-                            x: int = ref["x"]
-                            y: int = ref["y"] + ref["height"]
+                            x = ref["x"]
+                            y = ref["y"] + ref["height"]
                         elif place == "leftof":
-                            x: int = ref["x"] - newmon["width"]
-                            y: int = ref["y"]
+                            x = ref["x"] - newmon["width"]
+                            y = ref["y"]
                         else:  # rightof
-                            x: int = ref["x"] + ref["width"]
-                            y: int = ref["y"]
+                            x = ref["x"] + ref["width"]
+                            y = ref["y"]
 
-                        configure_monitors(monitors, screenid, x, y)
-                        return
-        if not noDefault:
-            default_command = self.config.get("unknown")
-            if default_command:
-                subprocess.call(default_command, shell=True)
+                        configure_monitors(monitors, monitor_name, x, y)
+                        return True
+        return False
```

### Comparing `pyprland-1.3.1/pyprland/plugins/scratchpads.py` & `pyprland-1.4.0/pyprland/plugins/scratchpads.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,269 +1,338 @@
-import subprocess
-from typing import Any
+" Scratchpads addon "
+import os
 import asyncio
+import subprocess
+from typing import Any, cast
+
 from ..ipc import (
     hyprctl,
     hyprctlJSON,
     get_focused_monitor_props,
 )
-import os
 
 from .interface import Plugin
 
 DEFAULT_MARGIN = 60
 
 
 async def get_client_props_by_address(addr: str):
+    "Returns client properties given its address"
     for client in await hyprctlJSON("clients"):
         assert isinstance(client, dict)
         if client.get("address") == addr:
             return client
 
 
 class Animations:
-    @classmethod
-    async def fromtop(cls, monitor, client, client_uid, margin):
+    "Animation store"
+
+    @staticmethod
+    async def fromtop(monitor, client, client_uid, margin):
+        "Slide from/to top"
+        scale = float(monitor["scale"])
         mon_x = monitor["x"]
         mon_y = monitor["y"]
-        mon_width = monitor["width"]
+        mon_width = int(monitor["width"] / scale)
 
         client_width = client["size"][0]
         margin_x = int((mon_width - client_width) / 2) + mon_x
+
         await hyprctl(f"movewindowpixel exact {margin_x} {mon_y + margin},{client_uid}")
 
-    @classmethod
-    async def frombottom(cls, monitor, client, client_uid, margin):
+    @staticmethod
+    async def frombottom(monitor, client, client_uid, margin):
+        "Slide from/to bottom"
+        scale = float(monitor["scale"])
         mon_x = monitor["x"]
         mon_y = monitor["y"]
-        mon_width = monitor["width"]
-        mon_height = monitor["height"]
+        mon_width = int(monitor["width"] / scale)
+        mon_height = int(monitor["height"] / scale)
 
         client_width = client["size"][0]
         client_height = client["size"][1]
         margin_x = int((mon_width - client_width) / 2) + mon_x
         await hyprctl(
             f"movewindowpixel exact {margin_x} {mon_y + mon_height - client_height - margin},{client_uid}"
         )
 
-    @classmethod
-    async def fromleft(cls, monitor, client, client_uid, margin):
+    @staticmethod
+    async def fromleft(monitor, client, client_uid, margin):
+        "Slide from/to left"
+        scale = float(monitor["scale"])
         mon_x = monitor["x"]
         mon_y = monitor["y"]
-        mon_height = monitor["height"]
+        mon_height = int(monitor["height"] / scale)
 
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
 
         await hyprctl(f"movewindowpixel exact {margin + mon_x} {margin_y},{client_uid}")
 
-    @classmethod
-    async def fromright(cls, monitor, client, client_uid, margin):
+    @staticmethod
+    async def fromright(monitor, client, client_uid, margin):
+        "Slide from/to right"
+        scale = float(monitor["scale"])
         mon_x = monitor["x"]
         mon_y = monitor["y"]
-        mon_width = monitor["width"]
-        mon_height = monitor["height"]
+        mon_width = int(monitor["width"] / scale)
+        mon_height = int(monitor["height"] / scale)
 
         client_width = client["size"][0]
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
         await hyprctl(
             f"movewindowpixel exact {mon_width - client_width - margin + mon_x } {margin_y},{client_uid}"
         )
 
 
 class Scratch:
+    "A scratchpad state including configuration & client state"
+
     def __init__(self, uid, opts):
         self.uid = uid
         self.pid = 0
         self.conf = opts
         self.visible = False
         self.just_created = True
-        self.clientInfo = {}
+        self.client_info = {}
 
     def isAlive(self) -> bool:
+        "is the process running ?"
         path = f"/proc/{self.pid}"
         if os.path.exists(path):
-            for line in open(os.path.join(path, "status"), "r").readlines():
-                if line.startswith("State"):
-                    state = line.split()[1]
-                    return state in "RSDTt"  # not "Z (zombie)"or "X (dead)"
+            with open(os.path.join(path, "status"), "r", encoding="utf-8") as f:
+                for line in f.readlines():
+                    if line.startswith("State"):
+                        state = line.split()[1]
+                        return state in "RSDTt"  # not "Z (zombie)"or "X (dead)"
         return False
 
     def reset(self, pid: int) -> None:
+        "clear the object"
         self.pid = pid
         self.visible = False
         self.just_created = True
-        self.clientInfo = {}
+        self.client_info = {}
 
     @property
     def address(self) -> str:
-        return str(self.clientInfo.get("address", ""))[2:]
+        "Returns the client address"
+        return str(self.client_info.get("address", ""))[2:]
 
-    async def updateClientInfo(self, clientInfo=None) -> None:
-        if clientInfo is None:
-            clientInfo = await get_client_props_by_address("0x" + self.address)
-        assert isinstance(clientInfo, dict)
-        self.clientInfo.update(clientInfo)
-
-
-class Extension(Plugin):
-    async def init(self) -> None:
-        self.procs: dict[str, subprocess.Popen] = {}
-        self.scratches: dict[str, Scratch] = {}
-        self.transitioning_scratches: set[str] = set()
-        self._respawned_scratches: set[str] = set()
-        self.scratches_by_address: dict[str, Scratch] = {}
-        self.scratches_by_pid: dict[int, Scratch] = {}
-        self.focused_window_tracking = dict()
+    async def updateClientInfo(self, client_info=None) -> None:
+        "update the internal client info property, if not provided, refresh based on the current address"
+        if client_info is None:
+            client_info = await get_client_props_by_address("0x" + self.address)
+        assert isinstance(client_info, dict)
+        self.client_info.update(client_info)
+
+    def __str__(self):
+        return f"{self.uid} {self.address} : {self.client_info} / {self.conf}"
+
+
+class Extension(Plugin):  # pylint: disable=missing-class-docstring
+    procs: dict[str, subprocess.Popen] = {}
+    scratches: dict[str, Scratch] = {}
+    transitioning_scratches: set[str] = set()
+    _new_scratches: set[str] = set()
+    _respawned_scratches: set[str] = set()
+    scratches_by_address: dict[str, Scratch] = {}
+    scratches_by_pid: dict[int, Scratch] = {}
+    focused_window_tracking: dict[str, dict] = {}
 
     async def exit(self) -> None:
+        "exit hook"
+
         async def die_in_piece(scratch: Scratch):
             proc = self.procs[scratch.uid]
             proc.terminate()
-            for n in range(10):
+            for _ in range(10):
                 if not scratch.isAlive():
                     break
                 await asyncio.sleep(0.1)
             if scratch.isAlive():
                 proc.kill()
             proc.wait()
 
         await asyncio.gather(
             *(die_in_piece(scratch) for scratch in self.scratches.values())
         )
 
-    async def load_config(self, config) -> None:
-        config: dict[str, dict[str, Any]] = config["scratchpads"]
-        scratches = {k: Scratch(k, v) for k, v in config.items()}
+    async def load_config(self, config: dict[str, Any]) -> None:
+        "config loader"
+        my_config: dict[str, dict[str, Any]] = config["scratchpads"]
+        scratches = {k: Scratch(k, v) for k, v in my_config.items()}
 
         new_scratches = set()
 
         for name in scratches:
             if name not in self.scratches:
                 self.scratches[name] = scratches[name]
                 new_scratches.add(name)
             else:
                 self.scratches[name].conf = scratches[name].conf
 
         # not known yet
         for name in new_scratches:
-            self.start_scratch_command(name)
+            if not self.scratches[name].conf.get("lazy", False):
+                await self.start_scratch_command(name, is_new=True)
 
-    def start_scratch_command(self, name: str) -> None:
+    async def start_scratch_command(self, name: str, is_new=False) -> None:
+        "spawns a given scratchpad's process"
+        if is_new:
+            self._new_scratches.add(name)
         self._respawned_scratches.add(name)
         scratch = self.scratches[name]
         old_pid = self.procs[name].pid if name in self.procs else 0
-        self.procs[name] = subprocess.Popen(
+        proc = subprocess.Popen(
             scratch.conf["command"],
             stdin=subprocess.DEVNULL,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
             shell=True,
         )
-        pid = self.procs[name].pid
+        self.procs[name] = proc
+        pid = proc.pid
         self.scratches[name].reset(pid)
-        self.scratches_by_pid[self.procs[name].pid] = scratch
+        self.scratches_by_pid[proc.pid] = scratch
+
         if old_pid and old_pid in self.scratches_by_pid:
             del self.scratches_by_pid[old_pid]
 
     # Events
     async def event_activewindowv2(self, addr) -> None:
+        "active windows hook"
         addr = addr.strip()
         scratch = self.scratches_by_address.get(addr)
         if scratch:
             if scratch.just_created:
+                self.log.debug("Hiding just created scratch %s", scratch.uid)
                 await self.run_hide(scratch.uid, force=True)
                 scratch.just_created = False
         else:
             for uid, scratch in self.scratches.items():
-                if scratch.clientInfo and scratch.address != addr:
+                if scratch.client_info and scratch.address != addr:
                     if (
                         scratch.visible
                         and scratch.conf.get("unfocus") == "hide"
                         and scratch.uid not in self.transitioning_scratches
                     ):
+                        self.log.debug("hide %s because another client is active", uid)
                         await self.run_hide(uid, autohide=True)
 
+    async def _alternative_lookup(self):
+        "if class attribute is defined, use class matching and return True"
+        class_lookup_hack = [
+            self.scratches[name]
+            for name in self._respawned_scratches
+            if self.scratches[name].conf.get("class")
+        ]
+        if not class_lookup_hack:
+            return False
+        self.log.debug("Lookup hack triggered")
+        for client in await hyprctlJSON("clients"):
+            assert isinstance(client, dict)
+            for pending_scratch in class_lookup_hack:
+                if pending_scratch.conf["class"] == client["class"]:
+                    self.scratches_by_address[client["address"][2:]] = pending_scratch
+                    self.log.debug("client class found: %s", client)
+                    await pending_scratch.updateClientInfo(client)
+        return True
+
     async def event_openwindow(self, params) -> None:
-        addr, wrkspc, kls, title = params.split(",", 3)
+        "open windows hook"
+        addr, wrkspc, _kls, _title = params.split(",", 3)
         if wrkspc.startswith("special"):
             item = self.scratches_by_address.get(addr)
             if not item and self._respawned_scratches:
-                await self.updateScratchInfo()
+                # hack for windows which aren't related to the process (see #8)
+                if not await self._alternative_lookup():
+                    await self.updateScratchInfo()
                 item = self.scratches_by_address.get(addr)
             if item and item.just_created:
+                if item.uid in self._new_scratches:
+                    await self.run_hide(item.uid, force=True)
+                self._new_scratches.discard(item.uid)
                 self._respawned_scratches.discard(item.uid)
-                await self.run_hide(item.uid, force=True)
                 item.just_created = False
 
     async def run_toggle(self, uid: str) -> None:
         """<name> toggles visibility of scratchpad "name" """
         uid = uid.strip()
         item = self.scratches.get(uid)
         if not item:
-            print(f"{uid} is not configured")
+            self.log.warning("%s is not configured", uid)
             return
+        self.log.debug("%s is visible = %s", uid, item.visible)
         if item.visible:
             await self.run_hide(uid)
         else:
             await self.run_show(uid)
 
+    async def _anim_hide(self, animation_type, scratch):
+        "animate hiding a scratchpad"
+        addr = "address:0x" + scratch.address
+        offset = scratch.conf.get("offset")
+        if offset is None:
+            if "size" not in scratch.client_info:
+                await self.updateScratchInfo(scratch)
+
+            offset = int(1.3 * scratch.client_info["size"][1])
+
+        if animation_type == "fromtop":
+            await hyprctl(f"movewindowpixel 0 -{offset},{addr}")
+        elif animation_type == "frombottom":
+            await hyprctl(f"movewindowpixel 0 {offset},{addr}")
+        elif animation_type == "fromleft":
+            await hyprctl(f"movewindowpixel -{offset} 0,{addr}")
+        elif animation_type == "fromright":
+            await hyprctl(f"movewindowpixel {offset} 0,{addr}")
+
+        if scratch.uid in self.transitioning_scratches:
+            return  # abort sequence
+        await asyncio.sleep(0.2)  # await for animation to finish
+
     async def updateScratchInfo(self, scratch: Scratch | None = None) -> None:
+        """Update every scratchpads information if no `scratch` given,
+        else update a specific scratchpad info"""
         if scratch is None:
             for client in await hyprctlJSON("clients"):
                 assert isinstance(client, dict)
                 scratch = self.scratches_by_address.get(client["address"][2:])
                 if not scratch:
                     scratch = self.scratches_by_pid.get(client["pid"])
                     if scratch:
                         self.scratches_by_address[client["address"][2:]] = scratch
                 if scratch:
                     await scratch.updateClientInfo(client)
         else:
-            add_to_address_book = ("address" not in scratch.clientInfo) or (
+            add_to_address_book = ("address" not in scratch.client_info) or (
                 scratch.address not in self.scratches_by_address
             )
             await scratch.updateClientInfo()
             if add_to_address_book:
-                self.scratches_by_address[scratch.clientInfo["address"][2:]] = scratch
+                self.scratches_by_address[scratch.client_info["address"][2:]] = scratch
 
     async def run_hide(self, uid: str, force=False, autohide=False) -> None:
         """<name> hides scratchpad "name" """
         uid = uid.strip()
-        item = self.scratches.get(uid)
-        if not item:
-            print(f"{uid} is not configured")
+        scratch = self.scratches.get(uid)
+        if not scratch:
+            self.log.warning("%s is not configured", uid)
             return
-        if not item.visible and not force:
-            print(f"{uid} is already hidden")
+        if not scratch.visible and not force:
+            self.log.warning("%s is already hidden", uid)
             return
-        item.visible = False
-        addr = "address:0x" + item.address
-        animation_type: str = item.conf.get("animation", "").lower()
+        self.log.info("Hiding %s", uid)
+        scratch.visible = False
+        addr = "address:0x" + scratch.address
+        animation_type: str = scratch.conf.get("animation", "").lower()
         if animation_type:
-            offset = item.conf.get("offset")
-            if offset is None:
-                if "size" not in item.clientInfo:
-                    await self.updateScratchInfo(item)
-
-                offset = int(1.3 * item.clientInfo["size"][1])
-
-            if animation_type == "fromtop":
-                await hyprctl(f"movewindowpixel 0 -{offset},{addr}")
-            elif animation_type == "frombottom":
-                await hyprctl(f"movewindowpixel 0 {offset},{addr}")
-            elif animation_type == "fromleft":
-                await hyprctl(f"movewindowpixel -{offset} 0,{addr}")
-            elif animation_type == "fromright":
-                await hyprctl(f"movewindowpixel {offset} 0,{addr}")
-
-            if uid in self.transitioning_scratches:
-                return  # abort sequence
-            await asyncio.sleep(0.2)  # await for animation to finish
+            await self._anim_hide(animation_type, scratch)
 
         if uid not in self.transitioning_scratches:
             await hyprctl(f"movetoworkspacesilent special:scratch_{uid},{addr}")
 
         if (
             animation_type and uid in self.focused_window_tracking
         ):  # focus got lost when animating
@@ -274,32 +343,37 @@
                 del self.focused_window_tracking[uid]
 
     async def run_show(self, uid, force=False) -> None:
         """<name> shows scratchpad "name" """
         uid = uid.strip()
         item = self.scratches.get(uid)
 
-        self.focused_window_tracking[uid] = await hyprctlJSON("activewindow")
+        self.focused_window_tracking[uid] = cast(
+            dict[str, Any], await hyprctlJSON("activewindow")
+        )
 
         if not item:
-            print(f"{uid} is not configured")
+            self.log.warning("%s is not configured", uid)
             return
 
         if item.visible and not force:
-            print(f"{uid} is already visible")
+            self.log.warning("%s is already visible", uid)
             return
 
+        self.log.info("Showing %s", uid)
+
         if not item.isAlive():
-            print(f"{uid} is not running, restarting...")
-            self.procs[uid].kill()
+            self.log.info("%s is not running, restarting...", uid)
+            if uid in self.procs:
+                self.procs[uid].kill()
             if item.pid in self.scratches_by_pid:
                 del self.scratches_by_pid[item.pid]
             if item.address in self.scratches_by_address:
                 del self.scratches_by_address[item.address]
-            self.start_scratch_command(uid)
+            await self.start_scratch_command(uid)
             while uid in self._respawned_scratches:
                 await asyncio.sleep(0.05)
 
         item.visible = True
         monitor = await get_focused_monitor_props()
         assert monitor
 
@@ -313,12 +387,12 @@
 
         self.transitioning_scratches.add(uid)
         await hyprctl(f"moveworkspacetomonitor special:scratch_{uid} {monitor['name']}")
         await hyprctl(f"movetoworkspacesilent {wrkspc},{addr}")
         if animation_type:
             margin = item.conf.get("margin", DEFAULT_MARGIN)
             fn = getattr(Animations, animation_type)
-            await fn(monitor, item.clientInfo, addr, margin)
+            await fn(monitor, item.client_info, addr, margin)
 
         await hyprctl(f"focuswindow {addr}")
         await asyncio.sleep(0.2)  # ensure some time for events to propagate
         self.transitioning_scratches.discard(uid)
```

### Comparing `pyprland-1.3.1/pyprland/plugins/shift_monitors.py` & `pyprland-1.4.0/pyprland/plugins/shift_monitors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+" shift workspaces across monitors "
+from typing import cast
 from .interface import Plugin
 
 from ..ipc import hyprctlJSON, hyprctl
 
 
-class Extension(Plugin):
+class Extension(Plugin):  # pylint: disable=missing-class-docstring
+    monitors: list[str] = []
+
     async def init(self):
-        self.monitors = [mon["name"] for mon in await hyprctlJSON("monitors")]
+        self.monitors: list[str] = [
+            mon["name"] for mon in cast(list[dict], await hyprctlJSON("monitors"))
+        ]
 
     async def run_shift_monitors(self, arg: str):
         """Swaps monitors' workspaces in the given direction"""
         direction: int = int(arg)
         if direction > 0:
             mon_list = self.monitors[:-1]
         else:
-            mon_list = reversed(self.monitors[1:])
+            mon_list = list(reversed(self.monitors[1:]))
 
         for i, mon in enumerate(mon_list):
             await hyprctl(f"swapactiveworkspaces {mon} {self.monitors[i+direction]}")
 
     async def event_monitoradded(self, monitor):
+        "keep track of monitors"
         self.monitors.append(monitor.strip())
 
     async def event_monitorremoved(self, monitor):
+        "keep track of monitors"
         self.monitors.remove(monitor.strip())
```

### Comparing `pyprland-1.3.1/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-1.4.0/pyprland/plugins/workspaces_follow_focus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-import asyncio
+""" Force workspaces to follow the focus / mouse """
+from typing import cast
 from .interface import Plugin
 
 from ..ipc import hyprctlJSON, hyprctl
 
 
-class Extension(Plugin):
+class Extension(Plugin):  # pylint: disable=missing-class-docstring
+    workspace_list: list[int] = []
+
     async def load_config(self, config):
+        "loads the config"
         await super().load_config(config)
         self.workspace_list = list(range(1, self.config.get("max_workspaces", 10) + 1))
 
     async def event_focusedmon(self, screenid_index):
+        "reacts to monitor changes"
         monitor_id, workspace_id = screenid_index.split(",")
         workspace_id = int(workspace_id)
         # move every free workspace to the currently focused desktop
         busy_workspaces = set(
             mon["activeWorkspace"]["id"]
-            for mon in await hyprctlJSON("monitors")
+            for mon in cast(list[dict], await hyprctlJSON("monitors"))
             if mon["name"] != monitor_id
         )
-        workspaces = [w["id"] for w in await hyprctlJSON("workspaces") if w["id"] > 0]
+        workspaces = [
+            w["id"]
+            for w in cast(list[dict], await hyprctlJSON("workspaces"))
+            if w["id"] > 0
+        ]
 
         batch: list[str | list[str]] = []
         for n in workspaces:
             if n in busy_workspaces or n == workspace_id:
                 continue
             batch.append(f"moveworkspacetomonitor {n} {monitor_id}")
         await hyprctl(batch)
@@ -32,14 +41,17 @@
         increment = int(direction)
         # get focused screen info
         monitors = await hyprctlJSON("monitors")
         assert isinstance(monitors, list)
         for monitor in monitors:
             if monitor["focused"]:
                 break
+        else:
+            self.log.error("Can not find a focused monitor")
+            return
         assert isinstance(monitor, dict)
         busy_workspaces = set(
             m["activeWorkspace"]["id"] for m in monitors if m["id"] != monitor["id"]
         )
         cur_workspace = monitor["activeWorkspace"]["id"]
         available_workspaces = [
             i for i in self.workspace_list if i not in busy_workspaces
```

