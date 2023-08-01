# Comparing `tmp/fv1_programmer-0.2.6.tar.gz` & `tmp/fv1_programmer-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.2.6.tar", max compression
+gzip compressed data, was "fv1_programmer-0.2.7.tar", max compression
```

## Comparing `fv1_programmer-0.2.6.tar` & `fv1_programmer-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/LICENSE
--rw-r--r--   0        0        0      613 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/README.md
--rw-r--r--   0        0        0     1140 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/adaptor/mcp2221.py
--rw-r--r--   0        0        0       30 2023-08-01 17:34:23.142765 fv1_programmer-0.2.6/asfv1/.git
--rw-r--r--   0        0        0     1157 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/LICENSE
--rw-r--r--   0        0        0    36334 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/README.md
--rw-r--r--   0        0        0    54482 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/asfv1.py
--rw-r--r--   0        0        0      561 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/example.asm
--rw-r--r--   0        0        0      801 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/setup.py
--rw-r--r--   0        0        0       31 2023-08-01 17:34:23.706807 fv1_programmer-0.2.6/disfv1/.git
--rw-r--r--   0        0        0     1157 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/LICENSE
--rw-r--r--   0        0        0     4816 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/README.md
--rw-r--r--   0        0        0    17532 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/disfv1.py
--rw-r--r--   0        0        0      512 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/example.bin
--rw-r--r--   0        0        0      798 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/setup.py
--rw-r--r--   0        0        0     6747 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/eeprom/eeprom.py
--rw-r--r--   0        0        0     1780 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/fv1.py
--rw-r--r--   0        0        0     3429 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/main.py
--rw-r--r--   0        0        0     3160 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/tui.css
--rw-r--r--   0        0        0    19020 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/tui.py
--rw-r--r--   0        0        0     1267 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 fv1_programmer-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/LICENSE
+-rw-r--r--   0        0        0      613 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/README.md
+-rw-r--r--   0        0        0     1140 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2023-08-01 20:33:17.468468 fv1_programmer-0.2.7/asfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2023-08-01 20:33:17.864487 fv1_programmer-0.2.7/disfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/setup.py
+-rw-r--r--   0        0        0     6747 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1717 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3081 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/main.py
+-rw-r--r--   0        0        0     3160 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    22358 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1267 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 fv1_programmer-0.2.7/PKG-INFO
```

### Comparing `fv1_programmer-0.2.6/LICENSE` & `fv1_programmer-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/README.md` & `fv1_programmer-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/adaptor/adapter.py` & `fv1_programmer-0.2.7/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/adaptor/mcp2221.py` & `fv1_programmer-0.2.7/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/asfv1/.gitignore` & `fv1_programmer-0.2.7/asfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/asfv1/LICENSE` & `fv1_programmer-0.2.7/asfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/asfv1/README.md` & `fv1_programmer-0.2.7/asfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/asfv1/asfv1.py` & `fv1_programmer-0.2.7/asfv1/asfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/asfv1/example.asm` & `fv1_programmer-0.2.7/asfv1/example.asm`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/asfv1/setup.py` & `fv1_programmer-0.2.7/asfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/disfv1/.gitignore` & `fv1_programmer-0.2.7/disfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/disfv1/LICENSE` & `fv1_programmer-0.2.7/disfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/disfv1/README.md` & `fv1_programmer-0.2.7/disfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/disfv1/disfv1.py` & `fv1_programmer-0.2.7/disfv1/disfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/disfv1/setup.py` & `fv1_programmer-0.2.7/disfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/eeprom/eeprom.py` & `fv1_programmer-0.2.7/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/fv1_programmer/fv1.py` & `fv1_programmer-0.2.7/fv1_programmer/fv1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from asfv1.asfv1 import fv1parse, ASFV1Error
+from disfv1.disfv1 import fv1deparse
 from typing import Tuple
 
 
-EMPTY_FV1_PROGRAM_ASM = """
-; Empty program
-
-start:
-    NOP
-end:
-    NOP
-"""
+FV1_PROGRAM_MAX_BYTES = 512
 
 class FV1Program(object):
     def __init__(self, asm) -> None:
         self.asm = asm
 
     def assemble(self, clamp=True, spinreals=False) -> Tuple[bytearray, str, str]:
- 
+        """
+        Assembles our internal asm to a bytearray, returning any errors and warnings
+        as concatenated strings.
+        """
         warnings = []
         errors = []
 
         def warning(msg):
             nonlocal warnings
             warnings.append(msg)
 
@@ -36,36 +33,30 @@
         except ASFV1Error:
             if len(errors) == 0:
                 errors = ["Failed to assemble program"]
             return None, warnings, errors
 
         return fp.program, warnings, errors
 
-    def as_markdown(self,) -> str:
-        return f"""```
-{self.asm}
-```"""
-
-
-class FV1FS(object):
-    """
-    A utility class representing the filesystem supported by the FV-1.
-
-    The EEPROM image supported by the FV-1 is effectively 8 chunks of
-    EEPROM of equal size (128 32-bit words each) containing the machine
-    code for 8 different presets.
-    """
-    def __init__(self, adaptor=None) -> None:
+    def from_bytearray(self, data : bytearray, relative=False, suppressraw=False) -> str:
         """
-        Create an FV1 filesystem. If adaptor is None, this will operate in simulation mode.
+        Disassembles a binary FV1 program and sets the internal asm property to
+        the disassembled output. Returns any warnings in a concatenated string.
         """
-        self.adaptor = adaptor
+        warnings = []
+
+        def warning(msg):
+            nonlocal warnings
+            warnings.append(msg)
 
-#     def set_eeprom()
+        fp = fv1deparse(data,
+                        relative=relative, nopraw=suppressraw,
+                        wfunc=warning)
+        fp.deparse()
+        self.asm = fp.listing
 
-# def __get_eeprom(args, adaptor):
-#     if args.sim:
-#         from eeprom.eeprom import DummyEEPROM
-#         return DummyEEPROM(args.sim, args.ee_size)
+        return warnings
 
-#     from eeprom.eeprom import I2CEEPROM
-#     return I2CEEPROM(adaptor, args.ee_size, page_size_in_bytes=args.ee_page_size)
+    def as_markdown(self,) -> str:
+        return f"""```
+{self.asm}
+```"""
```

### Comparing `fv1_programmer-0.2.6/fv1_programmer/main.py` & `fv1_programmer-0.2.7/fv1_programmer/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,83 @@
 import argparse
-# from pathlib import Path
-# import sys
+from pathlib import Path
+import sys
 
 
 def parse_command_line_arguments():
     parser = argparse.ArgumentParser()
-#     parser.add_argument('--programmer', default='MCP2221', choices=['MCP2221'],
-#                         help='The type of programmer to use')
-#     parser.add_argument('--i2c-address', default=0x50, type=lambda x: int(x, base=0),
-#                         help='The I2C address of the target EEPROM')
-#     parser.add_argument('--i2c-clock-speed', type=int, default=100000, choices=[47000, 100000, 400000],
-#                         help='The I2C clock speed to use')
-#     parser.add_argument('--ee-size', default=4096, type=int,
-#                         help='The size (in bytes) of the EEPROM')
-#     parser.add_argument('--ee-page-size', default=32, type=int,
-#                         help='The EEPROM page size (in bytes)')
-#     parser.add_argument('--pad-value', default=0xFF, type=lambda x: int(x, base=0) & 0xFF,
-#                         help='The padding byte value (when loading a .hex file)')
-#     parser.add_argument('--load-file', type=Path, default=None,
-#                         help='If given, load the specified file (.hex or .bin) onto the device')
-#     parser.add_argument('--save-file', type=Path, default=None,
-#                         help='If given, read the entire contents of EEPROM and save to the specified file')
-#     parser.add_argument('--verify', action="store_true", default=False,
-#                         help='Verify the EEPROM contents after loading a .hex file')
+    parser.add_argument('--i2c-address', default=0x50, type=lambda x: int(x, base=0),
+                        help='The I2C address of the target EEPROM')
+    parser.add_argument('--i2c-clock-speed', type=int, default=100000, choices=[47000, 100000, 400000],
+                        help='The I2C clock speed to use')
+    parser.add_argument('--ee-size', default=4096, type=int,
+                        help='The size (in bytes) of the EEPROM')
+    parser.add_argument('--ee-page-size', default=32, type=int,
+                        help='The EEPROM page size (in bytes)')
+    parser.add_argument('--pad-value', default=0xFF, type=lambda x: int(x, base=0) & 0xFF,
+                        help='The padding byte value (when loading a .hex file)')
+    parser.add_argument('--load-file', type=Path, default=None,
+                        help='If given, load the specified file (.hex or .bin) onto the device and exit')
+    parser.add_argument('--save-file', type=Path, default=None,
+                        help='If given, read the entire contents of EEPROM, save to the specified file and exit')
+    parser.add_argument('--verify', action="store_true", default=True,
+                        help='Verify the EEPROM contents after loading a .hex file')
     parser.add_argument('--debug', action="store_true", default=False,
                         help='Log debug messages')
-#     parser.add_argument('--sim', type=Path, default=None,
-#                         help='If specified, use the given file to emulate an EEPROM instead of a physical one')
+    parser.add_argument('--sim', type=Path, default=None,
+                        help='If specified, use the given file to emulate an EEPROM instead of a physical one')
     args = parser.parse_args()
 
     return args
 
 
-# def __get_adapter(args):
-#     if args.sim:
-#         return None
-#     elif args.programmer == 'MCP2221':
-#         from adaptor.mcp2221 import MCP2221I2CAdaptor
-#         return MCP2221I2CAdaptor(args.i2c_address, i2c_clock_speed=args.i2c_clock_speed)
-
-#     raise ValueError(f"Unknown programmer {args.programmer}!")
-
-
-# def __get_eeprom(args, adaptor):
-#     if args.sim:
-#         from eeprom.eeprom import DummyEEPROM
-#         return DummyEEPROM(args.sim, args.ee_size)
-
-#     from eeprom.eeprom import I2CEEPROM
-#     return I2CEEPROM(adaptor, args.ee_size, page_size_in_bytes=args.ee_page_size)
-
-
-# def save_file(args):
-#     adaptor = __get_adapter(args)
-#     if adaptor is not None:
-#         adaptor.open()
-#     ee = __get_eeprom(args, adaptor)
-#     ee.save_file(args.save_file)
-#     print(f"EEPROM content saved to '{str(args.save_file)}'")
-#     return 0
-
-
-# def load_file(args):
-#     adaptor = __get_adapter(args)
-#     if adaptor is not None:
-#         adaptor.open()
-#     ee = __get_eeprom(args, adaptor)
-#     print(f"Loading{' (and verifying):' if args.verify else ':'} {str(args.load_file)}")
-#     ee.load_file(args.load_file, padding=args.pad_value, verify=args.verify)
-#     return 0
+def __get_adapter(args):
+    if args.sim:
+        return None
+
+    from adaptor.mcp2221 import MCP2221I2CAdaptor
+    return MCP2221I2CAdaptor(args.i2c_address, i2c_clock_speed=args.i2c_clock_speed)
+
+
+def __get_eeprom(args, adaptor):
+    if args.sim:
+        from eeprom.eeprom import DummyEEPROM
+        return DummyEEPROM(args.sim, args.ee_size)
+
+    from eeprom.eeprom import I2CEEPROM
+    return I2CEEPROM(adaptor, args.ee_size, page_size_in_bytes=args.ee_page_size)
+
+
+def save_file(args):
+    adaptor = __get_adapter(args)
+    if adaptor is not None:
+        adaptor.open()
+    ee = __get_eeprom(args, adaptor)
+    ee.save_file(args.save_file)
+    print(f"EEPROM content saved to '{str(args.save_file)}'")
+    return 0
+
+
+def load_file(args):
+    adaptor = __get_adapter(args)
+    if adaptor is not None:
+        adaptor.open()
+    ee = __get_eeprom(args, adaptor)
+    print(f"Loading{' (and verifying):' if args.verify else ':'} {str(args.load_file)}")
+    ee.load_file(args.load_file, padding=args.pad_value, verify=args.verify)
+    return 0
 
 def run():
     args = parse_command_line_arguments()
 
-    # if args.save_file is not None:
-    #     sys.exit(save_file(args))
+    if args.save_file is not None:
+        sys.exit(save_file(args))
 
-    # if args.load_file is not None:
-    #     sys.exit(load_file(args))
+    if args.load_file is not None:
+        sys.exit(load_file(args))
 
     from fv1_programmer.tui import FV1App
     app = FV1App(args)
     app.run()
 
 
 if __name__ == '__main__':
```

### Comparing `fv1_programmer-0.2.6/fv1_programmer/tui.css` & `fv1_programmer-0.2.7/fv1_programmer/tui.css`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.6/fv1_programmer/tui.py` & `fv1_programmer-0.2.7/fv1_programmer/tui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import logging
 import json
+import re
 
 from rich.console import RenderableType
 
 from textual import on
 from textual import work
 from textual.reactive import reactive
 from textual.app import App, ComposeResult
@@ -29,19 +30,19 @@
     Label,
     LoadingIndicator,
     Input,
 )
 
 from typing import Iterable
 from pathlib import Path
-from fv1_programmer.fv1 import EMPTY_FV1_PROGRAM_ASM, FV1Program, FV1FS
+from fv1_programmer.fv1 import FV1Program, FV1_PROGRAM_MAX_BYTES
 import pyperclip
 
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 _title = "FV1 Programmer"
 
 class BusyScreen(ModalScreen):
     def __init__(self, message : str) -> None:
         self.message = message
         super().__init__()
@@ -218,15 +219,14 @@
 
 
 
 class Sidebar(Container):
     def compose(self) -> ComposeResult:
         with VerticalScroll():
             yield Title("Settings")
-            yield OptionSwitch("setting_simulate", "Simulation Mode")
             yield OptionSwitch("setting_verify_writes", "Verify Writes")
             yield OptionSwitch("setting_asfv1_clamp", "Clamp Values (asfv1)")
             yield OptionSwitch("setting_asfv1_spinreals", "Spin Reals (asfv1)")
             yield OptionSwitch("setting_disfv1_relative", "Use Relative SKP Targets (disfv1)")
             yield OptionSwitch("setting_disfv1_suppressraw", "Convert Invalid Statements to NOP (disfv1)")
 
 
@@ -238,19 +238,19 @@
     def write(self, s):
         self.log(str(s).rstrip())
 
 
 class MainScreen(Screen):
     TITLE = _title
     BINDINGS = [
-        ("ctrl+l", "load_file", "Load File"),
-        # ("ctrl+r", "read_eeprom", "Read EEPROM"),
+        ("ctrl+l", "load_file", "Load"),
         ("ctrl+s", "save", "Save"),
-        ("ctrl+w", "write_eeprom", "Write EEPROM"),
-        ("f1", "app.toggle_class('TextLog', '-hidden')", "Show Log"),
+        ("ctrl+r", "read_eeprom", "Read"),
+        ("ctrl+w", "write_eeprom", "Write"),
+        ("f1", "app.toggle_class('TextLog', '-hidden')", "Log"),
         ("f2", "toggle_sidebar", "Settings"),
         ("ctrl+q", "request_quit", "Quit"),
         Binding("ctrl+v", "paste", "Paste", show=False, priority=True),
         Binding("ctrl+t", "paste", "Paste", show=False, priority=True),
         Binding("ctrl+d", "delete", "Delete Program", show=False, priority=True),
     ]
 
@@ -258,14 +258,20 @@
 
     class WriteEepromResult(Message):
         def __init__(self, programs : Iterable[dict], error=None) -> None:
             self.programs = programs
             self.error = error
             super().__init__()
 
+    class ReadEepromResult(Message):
+        def __init__(self, programs : Iterable[dict], error = None) -> None:
+            self.programs = programs
+            self.error = error
+            super().__init__()
+
     def compose(self) -> ComposeResult:
         with Container():
             yield Sidebar(classes="-hidden")
             yield Header(show_clock=True)
             yield TextLog(id="consolelog", classes="-hidden", wrap=False, highlight=True, markup=True)
             yield ProgramTabs()
             yield Footer()
@@ -307,17 +313,14 @@
                         program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
                         if programs[i - 1] is not None:
                             program_pane.program = FV1Program(programs[i - 1])
                 self.app.show_toast(f"Loaded programs from {path}")
 
         self.app.push_screen(LoadFileScreen(), handle_load_file)
 
-    def action_read_eeprom(self) -> None:
-        self.app.logger.info("Read EEPROM (Not Implemented)")
-
     def action_save(self) -> None:
         d = {"programs" : []}
 
         for i in range(1,9):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             d["programs"].append(program_pane.program.asm if program_pane.program is not None else None)
 
@@ -345,38 +348,42 @@
         programs = []
         for i in range(1,9):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             if program_pane.program is not None:
                 bin_array, warnings, errors = program_pane.program.assemble(
                                                             clamp=self.app.setting_asfv1_clamp,
                                                             spinreals=self.app.setting_asfv1_spinreals)
-                programs.append({"program": i, "address" : (i - 1)*512, "data" : bin_array})
+                programs.append({"program": i, "address" : (i - 1)*FV1_PROGRAM_MAX_BYTES, "data" : bin_array})
         if len(programs) == 0:
             self.app.show_toast("Nothing to do!", severity="warning")
         else:
             self.app.push_screen(BusyScreen("Downloading to pedal..."))
             self.write_eeprom(programs, self.app.setting_simulate)
 
-    @work(exclusive=True)
-    def write_eeprom(self, programs : Iterable[dict], simulate : bool) -> None:
-        worker = get_current_worker()
-        eeprom = None
+    def _get_eeprom(self,):
         if self.app.setting_simulate:
             from eeprom.eeprom import DummyEEPROM
-            eeprom = DummyEEPROM(Path('sim.bin'), 4096)
+            return DummyEEPROM(Path(self.app.cmdline_args.sim), self.app.cmdline_args.ee_size)
         else:
             from adaptor.mcp2221 import MCP2221I2CAdaptor
             from eeprom.eeprom import I2CEEPROM
-            try:
-                adaptor = MCP2221I2CAdaptor(0x50, i2c_clock_speed=100000)
-                adaptor.open()
-                eeprom = I2CEEPROM(adaptor, 4096, page_size_in_bytes=32)
-            except Exception as e:
-                if not worker.is_cancelled:
-                    self.post_message(self.WriteEepromResult(programs, error=e))
+            adaptor = MCP2221I2CAdaptor(self.app.cmdline_args.i2c_address,
+                                        i2c_clock_speed=self.app.cmdline_args.i2c_clock_speed)
+            adaptor.open()
+            return I2CEEPROM(adaptor, self.app.cmdline_args.ee_size,
+                             page_size_in_bytes=self.app.cmdline_args.ee_page_size)
+
+    @work(exclusive=True)
+    def write_eeprom(self, programs : Iterable[dict], simulate : bool) -> None:
+        worker = get_current_worker()
+        try:
+            eeprom = self._get_eeprom()
+        except Exception as e:
+            if not worker.is_cancelled:
+                self.post_message(self.WriteEepromResult(programs, error=e))
 
         if eeprom is not None:
             for program in programs:
                 addr = program["address"]
                 data = program["data"]
                 eeprom.write_bytes(addr, data)
 
@@ -391,25 +398,95 @@
                         error = ValueError("EEPROM write failed verification!")
                         break
 
             if not worker.is_cancelled:
                 self.post_message(self.WriteEepromResult(programs, error=error))
 
     def on_main_screen_write_eeprom_result(self, message : MainScreen.WriteEepromResult) -> None:
-        """Called write eeprom operation is finished."""
+        """Called when a write eeprom operation is finished."""
         self.app.pop_screen()
         if message.error is not None:
             self.app.logger.error(str(message.error))
             self.app.show_toast("EEPROM write failed! See log for details.", title="Error", severity="error")
         else:
             # total_bytes = sum([len(w["data"]) for w in message.programs])
             self.app.show_toast(f"Wrote to program slots {[w['program'] for w in message.programs]}{' (simulation)' if self.app.setting_simulate else ''}")
             if self.app.setting_verify_writes:
                 self.app.logger.info("All programs verified successfully.")
 
+    def action_read_eeprom(self) -> None:
+        def do_read_eeprom():
+            self.app.push_screen(BusyScreen("Reading from pedal..."))
+            self.read_eeprom(self.app.setting_simulate,
+                             self.app.setting_disfv1_relative,
+                             self.app.setting_disfv1_suppressraw)
+
+        num_programs = 0
+        for i in range(1,9):
+            program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
+            if program_pane.program is not None:
+                num_programs += 1
+
+        if num_programs > 0:
+            # Ask the user if they want to overwrite their current programs
+            def check_overwrite(should_overwrite : bool) -> None:
+                if should_overwrite:
+                    do_read_eeprom()
+            self.app.push_screen(YesNoScreen("This will overwrite your current programs.\nAre you sure?"), check_overwrite)
+
+        else:
+            do_read_eeprom()
+
+    @work(exclusive=True)
+    def read_eeprom(self, simulate : bool, relative : bool, suppressraw : bool) -> None:
+        worker = get_current_worker()
+        eeprom = None
+        try:
+            eeprom = self._get_eeprom()
+        except Exception as e:
+            if not worker.is_cancelled:
+                self.post_message(self.ReadEepromResult({}, error=e))
+
+        if eeprom is not None:
+            programs = []
+            program_data = eeprom.read_bytes(0, FV1_PROGRAM_MAX_BYTES*8)
+            for offset in range(0, 8*FV1_PROGRAM_MAX_BYTES, FV1_PROGRAM_MAX_BYTES):
+                program = FV1Program("")
+                warnings = program.from_bytearray(program_data[offset:offset + FV1_PROGRAM_MAX_BYTES],
+                                                  relative=relative, suppressraw=suppressraw)
+                programs.append({"program" : program, "warnings" : warnings})
+
+            if not worker.is_cancelled:
+                self.post_message(self.ReadEepromResult(programs))
+
+    def on_main_screen_read_eeprom_result(self, message : MainScreen.ReadEepromResult) -> None:
+        """Called when a read eeprom operation is finished."""
+        self.app.pop_screen()
+        if message.error is not None:
+            self.app.logger.error(str(message.error))
+            self.app.show_toast("EEPROM read failed! See log for details.", title="Error", severity="error")
+            return
+
+        were_warnings = False
+        for i in range(1,9):
+            program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
+            program_pane.program = message.programs[i - 1]["program"]
+            warnings = message.programs[i - 1]["warnings"]
+            if warnings is not None:
+                for warning in warnings:
+                    self.app.logger.info(warning)
+                    m = re.match("info: Read (\d+) instructions\.", warning)
+                    # Only worry about real warnings
+                    if m.group(0) != warning:
+                        were_warnings = True
+
+        if were_warnings:
+            self.app.show_toast("EEPROM read succeeded with warnings. See log for details.", title="Warning", severity="warning")
+        else:
+            self.app.show_toast("EEPROM read complete.")
 
     def action_paste(self) -> None:
         # Validate program
         new_program = FV1Program(pyperclip.paste())
         bin_array, warnings, errors = new_program.assemble(clamp=self.app.setting_asfv1_clamp,
                                                            spinreals=self.app.setting_asfv1_spinreals)
         [self.app.logger.info(w) for w in warnings]
@@ -425,52 +502,46 @@
         active_program_pane.program = None
 
 
 from dataclasses import dataclass
 @dataclass
 class Args:
     """Class emulating command line arguments to allow running via `textual run --dev`"""
-    programmer:str
     i2c_addr:int
     i2c_clock_speed:int
     ee_size:int
     ee_page_size:int
     pad_value:int
-    load_File:Path
-    save_File:Path
     verify:bool
     debug:bool
-    sim:bool
+    sim:Path
 
 
 class FV1App(App[None]):
     CSS_PATH = "tui.css"
     SCREENS = {"main" : MainScreen()}
 
     def __init__(self, cmdline_args=None, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.cmdline_args = cmdline_args
 
         # See if we're being run by `textual run --dev`
         if 'devtools' in self.features:
-            self.cmdline_args = Args('MCP2221',
-                                     0x50,
+            self.cmdline_args = Args(0x50,
                                      100000,
                                      4096,
                                      32,
                                      0xFF,
-                                     None,
-                                     None,
                                      True,
                                      False,
-                                     True)
+                                     Path('backup.bin'))
 
         # Whether to use a programmer or just simulate
-        self.setting_simulate = False
-        self.setting_verify_writes = True
+        self.setting_simulate = self.cmdline_args.sim is not None
+        self.setting_verify_writes = self.cmdline_args.verify
 
         # asfv1 options
         self.setting_asfv1_clamp = True
         self.setting_asfv1_spinreals = False
 
         # disfv1 options
         self.setting_disfv1_relative = False
@@ -482,16 +553,14 @@
         self.logger.setLevel(logging.DEBUG if self.cmdline_args.debug else logging.INFO)
         if self.cmdline_args.debug:
             fh = logging.FileHandler('app_debug.log', encoding='utf-8', mode='w')
             fh.setLevel(logging.DEBUG)
             fh.setFormatter(logging.Formatter('%(asctime)s [%(levelname)s] %(message)s'))
             self.logger.addHandler(fh)
 
-        self.EEPROM = None
-
     # Intercept the app exit (the only thing connected to this should be Ctrl+C)
     # and make it behave like Copy
     def exit(self, result = None) -> None:
         active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
         if active_program_pane.program is not None:
             pyperclip.copy(active_program_pane.program.asm)
             self.show_toast("Current program copied to clipboard")
```

### Comparing `fv1_programmer-0.2.6/pyproject.toml` & `fv1_programmer-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.2.6"
+version = "0.2.7"
 description = "An EEPROM programming tool for the FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `fv1_programmer-0.2.6/PKG-INFO` & `fv1_programmer-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fv1-programmer
-Version: 0.2.6
+Version: 0.2.7
 Summary: An EEPROM programming tool for the FV-1 DSP
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@audiofab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

