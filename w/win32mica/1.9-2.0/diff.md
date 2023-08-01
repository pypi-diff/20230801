# Comparing `tmp/win32mica-1.9.tar.gz` & `tmp/win32mica-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win32mica-1.9.tar", last modified: Tue Jun 13 11:27:16 2023, max compression
+gzip compressed data, was "win32mica-2.0.tar", last modified: Tue Aug  1 09:27:27 2023, max compression
```

## Comparing `win32mica-1.9.tar` & `win32mica-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 11:27:04.000000 win32mica-1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 11:27:16.360606 win32mica-1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-13 11:27:04.000000 win32mica-1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 11:27:04.000000 win32mica-1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:27:16.360606 win32mica-1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 11:27:04.000000 win32mica-1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/src/win32mica/
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-13 11:27:04.000000 win32mica-1.9/src/win32mica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/src/win32mica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:27:27.412025 win32mica-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 09:27:16.000000 win32mica-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-08-01 09:27:27.412025 win32mica-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-01 09:27:16.000000 win32mica-2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 09:27:16.000000 win32mica-2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:27:27.412025 win32mica-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-01 09:27:16.000000 win32mica-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:27:27.408025 win32mica-2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:27:27.408025 win32mica-2.0/src/win32mica/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-08-01 09:27:16.000000 win32mica-2.0/src/win32mica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:27:27.412025 win32mica-2.0/src/win32mica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-08-01 09:27:27.000000 win32mica-2.0/src/win32mica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-01 09:27:27.000000 win32mica-2.0/src/win32mica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:27:27.000000 win32mica-2.0/src/win32mica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 09:27:27.000000 win32mica-2.0/src/win32mica.egg-info/top_level.txt
```

### Comparing `win32mica-1.9/LICENSE` & `win32mica-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `win32mica-1.9/PKG-INFO` & `win32mica-2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win32mica
-Version: 1.9
+Version: 2.0
 Summary: Apply mica background (if supported) and immersive dark mode to Windows 11 Win32 apps made with python, such as Tkinter or PyQt/PySide apps
 Home-page: https://github.com/marticliment/win32mica
 Author: Martí Climent
 Author-email: marticlilop@gmail.com
 Project-URL: Bug Tracker, https://github.com/marticliment/win32mica/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 ```pwsh
 python -m pip install win32mica
 ```
 
 ## Requirements:
  - Windows 11
  - A window set to not have a transparent background and to have extended composition enabled* (It might work with other settings, but nothing is guaranteed.)
- - The HWND (identifier) of that window. More info: [what is a hwnd?](https://stackoverflow.com/questions/1635645/what-is-hwnd-in-vc) 
+ - The hWnd (identifier) of that window. More info: [what is a hWnd?](https://stackoverflow.com/questions/1635645/what-is-hwnd-in-vc) 
  - OPTIONAL: The window must have semi-transparent widgets/controls in order to recreate the transparency effect on the controls.
  - OPTIONAL: Know if Windows has dark or light mode enabled. This can be checked with the [`darkdetect` module](https://pypi.org/project/darkdetect/)
 
 ## Usage:
 
 ```python
 #####################################################################
@@ -48,42 +48,35 @@
 #                                                                   #
 #####################################################################
 
 hwnd = qtwindow.winId().__int__() # On a PyQt/PySide window
 hwnd = tkwindow.frame() # On a tkinter window
 # You'll need to adjust this to your program
 
-from win32mica import MICAMODE, ApplyMica
+from win32mica import MicaMode, ApplyMica
 
-mode = MICAMODE.DARK  # Dark mode mica effect
-mode = MICAMODE.LIGHT # Light mode mica effect
+mode = MicaMode.DARK  # Dark mode mica effect
+mode = MicaMode.LIGHT # Light mode mica effect
+mode = MicaMode.AUTO # Apply system theme, and change it if system theme changes
 # Choose one of them following your app color scheme
 
-import darkdetect # You can pass the darkdetect return value directly, since the ColorMode accepts bool values (True -> dark, False -> light)
-mode = darkdetect.isDark()
+def callbackFunction():
+    print("Theme has changed!")
+
+win32mica.ApplyMica(HWND=hwnd, ColorMode=mode, onThemeChange=callbackFunction)
+
+# Function arguments:
+#    HWND -- a handle to a window (it being an integer value)
+#    ColorMode -- MicaMode.DARK or MicaMode.LIGHT, depending on the preferred UI theme. A boolean value can also be passed, True meaning Dark and False meaning Light
+#    onThemeChange -- a function without arguments that will be called when the system theme changes. This parameter is effective only if the theme is set to MicaMode.AUTO
 
-win32mica.ApplyMica(hwnd, mode)
-# Will return 0x32 if the system does not support Mica textures (Windows 10 or less). Immersive dark mode will still be applied (if selected theme is MICAMODE.DARK)
-# Will return 0x00 if mica is applied successfully
-# If DwmSetWindowAttribute fails, the output code will be returned 
 ```
 
 You can check out the [examples folder](https://github.com/martinet101/win32mica/tree/main/examples) for detailed use in Tk and PySide/PyQt.
 
 ## Result:
 
 ![image](https://user-images.githubusercontent.com/53119851/188261331-15e17447-590f-452a-be62-07c67a3db673.png)<br>
 ![image](https://user-images.githubusercontent.com/53119851/188261398-83f5d904-586f-47ce-b6af-d4521eb3f68f.png)
 
 _Those are PySide2 windows with custom widgets._
 
-
-## Troubleshooting:
-
-For more information about possible errors/mistakes, make sure to add the following before using win32mica:
-
-
-```python
-# Add these lines at the very start of your script
-import win32mica
-win32mica.debugging = True
-```
```

### Comparing `win32mica-1.9/README.md` & `win32mica-2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```pwsh
 python -m pip install win32mica
 ```
 
 ## Requirements:
  - Windows 11
  - A window set to not have a transparent background and to have extended composition enabled* (It might work with other settings, but nothing is guaranteed.)
- - The HWND (identifier) of that window. More info: [what is a hwnd?](https://stackoverflow.com/questions/1635645/what-is-hwnd-in-vc) 
+ - The hWnd (identifier) of that window. More info: [what is a hWnd?](https://stackoverflow.com/questions/1635645/what-is-hwnd-in-vc) 
  - OPTIONAL: The window must have semi-transparent widgets/controls in order to recreate the transparency effect on the controls.
  - OPTIONAL: Know if Windows has dark or light mode enabled. This can be checked with the [`darkdetect` module](https://pypi.org/project/darkdetect/)
 
 ## Usage:
 
 ```python
 #####################################################################
@@ -32,42 +32,35 @@
 #                                                                   #
 #####################################################################
 
 hwnd = qtwindow.winId().__int__() # On a PyQt/PySide window
 hwnd = tkwindow.frame() # On a tkinter window
 # You'll need to adjust this to your program
 
-from win32mica import MICAMODE, ApplyMica
+from win32mica import MicaMode, ApplyMica
 
-mode = MICAMODE.DARK  # Dark mode mica effect
-mode = MICAMODE.LIGHT # Light mode mica effect
+mode = MicaMode.DARK  # Dark mode mica effect
+mode = MicaMode.LIGHT # Light mode mica effect
+mode = MicaMode.AUTO # Apply system theme, and change it if system theme changes
 # Choose one of them following your app color scheme
 
-import darkdetect # You can pass the darkdetect return value directly, since the ColorMode accepts bool values (True -> dark, False -> light)
-mode = darkdetect.isDark()
+def callbackFunction():
+    print("Theme has changed!")
+
+win32mica.ApplyMica(HWND=hwnd, ColorMode=mode, onThemeChange=callbackFunction)
+
+# Function arguments:
+#    HWND -- a handle to a window (it being an integer value)
+#    ColorMode -- MicaMode.DARK or MicaMode.LIGHT, depending on the preferred UI theme. A boolean value can also be passed, True meaning Dark and False meaning Light
+#    onThemeChange -- a function without arguments that will be called when the system theme changes. This parameter is effective only if the theme is set to MicaMode.AUTO
 
-win32mica.ApplyMica(hwnd, mode)
-# Will return 0x32 if the system does not support Mica textures (Windows 10 or less). Immersive dark mode will still be applied (if selected theme is MICAMODE.DARK)
-# Will return 0x00 if mica is applied successfully
-# If DwmSetWindowAttribute fails, the output code will be returned 
 ```
 
 You can check out the [examples folder](https://github.com/martinet101/win32mica/tree/main/examples) for detailed use in Tk and PySide/PyQt.
 
 ## Result:
 
 ![image](https://user-images.githubusercontent.com/53119851/188261331-15e17447-590f-452a-be62-07c67a3db673.png)<br>
 ![image](https://user-images.githubusercontent.com/53119851/188261398-83f5d904-586f-47ce-b6af-d4521eb3f68f.png)
 
 _Those are PySide2 windows with custom widgets._
 
-
-## Troubleshooting:
-
-For more information about possible errors/mistakes, make sure to add the following before using win32mica:
-
-
-```python
-# Add these lines at the very start of your script
-import win32mica
-win32mica.debugging = True
-```
```

### Comparing `win32mica-1.9/setup.py` & `win32mica-2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="win32mica",
-    version="1.9",
+    version="2.0",
     author="Martí Climent",
     author_email="marticlilop@gmail.com",
     description="Apply mica background (if supported) and immersive dark mode to Windows 11 Win32 apps made with python, such as Tkinter or PyQt/PySide apps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marticliment/win32mica",
     project_urls={
```

### Comparing `win32mica-1.9/src/win32mica/__init__.py` & `win32mica-2.0/src/win32mica/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import ctypes, sys, threading, time, winreg
 
 class MICAMODE():
-    DARK = True
-    LIGHT = False
+    DARK = 1
+    LIGHT = 0
+    AUTO = 2
+
+class MicaMode():
+    DARK = 1
+    LIGHT = 0
+    AUTO = 2
 
 
 debugging = False
 
 def readRegedit(aKey, sKey, default, storage=winreg.HKEY_CURRENT_USER):
     registry = winreg.ConnectRegistry(None, storage)
     reg_keypath = aKey
@@ -25,130 +31,131 @@
                 return value
         except OSError as e:
             return default
         except Exception as e:
             print(e)
             return default
 
-
-def ApplyMica(HWND: int, ColorMode: bool = MICAMODE.LIGHT, darkModeMode: int = 20) -> int:
+def nullFunction():
+    pass
+    
+def ApplyMica(HWND: int, ColorMode: bool = MicaMode.LIGHT, onThemeChange = nullFunction) -> int:
     """Apply the new mica effect on a window making use of the hidden win32api and return an integer depending on the result of the operation
     
     Keyword arguments:
     HWND -- a handle to a window (it being an integer value)
-    ColorMode -- MICAMODE.DARK or MICAMODE.LIGHT, depending on the preferred UI theme. A boolean value can also be passed, True meaning Dark and False meaning Light
+    ColorMode -- MicaMode.DARK or MicaMode.LIGHT, depending on the preferred UI theme. A boolean value can also be passed, True meaning Dark and False meaning Light
+    onThemeChange -- a function to call when the system theme changes. Will be called only if ColorMode is set to MicaMode.AUTO
     """
     try:
-        HWND = int(HWND)
-    except ValueError:
-        HWND = int(str(HWND), 16)
-    
-    user32 = ctypes.windll.user32
-    dwm = ctypes.windll.dwmapi
+        try:
+            HWND = int(HWND)
+        except ValueError:
+            HWND = int(str(HWND), 16)
+        
+        user32 = ctypes.windll.user32
+        dwm = ctypes.windll.dwmapi
 
-    class AccentPolicy(ctypes.Structure):
-        _fields_ = [
-            ("AccentState", ctypes.c_uint),
-            ("AccentFlags", ctypes.c_uint),
-            ("GradientColor", ctypes.c_uint),
-            ("AnimationId", ctypes.c_uint)
-        ]
-
-    class WindowCompositionAttribute(ctypes.Structure):
-        _fields_ = [
-            ("Attribute", ctypes.c_int),
-            ("Data", ctypes.POINTER(ctypes.c_int)),
-            ("SizeOfData", ctypes.c_size_t)
-        ]
-
-    class _MARGINS(ctypes.Structure):
-        _fields_ = [("cxLeftWidth", ctypes.c_int),
-                    ("cxRightWidth", ctypes.c_int),
-                    ("cyTopHeight", ctypes.c_int),
-                    ("cyBottomHeight", ctypes.c_int)
-                    ]
+        class AccentPolicy(ctypes.Structure):
+            _fields_ = [
+                ("AccentState", ctypes.c_uint),
+                ("AccentFlags", ctypes.c_uint),
+                ("GradientColor", ctypes.c_uint),
+                ("AnimationId", ctypes.c_uint)
+            ]
+
+        class WindowCompositionAttribute(ctypes.Structure):
+            _fields_ = [
+                ("Attribute", ctypes.c_int),
+                ("Data", ctypes.POINTER(ctypes.c_int)),
+                ("SizeOfData", ctypes.c_size_t)
+            ]
+
+        class _MARGINS(ctypes.Structure):
+            _fields_ = [("cxLeftWidth", ctypes.c_int),
+                        ("cxRightWidth", ctypes.c_int),
+                        ("cyTopHeight", ctypes.c_int),
+                        ("cyBottomHeight", ctypes.c_int)
+                        ]
 
-    DWM_UNDOCUMENTED_MICA_ENTRY = 1029 # Undocumented MICA (Windows 11 22523-)
-    DWM_UNDOCUMENTED_MICA_VALUE = 0x01 # Undocumented MICA (Windows 11 22523-)
-    
-    DWM_DOCUMENTED_MICA_ENTRY = 38     # Documented MICA (Windows 11 22523+)
-    DWM_DOCUMENTED_MICA_VALUE = 0x02   # Documented MICA (Windows 11 22523+)
-    DWMW_USE_IMMERSIVE_DARK_MODE = 20
-    
+        DWM_UNDOCUMENTED_MICA_ENTRY = 1029 # Undocumented MICA (Windows 11 22523-)
+        DWM_UNDOCUMENTED_MICA_VALUE = 0x01 # Undocumented MICA (Windows 11 22523-)
+        
+        DWM_DOCUMENTED_MICA_ENTRY = 38     # Documented MICA (Windows 11 22523+)
+        DWM_DOCUMENTED_MICA_VALUE = 0x02   # Documented MICA (Windows 11 22523+)
+        DWMW_USE_IMMERSIVE_DARK_MODE = 20
+        
 
-    SetWindowCompositionAttribute = user32.SetWindowCompositionAttribute
-    DwmSetWindowAttribute = dwm.DwmSetWindowAttribute 
-    DwmExtendFrameIntoClientArea = dwm.DwmExtendFrameIntoClientArea
+        SetWindowCompositionAttribute = user32.SetWindowCompositionAttribute
+        DwmSetWindowAttribute = dwm.DwmSetWindowAttribute 
+        DwmExtendFrameIntoClientArea = dwm.DwmExtendFrameIntoClientArea
+        
+        MODE = 0x00
 
-    if ColorMode == MICAMODE.DARK: # Apply dark mode
         def setMode():
-            oldMode = -1
+            nonlocal MODE
+            OldMode = -1
             while True:
-                mode = readRegedit(r"Software\Microsoft\Windows\CurrentVersion\Themes\Personalize", "AppsUseLightTheme", 0)
-                if oldMode != mode:
-                    oldMode = mode
-                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(0x01)), ctypes.sizeof(ctypes.c_int))
+                CurrentMode = readRegedit(r"Software\Microsoft\Windows\CurrentVersion\Themes\Personalize", "AppsUseLightTheme", 0)
+                if OldMode != CurrentMode:
+                    
+                    OldMode = CurrentMode
+                    if MODE == 0x01:
+                        ModeToSet = 0x01
+                    elif MODE == 0x00:
+                        ModeToSet = 0x00
+                    else:
+                        ModeToSet = 0x00 if CurrentMode != 0 else 0x01
+                        try:
+                            onThemeChange()
+                        except:
+                            pass
+                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(ModeToSet)), ctypes.sizeof(ctypes.c_int))
                     time.sleep(0.5)
-                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(0x01)), ctypes.sizeof(ctypes.c_int))
+                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(ModeToSet)), ctypes.sizeof(ctypes.c_int))
                     time.sleep(0.5)
-                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(0x01)), ctypes.sizeof(ctypes.c_int))
+                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(ModeToSet)), ctypes.sizeof(ctypes.c_int))
                     time.sleep(0.5)
-                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(0x01)), ctypes.sizeof(ctypes.c_int))
+                    DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(ModeToSet)), ctypes.sizeof(ctypes.c_int))
                     time.sleep(0.5)
                 time.sleep(0.1)
-                    
-
-
-        threading.Thread(target=setMode, daemon=True, name="win32mica: ensure dark mode").start()
         
-    else: # Apply light mode
-        DwmSetWindowAttribute(HWND, DWMW_USE_IMMERSIVE_DARK_MODE, ctypes.byref(ctypes.c_int(0x00)), ctypes.sizeof(ctypes.c_int)) 
-
-
-    if sys.platform == "win32" and sys.getwindowsversion().build >= 22000:
+        if ColorMode == MicaMode.DARK:
+            MODE = 0x01
+        elif ColorMode == MicaMode.LIGHT:
+            MODE = 0x00
+        else: # ColorMode == MicaMode.AUTO
+            MODE = 0x02
+        
+        threading.Thread(target=setMode, daemon=True, name="win32mica: theme thread").start()
 
-        Acp = AccentPolicy()
-        Acp.GradientColor = int("00cccccc", base=16)
-        Acp.AccentState = 5
-        Acp.AccentPolicy = 19
+        if sys.platform == "win32" and sys.getwindowsversion().build >= 22000:
 
-        Wca = WindowCompositionAttribute()
-        Wca.Attribute = 20
-        Wca.SizeOfData = ctypes.sizeof(Acp)
-        Wca.Data = ctypes.cast(ctypes.pointer(Acp), ctypes.POINTER(ctypes.c_int))
+            Acp = AccentPolicy()
+            Acp.GradientColor = int("00cccccc", base=16)
+            Acp.AccentState = 5
+            Acp.AccentPolicy = 19
+
+            Wca = WindowCompositionAttribute()
+            Wca.Attribute = 20
+            Wca.SizeOfData = ctypes.sizeof(Acp)
+            Wca.Data = ctypes.cast(ctypes.pointer(Acp), ctypes.POINTER(ctypes.c_int))
+
+            Mrg = _MARGINS(-1, -1, -1, -1)
+            
+            o = DwmExtendFrameIntoClientArea(HWND, ctypes.byref(Mrg))
+            try:
+                o = SetWindowCompositionAttribute(HWND, Wca)
+            except ctypes.ArgumentError:
+                pass
 
-        Mrg = _MARGINS(-1, -1, -1, -1)
-        
-        o = DwmExtendFrameIntoClientArea(HWND, ctypes.byref(Mrg))
-        if debugging:
-            if o != 0:
-                print("Win32mica: Failed to DwmExtendFrameIntoClientArea", hex(o+0xffffffff))
-            else:
-                print("Win32mica: DwmExtendFrameIntoClientArea Ok")
-        o = SetWindowCompositionAttribute(HWND, Wca)
-        if debugging:
-            if o != 0:
-                print("Win32mica: Failed to SetWindowCompositionAttribute", o)
+            if sys.getwindowsversion().build < 22523:
+                return DwmSetWindowAttribute(HWND, DWM_UNDOCUMENTED_MICA_ENTRY, ctypes.byref(ctypes.c_int(DWM_UNDOCUMENTED_MICA_VALUE)), ctypes.sizeof(ctypes.c_int))
             else:
-                print("Win32mica: SetWindowCompositionAttribute Ok")
-        
-        if ColorMode == MICAMODE.DARK:
-            Wca.Attribute = 1
-            o = SetWindowCompositionAttribute(HWND, Wca)
-            if debugging:
-                if o != 0:
-                    print("Win32mica: Failed to SetWindowCompositionAttribute (dark mode)", o)
-                else:
-                    print("Win32mica: SetWindowCompositionAttribute OK (dark mode)", o)
+                return DwmSetWindowAttribute(HWND, DWM_DOCUMENTED_MICA_ENTRY, ctypes.byref(ctypes.c_int(DWM_DOCUMENTED_MICA_VALUE)), ctypes.sizeof(ctypes.c_int))    
         else:
-            if debugging:
-                print("Win32mica: No SetWindowCompositionAttribute (light mode)")
-
-        if sys.getwindowsversion().build < 22523: # If mica is not a public API
-            return DwmSetWindowAttribute(HWND, DWM_UNDOCUMENTED_MICA_ENTRY, ctypes.byref(ctypes.c_int(DWM_UNDOCUMENTED_MICA_VALUE)), ctypes.sizeof(ctypes.c_int))
-        else: # If mica is present in the public API
-            return DwmSetWindowAttribute(HWND, DWM_DOCUMENTED_MICA_ENTRY, ctypes.byref(ctypes.c_int(DWM_DOCUMENTED_MICA_VALUE)), ctypes.sizeof(ctypes.c_int))    
-    else:
-        print(f"Win32Mica Error: {sys.platform} version {sys.getwindowsversion().build} is not supported")
-        return 0x32
+            print(f"Win32Mica Error: {sys.platform} version {sys.getwindowsversion().build} is not supported")
+            return 0x32
+    except Exception as e:
+        print("Win32mica: "+str(type(e))+": "+str(e))
```

### Comparing `win32mica-1.9/src/win32mica.egg-info/PKG-INFO` & `win32mica-2.0/src/win32mica.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win32mica
-Version: 1.9
+Version: 2.0
 Summary: Apply mica background (if supported) and immersive dark mode to Windows 11 Win32 apps made with python, such as Tkinter or PyQt/PySide apps
 Home-page: https://github.com/marticliment/win32mica
 Author: Martí Climent
 Author-email: marticlilop@gmail.com
 Project-URL: Bug Tracker, https://github.com/marticliment/win32mica/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 ```pwsh
 python -m pip install win32mica
 ```
 
 ## Requirements:
  - Windows 11
  - A window set to not have a transparent background and to have extended composition enabled* (It might work with other settings, but nothing is guaranteed.)
- - The HWND (identifier) of that window. More info: [what is a hwnd?](https://stackoverflow.com/questions/1635645/what-is-hwnd-in-vc) 
+ - The hWnd (identifier) of that window. More info: [what is a hWnd?](https://stackoverflow.com/questions/1635645/what-is-hwnd-in-vc) 
  - OPTIONAL: The window must have semi-transparent widgets/controls in order to recreate the transparency effect on the controls.
  - OPTIONAL: Know if Windows has dark or light mode enabled. This can be checked with the [`darkdetect` module](https://pypi.org/project/darkdetect/)
 
 ## Usage:
 
 ```python
 #####################################################################
@@ -48,42 +48,35 @@
 #                                                                   #
 #####################################################################
 
 hwnd = qtwindow.winId().__int__() # On a PyQt/PySide window
 hwnd = tkwindow.frame() # On a tkinter window
 # You'll need to adjust this to your program
 
-from win32mica import MICAMODE, ApplyMica
+from win32mica import MicaMode, ApplyMica
 
-mode = MICAMODE.DARK  # Dark mode mica effect
-mode = MICAMODE.LIGHT # Light mode mica effect
+mode = MicaMode.DARK  # Dark mode mica effect
+mode = MicaMode.LIGHT # Light mode mica effect
+mode = MicaMode.AUTO # Apply system theme, and change it if system theme changes
 # Choose one of them following your app color scheme
 
-import darkdetect # You can pass the darkdetect return value directly, since the ColorMode accepts bool values (True -> dark, False -> light)
-mode = darkdetect.isDark()
+def callbackFunction():
+    print("Theme has changed!")
+
+win32mica.ApplyMica(HWND=hwnd, ColorMode=mode, onThemeChange=callbackFunction)
+
+# Function arguments:
+#    HWND -- a handle to a window (it being an integer value)
+#    ColorMode -- MicaMode.DARK or MicaMode.LIGHT, depending on the preferred UI theme. A boolean value can also be passed, True meaning Dark and False meaning Light
+#    onThemeChange -- a function without arguments that will be called when the system theme changes. This parameter is effective only if the theme is set to MicaMode.AUTO
 
-win32mica.ApplyMica(hwnd, mode)
-# Will return 0x32 if the system does not support Mica textures (Windows 10 or less). Immersive dark mode will still be applied (if selected theme is MICAMODE.DARK)
-# Will return 0x00 if mica is applied successfully
-# If DwmSetWindowAttribute fails, the output code will be returned 
 ```
 
 You can check out the [examples folder](https://github.com/martinet101/win32mica/tree/main/examples) for detailed use in Tk and PySide/PyQt.
 
 ## Result:
 
 ![image](https://user-images.githubusercontent.com/53119851/188261331-15e17447-590f-452a-be62-07c67a3db673.png)<br>
 ![image](https://user-images.githubusercontent.com/53119851/188261398-83f5d904-586f-47ce-b6af-d4521eb3f68f.png)
 
 _Those are PySide2 windows with custom widgets._
 
-
-## Troubleshooting:
-
-For more information about possible errors/mistakes, make sure to add the following before using win32mica:
-
-
-```python
-# Add these lines at the very start of your script
-import win32mica
-win32mica.debugging = True
-```
```

