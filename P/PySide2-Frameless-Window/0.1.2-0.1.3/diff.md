# Comparing `tmp/PySide2-Frameless-Window-0.1.2.tar.gz` & `tmp/PySide2-Frameless-Window-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Frameless-Window-0.1.2.tar", last modified: Sat Jul  8 13:17:20 2023, max compression
+gzip compressed data, was "dist\PySide2-Frameless-Window-0.1.3.tar", last modified: Tue Aug  1 03:51:13 2023, max compression
```

## Comparing `PySide2-Frameless-Window-0.1.2.tar` & `PySide2-Frameless-Window-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.621784 PySide2-Frameless-Window-0.1.2/
--rw-rw-rw-   0        0        0     7815 2023-07-08 13:07:29.000000 PySide2-Frameless-Window-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5496 2023-07-08 13:17:20.619395 PySide2-Frameless-Window-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.574522 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5496 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4906 2023-07-08 13:12:31.000000 PySide2-Frameless-Window-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.581021 PySide2-Frameless-Window-0.1.2/qframelesswindow/
--rw-rw-rw-   0        0        0     2314 2023-07-08 13:15:23.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.582795 PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2730 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.591507 PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2878 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-07-08 13:13:12.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.595847 PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3024 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4314 2023-07-08 13:12:55.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.599358 PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4942 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.611234 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7973 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.617133 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     7078 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8810 2023-07-08 13:12:43.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-07-08 13:17:20.621784 PySide2-Frameless-Window-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-07-08 13:14:31.000000 PySide2-Frameless-Window-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.834451 PySide2-Frameless-Window-0.1.3/
+-rw-rw-rw-   0        0        0     7815 2023-08-01 03:44:09.000000 PySide2-Frameless-Window-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5649 2023-08-01 03:51:13.833439 PySide2-Frameless-Window-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.804192 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5649 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5036 2023-08-01 03:50:45.000000 PySide2-Frameless-Window-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.805435 PySide2-Frameless-Window-0.1.3/qframelesswindow/
+-rw-rw-rw-   0        0        0     2314 2023-08-01 03:49:25.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.808873 PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2730 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.812587 PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2878 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.816031 PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3024 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4314 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.819507 PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4942 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.825691 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     7973 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.830943 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     7214 2023-08-01 03:49:09.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4013 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8810 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:51:13.834451 PySide2-Frameless-Window-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-08-01 03:49:22.000000 PySide2-Frameless-Window-0.1.3/setup.py
```

### Comparing `PySide2-Frameless-Window-0.1.2/LICENSE` & `PySide2-Frameless-Window-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/PKG-INFO` & `PySide2-Frameless-Window-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.2
+Version: 0.1.3
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -119,16 +120,19 @@
 5. If you are using PyQt5, PyQt6 or PySide6, you can download the code in [PyQt5](https://github.com/zhiyiYo/PyQt-Frameless-Window) or [PyQt6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6) or [PySide6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6) branch.
 
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
+* [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://github.com/zhiyiYo/QMaterialWidgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide2-Frameless-Window is licensed under [LGPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
+
```

### Comparing `PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/PKG-INFO` & `PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.2
+Version: 0.1.3
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -119,16 +120,19 @@
 5. If you are using PyQt5, PyQt6 or PySide6, you can download the code in [PyQt5](https://github.com/zhiyiYo/PyQt-Frameless-Window) or [PyQt6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6) or [PySide6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6) branch.
 
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
+* [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://github.com/zhiyiYo/QMaterialWidgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide2-Frameless-Window is licensed under [LGPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
+
```

### Comparing `PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/SOURCES.txt` & `PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/README.md` & `PySide2-Frameless-Window-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 5. If you are using PyQt5, PyQt6 or PySide6, you can download the code in [PyQt5](https://github.com/zhiyiYo/PyQt-Frameless-Window) or [PyQt6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6) or [PySide6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6) branch.
 
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
+* [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://github.com/zhiyiYo/QMaterialWidgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide2-Frameless-Window is licensed under [LGPLv3](./LICENSE).
```

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/__init__.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 import sys
 
 from PySide2.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,21 @@
             return super().nativeEvent(eventType, message)
 
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

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py` & `PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.2/setup.py` & `PySide2-Frameless-Window-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Frameless-Window",
-    version="0.1.2",
+    version="0.1.3",
     keywords="pyside2 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

