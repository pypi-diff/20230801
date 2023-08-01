# Comparing `tmp/PySideSix-Frameless-Window-0.1.1.tar.gz` & `tmp/PySideSix-Frameless-Window-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySideSix-Frameless-Window-0.1.1.tar", last modified: Sat Jul  8 13:11:41 2023, max compression
+gzip compressed data, was "dist\PySideSix-Frameless-Window-0.1.2.tar", last modified: Tue Aug  1 03:47:21 2023, max compression
```

## Comparing `PySideSix-Frameless-Window-0.1.1.tar` & `PySideSix-Frameless-Window-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.949763 PySideSix-Frameless-Window-0.1.1/
--rw-rw-rw-   0        0        0     7815 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5519 2023-07-08 13:11:41.948742 PySideSix-Frameless-Window-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.900262 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5519 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4927 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.911055 PySideSix-Frameless-Window-0.1.1/qframelesswindow/
--rw-rw-rw-   0        0        0     1614 2023-07-08 13:08:40.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.915335 PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.919688 PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     4320 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3147 2023-07-08 13:08:00.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.924514 PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     4529 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4549 2023-07-08 13:07:53.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.928272 PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5062 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.934270 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8093 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.942680 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     8243 2023-07-08 13:09:21.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     9369 2023-07-08 13:07:42.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-07-08 13:11:41.949763 PySideSix-Frameless-Window-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-07-08 13:08:36.000000 PySideSix-Frameless-Window-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.105693 PySideSix-Frameless-Window-0.1.2/
+-rw-rw-rw-   0        0        0     7815 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5542 2023-08-01 03:47:21.105693 PySideSix-Frameless-Window-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.070856 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5542 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4927 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.073021 PySideSix-Frameless-Window-0.1.2/qframelesswindow/
+-rw-rw-rw-   0        0        0     1614 2023-08-01 03:44:50.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.077719 PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.081891 PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     4320 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3147 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.085743 PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     4529 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4549 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.089379 PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5062 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.097688 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8093 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.103691 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     8379 2023-08-01 03:45:56.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9369 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:47:21.106694 PySideSix-Frameless-Window-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-08-01 03:44:44.000000 PySideSix-Frameless-Window-0.1.2/setup.py
```

### Comparing `PySideSix-Frameless-Window-0.1.1/LICENSE` & `PySideSix-Frameless-Window-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/PKG-INFO` & `PySideSix-Frameless-Window-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -128,7 +129,9 @@
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide6-Frameless-Window is licensed under [LGPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
+
```

### Comparing `PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/PKG-INFO` & `PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -128,7 +129,9 @@
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide6-Frameless-Window is licensed under [LGPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
+
```

### Comparing `PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/SOURCES.txt` & `PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/README.md` & `PySideSix-Frameless-Window-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/__init__.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 import sys
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,21 @@
             return False, 0
 
         if msg.message == win32con.WM_NCHITTEST and self._isResizeEnabled:
             pos = QCursor.pos()
             xPos = pos.x() - self.x()
             yPos = pos.y() - self.y()
             w, h = self.width(), self.height()
-            lx = xPos < self.BORDER_WIDTH
-            rx = xPos > w - self.BORDER_WIDTH
-            ty = yPos < self.BORDER_WIDTH
-            by = yPos > h - self.BORDER_WIDTH
+
+            # fixes https://github.com/zhiyiYo/PyQt-Frameless-Window/issues/98
+            bw = 0 if win_utils.isMaximized(msg.hWnd) or win_utils.isFullScreen(msg.hWnd) else self.BORDER_WIDTH
+            lx = xPos < bw
+            rx = xPos > w - bw
+            ty = yPos < bw
+            by = yPos > h - bw
             if lx and ty:
                 return True, win32con.HTTOPLEFT
             elif rx and by:
                 return True, win32con.HTBOTTOMRIGHT
             elif rx and ty:
                 return True, win32con.HTTOPRIGHT
             elif lx and by:
```

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py` & `PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.1/setup.py` & `PySideSix-Frameless-Window-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySideSix-Frameless-Window",
-    version="0.1.1",
+    version="0.1.2",
     keywords="pyside6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

