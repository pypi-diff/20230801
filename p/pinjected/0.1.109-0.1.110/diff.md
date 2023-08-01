# Comparing `tmp/pinjected-0.1.109.tar.gz` & `tmp/pinjected-0.1.110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.1.109.tar", max compression
+gzip compressed data, was "pinjected-0.1.110.tar", max compression
```

## Comparing `pinjected-0.1.109.tar` & `pinjected-0.1.110.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.1.109/LICENSE
--rw-r--r--   0        0        0      407 2023-08-01 10:55:32.734086 pinjected-0.1.109/pinjected/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.1.109/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.1.109/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     2522 2023-08-01 10:55:32.770639 pinjected-0.1.109/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      635 2023-08-01 10:55:32.714575 pinjected-0.1.109/pinjected/di/applicative.py
--rw-r--r--   0        0        0     6656 2023-08-01 10:55:32.760069 pinjected-0.1.109/pinjected/di/ast.py
--rw-r--r--   0        0        0     1145 2023-08-01 10:55:32.707779 pinjected-0.1.109/pinjected/di/bindings.py
--rw-r--r--   0        0        0     1009 2023-08-01 10:55:32.748920 pinjected-0.1.109/pinjected/di/design.py
--rw-r--r--   0        0        0     1918 2023-08-01 10:55:32.712483 pinjected-0.1.109/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.1.109/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    21758 2023-08-01 10:55:32.754770 pinjected-0.1.109/pinjected/di/graph.py
--rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinjected-0.1.109/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    32975 2023-08-01 10:55:32.744821 pinjected-0.1.109/pinjected/di/injected.py
--rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinjected-0.1.109/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0     2931 2023-08-01 10:55:32.737082 pinjected-0.1.109/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinjected-0.1.109/pinjected/di/permissioned/__init__.py
--rw-r--r--   0        0        0     7805 2023-08-01 10:55:32.728581 pinjected-0.1.109/pinjected/di/permissioned/blueprint.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.1.109/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.1.109/pinjected/di/provider.py
--rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinjected-0.1.109/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.1.109/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.1.109/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6169 2023-08-01 10:55:32.723083 pinjected-0.1.109/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.1.109/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      980 2023-08-01 10:55:32.724965 pinjected-0.1.109/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2023-08-01 10:55:32.752600 pinjected-0.1.109/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2239 2023-08-01 10:55:32.766231 pinjected-0.1.109/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      690 2023-08-01 10:55:32.735563 pinjected-0.1.109/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0    18907 2023-08-01 10:55:32.742623 pinjected-0.1.109/pinjected/di/util.py
--rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinjected-0.1.109/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinjected-0.1.109/pinjected/global_configs
--rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinjected-0.1.109/pinjected/global_configs.py
--rw-r--r--   0        0        0     2725 2023-08-01 10:55:32.769019 pinjected-0.1.109/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     1733 2023-08-01 10:55:32.719258 pinjected-0.1.109/pinjected/helper_structure.py
--rw-r--r--   0        0        0     7941 2023-08-01 10:55:32.763721 pinjected-0.1.109/pinjected/helpers.py
--rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinjected-0.1.109/pinjected/module_inspector.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.1.109/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0    23588 2023-08-01 10:55:32.721408 pinjected-0.1.109/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1580 2023-08-01 10:55:32.732359 pinjected-0.1.109/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0      928 2023-08-01 10:55:32.750717 pinjected-0.1.109/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.1.109/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      370 2023-08-01 10:55:32.730320 pinjected-0.1.109/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0    18619 2023-08-01 10:55:32.710604 pinjected-0.1.109/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.1.109/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       73 2023-08-01 10:55:32.761801 pinjected-0.1.109/pinjected/viz/graph.py
--rw-r--r--   0        0        0      699 2023-08-01 10:56:59.666862 pinjected-0.1.109/pyproject.toml
--rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 pinjected-0.1.109/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.1.110/LICENSE
+-rw-r--r--   0        0        0      407 2023-08-01 10:55:32.734086 pinjected-0.1.110/pinjected/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.1.110/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.1.110/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     2522 2023-08-01 10:55:32.770639 pinjected-0.1.110/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      635 2023-08-01 10:55:32.714575 pinjected-0.1.110/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     6641 2023-08-01 10:58:43.087334 pinjected-0.1.110/pinjected/di/ast.py
+-rw-r--r--   0        0        0     1145 2023-08-01 10:55:32.707779 pinjected-0.1.110/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     1009 2023-08-01 10:55:32.748920 pinjected-0.1.110/pinjected/di/design.py
+-rw-r--r--   0        0        0     1918 2023-08-01 10:55:32.712483 pinjected-0.1.110/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.1.110/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    21758 2023-08-01 10:55:32.754770 pinjected-0.1.110/pinjected/di/graph.py
+-rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinjected-0.1.110/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    32965 2023-08-01 10:58:43.085630 pinjected-0.1.110/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinjected-0.1.110/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0     2931 2023-08-01 10:55:32.737082 pinjected-0.1.110/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinjected-0.1.110/pinjected/di/permissioned/__init__.py
+-rw-r--r--   0        0        0     7805 2023-08-01 10:55:32.728581 pinjected-0.1.110/pinjected/di/permissioned/blueprint.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.1.110/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.1.110/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinjected-0.1.110/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.1.110/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.1.110/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6169 2023-08-01 10:55:32.723083 pinjected-0.1.110/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.1.110/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      980 2023-08-01 10:55:32.724965 pinjected-0.1.110/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1500 2023-08-01 10:55:32.752600 pinjected-0.1.110/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2239 2023-08-01 10:55:32.766231 pinjected-0.1.110/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      690 2023-08-01 10:55:32.735563 pinjected-0.1.110/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0    18907 2023-08-01 10:55:32.742623 pinjected-0.1.110/pinjected/di/util.py
+-rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinjected-0.1.110/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinjected-0.1.110/pinjected/global_configs
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.1.110/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2725 2023-08-01 10:55:32.769019 pinjected-0.1.110/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     1733 2023-08-01 10:55:32.719258 pinjected-0.1.110/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     7936 2023-08-01 10:58:43.088847 pinjected-0.1.110/pinjected/helpers.py
+-rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinjected-0.1.110/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.1.110/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0    23563 2023-08-01 10:58:43.077925 pinjected-0.1.110/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1580 2023-08-01 10:55:32.732359 pinjected-0.1.110/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0      928 2023-08-01 10:55:32.750717 pinjected-0.1.110/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.1.110/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      365 2023-08-01 10:58:43.080069 pinjected-0.1.110/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0    18619 2023-08-01 10:55:32.710604 pinjected-0.1.110/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.1.110/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       73 2023-08-01 10:55:32.761801 pinjected-0.1.110/pinjected/viz/graph.py
+-rw-r--r--   0        0        0      694 2023-08-01 11:01:03.613382 pinjected-0.1.110/pyproject.toml
+-rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 pinjected-0.1.110/PKG-INFO
```

### Comparing `pinjected-0.1.109/LICENSE` & `pinjected-0.1.110/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/app_designed.py` & `pinjected-0.1.110/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/app_injected.py` & `pinjected-0.1.110/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/applicative.py` & `pinjected-0.1.110/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/ast.py` & `pinjected-0.1.110/pinjected/di/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Generic, Tuple, Dict, Any, Callable, Optional, TypeVar
 
 from frozendict import frozendict
 
 from pinjected.di.injected_analysis import get_instance_origin
-from pinjected.global_configs import PINJECT_DESIGN_TRACK_ORIGIN
+from pinjected.global_configs import pinjected_TRACK_ORIGIN
 
 T = TypeVar("T")
 
 
 class Expr(Generic[T], ABC):
     """
     I want to know where this instance is instantiated
     """
 
     def __post_init__(self):
         # this takes time so... we need to toggle it
-        if PINJECT_DESIGN_TRACK_ORIGIN:
-            self.origin_frame = get_instance_origin('pinject_design')
+        if pinjected_TRACK_ORIGIN:
+            self.origin_frame = get_instance_origin('pinjected')
         else:
             self.origin_frame = None
 
     def __getattr__(self, item: str):
         return Attr(self, item)
 
     def _wrap_if_non_expr(self, item) -> "Expr":
```

### Comparing `pinjected-0.1.109/pinjected/di/bindings.py` & `pinjected-0.1.110/pinjected/di/bindings.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/design.py` & `pinjected-0.1.110/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/designed.py` & `pinjected-0.1.110/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/dynamic_proxy.py` & `pinjected-0.1.110/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/graph.py` & `pinjected-0.1.110/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/injected.py` & `pinjected-0.1.110/pinjected/di/injected.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,16 +602,16 @@
     # since the behavior differs in classes extending Generic[T]
     __match_args__ = ("target_function", "kwargs_mapping")
 
     def __init__(self,
                  target_function: Callable,
                  kwargs_mapping: Dict[str, Union[str, type, Callable, Injected, DelegatedVar]]
                  ):
-        # I think we need to know where this class is instantiated outside of pinject_design_package
-        self.origin_frame = get_instance_origin("pinject_design")
+        # I think we need to know where this class is instantiated outside of pinjected_package
+        self.origin_frame = get_instance_origin("pinjected")
         super().__init__()
         assert not isinstance(target_function, (Injected, DelegatedVar))
         assert callable(target_function)
         self.target_function = target_function
         self.kwargs_mapping = copy(kwargs_mapping)
         for k, v in self.kwargs_mapping.items():
             assert v is not None, f"injected got None binding for key:{k}"
```

### Comparing `pinjected-0.1.109/pinjected/di/injected_analysis.py` & `pinjected-0.1.110/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/modular_injected.py` & `pinjected-0.1.110/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/permissioned/blueprint.py` & `pinjected-0.1.110/pinjected/di/permissioned/blueprint.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/proxiable.py` & `pinjected-0.1.110/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/session.py` & `pinjected-0.1.110/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/sessioned.py` & `pinjected-0.1.110/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/static_proxy.py` & `pinjected-0.1.110/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.1.110/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/test_graph.py` & `pinjected-0.1.110/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/test_injected.py` & `pinjected-0.1.110/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/test_proxiable.py` & `pinjected-0.1.110/pinjected/di/test_proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/di/util.py` & `pinjected-0.1.110/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/exceptions.py` & `pinjected-0.1.110/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/graph_inspection.py` & `pinjected-0.1.110/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/helper_structure.py` & `pinjected-0.1.110/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/helpers.py` & `pinjected-0.1.110/pinjected/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # then return a ModulePath
         raise NotImplementedError
 
 
 @dataclass
 class RunnableSpec:
     tgt_path: ModulePath
-    design_path: ModulePath = field(default_factory=lambda:ModulePath("pinject_design.di.util.EmptyDesign"))
+    design_path: ModulePath = field(default_factory=lambda:ModulePath("pinjected.di.util.EmptyDesign"))
 
     @property
     def target_name(self):
         return self.tgt_path.var_name
 
     @property
     def design_name(self):
```

### Comparing `pinjected-0.1.109/pinjected/module_inspector.py` & `pinjected-0.1.110/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/nx_graph_util.py` & `pinjected-0.1.110/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/run_config_utils.py` & `pinjected-0.1.110/pinjected/run_config_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 import loguru
 import returns.maybe as raybe
 from cytoolz import memoize
 from expression import Nothing
 from returns.maybe import Maybe, Some, maybe
 from returns.result import safe, Success, Failure
 
-import pinject_design.global_configs
+import pinjected.global_configs
 from pinjected import Injected, Design
 from pinjected.di.injected import injected_function
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.di.util import instances, providers
 from pinjected.helper_structure import IdeaRunConfigurations, RunnablePair, RunnableValue, \
     IdeaRunConfiguration
 from pinjected.helpers import inspect_and_make_configurations, load_variable_by_module_path, \
@@ -386,26 +386,26 @@
         module_path,
         default_design_path=None,
         entrypoint_path=None,
         interpreter_path=None,
         working_dir=None,
         print_to_stdout=True,
 ):
-    pinject_design.global_configs.PINJECT_DESIGN_TRACK_ORIGIN = False
+    pinjected.global_configs.pinjected_TRACK_ORIGIN = False
     args = ConfigCreationArgs(
         module_path=module_path,
         default_design_path=default_design_path,
         entrypoint_path=entrypoint_path,
         interpreter_path=interpreter_path,
         working_dir=working_dir,
     )
     design = args.to_design()
     g = design.to_graph()
     configs: IdeaRunConfigurations = g[inspect_and_make_configurations(module_path)]
-    pinject_design.global_configs.PINJECT_DESIGN_TRACK_ORIGIN = True
+    pinjected.global_configs.pinjected_TRACK_ORIGIN = True
     logger.info(f"configs:{configs}")
     if print_to_stdout:
         print(configs.model_dump_json())
     else:
         return configs
```

### Comparing `pinjected-0.1.109/pinjected/run_config_utils_v2.py` & `pinjected-0.1.110/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/test_package/__init__.py` & `pinjected-0.1.110/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pinjected/visualize_di.py` & `pinjected-0.1.110/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.109/pyproject.toml` & `pinjected-0.1.110/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.1.109"
+version = "0.1.110"
 description = "immutable wrapper for pinject"
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "^0.21.0"
@@ -22,11 +22,11 @@
 pydantic = "^2.1.1"
 networkx = "^3.1"
 pyvis = "^0.3.2"
 makefun = "^1.15.1"
 loguru = "^0.7.0"
 
 [tool.poetry.scripts]
-pinject_design_config = "pinject_design.run_config_utils:main"
+pinject_design_config = "pinjected.run_config_utils:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
```

### Comparing `pinjected-0.1.109/PKG-INFO` & `pinjected-0.1.110/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.1.109
+Version: 0.1.110
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

