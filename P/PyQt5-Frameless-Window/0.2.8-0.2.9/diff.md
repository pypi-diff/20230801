# Comparing `tmp/PyQt5-Frameless-Window-0.2.8.tar.gz` & `tmp/PyQt5-Frameless-Window-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.8.tar", last modified: Sat Jul  8 13:06:26 2023, max compression
+gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.9.tar", last modified: Tue Aug  1 03:30:35 2023, max compression
```

## Comparing `PyQt5-Frameless-Window-0.2.8.tar` & `PyQt5-Frameless-Window-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/
--rw-rw-rw-   0        0        0    35823 2023-07-08 12:30:11.000000 PyQt5-Frameless-Window-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     5320 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.865163 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5320 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4750 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.867253 PyQt5-Frameless-Window-0.2.8/qframelesswindow/
--rw-rw-rw-   0        0        0     1679 2023-07-08 13:05:13.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.871000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.875613 PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2891 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3119 2023-07-08 13:00:28.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.880237 PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     2994 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4334 2023-07-08 13:00:17.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.885460 PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4984 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9057 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.893014 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8352 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6942 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4263 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8987 2023-07-08 12:59:48.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-07-08 13:03:03.000000 PyQt5-Frameless-Window-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.769915 PyQt5-Frameless-Window-0.2.9/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 13:18:44.000000 PyQt5-Frameless-Window-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     5932 2023-08-01 03:30:35.768914 PyQt5-Frameless-Window-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.731007 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5932 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5341 2023-08-01 03:27:51.000000 PyQt5-Frameless-Window-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.741038 PyQt5-Frameless-Window-0.2.9/qframelesswindow/
+-rw-rw-rw-   0        0        0     1679 2023-08-01 03:20:49.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.744632 PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.747135 PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2891 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3119 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.750756 PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     2994 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4334 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.754417 PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4984 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9057 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.761485 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.767915 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     7084 2023-08-01 03:18:28.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4263 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8987 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:30:35.769915 PyQt5-Frameless-Window-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-08-01 03:20:42.000000 PyQt5-Frameless-Window-0.2.9/setup.py
```

### Comparing `PyQt5-Frameless-Window-0.2.8/LICENSE` & `PyQt5-Frameless-Window-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/PKG-INFO` & `PyQt5-Frameless-Window-0.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.8
+Version: 0.2.9
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img width="15%" align="center" src="screenshot/logo.png" alt="logo">
+  <img width="15%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/logo.png" alt="logo">
 </p>
   <h1 align="center">
   PyQt-Frameless-Window
 </h1>
 <p align="center">
   A cross-platform frameless window based on PyQt5
 </p>
@@ -33,15 +34,15 @@
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 </p>
 
-![Cover](screenshot/cover.jpg)
+![Cover](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/cover.jpg)
 
 
 ## Features
 * Moving
 * Stretching
 * Window shadow
 * Window animation
@@ -90,29 +91,29 @@
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     demo = Window()
     demo.show()
     sys.exit(app.exec_())
 ```
-For more complex requirements, see [demo.py](./examples/demo.py) and [main_window.py](./examples/main_window.py).
+For more complex requirements, see [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) and [main_window.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/main_window.py).
 
 ## Examples
 * Normal frameless window
-![Normal Frameless Window](screenshot/normal_frameless_window.gif)
+![Normal Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/normal_frameless_window.gif)
 * Acrylic frameless window
-![Acrylic Frameless Window](screenshot/acrylic_window.jpg)
+![Acrylic Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/acrylic_window.jpg)
 
 
 ## Document
 Want to know more about PyQt-Frameless-Window? Please read the [help document](https://pyqt-frameless-window.readthedocs.io/) 👈
 
 
 ## Notes
-1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](./examples/demo.py) does.
+1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) does.
 
 2. Moving the acrylic window on Win10 may get stuck. At present, there is no good solution. Maybe you can disable the acrylic effect when moving the window, but I haven't done this in the source code.
 3. Snap layout is not enabled by default. See [#56](https://github.com/zhiyiYo/PyQt-Frameless-Window/issues/56) to learn how to enable it.
 
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
 
@@ -124,16 +125,18 @@
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
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
 PyQt-Frameless-Window is licensed under [GPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
```

### Comparing `PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/PKG-INFO` & `PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.8
+Version: 0.2.9
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img width="15%" align="center" src="screenshot/logo.png" alt="logo">
+  <img width="15%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/logo.png" alt="logo">
 </p>
   <h1 align="center">
   PyQt-Frameless-Window
 </h1>
 <p align="center">
   A cross-platform frameless window based on PyQt5
 </p>
@@ -33,15 +34,15 @@
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 </p>
 
-![Cover](screenshot/cover.jpg)
+![Cover](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/cover.jpg)
 
 
 ## Features
 * Moving
 * Stretching
 * Window shadow
 * Window animation
@@ -90,29 +91,29 @@
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     demo = Window()
     demo.show()
     sys.exit(app.exec_())
 ```
-For more complex requirements, see [demo.py](./examples/demo.py) and [main_window.py](./examples/main_window.py).
+For more complex requirements, see [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) and [main_window.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/main_window.py).
 
 ## Examples
 * Normal frameless window
-![Normal Frameless Window](screenshot/normal_frameless_window.gif)
+![Normal Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/normal_frameless_window.gif)
 * Acrylic frameless window
-![Acrylic Frameless Window](screenshot/acrylic_window.jpg)
+![Acrylic Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/acrylic_window.jpg)
 
 
 ## Document
 Want to know more about PyQt-Frameless-Window? Please read the [help document](https://pyqt-frameless-window.readthedocs.io/) 👈
 
 
 ## Notes
-1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](./examples/demo.py) does.
+1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) does.
 
 2. Moving the acrylic window on Win10 may get stuck. At present, there is no good solution. Maybe you can disable the acrylic effect when moving the window, but I haven't done this in the source code.
 3. Snap layout is not enabled by default. See [#56](https://github.com/zhiyiYo/PyQt-Frameless-Window/issues/56) to learn how to enable it.
 
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
 
@@ -124,16 +125,18 @@
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
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
 PyQt-Frameless-Window is licensed under [GPLv3](./LICENSE).
 
 Copyright © 2021 by zhiyiYo.
+
```

### Comparing `PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/SOURCES.txt` & `PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/README.md` & `PyQt5-Frameless-Window-0.2.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img width="15%" align="center" src="screenshot/logo.png" alt="logo">
+  <img width="15%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/logo.png" alt="logo">
 </p>
   <h1 align="center">
   PyQt-Frameless-Window
 </h1>
 <p align="center">
   A cross-platform frameless window based on PyQt5
 </p>
@@ -18,15 +18,15 @@
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 </p>
 
-![Cover](screenshot/cover.jpg)
+![Cover](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/cover.jpg)
 
 
 ## Features
 * Moving
 * Stretching
 * Window shadow
 * Window animation
@@ -75,29 +75,29 @@
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     demo = Window()
     demo.show()
     sys.exit(app.exec_())
 ```
-For more complex requirements, see [demo.py](./examples/demo.py) and [main_window.py](./examples/main_window.py).
+For more complex requirements, see [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) and [main_window.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/main_window.py).
 
 ## Examples
 * Normal frameless window
-![Normal Frameless Window](screenshot/normal_frameless_window.gif)
+![Normal Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/normal_frameless_window.gif)
 * Acrylic frameless window
-![Acrylic Frameless Window](screenshot/acrylic_window.jpg)
+![Acrylic Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/acrylic_window.jpg)
 
 
 ## Document
 Want to know more about PyQt-Frameless-Window? Please read the [help document](https://pyqt-frameless-window.readthedocs.io/) 👈
 
 
 ## Notes
-1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](./examples/demo.py) does.
+1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) does.
 
 2. Moving the acrylic window on Win10 may get stuck. At present, there is no good solution. Maybe you can disable the acrylic effect when moving the window, but I haven't done this in the source code.
 3. Snap layout is not enabled by default. See [#56](https://github.com/zhiyiYo/PyQt-Frameless-Window/issues/56) to learn how to enable it.
 
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
 
@@ -109,14 +109,15 @@
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
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
 PyQt-Frameless-Window is licensed under [GPLv3](./LICENSE).
```

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/__init__.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 import sys
 
 from PyQt5.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/resource.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/__init__.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/window_effect.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/__init__.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/window_effect.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/__init__.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/__init__.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/linux_utils.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/mac_utils.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/win32_utils.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/__init__.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,18 +75,21 @@
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
+            # fixes issue https://github.com/zhiyiYo/PyQt-Frameless-Window/issues/98
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

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/c_structures.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/window_effect.py` & `PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.8/setup.py` & `PyQt5-Frameless-Window-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt5-Frameless-Window",
-    version="0.2.8",
+    version="0.2.9",
     keywords="pyqt frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

