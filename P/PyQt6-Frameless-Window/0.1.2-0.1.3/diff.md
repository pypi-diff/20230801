# Comparing `tmp/PyQt6-Frameless-Window-0.1.2.tar.gz` & `tmp/PyQt6-Frameless-Window-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Frameless-Window-0.1.2.tar", last modified: Sat Jul  8 13:24:26 2023, max compression
+gzip compressed data, was "dist\PyQt6-Frameless-Window-0.1.3.tar", last modified: Tue Aug  1 03:43:45 2023, max compression
```

## Comparing `PyQt6-Frameless-Window-0.1.2.tar` & `PyQt6-Frameless-Window-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/
--rw-rw-rw-   0        0        0    35823 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5582 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.625336 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5582 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5007 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.638633 PyQt6-Frameless-Window-0.1.2/qframelesswindow/
--rw-rw-rw-   0        0        0     1678 2023-07-08 13:23:07.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.643174 PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.647615 PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     3110 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3149 2023-07-08 13:19:21.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.649625 PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3015 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4563 2023-07-08 13:19:46.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.658001 PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5083 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9205 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.666179 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0      644 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8352 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6624 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     9413 2023-07-08 13:18:53.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-07-08 13:20:08.000000 PyQt6-Frameless-Window-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.924931 PyQt6-Frameless-Window-0.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5603 2023-08-01 03:43:45.923741 PyQt6-Frameless-Window-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.886735 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5603 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5007 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.897214 PyQt6-Frameless-Window-0.1.3/qframelesswindow/
+-rw-rw-rw-   0        0        0     1678 2023-08-01 03:42:22.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.900316 PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.903414 PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     3110 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3149 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.906507 PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3015 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4563 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.909841 PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5083 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9205 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.916234 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.921299 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6760 2023-08-01 03:34:35.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9413 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:43:45.924931 PyQt6-Frameless-Window-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-08-01 03:42:26.000000 PyQt6-Frameless-Window-0.1.3/setup.py
```

### Comparing `PyQt6-Frameless-Window-0.1.2/LICENSE` & `PyQt6-Frameless-Window-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/PKG-INFO` & `PyQt6-Frameless-Window-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.2
+Version: 0.1.3
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -128,7 +129,8 @@
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PyQt6-Frameless-Window is licensed under [GPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
```

### Comparing `PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/PKG-INFO` & `PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.2
+Version: 0.1.3
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -128,7 +129,8 @@
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PyQt6-Frameless-Window is licensed under [GPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
```

### Comparing `PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/SOURCES.txt` & `PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/README.md` & `PyQt6-Frameless-Window-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/__init__.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 import sys
 
 from PyQt6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,18 +74,21 @@
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

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py` & `PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.2/setup.py` & `PyQt6-Frameless-Window-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Frameless-Window",
-    version="0.1.2",
+    version="0.1.3",
     keywords="pyqt6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

