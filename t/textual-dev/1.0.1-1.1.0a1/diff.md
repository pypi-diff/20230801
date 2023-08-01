# Comparing `tmp/textual_dev-1.0.1.tar.gz` & `tmp/textual_dev-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_dev-1.0.1.tar", max compression
+gzip compressed data, was "textual_dev-1.1.0a1.tar", max compression
```

## Comparing `textual_dev-1.0.1.tar` & `textual_dev-1.1.0a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-10-25 13:47:18.602610 textual_dev-1.0.1/LICENSE
--rw-r--r--   0        0        0      240 2023-07-03 15:24:39.076207 textual_dev-1.0.1/README.md
--rw-r--r--   0        0        0     1680 2023-07-03 15:25:02.977974 textual_dev-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-27 12:09:27.878115 textual_dev-1.0.1/src/textual_dev/__init__.py
--rw-r--r--   0        0        0       59 2023-06-27 12:09:27.878216 textual_dev-1.0.1/src/textual_dev/__main__.py
--rw-r--r--   0        0        0     6124 2023-06-27 12:09:27.878759 textual_dev-1.0.1/src/textual_dev/cli.py
--rw-r--r--   0        0        0     9776 2023-06-27 12:09:27.878909 textual_dev-1.0.1/src/textual_dev/client.py
--rw-r--r--   0        0        0      246 2023-06-27 12:09:27.879032 textual_dev-1.0.1/src/textual_dev/previews/__init__.py
--rw-r--r--   0        0        0     1736 2023-06-27 12:09:27.879537 textual_dev-1.0.1/src/textual_dev/previews/borders.py
--rw-r--r--   0        0        0     5903 2023-06-27 12:09:27.879653 textual_dev-1.0.1/src/textual_dev/previews/colors.css
--rw-r--r--   0        0        0     2118 2023-06-27 12:09:27.879770 textual_dev-1.0.1/src/textual_dev/previews/colors.py
--rw-r--r--   0        0        0      748 2023-06-27 12:09:27.879871 textual_dev-1.0.1/src/textual_dev/previews/easing.css
--rw-r--r--   0        0        0     3691 2023-06-27 12:09:27.879984 textual_dev-1.0.1/src/textual_dev/previews/easing.py
--rw-r--r--   0        0        0     1861 2023-06-27 12:09:27.880054 textual_dev-1.0.1/src/textual_dev/previews/keys.py
--rw-r--r--   0        0        0        0 2023-06-27 12:09:27.880084 textual_dev-1.0.1/src/textual_dev/py.typed
--rw-r--r--   0        0        0     4278 2023-06-27 12:09:27.880682 textual_dev-1.0.1/src/textual_dev/redirect_output.py
--rw-r--r--   0        0        0     4237 2023-06-27 12:09:27.881448 textual_dev-1.0.1/src/textual_dev/renderables.py
--rw-r--r--   0        0        0     2278 2023-06-27 12:09:27.881594 textual_dev-1.0.1/src/textual_dev/server.py
--rw-r--r--   0        0        0    11060 2023-06-27 12:09:27.881773 textual_dev-1.0.1/src/textual_dev/service.py
--rw-r--r--   0        0        0     4514 2023-06-27 12:09:27.881905 textual_dev-1.0.1/src/textual_dev/tools/diagnose.py
--rw-r--r--   0        0        0     3901 2023-06-27 12:09:27.881987 textual_dev-1.0.1/src/textual_dev/tools/run.py
--rw-r--r--   0        0        0      627 2023-06-27 12:09:27.882134 textual_dev-1.0.1/tests/devtools/__init__.py
--rw-r--r--   0        0        0      791 2023-06-27 12:09:27.882199 textual_dev-1.0.1/tests/devtools/conftest.py
--rw-r--r--   0        0        0     2889 2023-06-27 12:09:27.882271 textual_dev-1.0.1/tests/devtools/test_devtools.py
--rw-r--r--   0        0        0     3774 2023-06-27 12:09:27.882343 textual_dev-1.0.1/tests/devtools/test_devtools_client.py
--rw-r--r--   0        0        0     3726 2023-06-27 12:09:27.882415 textual_dev-1.0.1/tests/devtools/test_redirect_output.py
--rw-r--r--   0        0        0      253 2023-06-27 12:09:27.882473 textual_dev-1.0.1/tests/test_cli.py
--rw-r--r--   0        0        0       46 2023-06-27 12:09:27.882573 textual_dev-1.0.1/tests/utilities/__init__.py
--rw-r--r--   0        0        0     1121 2023-06-27 12:09:27.882648 textual_dev-1.0.1/tests/utilities/wait_for_predicate.py
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 textual_dev-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-10-25 13:47:18.602610 textual_dev-1.1.0a1/LICENSE
+-rw-r--r--   0        0        0      352 2023-08-01 15:24:52.501454 textual_dev-1.1.0a1/README.md
+-rw-r--r--   0        0        0     1721 2023-08-01 15:27:36.609518 textual_dev-1.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-27 12:09:27.878115 textual_dev-1.1.0a1/src/textual_dev/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-27 12:09:27.878216 textual_dev-1.1.0a1/src/textual_dev/__main__.py
+-rw-r--r--   0        0        0     6124 2023-06-27 12:09:27.878759 textual_dev-1.1.0a1/src/textual_dev/cli.py
+-rw-r--r--   0        0        0     9776 2023-06-27 12:09:27.878909 textual_dev-1.1.0a1/src/textual_dev/client.py
+-rw-r--r--   0        0        0      246 2023-06-27 12:09:27.879032 textual_dev-1.1.0a1/src/textual_dev/previews/__init__.py
+-rw-r--r--   0        0        0     1815 2023-08-01 15:24:52.502754 textual_dev-1.1.0a1/src/textual_dev/previews/borders.py
+-rw-r--r--   0        0        0     5961 2023-08-01 15:24:52.503029 textual_dev-1.1.0a1/src/textual_dev/previews/colors.css
+-rw-r--r--   0        0        0     2937 2023-08-01 15:24:52.503208 textual_dev-1.1.0a1/src/textual_dev/previews/colors.py
+-rw-r--r--   0        0        0      748 2023-06-27 12:09:27.879871 textual_dev-1.1.0a1/src/textual_dev/previews/easing.css
+-rw-r--r--   0        0        0     3691 2023-06-27 12:09:27.879984 textual_dev-1.1.0a1/src/textual_dev/previews/easing.py
+-rw-r--r--   0        0        0     1861 2023-08-01 15:27:36.609856 textual_dev-1.1.0a1/src/textual_dev/previews/keys.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:09:27.880084 textual_dev-1.1.0a1/src/textual_dev/py.typed
+-rw-r--r--   0        0        0     4278 2023-06-27 12:09:27.880682 textual_dev-1.1.0a1/src/textual_dev/redirect_output.py
+-rw-r--r--   0        0        0     4237 2023-06-27 12:09:27.881448 textual_dev-1.1.0a1/src/textual_dev/renderables.py
+-rw-r--r--   0        0        0     2278 2023-06-27 12:09:27.881594 textual_dev-1.1.0a1/src/textual_dev/server.py
+-rw-r--r--   0        0        0    11068 2023-08-01 15:24:52.503410 textual_dev-1.1.0a1/src/textual_dev/service.py
+-rw-r--r--   0        0        0     4514 2023-06-27 12:09:27.881905 textual_dev-1.1.0a1/src/textual_dev/tools/diagnose.py
+-rw-r--r--   0        0        0     3901 2023-06-27 12:09:27.881987 textual_dev-1.1.0a1/src/textual_dev/tools/run.py
+-rw-r--r--   0        0        0      627 2023-06-27 12:09:27.882134 textual_dev-1.1.0a1/tests/devtools/__init__.py
+-rw-r--r--   0        0        0      776 2023-08-01 15:24:52.503597 textual_dev-1.1.0a1/tests/devtools/conftest.py
+-rw-r--r--   0        0        0     2884 2023-08-01 15:24:52.503778 textual_dev-1.1.0a1/tests/devtools/test_devtools.py
+-rw-r--r--   0        0        0     3723 2023-08-01 15:24:52.503936 textual_dev-1.1.0a1/tests/devtools/test_devtools_client.py
+-rw-r--r--   0        0        0     3721 2023-08-01 15:24:52.504254 textual_dev-1.1.0a1/tests/devtools/test_redirect_output.py
+-rw-r--r--   0        0        0      253 2023-08-01 15:24:52.504413 textual_dev-1.1.0a1/tests/test_cli.py
+-rw-r--r--   0        0        0       46 2023-06-27 12:09:27.882573 textual_dev-1.1.0a1/tests/utilities/__init__.py
+-rw-r--r--   0        0        0     1123 2023-08-01 15:24:52.504707 textual_dev-1.1.0a1/tests/utilities/wait_for_predicate.py
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 textual_dev-1.1.0a1/PKG-INFO
```

### Comparing `textual_dev-1.0.1/LICENSE` & `textual_dev-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/pyproject.toml` & `textual_dev-1.1.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-dev"
-version = "1.0.1"
+version = "1.1.0a1"
 homepage = "https://github.com/Textualize/textual-dev"
 description = "Development tools for working with Textual"
 authors = ["Will McGugan <will@textualize.io>", "Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
 include = [
     "src/textual_dev/py.typed",
     { path = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-textual = ">=0.29.0"
+textual = ">=0.32.0"
 aiohttp = ">=3.8.1"
 click = ">=8.1.2"
 msgpack = ">=1.0.3"
 typing-extensions = "^4.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
@@ -55,7 +55,10 @@
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = ["tests"]
 addopts = "--strict-markers"
 markers = [
     "integration_test: marks tests as slow integration tests (deselect with '-m \"not integration_test\"')",
 ]
+
+[tool.mypy]
+implicit_reexport = false
```

### Comparing `textual_dev-1.0.1/src/textual_dev/cli.py` & `textual_dev-1.1.0a1/src/textual_dev/cli.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/client.py` & `textual_dev-1.1.0a1/src/textual_dev/client.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/previews/borders.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/borders.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from typing import cast
 from textual.app import App, ComposeResult
 from textual.containers import Vertical
 from textual.css.constants import VALID_BORDER
+from textual.css.types import EdgeType
 from textual.widgets import Button, Label
 
 TEXT = """I must not fear.
 Fear is the mind-killer.
 Fear is the little-death that brings total obliteration.
 I will face my fear.
 I will permit it to pass over me and through me.
@@ -56,14 +58,14 @@
         self.text.shrink = True
         self.text.border_title = "solid"
         yield self.text
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         self.text.border_title = event.button.id
         self.text.styles.border = (
-            event.button.id,
+            cast(EdgeType, event.button.id),
             self.stylesheet._variables["secondary"],
         )
 
 
 if __name__ == "__main__":
     BorderApp().run()
```

### Comparing `textual_dev-1.0.1/src/textual_dev/previews/colors.css` & `textual_dev-1.1.0a1/src/textual_dev/previews/colors.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Label {
     width: 100%;
 }
 
-ColorButtons {
+ThemeColorButtons {
     dock: left;
     overflow-y: auto;
     width: 30;
 }
 
-ColorButtons > Button {
+ThemeColorButtons > Button {
     width: 100%;
 }
 
 ColorsView {
     width: 100%;
     height: 100%;
     align: center middle;
@@ -57,14 +57,18 @@
     border: wide $secondary;
 }
 
 .text {
     color: $text;
 }
 
+.text-left {
+    content-align: left middle;
+}
+
 .muted {
     color: $text-muted;
 }
 
 
 .disabled {
     color: $text-disabled;
```

### Comparing `textual_dev-1.0.1/src/textual_dev/previews/colors.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/colors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from textual._color_constants import COLOR_NAME_TO_RGB
 from textual.app import App, ComposeResult
+from textual.color import Color
 from textual.containers import Horizontal, Vertical, VerticalScroll
 from textual.design import ColorSystem
-from textual.widgets import Button, Footer, Label, Static
+from textual.widgets import Button, Footer, Label, Static, TabbedContent
 
 
-class ColorButtons(VerticalScroll):
+class ThemeColorButtons(VerticalScroll):
     def compose(self) -> ComposeResult:
-        for border in ColorSystem.COLOR_NAMES:
-            if border:
-                yield Button(border, id=border)
+        for color_name in ColorSystem.COLOR_NAMES:
+            yield Button(color_name, id=color_name)
 
 
 class ColorBar(Static):
     pass
 
 
 class ColorItem(Horizontal):
@@ -24,14 +25,34 @@
 
 
 class Content(Vertical):
     pass
 
 
 class ColorsView(VerticalScroll):
+    pass
+
+
+class ColorTabs(TabbedContent, inherit_css=False):
+    pass
+
+
+class NamedColorsView(ColorsView):
+    def compose(self) -> ComposeResult:
+        with ColorGroup(id=f"group-named"):
+            for name, rgb in COLOR_NAME_TO_RGB.items():
+                color = Color(*rgb)
+                with ColorItem() as ci:
+                    ci.styles.background = name
+                    yield ColorBar(name, classes="text")
+                    yield ColorBar(f"{color.hex6}", classes="text")
+                    yield ColorBar(f"{color.rgb}", classes="text text-left")
+
+
+class ThemeColorsView(ColorsView):
     def compose(self) -> ComposeResult:
         LEVELS = [
             "darken-3",
             "darken-2",
             "darken-1",
             "",
             "lighten-1",
@@ -52,23 +73,25 @@
 
 class ColorsApp(App[None]):
     CSS_PATH = "colors.css"
 
     BINDINGS = [("d", "toggle_dark", "Toggle dark mode")]
 
     def compose(self) -> ComposeResult:
-        yield Content(ColorButtons())
         yield Footer()
+        with ColorTabs("Theme Colors", "Named Colors"):
+            yield Content(ThemeColorButtons())
+            yield Vertical(NamedColorsView())
 
     def on_mount(self) -> None:
         self.call_after_refresh(self.update_view)
 
     def update_view(self) -> None:
         content = self.query_one("Content", Content)
-        content.mount(ColorsView())
+        content.mount(ThemeColorsView())
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         self.query(ColorGroup).remove_class("-active")
         group = self.query_one(f"#group-{event.button.id}", ColorGroup)
         group.add_class("-active")
         group.scroll_visible(top=True, speed=150)
```

### Comparing `textual_dev-1.0.1/src/textual_dev/previews/easing.css` & `textual_dev-1.1.0a1/src/textual_dev/previews/easing.css`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/previews/easing.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/easing.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/previews/keys.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/keys.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 from rich.panel import Panel
 from rich.text import Text
 from textual import events
 from textual.app import App, ComposeResult
 from textual.containers import Horizontal
 from textual.reactive import var
-from textual.widgets import Button, Header, TextLog
+from textual.widgets import Button, Header, RichLog
 
 INSTRUCTIONS = """\
 [u]Press some keys![/]
 
 To quit the app press [b]ctrl+c[/b] [i]twice[/i] or press the Quit button below.\
 """
 
 
-class KeyLog(TextLog, inherit_bindings=False):
+class KeyLog(RichLog, inherit_bindings=False):
     """We don't want to handle scroll keys."""
 
 
 class KeysApp(App[None], inherit_bindings=False):
     """Show key events in a text log."""
 
     TITLE = "Textual Keys"
```

### Comparing `textual_dev-1.0.1/src/textual_dev/redirect_output.py` & `textual_dev-1.1.0a1/src/textual_dev/redirect_output.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/renderables.py` & `textual_dev-1.1.0a1/src/textual_dev/renderables.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/server.py` & `textual_dev-1.1.0a1/src/textual_dev/server.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/service.py` & `textual_dev-1.1.0a1/src/textual_dev/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 import pickle
 from json import JSONDecodeError
 from typing import Any
 
 import msgpack
 from aiohttp import WSMsgType
-from aiohttp.abc import Request
+from aiohttp.web_request import Request
 from aiohttp.web_ws import WebSocketResponse
 from rich.console import Console
 from rich.markup import escape
 from textual._log import LogGroup
 from textual._time import time
 
 from textual_dev.renderables import DevConsoleHeader, DevConsoleLog, DevConsoleNotice
```

### Comparing `textual_dev-1.0.1/src/textual_dev/tools/diagnose.py` & `textual_dev-1.1.0a1/src/textual_dev/tools/diagnose.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/src/textual_dev/tools/run.py` & `textual_dev-1.1.0a1/src/textual_dev/tools/run.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/tests/devtools/__init__.py` & `textual_dev-1.1.0a1/tests/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.0.1/tests/devtools/conftest.py` & `textual_dev-1.1.0a1/tests/devtools/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
-from textual.devtools.client import DevtoolsClient
-from textual.devtools.server import _make_devtools_aiohttp_app
-from textual.devtools.service import DevtoolsService
+from textual_dev.client import DevtoolsClient
+from textual_dev.server import _make_devtools_aiohttp_app
+from textual_dev.service import DevtoolsService
 
 
 @pytest.fixture
 async def server(aiohttp_server, unused_tcp_port):
     app = _make_devtools_aiohttp_app(
         size_change_poll_delay_secs=0.001,
     )
```

### Comparing `textual_dev-1.0.1/tests/devtools/test_devtools.py` & `textual_dev-1.1.0a1/tests/devtools/test_devtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import msgpack
 import pytest
 import time_machine
 from rich.align import Align
 from rich.console import Console
 from rich.segment import Segment
 
-from textual.devtools.renderables import DevConsoleLog, DevConsoleNotice
+from textual_dev.renderables import DevConsoleLog, DevConsoleNotice
 
 from utilities.wait_for_predicate import wait_for_predicate
 
 TIMESTAMP = 1649166819
 WIDTH = 40
 # The string "Hello, world!" is encoded in the payload below
 _EXAMPLE_LOG = {
```

### Comparing `textual_dev-1.0.1/tests/devtools/test_devtools_client.py` & `textual_dev-1.1.0a1/tests/devtools/test_devtools_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 from datetime import datetime
 
 import msgpack
 import time_machine
 from aiohttp.web_ws import WebSocketResponse
 from rich.console import ConsoleDimensions
 from rich.panel import Panel
-
 from textual.constants import DEVTOOLS_PORT
-from textual.devtools.client import DevtoolsClient
-from textual.devtools.redirect_output import DevtoolsLog
-
+from textual_dev.client import DevtoolsClient, DevtoolsLog
 from utilities.wait_for_predicate import wait_for_predicate
 
 CALLER_LINENO = 123
 CALLER_PATH = "a/b/c.py"
 CALLER = types.SimpleNamespace(filename=CALLER_PATH, lineno=CALLER_LINENO)
 TIMESTAMP = 1649166819
```

### Comparing `textual_dev-1.0.1/tests/devtools/test_redirect_output.py` & `textual_dev-1.1.0a1/tests/devtools/test_redirect_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from contextlib import redirect_stdout
 from datetime import datetime
 
 import msgpack
 import time_machine
 
-from textual.devtools.redirect_output import StdoutRedirector
+from textual_dev.redirect_output import StdoutRedirector
 
 TIMESTAMP = 1649166819
 
 
 @time_machine.travel(datetime.utcfromtimestamp(TIMESTAMP))
 async def test_print_redirect_to_devtools_only(devtools):
     await devtools._stop_log_queue_processing()
```

### Comparing `textual_dev-1.0.1/tests/utilities/wait_for_predicate.py` & `textual_dev-1.1.0a1/tests/utilities/wait_for_predicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Args:
         predicate (Callable[[], bool]): The predicate function which will be called repeatedly.
         timeout_secs (float): If the predicate doesn't evaluate to True after this number of
             seconds, the test will fail.
         poll_delay_secs (float): The number of seconds to wait between each call to the
             predicate function.
     """
-    time_taken = 0
+    time_taken = 0.0
     while True:
         result = predicate()
         if result:
             return
         await asyncio.sleep(poll_delay_secs)
         time_taken += poll_delay_secs
         if time_taken > timeout_secs:
```

### Comparing `textual_dev-1.0.1/PKG-INFO` & `textual_dev-1.1.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-dev
-Version: 1.0.1
+Version: 1.1.0a1
 Summary: Development tools for working with Textual
 Home-page: https://github.com/Textualize/textual-dev
 License: MIT
 Author: Will McGugan
 Author-email: will@textualize.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -26,19 +26,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3.8.1)
 Requires-Dist: click (>=8.1.2)
 Requires-Dist: msgpack (>=1.0.3)
-Requires-Dist: textual (>=0.29.0)
+Requires-Dist: textual (>=0.32.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # textual-dev
 
 Development tools for Textual.
 
+![checks](https://github.com/Textualize/textual-dev/actions/workflows/pythonpackage.yml/badge.svg?event=push)
+
+
 This package contains the `textual` command line app, which will help to develop Textual applications.
 
 See [Getting Started](https://textual.textualize.io/getting_started/) for how to use it.
```

