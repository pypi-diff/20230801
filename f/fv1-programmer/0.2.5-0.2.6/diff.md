# Comparing `tmp/fv1_programmer-0.2.5.tar.gz` & `tmp/fv1_programmer-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.2.5.tar", max compression
+gzip compressed data, was "fv1_programmer-0.2.6.tar", max compression
```

## Comparing `fv1_programmer-0.2.5.tar` & `fv1_programmer-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/LICENSE
--rw-r--r--   0        0        0      613 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/README.md
--rw-r--r--   0        0        0     1140 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/adaptor/mcp2221.py
--rw-r--r--   0        0        0       30 2023-07-19 02:10:47.524362 fv1_programmer-0.2.5/asfv1/.git
--rw-r--r--   0        0        0     1157 2023-07-19 02:10:48.756359 fv1_programmer-0.2.5/asfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-07-19 02:10:48.756359 fv1_programmer-0.2.5/asfv1/LICENSE
--rw-r--r--   0        0        0    36334 2023-07-19 02:10:48.756359 fv1_programmer-0.2.5/asfv1/README.md
--rw-r--r--   0        0        0    54482 2023-07-19 02:10:48.756359 fv1_programmer-0.2.5/asfv1/asfv1.py
--rw-r--r--   0        0        0      561 2023-07-19 02:10:48.756359 fv1_programmer-0.2.5/asfv1/example.asm
--rw-r--r--   0        0        0      801 2023-07-19 02:10:48.756359 fv1_programmer-0.2.5/asfv1/setup.py
--rw-r--r--   0        0        0       31 2023-07-19 02:10:47.924361 fv1_programmer-0.2.5/disfv1/.git
--rw-r--r--   0        0        0     1157 2023-07-19 02:10:48.764359 fv1_programmer-0.2.5/disfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-07-19 02:10:48.764359 fv1_programmer-0.2.5/disfv1/LICENSE
--rw-r--r--   0        0        0     4816 2023-07-19 02:10:48.764359 fv1_programmer-0.2.5/disfv1/README.md
--rw-r--r--   0        0        0    17532 2023-07-19 02:10:48.764359 fv1_programmer-0.2.5/disfv1/disfv1.py
--rw-r--r--   0        0        0      512 2023-07-19 02:10:48.764359 fv1_programmer-0.2.5/disfv1/example.bin
--rw-r--r--   0        0        0      798 2023-07-19 02:10:48.764359 fv1_programmer-0.2.5/disfv1/setup.py
--rw-r--r--   0        0        0     6747 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/eeprom/eeprom.py
--rw-r--r--   0        0        0     1780 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/fv1_programmer/fv1.py
--rw-r--r--   0        0        0     3429 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/fv1_programmer/main.py
--rw-r--r--   0        0        0     2992 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/fv1_programmer/tui.css
--rw-r--r--   0        0        0    15850 2023-07-19 02:10:46.992364 fv1_programmer-0.2.5/fv1_programmer/tui.py
--rw-r--r--   0        0        0     1267 2023-07-19 02:10:46.996364 fv1_programmer-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 fv1_programmer-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/LICENSE
+-rw-r--r--   0        0        0      613 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/README.md
+-rw-r--r--   0        0        0     1140 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2023-08-01 17:34:23.142765 fv1_programmer-0.2.6/asfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2023-08-01 17:34:24.882895 fv1_programmer-0.2.6/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2023-08-01 17:34:23.706807 fv1_programmer-0.2.6/disfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2023-08-01 17:34:24.890896 fv1_programmer-0.2.6/disfv1/setup.py
+-rw-r--r--   0        0        0     6747 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1780 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3429 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/main.py
+-rw-r--r--   0        0        0     3160 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    19020 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1267 2023-08-01 17:34:22.422711 fv1_programmer-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 fv1_programmer-0.2.6/PKG-INFO
```

### Comparing `fv1_programmer-0.2.5/LICENSE` & `fv1_programmer-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/README.md` & `fv1_programmer-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/adaptor/adapter.py` & `fv1_programmer-0.2.6/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/adaptor/mcp2221.py` & `fv1_programmer-0.2.6/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/asfv1/.gitignore` & `fv1_programmer-0.2.6/asfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/asfv1/LICENSE` & `fv1_programmer-0.2.6/asfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/asfv1/README.md` & `fv1_programmer-0.2.6/asfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/asfv1/asfv1.py` & `fv1_programmer-0.2.6/asfv1/asfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/asfv1/example.asm` & `fv1_programmer-0.2.6/asfv1/example.asm`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/asfv1/setup.py` & `fv1_programmer-0.2.6/asfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/disfv1/.gitignore` & `fv1_programmer-0.2.6/disfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/disfv1/LICENSE` & `fv1_programmer-0.2.6/disfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/disfv1/README.md` & `fv1_programmer-0.2.6/disfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/disfv1/disfv1.py` & `fv1_programmer-0.2.6/disfv1/disfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/disfv1/setup.py` & `fv1_programmer-0.2.6/disfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/eeprom/eeprom.py` & `fv1_programmer-0.2.6/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/fv1_programmer/fv1.py` & `fv1_programmer-0.2.6/fv1_programmer/fv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/fv1_programmer/main.py` & `fv1_programmer-0.2.6/fv1_programmer/main.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.5/fv1_programmer/tui.css` & `fv1_programmer-0.2.6/fv1_programmer/tui.css`

 * *Files 4% similar despite different names*

```diff
@@ -112,47 +112,58 @@
     offset-y: 100%;
 }
 
 ModalScreen {
     align: center middle;
 }
 
-#quitdialog {
+#yesnodialog {
     grid-size: 2;
     grid-gutter: 1 2;
     grid-rows: 1fr 3;
     padding: 0 1;
     width: 60;
     height: 11;
     border: thick $background 80%;
     background: $surface;
 }
 
-#question {
+#yesnomessage {
     column-span: 2;
     height: 1fr;
     width: 1fr;
     content-align: center middle;
 }
 
-#quitdialog > Button {
+#yesnodialog > Button {
     width: 100%;
 }
 
-#fileselectiondialog {
+#filedialog {
     grid-size: 2;
     grid-gutter: 1 2;
     grid-rows: 1fr 3;
     padding: 0 1;
     width: 90vw;
     height: 90vh;
     border: thick $background 80%;
     background: $surface;
 }
 
+#filesavedialog {
+    grid-size: 2;
+    grid-gutter: 1 2;
+    grid-rows: 1fr 3;
+    padding: 0 1;
+    width: 90vw;
+    height: 30vh;
+    border: thick $background 80%;
+    background: $surface;
+}
+
 #fileselectlabel {
     column-span: 2;
     content-align: left bottom;
     width: 100%;
     height: auto;
     dock: top;
 }
@@ -162,22 +173,22 @@
     content-align: center middle;
     width: 100%;
     height: 100%;
     margin-top: 1;
     margin-bottom: 1;
 }
 
-#fileselectiondialog > #cancel {
+#filedialogcancel {
     dock: bottom;
     width: 30;
     margin-left: 5;
     align: left top;
 }
 
-#fileselectiondialog > #select {
+#filedialogselect {
     dock: bottom;
     width: 30;
     margin-right: 5;
     align: right top;
 }
 
 #busyscreen {
```

### Comparing `fv1_programmer-0.2.5/fv1_programmer/tui.py` & `fv1_programmer-0.2.6/fv1_programmer/tui.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rich.console import RenderableType
 
 from textual import on
 from textual import work
 from textual.reactive import reactive
 from textual.app import App, ComposeResult
 from textual.binding import Binding
-from textual.containers import Container, Grid, Horizontal, Vertical
+from textual.containers import Container, Grid, Horizontal, Vertical, VerticalScroll
 from textual.screen import Screen, ModalScreen
 from textual.worker import Worker, get_current_worker
 from textual.message import Message
 from textual.widget import Widget
 from textual.widgets import (
     Footer,
     Header,
@@ -21,78 +21,113 @@
     TextLog,
     Button,
     TabbedContent,
     TabPane,
     Switch,
     Markdown,
     DirectoryTree,
+    Tree,
     Label,
     LoadingIndicator,
+    Input,
 )
 
 from typing import Iterable
 from pathlib import Path
 from fv1_programmer.fv1 import EMPTY_FV1_PROGRAM_ASM, FV1Program, FV1FS
 import pyperclip
 
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 _title = "FV1 Programmer"
 
 class BusyScreen(ModalScreen):
     def __init__(self, message : str) -> None:
         self.message = message
-        super().__init__(id)
+        super().__init__()
 
     def compose(self) -> ComposeResult:
         yield Grid(
             Label(self.message),
             LoadingIndicator(),
             id="busyscreen"
         )
 
 
 class FilteredDirectoryTree(DirectoryTree):
+    def __init__(self, *args, **kwargs):
+        self.valid_suffixes = []
+        try:
+            self.valid_suffixes = kwargs.pop("valid_suffixes")
+        except KeyError:
+            pass
+        super().__init__(*args, **kwargs)
+
     def filter_paths(self, paths: Iterable[Path]) -> Iterable[Path]:
         return [path for path in paths if not path.name.startswith(".") and \
                     # TODO: Support SpinCAD file types as well!
-                    path.is_dir() or (path.is_file() and path.suffix.lower() in ['.json'])]
+                    path.is_dir() or (path.is_file() and path.suffix.lower() in self.valid_suffixes)]
 
 
-class FileSelectionScreen(ModalScreen[Path]):
+class LoadFileScreen(ModalScreen[Path]):
     selection : reactive[Path | None] = reactive(None)
 
     def compose(self) -> ComposeResult:
-        # TODO: Support setting the root folder and drive
         yield Grid(
             Static("Choose a file:", id="fileselectlabel"),
-            FilteredDirectoryTree("./", id="filetree"),
-            Button("Cancel", variant="primary", id="cancel"),
-            Button("Select", variant="primary", id="select"),
-            id="fileselectiondialog",
+            FilteredDirectoryTree("./", id="filetree", valid_suffixes=[".json"]),
+            Button("Cancel", variant="error", id="filedialogcancel"),
+            Button("Select", variant="primary", id="filedialogselect"),
+            id="filedialog",
         )
 
     @on(DirectoryTree.FileSelected, "#filetree")
     def do_file_selected(self, event : DirectoryTree.FileSelected):
         self.selection = event.path
 
     def watch_selection(self, new_path: Path):
         self.selection = new_path
         enabled = self.selection is not None
-        select_button = self.query_one("#select", Button)
+        select_button = self.query_one("#filedialogselect", Button)
         select_button.disabled = not enabled
         if enabled:
             select_button.focus()
 
-    @on(Button.Pressed, "#select")
+    @on(Button.Pressed, "#filedialogselect")
     def do_select(self):
         self.dismiss(self.selection)
 
-    @on(Button.Pressed, "#cancel")
+    @on(Button.Pressed, "#filedialogcancel")
+    def cancel(self):
+        self.dismiss(None)
+
+
+class SaveFileScreen(ModalScreen[Path]):
+    filename : reactive("")
+
+    def compose(self) -> ComposeResult:
+        yield Grid(
+            Static("Please specify a filename:", id="fileselectlabel"),
+            Input("my_programs", id="filesavefilename"),
+            Button("Cancel", variant="error", id="filedialogcancel"),
+            Button("Save", variant="primary", id="filedialogselect"),
+            id="filesavedialog",
+        )
+
+    @on(Input.Changed)
+    def check_filename(self, event: Input.Changed) -> None:
+        self.query_one("#filedialogselect", Button).disabled = \
+                    len(self.query_one("#filesavefilename", Input).value) < 1
+
+    @on(Button.Pressed, "#filedialogselect")
+    def do_save(self):
+        self.dismiss(self.query_one("#filesavefilename", Input).value)
+
+    @on(Button.Pressed, "#filedialogcancel")
     def cancel(self):
         self.dismiss(None)
 
 
 class FV1ProgramPane(Widget):
     program : reactive[FV1Program | None] = reactive(None)
 
@@ -126,29 +161,39 @@
                 yield FV1ProgramPane(id="fv1prog6")
             with TabPane("Program 7", id="prog7"):
                 yield FV1ProgramPane(id="fv1prog7")
             with TabPane("Program 8", id="prog8"):
                 yield FV1ProgramPane(id="fv1prog8")
 
 
-class QuitScreen(ModalScreen[bool]):
+class YesNoScreen(ModalScreen[bool]):
+    def __init__(self, message, no_text="No", yes_text="Yes",
+                 no_variant="primary", yes_variant="primary",
+                 *args, **kwargs):
+        self.message = message
+        self.no_text = no_text
+        self.yes_text = yes_text
+        self.no_variant = no_variant
+        self.yes_variant = yes_variant
+        super().__init__(*args, **kwargs)
+
     def compose(self) -> ComposeResult:
         yield Grid(
-            Static("Are you sure you want to quit?", id="question"),
-            Button("Cancel", variant="primary", id="cancel"),
-            Button("Quit", variant="error", id="quit"),
-            id="quitdialog",
+            Static(self.message, id="yesnomessage"),
+            Button(self.no_text, variant=self.no_variant, id="yesnono"),
+            Button(self.yes_text, variant=self.yes_variant, id="yesnoyes"),
+            id="yesnodialog",
         )
 
-    @on(Button.Pressed, "#quit")
-    def quit(self):
+    @on(Button.Pressed, "#yesnoyes")
+    def yes(self):
         self.dismiss(True)
 
-    @on(Button.Pressed, "#cancel")
-    def cancel(self):
+    @on(Button.Pressed, "#yesnono")
+    def no(self):
         self.dismiss(False)
 
 
 class Title(Static):
     pass
 
 
@@ -171,17 +216,18 @@
     def on_switch_changed(self, event: Switch.Changed) -> None:
         setattr(self.app, self.option_name, event.value)
 
 
 
 class Sidebar(Container):
     def compose(self) -> ComposeResult:
-        with Vertical():
+        with VerticalScroll():
             yield Title("Settings")
             yield OptionSwitch("setting_simulate", "Simulation Mode")
+            yield OptionSwitch("setting_verify_writes", "Verify Writes")
             yield OptionSwitch("setting_asfv1_clamp", "Clamp Values (asfv1)")
             yield OptionSwitch("setting_asfv1_spinreals", "Spin Reals (asfv1)")
             yield OptionSwitch("setting_disfv1_relative", "Use Relative SKP Targets (disfv1)")
             yield OptionSwitch("setting_disfv1_suppressraw", "Convert Invalid Statements to NOP (disfv1)")
 
 
 class ConsoleLogStream:
@@ -244,45 +290,60 @@
         self.app.logger.info(f"FV1 Programmer version {__version__}")
 
     def action_request_quit(self,) -> None:
         def check_quit(should_quit : bool) -> None:
             if should_quit:
                 self.app.do_exit()
 
-        self.app.push_screen(QuitScreen(), check_quit)
+        self.app.push_screen(YesNoScreen("Are you sure you want to quit?",
+                                         yes_variant="error"), check_quit)
 
     def action_load_file(self) -> None:
         def handle_load_file(path : Path) -> None:
-            if path.exists() and path.is_file():
+            if path is not None and path.exists() and path.is_file():
                 with open(str(path), 'r') as f:
                     d = json.load(f)
                     programs = d.get("programs", [None]*8)
                     for i in range(1,9):
                         program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
                         if programs[i - 1] is not None:
                             program_pane.program = FV1Program(programs[i - 1])
-            self.app.show_toast(f"Loaded programs from {path}")
+                self.app.show_toast(f"Loaded programs from {path}")
 
-        self.app.push_screen(FileSelectionScreen(), handle_load_file)
+        self.app.push_screen(LoadFileScreen(), handle_load_file)
 
     def action_read_eeprom(self) -> None:
         self.app.logger.info("Read EEPROM (Not Implemented)")
 
     def action_save(self) -> None:
         d = {"programs" : []}
 
         for i in range(1,9):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             d["programs"].append(program_pane.program.asm if program_pane.program is not None else None)
 
-        fname = 'fv1_programs.json'
-        with open(fname, 'w') as f:
-            json.dump(d, f, indent=2)
-            self.app.show_toast(f"Programs saved to {fname}")
+        def handle_save_file(filename : str) -> None:
+            def do_save_file(file_path):
+                with open(file_path, 'w') as f:
+                    json.dump(d, f, indent=2)
+                    self.app.show_toast(f"Programs saved to {file_path}")
+
+            if filename is not None:
+                # Does filename already exist?
+                save_path = Path(Path(".") / filename if filename.endswith(".json") else f"{filename}.json")
+                if save_path.exists() and save_path.is_file():
+                    def check_overwrite(should_overwrite : bool) -> None:
+                        if should_overwrite:
+                            do_save_file(save_path)
+                    self.app.push_screen(YesNoScreen("File exists. Overwrite?"), check_overwrite)
+
+                else:
+                    do_save_file(save_path)
 
+        self.app.push_screen(SaveFileScreen(), handle_save_file)
 
     def action_write_eeprom(self) -> None:
         programs = []
         for i in range(1,9):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             if program_pane.program is not None:
                 bin_array, warnings, errors = program_pane.program.assemble(
@@ -315,26 +376,40 @@
 
         if eeprom is not None:
             for program in programs:
                 addr = program["address"]
                 data = program["data"]
                 eeprom.write_bytes(addr, data)
 
+            error = None
+            # Read back all the data and verify
+            if self.app.setting_verify_writes:
+                for program in programs:
+                    addr = program["address"]
+                    data = program["data"]
+                    read_data = eeprom.read_bytes(addr, len(data))
+                    if read_data != data:
+                        error = ValueError("EEPROM write failed verification!")
+                        break
+
             if not worker.is_cancelled:
-                self.post_message(self.WriteEepromResult(programs))
+                self.post_message(self.WriteEepromResult(programs, error=error))
 
     def on_main_screen_write_eeprom_result(self, message : MainScreen.WriteEepromResult) -> None:
-        """Called when the worker state changes."""
+        """Called write eeprom operation is finished."""
         self.app.pop_screen()
         if message.error is not None:
             self.app.logger.error(str(message.error))
-            self.app.show_toast("Failed to find Easy Spin! See log for details.", title="Error", severity="error")
+            self.app.show_toast("EEPROM write failed! See log for details.", title="Error", severity="error")
         else:
             # total_bytes = sum([len(w["data"]) for w in message.programs])
             self.app.show_toast(f"Wrote to program slots {[w['program'] for w in message.programs]}{' (simulation)' if self.app.setting_simulate else ''}")
+            if self.app.setting_verify_writes:
+                self.app.logger.info("All programs verified successfully.")
+
 
     def action_paste(self) -> None:
         # Validate program
         new_program = FV1Program(pyperclip.paste())
         bin_array, warnings, errors = new_program.assemble(clamp=self.app.setting_asfv1_clamp,
                                                            spinreals=self.app.setting_asfv1_spinreals)
         [self.app.logger.info(w) for w in warnings]
@@ -387,14 +462,15 @@
                                      None,
                                      True,
                                      False,
                                      True)
 
         # Whether to use a programmer or just simulate
         self.setting_simulate = False
+        self.setting_verify_writes = True
 
         # asfv1 options
         self.setting_asfv1_clamp = True
         self.setting_asfv1_spinreals = False
 
         # disfv1 options
         self.setting_disfv1_relative = False
```

### Comparing `fv1_programmer-0.2.5/pyproject.toml` & `fv1_programmer-0.2.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.2.5"
+version = "0.2.6"
 description = "An EEPROM programming tool for the FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `fv1_programmer-0.2.5/PKG-INFO` & `fv1_programmer-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fv1-programmer
-Version: 0.2.5
+Version: 0.2.6
 Summary: An EEPROM programming tool for the FV-1 DSP
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@audiofab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

