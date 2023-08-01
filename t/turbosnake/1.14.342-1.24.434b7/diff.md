# Comparing `tmp/turbosnake-1.14.342.tar.gz` & `tmp/turbosnake-1.24.434b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\code\py3-1111\dist\tmpeceh7brq\turbosnake-1.14.342.tar", last modified: Mon Feb 21 17:48:13 2022, max compression
+gzip compressed data, was "turbosnake-1.24.434b7.tar", last modified: Tue Aug  1 08:12:07 2023, max compression
```

## Comparing `turbosnake-1.14.342.tar` & `turbosnake-1.24.434b7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-02-21 17:48:13.431900 turbosnake-1.14.342/
--rw-rw-rw-   0        0        0     1095 2021-09-10 12:31:06.000000 turbosnake-1.14.342/LICENCE
--rw-rw-rw-   0        0        0     5472 2022-02-21 17:48:13.430904 turbosnake-1.14.342/PKG-INFO
--rw-rw-rw-   0        0        0     4682 2021-10-29 11:28:47.000000 turbosnake-1.14.342/README.md
--rw-rw-rw-   0        0        0       42 2022-02-21 17:48:13.431900 turbosnake-1.14.342/setup.cfg
--rw-rw-rw-   0        0        0     1050 2022-02-20 19:14:59.000000 turbosnake-1.14.342/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-21 17:48:13.259650 turbosnake-1.14.342/turbosnake/
--rw-rw-rw-   0        0        0      850 2022-02-19 13:27:01.000000 turbosnake-1.14.342/turbosnake/__init__.py
--rw-rw-rw-   0        0        0     5655 2022-02-20 15:47:40.000000 turbosnake-1.14.342/turbosnake/_async.py
--rw-rw-rw-   0        0        0    18341 2022-02-20 15:36:24.000000 turbosnake-1.14.342/turbosnake/_components.py
--rw-rw-rw-   0        0        0     3496 2021-10-21 12:54:45.000000 turbosnake-1.14.342/turbosnake/_context.py
--rw-rw-rw-   0        0        0     3183 2021-10-21 11:44:14.000000 turbosnake-1.14.342/turbosnake/_functional_component.py
--rw-rw-rw-   0        0        0    11875 2021-11-02 13:29:06.000000 turbosnake-1.14.342/turbosnake/_hooks.py
--rw-rw-rw-   0        0        0     1021 2021-09-09 20:18:41.000000 turbosnake-1.14.342/turbosnake/_render_context.py
--rw-rw-rw-   0        0        0     3717 2021-11-02 13:53:18.000000 turbosnake-1.14.342/turbosnake/_slotted_component.py
--rw-rw-rw-   0        0        0     2910 2021-11-01 12:00:37.000000 turbosnake-1.14.342/turbosnake/_utils.py
--rw-rw-rw-   0        0        0     1529 2022-02-20 15:24:42.000000 turbosnake-1.14.342/turbosnake/_utils0.py
-drwxrwxrwx   0        0        0        0 2022-02-21 17:48:13.286765 turbosnake-1.14.342/turbosnake/test_helpers/
--rw-rw-rw-   0        0        0       51 2021-09-09 20:11:59.000000 turbosnake-1.14.342/turbosnake/test_helpers/__init__.py
--rw-rw-rw-   0        0        0     3589 2021-10-21 11:54:08.000000 turbosnake-1.14.342/turbosnake/test_helpers/_selectors.py
--rw-rw-rw-   0        0        0     3015 2022-02-20 15:27:46.000000 turbosnake-1.14.342/turbosnake/test_helpers/_test_helpers.py
-drwxrwxrwx   0        0        0        0 2022-02-21 17:48:13.418442 turbosnake-1.14.342/turbosnake/ttk/
--rw-rw-rw-   0        0        0      517 2022-01-27 16:27:11.000000 turbosnake-1.14.342/turbosnake/ttk/__init__.py
--rw-rw-rw-   0        0        0     7521 2022-01-27 15:48:04.000000 turbosnake-1.14.342/turbosnake/ttk/_adapters.py
--rw-rw-rw-   0        0        0     3670 2022-01-27 16:27:11.000000 turbosnake-1.14.342/turbosnake/ttk/_composite.py
--rw-rw-rw-   0        0        0     6708 2022-02-20 15:24:42.000000 turbosnake-1.14.342/turbosnake/ttk/_core.py
--rw-rw-rw-   0        0        0     7925 2021-11-02 13:54:25.000000 turbosnake-1.14.342/turbosnake/ttk/_layout.py
--rw-rw-rw-   0        0        0     6865 2021-10-01 15:09:56.000000 turbosnake-1.14.342/turbosnake/ttk/_menu.py
--rw-rw-rw-   0        0        0    12386 2022-02-12 14:46:51.000000 turbosnake-1.14.342/turbosnake/ttk/_style.py
--rw-rw-rw-   0        0        0     1625 2021-09-19 14:36:15.000000 turbosnake-1.14.342/turbosnake/ttk/_utils.py
-drwxrwxrwx   0        0        0        0 2022-02-21 17:48:13.282616 turbosnake-1.14.342/turbosnake.egg-info/
--rw-rw-rw-   0        0        0     5472 2022-02-21 17:48:12.000000 turbosnake-1.14.342/turbosnake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2022-02-21 17:48:13.000000 turbosnake-1.14.342/turbosnake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-21 17:48:12.000000 turbosnake-1.14.342/turbosnake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-02-21 17:48:13.000000 turbosnake-1.14.342/turbosnake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.229843 turbosnake-1.24.434b7/
+-rw-rw-rw-   0        0        0     1095 2021-09-10 12:31:06.000000 turbosnake-1.24.434b7/LICENCE
+-rw-rw-rw-   0        0        0     5452 2023-08-01 08:12:07.228843 turbosnake-1.24.434b7/PKG-INFO
+-rw-rw-rw-   0        0        0     4682 2021-10-29 11:28:47.000000 turbosnake-1.24.434b7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:12:07.229843 turbosnake-1.24.434b7/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-08-01 08:07:06.000000 turbosnake-1.24.434b7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.204293 turbosnake-1.24.434b7/turbosnake/
+-rw-rw-rw-   0        0        0      850 2022-02-19 13:27:01.000000 turbosnake-1.24.434b7/turbosnake/__init__.py
+-rw-rw-rw-   0        0        0     5655 2022-02-20 15:47:40.000000 turbosnake-1.24.434b7/turbosnake/_async.py
+-rw-rw-rw-   0        0        0    18341 2023-08-01 05:59:14.000000 turbosnake-1.24.434b7/turbosnake/_components.py
+-rw-rw-rw-   0        0        0     3496 2021-10-21 12:54:45.000000 turbosnake-1.24.434b7/turbosnake/_context.py
+-rw-rw-rw-   0        0        0     3159 2023-08-01 05:59:30.000000 turbosnake-1.24.434b7/turbosnake/_functional_component.py
+-rw-rw-rw-   0        0        0    11875 2021-11-02 13:29:06.000000 turbosnake-1.24.434b7/turbosnake/_hooks.py
+-rw-rw-rw-   0        0        0     1021 2021-09-09 20:18:41.000000 turbosnake-1.24.434b7/turbosnake/_render_context.py
+-rw-rw-rw-   0        0        0     3717 2021-11-02 13:53:18.000000 turbosnake-1.24.434b7/turbosnake/_slotted_component.py
+-rw-rw-rw-   0        0        0     2910 2021-11-01 12:00:37.000000 turbosnake-1.24.434b7/turbosnake/_utils.py
+-rw-rw-rw-   0        0        0     1529 2022-02-20 15:24:42.000000 turbosnake-1.24.434b7/turbosnake/_utils0.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.217873 turbosnake-1.24.434b7/turbosnake/test_helpers/
+-rw-rw-rw-   0        0        0       51 2021-09-09 20:11:59.000000 turbosnake-1.24.434b7/turbosnake/test_helpers/__init__.py
+-rw-rw-rw-   0        0        0     3589 2021-10-21 11:54:08.000000 turbosnake-1.24.434b7/turbosnake/test_helpers/_selectors.py
+-rw-rw-rw-   0        0        0     3015 2022-02-20 15:27:46.000000 turbosnake-1.24.434b7/turbosnake/test_helpers/_test_helpers.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.227847 turbosnake-1.24.434b7/turbosnake/ttk/
+-rw-rw-rw-   0        0        0      517 2022-01-27 16:27:11.000000 turbosnake-1.24.434b7/turbosnake/ttk/__init__.py
+-rw-rw-rw-   0        0        0     7521 2022-01-27 15:48:04.000000 turbosnake-1.24.434b7/turbosnake/ttk/_adapters.py
+-rw-rw-rw-   0        0        0     3670 2022-01-27 16:27:11.000000 turbosnake-1.24.434b7/turbosnake/ttk/_composite.py
+-rw-rw-rw-   0        0        0     6748 2023-08-01 06:03:31.000000 turbosnake-1.24.434b7/turbosnake/ttk/_core.py
+-rw-rw-rw-   0        0        0     7925 2021-11-02 13:54:25.000000 turbosnake-1.24.434b7/turbosnake/ttk/_layout.py
+-rw-rw-rw-   0        0        0     6841 2023-08-01 06:00:17.000000 turbosnake-1.24.434b7/turbosnake/ttk/_menu.py
+-rw-rw-rw-   0        0        0    12386 2022-02-12 14:46:51.000000 turbosnake-1.24.434b7/turbosnake/ttk/_style.py
+-rw-rw-rw-   0        0        0     1618 2023-08-01 06:06:46.000000 turbosnake-1.24.434b7/turbosnake/ttk/_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.214913 turbosnake-1.24.434b7/turbosnake.egg-info/
+-rw-rw-rw-   0        0        0     5452 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/top_level.txt
```

### Comparing `turbosnake-1.14.342/LICENCE` & `turbosnake-1.24.434b7/LICENCE`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/PKG-INFO` & `turbosnake-1.24.434b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: turbosnake
-Version: 1.14.342
+Version: 1.24.434b7
 Summary: React.js-like framework with components for native user interfaces
 Home-page: https://github.com/AlexeyBond/turbosnake
 Author: Alexey Bondarenko
 Author-email: alexey.bond.94.55+turbosnake@gmail.com
 License: MIT
 Keywords: ui,reactive,tkinter
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/AlexeyBond/turbosnake/workflows/Tests/badge.svg)](https://github.com/AlexeyBond/turbosnake/actions?query=workflow%3ATests)
 [![Coverage Status](https://coveralls.io/repos/github/AlexeyBond/turbosnake/badge.svg?branch=master)](https://coveralls.io/github/AlexeyBond/turbosnake?branch=master)
@@ -157,9 +156,7 @@
 Storybook. The tool tracks changes in component file and renders the most recent version in a window.
 
 Current version of preview tool tracks changes only in the preview file itself. Tracking of changes in dependencies may
 be added later.
 
 See [preview_example.py](https://github.com/AlexeyBond/turbosnake/blob/master/examples/preview_example.py) for example
 of preview tool use.
-
-
```

### Comparing `turbosnake-1.14.342/README.md` & `turbosnake-1.24.434b7/README.md`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/setup.py` & `turbosnake-1.24.434b7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open("README.md", encoding="utf-8") as fp:
     long_description = fp.read()
 
 setup(
     name='turbosnake',
-    version='1.14.342',
+    version='1.24.434-beta7',
     packages=['turbosnake', 'turbosnake.ttk', 'turbosnake.test_helpers'],
     url='https://github.com/AlexeyBond/turbosnake',
     author='Alexey Bondarenko',
     author_email='alexey.bond.94.55+turbosnake@gmail.com',
     description='React.js-like framework with components for native user interfaces',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -17,12 +17,12 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: Unix',
         'Operating System :: MacOS',
-        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: User Interfaces',
     ],
     license='MIT',
 )
```

### Comparing `turbosnake-1.14.342/turbosnake/__init__.py` & `turbosnake-1.24.434b7/turbosnake/__init__.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/_async.py` & `turbosnake-1.24.434b7/turbosnake/_async.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/_components.py` & `turbosnake-1.24.434b7/turbosnake/_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import queue
 from abc import abstractmethod, ABCMeta
-from collections import OrderedDict, Counter, Iterable
+from collections import OrderedDict, Counter
 from functools import wraps
-from typing import Optional, Type, Union, Callable
+from typing import Optional, Type, Union, Callable, Iterable
 
 from ._render_context import get_render_context, render_context_manager, enter_render_context
 from ._utils0 import have_differences_by_keys
 
 
 class Ref:
     def __init__(self):
```

### Comparing `turbosnake-1.14.342/turbosnake/_context.py` & `turbosnake-1.24.434b7/turbosnake/_context.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/_functional_component.py` & `turbosnake-1.24.434b7/turbosnake/_functional_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import inspect
-from collections import Iterable
 from functools import update_wrapper
-from typing import Optional, Union
+from typing import Optional, Union, Iterable
 
 from ._components import Component, ParentComponent, DynamicComponent, component_inserter
 from ._hooks import ComponentWithHooks
 from ._slotted_component import PropSlotsComponent
 
 
 def functional_component(
```

### Comparing `turbosnake-1.14.342/turbosnake/_hooks.py` & `turbosnake-1.24.434b7/turbosnake/_hooks.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/_render_context.py` & `turbosnake-1.24.434b7/turbosnake/_render_context.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/_slotted_component.py` & `turbosnake-1.24.434b7/turbosnake/_slotted_component.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/_utils.py` & `turbosnake-1.24.434b7/turbosnake/_utils.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/_utils0.py` & `turbosnake-1.24.434b7/turbosnake/_utils0.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/test_helpers/_selectors.py` & `turbosnake-1.24.434b7/turbosnake/test_helpers/_selectors.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/test_helpers/_test_helpers.py` & `turbosnake-1.24.434b7/turbosnake/test_helpers/_test_helpers.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/ttk/__init__.py` & `turbosnake-1.24.434b7/turbosnake/ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/ttk/_adapters.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_adapters.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/ttk/_composite.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_composite.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/ttk/_core.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import asyncio
 import sys
 import tkinter as tk
 import traceback
 from abc import abstractmethod, ABCMeta, ABC
-from collections import Generator
 from functools import cache
 from tkinter.ttk import Style
-from typing import Optional
+from typing import Optional, Generator
 
 from turbosnake import Component, Tree
 from turbosnake._utils0 import create_daemon_event_loop
 from turbosnake.ttk._layout import get_layout_manager_class, DEFAULT_LAYOUT_MANAGER, LayoutManagerABC
 
 """
 _core.py
@@ -40,15 +39,15 @@
     def on_tk_child_updated(self, child):
         ...
 
     def on_tk_child_unmounted(self, child):
         ...
 
     @abstractmethod
-    def get_tk_children(self) -> Generator['TkComponent']:
+    def get_tk_children(self) -> Generator['TkComponent', None, None]:
         ...
 
 
 class TkContainerBase(TkBase, ABC):
     def init_container(self, layout_manager=DEFAULT_LAYOUT_MANAGER, **kwargs):
         self._layout_manager: LayoutManagerABC = get_layout_manager_class(layout_manager)(
             container=self,
@@ -79,15 +78,15 @@
         self._layout_manager.on_child_updated(child)
 
     def on_tk_child_unmounted(self, child):
         super().on_tk_child_unmounted(child)
         self._layout_manager.on_child_removed(child)
 
 
-def _get_tk_children(component: Component):
+def _get_tk_children(component: Component) -> Generator['TkComponent', None, None]:
     for child in component.first_matching_descendants(TkComponent.__instancecheck__):
         if not child.tk_ignore_subtree:
             yield child
 
 
 def configure_window(
         widget,
@@ -197,15 +196,15 @@
 
         del self.tk_parent
         del self.__widget
 
     def get_tk_parent(self) -> TkBase:
         return self.first_matching_ascendant(TkBase.__instancecheck__)
 
-    def get_tk_children(self) -> Generator['TkComponent']:
+    def get_tk_children(self) -> Generator['TkComponent', None, None]:
         return _get_tk_children(self)
 
     def _create_and_configure_widget(self):
         if self.__widget:
             self.__widget.destroy()
 
         widget = self.create_widget(self.tk_parent.widget)
```

### Comparing `turbosnake-1.14.342/turbosnake/ttk/_layout.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_layout.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/ttk/_menu.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import tkinter as tk
 from abc import abstractmethod, ABCMeta, ABC
-from collections import Iterable
-from typing import Optional, Callable, Any
+from typing import Optional, Callable, Any, Iterable
 
 from ._adapters import TkRadioGroup
 from ._core import TkComponent
 from .. import Component, Wrapper, event_prop_invoker, component, noop_handler
 
 """
 _menu.py
```

### Comparing `turbosnake-1.14.342/turbosnake/ttk/_style.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_style.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.14.342/turbosnake/ttk/_utils.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import tkinter as tk
-from collections import Iterable
+from typing import Mapping
 
 from turbosnake import event_prop_invoker
 from ._core import TkComponent, TkTree
 
 
 def tk_app(widget=None, **options):
     """Shortcut function that creates TkTree, renders it's content and starts main loop.
@@ -24,15 +24,15 @@
             tree.__exit__(exc_type, exc_val, exc_tb)
 
             tree.main_loop()
 
     return _App()
 
 
-def tk_with_events(event_map: Iterable[str, str]):
+def tk_with_events(event_map: Mapping[str, str]):
     """Decorator for tk-component that invokes event handlers from it's props when tk's events happen.
 
     @tk_with_events({
         '<<Button-1>>': 'on_mouse_down',
     })
     class MyComponent(TkComponent):
         ...
```

### Comparing `turbosnake-1.14.342/turbosnake.egg-info/PKG-INFO` & `turbosnake-1.24.434b7/turbosnake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: turbosnake
-Version: 1.14.342
+Version: 1.24.434b7
 Summary: React.js-like framework with components for native user interfaces
 Home-page: https://github.com/AlexeyBond/turbosnake
 Author: Alexey Bondarenko
 Author-email: alexey.bond.94.55+turbosnake@gmail.com
 License: MIT
 Keywords: ui,reactive,tkinter
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/AlexeyBond/turbosnake/workflows/Tests/badge.svg)](https://github.com/AlexeyBond/turbosnake/actions?query=workflow%3ATests)
 [![Coverage Status](https://coveralls.io/repos/github/AlexeyBond/turbosnake/badge.svg?branch=master)](https://coveralls.io/github/AlexeyBond/turbosnake?branch=master)
@@ -157,9 +156,7 @@
 Storybook. The tool tracks changes in component file and renders the most recent version in a window.
 
 Current version of preview tool tracks changes only in the preview file itself. Tracking of changes in dependencies may
 be added later.
 
 See [preview_example.py](https://github.com/AlexeyBond/turbosnake/blob/master/examples/preview_example.py) for example
 of preview tool use.
-
-
```

### Comparing `turbosnake-1.14.342/turbosnake.egg-info/SOURCES.txt` & `turbosnake-1.24.434b7/turbosnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

