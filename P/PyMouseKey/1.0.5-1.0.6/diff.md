# Comparing `tmp/PyMouseKey-1.0.5-py3-none-any.whl.zip` & `tmp/PyMouseKey-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5971 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    18647 b- defN 23-May-21 21:22 pymousekey/__init__.py
--rw-rw-rw-  2.0 fat      443 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/RECORD
-5 files, 19582 bytes uncompressed, 5245 bytes compressed:  73.2%
+Zip file size: 6505 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    20833 b- defN 23-Aug-01 08:47 pymousekey/__init__.py
+-rw-rw-rw-  2.0 fat      470 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      389 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/RECORD
+5 files, 21795 bytes uncompressed, 5779 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pymousekey/__init__.py
 Comment: 
 
-Filename: PyMouseKey-1.0.5.dist-info/METADATA
+Filename: PyMouseKey-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: PyMouseKey-1.0.5.dist-info/WHEEL
+Filename: PyMouseKey-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: PyMouseKey-1.0.5.dist-info/top_level.txt
+Filename: PyMouseKey-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMouseKey-1.0.5.dist-info/RECORD
+Filename: PyMouseKey-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymousekey/__init__.py

```diff
@@ -1,13 +1,16 @@
 import time
 import math
 import ctypes
+import ctypes.wintypes
 import threading
 
 autoclickState = False
+registered_hotkeys = {}
+hotkey_threads = {}
 
 PAUSE = 0.1
 MOUSEEVENTF_ABSOLUTE = 0x8000
 MOUSEEVENTF_LEFTDOWN = 0x0002
 MOUSEEVENTF_LEFTUP = 0x0004
 MOUSEEVENTF_MIDDLEDOWN = 0x0020
 MOUSEEVENTF_MIDDLEUP = 0x0040
@@ -31,23 +34,26 @@
 KEYEVENTF_SCANCODE = 0x0008
 KEYEVENTF_UNICODE = 0x0004
 
 WM_ACTIVATE = 0x6
 WM_CHAR = 0x102
 WA_ACTIVE = 0x1
 
+WM_QUIT = 0x0012
+
 WM_LBUTTONDOWN = 0x0201
 WM_LBUTTONUP = 0x0202
 WM_LBUTTONCLICK = WM_LBUTTONDOWN + WM_LBUTTONUP
 WM_RBUTTONDOWN = 0x0204
 WM_RBUTTONUP = 0x0205
 WM_RBUTTONCLICK = WM_RBUTTONDOWN + WM_RBUTTONUP
 WM_MBUTTONDOWN = 0x0207
 WM_MBUTTONUP = 0x0208
 WM_MBUTTONCLICK = WM_MBUTTONDOWN + WM_MBUTTONUP
+WM_HOTKEY = 0x0312
 
 WM_NCHITTEST = 0x0084
 WM_MOUSEMOVE = 0x0200
 WM_SETCURSOR = 0x0020
 
 MK_LBUTTON = 0x0001
 MK_MBUTTON = 0x0010
@@ -529,15 +535,73 @@
     if not key.lower() in KEYS or KEYS[key.lower()] is None:
         return
 
     ii_ = Input_I()
     ii_.ki = KeyBdInput(0, KEYS[key.lower()], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
     x = Input(ctypes.c_ulong(1), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
+
+
+def add_hotkey(key, callback, args=None):
+    """
+    Registers a system wide hotkey with optional args using ctypes and GetMessageW starting it in a seperate thread
+
+    """
+    def add_hotkey_thread(key, callback, args=None):
+        key_id = len(registered_hotkeys) + 1
+        registered_hotkeys[VK_KEYS[key]] = key_id
+        hotkey_threads[VK_KEYS[key]] = hotkey_thread.native_id
+
+        ctypes.windll.user32.RegisterHotKey(None, key_id , None, VK_KEYS[key])
+        
+        msg = ctypes.wintypes.MSG()
+
+        while ctypes.windll.user32.GetMessageW(ctypes.byref(msg), 0, 0, 0) != 0:
+            if msg.message == WM_HOTKEY:
+                if args:
+                    callback(args)
+                else:
+                    callback()
+                ctypes.windll.user32.TranslateMessage(ctypes.byref(msg))
+                ctypes.windll.user32.DispatchMessageW(ctypes.byref(msg))
+        
+        try:
+            ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[VK_KEYS[key]])
+        except(KeyError):
+            pass
+    if key in VK_KEYS:
+        hotkey_thread = threading.Thread(target=add_hotkey_thread, args=[key, callback, args])
+        hotkey_thread.start()
+
+
+def remove_hotkey(key):
+    """
+    Unregisters and removes the specified hotkey if it was registered previously
+
+    """
+    if VK_KEYS[key] in registered_hotkeys:
+        ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[VK_KEYS[key]])
+        ctypes.windll.user32.PostThreadMessageW(hotkey_threads[VK_KEYS[key]], WM_QUIT, 0, 0)
+        del registered_hotkeys[VK_KEYS[key]]
+        del hotkey_threads[VK_KEYS[key]]
+
+
+def remove_all_hotkeys():
+    """
+    Unregisters and removes all currently registered hotkeys
     
+    """
+    for key in registered_hotkeys.values():
+        ctypes.windll.user32.UnregisterHotKey(None, key)
+        
+    for threads in hotkey_threads.values():
+        ctypes.windll.user32.PostThreadMessageW(threads, WM_QUIT, 0, 0)
+
+    registered_hotkeys.clear()
+    hotkey_threads.clear()
 
 def typeWrite(message, interval=0.0, _pause=True):
     """
     Types out a given message, letters suppors lowercase and uppercase letters\n
     message(str): The message you want typed out\n
     interval(float): The sleep after the key has been pressed so you can set your own intervals per call\n
     _pause is the sleep after every function call
@@ -613,8 +677,8 @@
         ctypes.windll.user32.PostMessageW(handle, WM_NCHITTEST, 0, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONDOWN, MK_RBUTTON, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONUP, MK_RBUTTON, lparam)
 
     elif button == 'middle':
         ctypes.windll.user32.PostMessageW(handle, WM_NCHITTEST, 0, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONDOWN, MK_MBUTTON, lparam)
-        ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONUP, MK_MBUTTON, lparam)
+        ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONUP, MK_MBUTTON, lparam)
```

