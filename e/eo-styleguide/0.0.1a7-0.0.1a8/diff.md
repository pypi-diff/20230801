# Comparing `tmp/eo_styleguide-0.0.1a7.tar.gz` & `tmp/eo_styleguide-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo_styleguide-0.0.1a7.tar", max compression
+gzip compressed data, was "eo_styleguide-0.0.1a8.tar", max compression
```

## Comparing `eo_styleguide-0.0.1a7.tar` & `eo_styleguide-0.0.1a8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3421 2023-07-29 14:37:37.987684 eo_styleguide-0.0.1a7/README.md
--rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a7/pyeo/__init__.py
--rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a7/pyeo/features/__init__.py
--rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a7/pyeo/features/feature.py
--rw-r--r--   0        0        0     1620 2023-07-29 22:13:02.772938 eo_styleguide-0.0.1a7/pyeo/features/final_object.py
--rw-r--r--   0        0        0     2811 2023-07-31 18:09:02.876772 eo_styleguide-0.0.1a7/pyeo/features/method_has_protocol.py
--rw-r--r--   0        0        0     2881 2023-07-29 22:13:02.773905 eo_styleguide-0.0.1a7/pyeo/features/no_code_in_ctors.py
--rw-r--r--   0        0        0     2046 2023-07-30 18:28:11.179784 eo_styleguide-0.0.1a7/pyeo/features/no_er_names.py
--rw-r--r--   0        0        0     1715 2023-07-29 22:13:02.774156 eo_styleguide-0.0.1a7/pyeo/features/no_property_methods.py
--rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a7/pyeo/features/no_reflection.py
--rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a7/pyeo/features/no_setters.py
--rw-r--r--   0        0        0     1794 2023-07-29 22:13:02.774412 eo_styleguide-0.0.1a7/pyeo/features/no_staticmethods.py
--rw-r--r--   0        0        0     1768 2023-07-31 18:09:17.461854 eo_styleguide-0.0.1a7/pyeo/features/object_has_protocol.py
--rw-r--r--   0        0        0     2128 2023-07-29 22:13:02.774645 eo_styleguide-0.0.1a7/pyeo/features/protocol_method_code_free.py
--rw-r--r--   0        0        0     3344 2023-07-31 18:09:39.535138 eo_styleguide-0.0.1a7/pyeo/main.py
--rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a7/pyeo/py.typed
--rw-r--r--   0        0        0        0 2023-07-29 22:13:02.774933 eo_styleguide-0.0.1a7/pyeo/utils/__init__.py
--rw-r--r--   0        0        0      268 2023-07-29 22:13:02.775282 eo_styleguide-0.0.1a7/pyeo/utils/decorator_name.py
--rw-r--r--   0        0        0      813 2023-07-31 18:10:25.678006 eo_styleguide-0.0.1a7/pyproject.toml
--rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a7/PKG-INFO
+-rw-r--r--   0        0        0     3421 2023-07-29 14:37:37.987684 eo_styleguide-0.0.1a8/README.md
+-rw-r--r--   0        0        0     1290 2023-08-01 13:26:02.937035 eo_styleguide-0.0.1a8/pyeo/__init__.py
+-rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a8/pyeo/features/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a8/pyeo/features/feature.py
+-rw-r--r--   0        0        0     1700 2023-08-01 13:26:02.937385 eo_styleguide-0.0.1a8/pyeo/features/final_object.py
+-rw-r--r--   0        0        0     3086 2023-08-01 13:26:02.937680 eo_styleguide-0.0.1a8/pyeo/features/method_has_protocol.py
+-rw-r--r--   0        0        0     3186 2023-08-01 13:26:02.937919 eo_styleguide-0.0.1a8/pyeo/features/no_code_in_ctors.py
+-rw-r--r--   0        0        0     2046 2023-07-30 18:28:11.179784 eo_styleguide-0.0.1a8/pyeo/features/no_er_names.py
+-rw-r--r--   0        0        0     1715 2023-07-29 22:13:02.774156 eo_styleguide-0.0.1a8/pyeo/features/no_property_methods.py
+-rw-r--r--   0        0        0     2491 2023-08-01 13:26:02.938148 eo_styleguide-0.0.1a8/pyeo/features/no_reflection.py
+-rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a8/pyeo/features/no_setters.py
+-rw-r--r--   0        0        0     1848 2023-08-01 13:26:02.938423 eo_styleguide-0.0.1a8/pyeo/features/no_staticmethods.py
+-rw-r--r--   0        0        0     1768 2023-07-31 18:09:17.461854 eo_styleguide-0.0.1a8/pyeo/features/object_has_protocol.py
+-rw-r--r--   0        0        0     2155 2023-08-01 13:26:02.938687 eo_styleguide-0.0.1a8/pyeo/features/protocol_method_code_free.py
+-rw-r--r--   0        0        0     3344 2023-08-01 12:29:38.522301 eo_styleguide-0.0.1a8/pyeo/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a8/pyeo/py.typed
+-rw-r--r--   0        0        0     1118 2023-08-01 13:26:02.938971 eo_styleguide-0.0.1a8/pyeo/utils/__init__.py
+-rw-r--r--   0        0        0     1459 2023-08-01 13:26:02.939196 eo_styleguide-0.0.1a8/pyeo/utils/decorator_name.py
+-rw-r--r--   0        0        0      813 2023-08-01 13:26:47.356083 eo_styleguide-0.0.1a8/pyproject.toml
+-rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a8/PKG-INFO
```

### Comparing `eo_styleguide-0.0.1a7/README.md` & `eo_styleguide-0.0.1a8/README.md`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyeo/__init__.py` & `eo_styleguide-0.0.1a8/pyeo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
-def elegant(class_):
+def elegant(eo_class):
     """Decorator for elegant objects and protocols.
 
-    :param class_: decorated class
-    :return class_: decorated class
+    :param eo_class: decorated class
+    :return: decorated class
     """
-    return class_
+    return eo_class
```

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/__init__.py` & `eo_styleguide-0.0.1a8/pyeo/features/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/feature.py` & `eo_styleguide-0.0.1a8/pyeo/features/feature.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/final_object.py` & `eo_styleguide-0.0.1a8/pyeo/features/final_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,11 +28,14 @@
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
-        if 'typing.final' not in {decorator.fullname for decorator in ctx.cls.decorators if isinstance(decorator, NameExpr)}:
+        if 'typing.final' not in self._decorator_names(ctx):
             ctx.api.fail("Class '{0}' must be final.".format(ctx.cls.name), ctx.cls)
             return False
         return True
+
+    def _decorator_names(self, ctx):
+        return {decorator.fullname for decorator in ctx.cls.decorators if isinstance(decorator, NameExpr)}
```

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/method_has_protocol.py` & `eo_styleguide-0.0.1a8/pyeo/features/method_has_protocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,25 +31,19 @@
 
         :param ctx: mypy context
         :return: bool
         """
         object_methods = {
             def_body.name: def_body
             for def_body in ctx.cls.defs.body
-            if isinstance(def_body, FuncDef) and not def_body.name.startswith('_') and not self._method_is_ctor(def_body)
+            if self._is_public_method(def_body)
         }
         if not ctx.cls.base_type_exprs:
             return False
-        extra_method_names = set(object_methods.keys()) - {  # noqa: WPS224 need a refactor
-            method
-            for base_type in ctx.cls.base_type_exprs
-            for node in base_type.node.mro
-            if hasattr(node.defn.info, 'names')
-            for method in node.defn.info.names
-        }
+        extra_method_names = object_methods.keys() - self._protocol_method_names(ctx.cls.base_type_exprs)
         if extra_method_names:
             failed_methods = [
                 method
                 for method_name, method in object_methods.items()
                 if method_name in extra_method_names
             ]
             for method in failed_methods:
@@ -58,14 +52,28 @@
                         ctx.cls.name,
                         method.name,
                     ),
                     method,
                 )
         return True
 
+    def _protocol_method_names(self, base_type_exprs):
+        res = []
+        for base_type in base_type_exprs:
+            for node in base_type.node.mro:
+                if not hasattr(node.defn.info, 'names'):
+                    continue
+                for method in node.defn.info.names:
+                    res.append(method)
+        return res
+
+    def _is_public_method(self, def_body):
+        is_func_def = isinstance(def_body, FuncDef)
+        return is_func_def and not def_body.name.startswith('_') and not self._method_is_ctor(def_body)
+
     def _method_is_ctor(self, def_body) -> bool:
         if not isinstance(def_body, Decorator):
             return False
         for dec in def_body.original_decorators:
             if dec.name == 'classmethod':
                 return True
         return False
```

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/no_code_in_ctors.py` & `eo_styleguide-0.0.1a8/pyeo/features/no_code_in_ctors.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,37 +16,41 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from mypy.nodes import AssignmentStmt, Block, Decorator, FuncDef, NameExpr, PassStmt, ReturnStmt
+from mypy.nodes import AssignmentStmt, Decorator, ExpressionStmt, FuncDef, PassStmt, ReturnStmt, StrExpr
 
 from pyeo.utils.decorator_name import decorator_name
 
 
 class NoCodeInCtorFeature(object):
     """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for func in ctx.cls.defs.body:
-            if isinstance(func, Decorator) and 'classmethod' in {decorator_name(dec) for dec in func.original_decorators}:
+            if self._is_secondary_ctor(func):
                 self._secondary_ctor_check(ctx, func)
             elif not isinstance(func, FuncDef):
                 continue
             elif func.name == '__init__':
                 self._primary_ctor_check(ctx, func)
         return True
 
+    def _is_secondary_ctor(self, func):
+        is_decorator = isinstance(func, Decorator)
+        return is_decorator and 'classmethod' in {decorator_name(dec) for dec in func.original_decorators}
+
     def _secondary_ctor_check(self, ctx, func):
         for elem in func.func.body.body:
             # TODO: ReturnStmt can contain logic like list comprehension
             # we must iter by nodes of expr and check all elements
             #
             # @classmethod
             # def secondary_ctor(cls, ages: list[str]):
@@ -55,16 +59,20 @@
             #     )
             if not isinstance(elem, ReturnStmt):
                 ctx.api.fail(
                     'Find code in ctor {0}.{1}.'.format(ctx.cls.name, func.name),
                     ctx.cls,
                 )
 
+    def _allowed_exprs(self, expr):
+        is_pass = isinstance(expr, PassStmt)
+        return is_pass or isinstance(expr, ExpressionStmt) and isinstance(expr.expr, StrExpr)
+
     def _primary_ctor_check(self, ctx, func):
         for elem in func.body.body:
-            if isinstance(elem, PassStmt):
+            if self._allowed_exprs(elem):
                 continue
             if not isinstance(elem, AssignmentStmt):
                 ctx.api.fail(
                     'Find code in ctor {0}.{1}.'.format(ctx.cls.name, func.name),
                     ctx.cls,
                 )
```

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/no_er_names.py` & `eo_styleguide-0.0.1a8/pyeo/features/no_er_names.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/no_property_methods.py` & `eo_styleguide-0.0.1a8/pyeo/features/no_property_methods.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/no_reflection.py` & `eo_styleguide-0.0.1a8/pyeo/features/no_reflection.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,51 +16,53 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from pprint import pprint
-
-from mypy.nodes import Block, CallExpr
+from mypy.nodes import CallExpr
 
 
 class NoReflectionFeature(object):
     """Checking each object method has protocol."""
 
+    _forbid_func_names = (
+        'builtins.isinstance',
+        'builtins.type',
+        'builtins.issubclass',
+        'builtins.hasattr',
+    )
+
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for elem in ctx.cls.defs.body:
             self._walk_expressions(ctx, elem)
         return True
 
     def _walk_expressions(self, ctx, expr):
-        forbid_func_names = (
-            'builtins.isinstance',
-            'builtins.type',
-            'builtins.issubclass',
-            'builtins.hasattr',
-        )
         if hasattr(expr, 'body'):
             self._walk_expressions(ctx, expr.body)
         if isinstance(expr, list):
             for elem in expr:
                 self._walk_expressions(ctx, elem)
         if hasattr(expr, 'expr'):
             self._walk_expressions(ctx, expr.expr)
         if isinstance(expr, CallExpr):
-            if expr.callee.fullname in forbid_func_names:
-                ctx.api.fail(
-                    "Class '{0}' has '{1}' reflection function call.".format(
-                        ctx.cls.name,
-                        expr.callee.fullname,
-                    ),
-                    ctx.cls,
-                )
-            if hasattr(expr, 'args'):
-                for elem in expr.args:
-                    self._walk_expressions(ctx, elem)
+            self._is_bad_expr(ctx, expr)
+
+    def _is_bad_expr(self, ctx, expr):
+        if expr.callee.fullname in self._forbid_func_names:
+            ctx.api.fail(
+                "Class '{0}' has '{1}' reflection function call.".format(
+                    ctx.cls.name,
+                    expr.callee.fullname,
+                ),
+                ctx.cls,
+            )
+        if hasattr(expr, 'args'):
+            for expr_arg in expr.args:
+                self._walk_expressions(ctx, expr_arg)
```

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/no_setters.py` & `eo_styleguide-0.0.1a8/pyeo/features/no_setters.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/no_staticmethods.py` & `eo_styleguide-0.0.1a8/pyeo/features/no_staticmethods.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,28 +16,31 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from mypy.nodes import AssignmentStmt, Decorator, ReturnStmt
+from mypy.nodes import Decorator
 
 from pyeo.utils.decorator_name import decorator_name
 
 
 class NoStaticmethodsFeature(object):
     """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for func in ctx.cls.defs.body:
-            if isinstance(func, Decorator) and 'staticmethod' in {decorator_name(dec) for dec in func.original_decorators}:
+            if isinstance(func, Decorator) and 'staticmethod' in self._decorator_names(func):
                 ctx.api.fail(
                     'Find staticmethod {0}.{1}.'.format(ctx.cls.name, func.name),
                     ctx.cls,
                 )
         return True
+
+    def _decorator_names(self, func):
+        return {decorator_name(dec) for dec in func.original_decorators}
```

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/object_has_protocol.py` & `eo_styleguide-0.0.1a8/pyeo/features/object_has_protocol.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyeo/features/protocol_method_code_free.py` & `eo_styleguide-0.0.1a8/pyeo/features/protocol_method_code_free.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from mypy.nodes import AssignmentStmt, EllipsisExpr, ExpressionStmt, FuncDef, PassStmt, StrExpr
+from mypy.nodes import EllipsisExpr, FuncDef, PassStmt, StrExpr
 
 
 class ProtocolMethodCodeFreeFeature(object):
     """Check protocol methods code free."""
 
     def analyze(self, ctx) -> bool:  # noqa: WPS231 need in refactor
         """Analyzing.
@@ -32,15 +32,18 @@
         :param ctx: mypy context
         :return: bool
         """
         for method in ctx.cls.defs.body:
             if not isinstance(method, FuncDef):
                 continue
             for body_item in method.body.body:
-                fail_args = ("Protocol '{0}' method '{1}' has implementation".format(ctx.cls.name, method.name), ctx.cls)
+                fail_args = (
+                    "Protocol '{0}' method '{1}' has implementation".format(ctx.cls.name, method.name),
+                    ctx.cls,
+                )
                 if isinstance(body_item, PassStmt):
                     continue
                 if not hasattr(body_item, 'expr'):  # noqa: WPS421 need in refactor
                     ctx.api.fail(*fail_args)
                     continue
                 if not isinstance(body_item.expr, (EllipsisExpr, StrExpr)):
                     ctx.api.fail(*fail_args)
```

### Comparing `eo_styleguide-0.0.1a7/pyeo/main.py` & `eo_styleguide-0.0.1a8/pyeo/main.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a7/pyproject.toml` & `eo_styleguide-0.0.1a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "eo-styleguide"
 packages = [
     {include = "pyeo"}
 ]
-version = "0.0.1-alpha7"
+version = "0.0.1-alpha8"
 description = "Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability."
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `eo_styleguide-0.0.1a7/PKG-INFO` & `eo_styleguide-0.0.1a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-styleguide
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability.
 License: MIT
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

