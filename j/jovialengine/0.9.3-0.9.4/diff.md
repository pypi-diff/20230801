# Comparing `tmp/jovialengine-0.9.3.tar.gz` & `tmp/jovialengine-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jovialengine-0.9.3.tar", last modified: Thu Aug 18 02:10:04 2022, max compression
+gzip compressed data, was "jovialengine-0.9.4.tar", last modified: Wed Aug 24 00:51:27 2022, max compression
```

## Comparing `jovialengine-0.9.3.tar` & `jovialengine-0.9.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 02:10:04.484026 jovialengine-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-18 02:09:50.000000 jovialengine-0.9.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-08-18 02:10:04.484026 jovialengine-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-18 02:09:50.000000 jovialengine-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-18 02:09:50.000000 jovialengine-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-08-18 02:10:04.484026 jovialengine-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-18 02:09:50.000000 jovialengine-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 02:10:04.480026 jovialengine-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 02:10:04.484026 jovialengine-0.9.3/src/jovialengine/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5018 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/animsprite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7344 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/fontwrap.py
--rw-r--r--   0 runner    (1001) docker     (121)     7390 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/game.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/input.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/modebase.py
--rw-r--r--   0 runner    (1001) docker     (121)    12718 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/modegamemenu.py
--rw-r--r--   0 runner    (1001) docker     (121)     5987 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/save.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/saveable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-08-18 02:09:50.000000 jovialengine-0.9.3/src/jovialengine/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 02:10:04.484026 jovialengine-0.9.3/src/jovialengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-08-18 02:10:04.000000 jovialengine-0.9.3/src/jovialengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-08-18 02:10:04.000000 jovialengine-0.9.3/src/jovialengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 02:10:04.000000 jovialengine-0.9.3/src/jovialengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-18 02:10:04.000000 jovialengine-0.9.3/src/jovialengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-18 02:10:04.000000 jovialengine-0.9.3/src/jovialengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 00:51:27.257465 jovialengine-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-24 00:51:14.000000 jovialengine-0.9.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-08-24 00:51:27.257465 jovialengine-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-24 00:51:14.000000 jovialengine-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-24 00:51:14.000000 jovialengine-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-08-24 00:51:27.261465 jovialengine-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-24 00:51:14.000000 jovialengine-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 00:51:27.257465 jovialengine-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 00:51:27.257465 jovialengine-0.9.4/src/jovialengine/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5018 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/animsprite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7432 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/fontwrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7485 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/input.py
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/modebase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12860 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/modegamemenu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6093 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/save.py
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/saveable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-08-24 00:51:14.000000 jovialengine-0.9.4/src/jovialengine/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 00:51:27.257465 jovialengine-0.9.4/src/jovialengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-08-24 00:51:27.000000 jovialengine-0.9.4/src/jovialengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-08-24 00:51:27.000000 jovialengine-0.9.4/src/jovialengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 00:51:27.000000 jovialengine-0.9.4/src/jovialengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-24 00:51:27.000000 jovialengine-0.9.4/src/jovialengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-24 00:51:27.000000 jovialengine-0.9.4/src/jovialengine.egg-info/top_level.txt
```

### Comparing `jovialengine-0.9.3/LICENSE.txt` & `jovialengine-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jovialengine-0.9.3/PKG-INFO` & `jovialengine-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jovialengine
-Version: 0.9.3
+Version: 0.9.4
 Summary: A Simple Pygame Engine
 Home-page: https://github.com/JovialKnoll/jovialengine
 Author: Brett Kaplan
 Author-email: BrettCKaplan@gmail.com
 Project-URL: Source, https://github.com/JovialKnoll/jovialengine
 Project-URL: Issue Tracker, https://github.com/JovialKnoll/jovialengine/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jovialengine-0.9.3/setup.cfg` & `jovialengine-0.9.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jovialengine
-version = 0.9.3
+version = 0.9.4
 author = Brett Kaplan
 author_email = BrettCKaplan@gmail.com
 description = A Simple Pygame Engine
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JovialKnoll/jovialengine
 project_urls =
```

### Comparing `jovialengine-0.9.3/src/jovialengine/animsprite.py` & `jovialengine-0.9.4/src/jovialengine/animsprite.py`

 * *Files identical despite different names*

### Comparing `jovialengine-0.9.3/src/jovialengine/config.py` & `jovialengine-0.9.4/src/jovialengine/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,38 +5,35 @@
 FULLSCREEN = 'Fullscreen'
 SCREEN_SCALE = 'ScreenScale'
 _DEFAULTS = {
     MAX_FRAMERATE: 1000,
     SCREEN_SCALE: 0,
     FULLSCREEN: False,
 }
-_TYPES = {
-    MAX_FRAMERATE: 'int',
-    SCREEN_SCALE: 'int',
-    FULLSCREEN: 'bool',
-}
 _SECTION = 'Game'
 _config = configparser.ConfigParser(_DEFAULTS, default_section=_SECTION)
-_config_file: str
+_config_file: str | None = None
 
 
 def init(config_file: str):
     global _config_file
+    if _config_file:
+        raise RuntimeError("error: _config_file is already set")
     _config_file = config_file
     _config.read(_config_file)
     for section in _config.sections():
         _config.remove_section(section)
 
 
 def get(key: str):
-    match _TYPES.get(key):
-        case 'int':
-            return _config.getint(_SECTION, key)
-        case 'bool':
+    match _DEFAULTS.get(key):
+        case bool():
             return _config.getboolean(_SECTION, key)
+        case int():
+            return _config.getint(_SECTION, key)
         case _:
             return _config.get(_SECTION, key)
 
 
 def update(key: str, value):
     _config.set(_SECTION, key, str(value))
```

### Comparing `jovialengine-0.9.3/src/jovialengine/display.py` & `jovialengine-0.9.4/src/jovialengine/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 _monitor_res: tuple[int, int]
 _upscale_max: int
 _windowed_flags: int
 _fullscreen_flags: int
 is_fullscreen: bool
 upscale: int
 _disp_res: tuple[int, int]
-screen: pygame.Surface
+screen: pygame.Surface | None = None
 _fullscreen_offset: tuple[int, int] | None
 _full_screen: pygame.Surface | None
 _disp_screen: pygame.Surface
 
 
 def init(
     screenshot_directory: str,
@@ -38,14 +38,16 @@
     global _title
     global _window_icon
     global is_fullscreen
     global upscale
     global screen
     global _fullscreen_offset
     global _full_screen
+    if screen:
+        raise RuntimeError("error: screen is already set")
     _screenshot_directory = screenshot_directory
     screen_size = screen_size_in
     _title = title
     _window_icon = None
     if window_icon:
         _window_icon = pygame.image.load(window_icon)
     _setupDisplay()
```

### Comparing `jovialengine-0.9.3/src/jovialengine/fontwrap.py` & `jovialengine-0.9.4/src/jovialengine/fontwrap.py`

 * *Files identical despite different names*

### Comparing `jovialengine-0.9.3/src/jovialengine/game.py` & `jovialengine-0.9.4/src/jovialengine/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
                 pygame.mixer.unpause()
             self._current_mode.cleanup()
             self._current_mode = self._current_mode.next_mode
             input.clearMouseButtonStatus()
         self._is_first_loop = False
         if not self.running:
             config.save()
+            self._current_mode = None
+            self.state = None
+            pygame.quit()
         return self.running
 
     def _filterInput(self, events: Iterable[pygame.event.Event]):
         """Take care of input that game modes should not take care of."""
         result = map(display.scaleMouseInput, events)
         result = filter(self._filterEvent, result)
         result = map(input.mapEvent, result)
@@ -195,15 +198,15 @@
     start_mode_cls - the class for the first mode
     state_cls - the class for holding general game state
     src_directory - directory of the program
     screen_size - size of the virtual screen
     title - title of the game (for titlebar)
     window_icon - location of icon of the game (for titlebar)
     max_players - maximum number of players the game supports
-    num_inputs - number of button / axis inputs for mapping to (not from)
+    num_inputs - number of virtual inputs that button / axis inputs map to
     font_location - location of default font for the game
     font_size - default font size
     font_height - default font height
     font_antialias - default font antialias
     """
     global _game
     if _game:
```

### Comparing `jovialengine-0.9.3/src/jovialengine/input.py` & `jovialengine-0.9.4/src/jovialengine/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,27 @@
         self.player_id = player_id
         self.action_type = action_type
         self.action_value = action_value
         self.type = event.type
         self.__dict__ = event.__dict__
 
 
-_pressed_mouse_buttons: dict[int, tuple[int, int]] = dict()
 _controller_states: list[list[float | int]] | None = None
+_pressed_mouse_buttons: dict[int, tuple[int, int]]
 
 
 def init(max_players: int, num_inputs: int):
     global _controller_states
+    global _pressed_mouse_buttons
+    if _controller_states:
+        raise RuntimeError("error: _controller_states is already set")
     # load in input mapping from config
     # make objects to hold onto current virtual gamepad states
     _controller_states = [[0] * num_inputs for x in range(max_players)]
+    _pressed_mouse_buttons = dict()
 
 
 def _getAction(event: pygame.event.Event):
     # do actual mapping
     # if mapping results in setting a value in controller state that is already set
     # for [player_id][action_type] then set action_type = Action.TYPE_NONE
     player_id = 0
```

### Comparing `jovialengine-0.9.3/src/jovialengine/load.py` & `jovialengine-0.9.4/src/jovialengine/load.py`

 * *Files identical despite different names*

### Comparing `jovialengine-0.9.3/src/jovialengine/modebase.py` & `jovialengine-0.9.4/src/jovialengine/modebase.py`

 * *Files identical despite different names*

### Comparing `jovialengine-0.9.3/src/jovialengine/modegamemenu.py` & `jovialengine-0.9.4/src/jovialengine/modegamemenu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 
 import pygame
 
 from . import game
 from . import display
+from . import input
 from .fontwrap import getDefaultFontWrap
 from .modebase import ModeBase
 from .save import Save
 from .saveable import Saveable
 
 
 class ModeGameMenu(ModeBase, abc.ABC):
@@ -49,18 +50,18 @@
             self._drawTextAlways(disp_text)
 
 
 class ModeGameMenuTop(ModeGameMenu):
     def _input(self, action):
         if action.type == pygame.QUIT:
             game.getGame().running = False
+        elif action.action_type == input.Action.TYPE_PAUSE:
+            self.next_mode = self._previous_mode
         elif action.type == pygame.KEYDOWN:
-            if action.key == pygame.K_ESCAPE:
-                self.next_mode = self._previous_mode
-            elif action.key == pygame.K_1:
+            if action.key == pygame.K_1:
                 self.next_mode = ModeGameMenuSave(self._previous_mode, self._background)
             elif action.key == pygame.K_2:
                 self.next_mode = ModeGameMenuLoad(self._previous_mode, self._background)
             elif action.key == pygame.K_3:
                 self.next_mode = ModeGameMenuOptions(self._previous_mode, self._background)
             elif action.key == pygame.K_4:
                 self._stopMixer()
@@ -103,30 +104,30 @@
     def _resetCursorBlink(self):
         self._cursor_switch = True
         self._cursor_timer = 0
 
     def _input(self, action):
         if action.type == pygame.QUIT:
             self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
+        elif self._save_success and action.type == pygame.KEYDOWN:
+            self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
+        elif action.action_type == input.Action.TYPE_PAUSE:
+            if self._confirm_overwrite:
+                self._confirm_overwrite = False
+                self._save_success = None
+            else:
+                self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
         elif action.type == pygame.KEYDOWN:
             char = action.unicode
             length = len(self._save_name)
-            if self._save_success:
-                self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
-            elif action.key == pygame.K_ESCAPE:
-                if self._confirm_overwrite:
-                    self._confirm_overwrite = False
-                    self._save_success = None
-                else:
-                    self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
-            elif action.key == pygame.K_RETURN:
+            if action.key == pygame.K_RETURN:
                 if self._save_name and isinstance(self._previous_mode, Saveable):
                     if Save.willOverwrite(self._save_name) and not self._confirm_overwrite:
                         self._confirm_overwrite = True
-                    elif not self._save_success:
+                    else:
                         new_save = Save.getFromMode(self._save_name, self._previous_mode)
                         self._save_success = new_save.save()
             elif action.key == pygame.K_LEFT:
                 self._cursor_position = max(self._cursor_position - 1, 0)
                 self._resetCursorBlink()
             elif action.key == pygame.K_RIGHT:
                 self._cursor_position = min(self._cursor_position + 1, length)
@@ -211,16 +212,18 @@
         self._loaded_save = False
         self._confirm_delete = False
         self._deleted_save = False
 
     def _input(self, action):
         if action.type == pygame.QUIT:
             self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
+        elif action.action_type == input.Action.TYPE_PAUSE:
+            self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
         elif action.type == pygame.KEYDOWN:
-            if action.key == pygame.K_ESCAPE or self._loaded_save:
+            if self._loaded_save:
                 self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
             elif self._deleted_save:
                 self._deleted_save = False
             elif self._confirm_delete:
                 if action.key == pygame.K_RETURN:
                     self._confirm_delete = False
                     self._saves[self._save_index].delete()
@@ -270,14 +273,16 @@
         screen.blit(self._menu_surface, (0, 0))
 
 
 class ModeGameMenuOptions(ModeGameMenu):
     def _input(self, action):
         if action.type == pygame.QUIT:
             self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
+        elif action.action_type == input.Action.TYPE_PAUSE:
+            self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
         elif action.type == pygame.KEYUP:
             if action.key in (
                     pygame.K_DOWN, pygame.K_s,
                     pygame.K_LEFT, pygame.K_a,
                     pygame.K_PAGEDOWN, pygame.K_MINUS,
             ):
                 display.changeScale(-1)
@@ -286,17 +291,15 @@
                     pygame.K_RIGHT, pygame.K_d,
                     pygame.K_PAGEUP, pygame.K_EQUALS,
             ):
                 display.changeScale(1)
             elif action.key in (pygame.K_f, pygame.K_F11,):
                 display.toggleFullscreen()
         elif action.type == pygame.KEYDOWN:
-            if action.key == pygame.K_ESCAPE:
-                self.next_mode = ModeGameMenuTop(self._previous_mode, self._background)
-            elif '1' <= action.unicode <= '9':
+            if '1' <= action.unicode <= '9':
                 target_scale = int(action.unicode)
                 display.setScale(target_scale)
 
     def _drawPreSprites(self, screen):
         disp_text = self._SHARED_DISP_TEXT
         disp_text += f"ARROWS) Upscaling: {display.upscale}" \
                      f"\nF) Fullscreen: {self.getTickBox(display.is_fullscreen)}"
```

### Comparing `jovialengine-0.9.3/src/jovialengine/save.py` & `jovialengine-0.9.4/src/jovialengine/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 _KEY_ELEMENTS = 'ELEMENTS'
 _KEY_MAXLEN = 'MAXLEN'
 _KEY_MODULE = 'MODULE'
 _KEY_CLASS = 'CLASS'
 _KEY_SAVEABLE = 'SAVEABLE'
 _SAVE_EXT = '.sav'
 _mode_module: ModuleType
-_save_directory: str
+_save_directory: str | None = None
 
 
 def init(mode_module: ModuleType, save_directory: str):
     global _mode_module
     global _save_directory
+    if _save_directory:
+        raise RuntimeError("error: _save_directory is already set")
     _mode_module = mode_module
     _save_directory = save_directory
 
 
 class _SaveableJSONEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, deque):
```

### Comparing `jovialengine-0.9.3/src/jovialengine/saveable.py` & `jovialengine-0.9.4/src/jovialengine/saveable.py`

 * *Files identical despite different names*

### Comparing `jovialengine-0.9.3/src/jovialengine/utility.py` & `jovialengine-0.9.4/src/jovialengine/utility.py`

 * *Files identical despite different names*

### Comparing `jovialengine-0.9.3/src/jovialengine.egg-info/PKG-INFO` & `jovialengine-0.9.4/src/jovialengine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jovialengine
-Version: 0.9.3
+Version: 0.9.4
 Summary: A Simple Pygame Engine
 Home-page: https://github.com/JovialKnoll/jovialengine
 Author: Brett Kaplan
 Author-email: BrettCKaplan@gmail.com
 Project-URL: Source, https://github.com/JovialKnoll/jovialengine
 Project-URL: Issue Tracker, https://github.com/JovialKnoll/jovialengine/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jovialengine-0.9.3/src/jovialengine.egg-info/SOURCES.txt` & `jovialengine-0.9.4/src/jovialengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

