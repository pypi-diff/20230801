# Comparing `tmp/tabb-0.3.3.tar.gz` & `tmp/tabb-0.4.2.tar.gz`

## Comparing `tabb-0.3.3.tar` & `tabb-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.3/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.3.3/config.json
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.3.3/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.3.3/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.3.3/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.3/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/__about__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/__init__.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/config.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/context.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/decorators.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/formatter.py
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/missing.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/nargs.py
--rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/py.typed
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/types.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/utils.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    32315 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.3.3/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.3.3/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.3.3/README.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.2/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.4.2/config.json
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 tabb-0.4.2/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.4.2/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.4.2/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.2/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/__about__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/config.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/context.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/missing.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/py.typed
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/types.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/utils.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    32341 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.4.2/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.4.2/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.4.2/PKG-INFO
```

### Comparing `tabb-0.3.3/.DS_Store` & `tabb-0.4.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/test.py` & `tabb-0.4.2/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,18 @@
     name: str | None = None
     email: Annotated[str | None, Depends(get_email)] = None
 
 
 @cli.command
 def test_depends(
     ctx: Context[None],
+    user: User,
     home: Annotated[str | None, Depends(get_home)],
     email: Annotated[str | None, Depends(get_email)],
     hod: Annotated[str, Depends(higher_order_dep)],
-    user: Annotated[User, Depends(User)],
 ) -> None:
     print(f"{ctx=} {home=} {email=} {hod=} {user=}")
 
 
 @cli.command
 def hello(
     name: Annotated[str, Argument(default="World")],
```

### Comparing `tabb-0.3.3/src/.DS_Store` & `tabb-0.4.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/__init__.py` & `tabb-0.4.2/src/tabb/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/base.py` & `tabb-0.4.2/src/tabb/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/callback.py` & `tabb-0.4.2/src/tabb/callback.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/command.py` & `tabb-0.4.2/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/config.py` & `tabb-0.4.2/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/context.py` & `tabb-0.4.2/src/tabb/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 @overload
 def get_current_context(silent: bool = ...) -> Context[Any] | None:
     ...
 
 
 def get_current_context(silent: bool = False) -> Context[Any] | None:
     try:
-        return cast("Context", _local.stack[-1])
+        return cast(Context[Any], _local.stack[-1])
     except (AttributeError, IndexError) as error:
         if not silent:
             raise RuntimeError("There is no active click context.") from error
 
     return None
```

### Comparing `tabb-0.3.3/src/tabb/decorators.py` & `tabb-0.4.2/src/tabb/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,20 @@
     short_help: str | None = None,
 ) -> Callable[[Callable[..., Any]], Group[Any]]:
     ...
 
 
 def group(
     name: Callable[..., Any] | str | None = None,
+    *args: Any,
     **kwargs: Any,
 ) -> Group[Any] | Callable[[Callable[..., Any]], Group[Any]]:
     if callable(name):
         return Group(name)
 
     def decorator(callback: Callable[..., Any]) -> Group[Any]:
         if isinstance(callback, Group):
             raise TypeError("Attempted to convert a callback into a group twice.")
 
-        return Group(callback, name=name, **kwargs)
+        return Group(callback, *args, name=name, **kwargs)
 
     return decorator
```

### Comparing `tabb-0.3.3/src/tabb/exceptions.py` & `tabb-0.4.2/src/tabb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/formatter.py` & `tabb-0.4.2/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/group.py` & `tabb-0.4.2/src/tabb/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,12 +245,11 @@
                 msg += f" Did you mean {possibilities[0]!r}?"
             elif possibilities:
                 options = ", ".join(sorted(possibilities))
                 msg += f" (Possible options: {options})"
 
             ctx.fail(msg)
 
-
         sub_ctx = command.make_context(command_name, args, ctx.environ, ctx.config, ctx)
 
         with sub_ctx:
             return command.invoke(sub_ctx)
```

### Comparing `tabb-0.3.3/src/tabb/nargs.py` & `tabb-0.4.2/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/parser.py` & `tabb-0.4.2/src/tabb/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/types.py` & `tabb-0.4.2/src/tabb/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/utils.py` & `tabb-0.4.2/src/tabb/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from functools import update_wrapper
 from shlex import shlex
 from types import ModuleType
 from typing import Any, ParamSpec, TextIO, TypeVar, cast
 
 P = ParamSpec("P")
 R = TypeVar("R")
-D = TypeVar("D")
 
 
 def to_kebab(name: str) -> str:
     return name.translate(str.maketrans("_ ", "--"))
 
 
 def to_snake(name: str) -> str:
@@ -94,19 +93,18 @@
     resulting from ``.flush()`` being called on a broken pipe.
     """
     return cast(TextIO, PacifyFlushWrapper(file))
 
 
 def safecall(
     fn: Callable[P, R],
-    default: D = None,
     exceptions: tuple[type[BaseException], ...] = (Exception,),
-) -> Callable[P, R | D]:
+) -> Callable[P, R | None]:
     "Wraps a function so that it swallows exceptions."
 
-    def wrapper(*args: P.args, **kwargs: P.kwargs) -> R | D:
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> R | None:
         try:
             return fn(*args, **kwargs)
         except exceptions:
-            return default
+            return None
 
     return update_wrapper(wrapper, fn)
```

### Comparing `tabb-0.3.3/src/tabb/parameter/__init__.py` & `tabb-0.4.2/src/tabb/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/parameter/base.py` & `tabb-0.4.2/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/parameter/depends.py` & `tabb-0.4.2/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/parameter/group.py` & `tabb-0.4.2/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/parameter/parser.py` & `tabb-0.4.2/src/tabb/parameter/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/src/tabb/parameter/resolve.py` & `tabb-0.4.2/src/tabb/parameter/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import inspect
 import pathlib
 import typing
 from collections.abc import Callable
-from typing import Any
+from typing import Any, cast
 
 from tabb.context import Context
 from tabb.missing import _MISSING_TYPE, MISSING
 from tabb.nargs import NArgs, NArgsLiteral
 from tabb.parameter.base import Parameter, ParameterKind
 from tabb.parameter.depends import DependsParameter
 from tabb.parameter.parser import ArgumentParameter, OptionParameter
@@ -42,14 +42,15 @@
     Choices,
     Depends,
     Greedy,
     Length,
     Matches,
     Option,
     Range,
+    Secret,
     Validate,
 )
 from tabb.utils import to_kebab
 
 
 def get_context(ctx: Context[Any]) -> Context[Any]:
     return ctx
@@ -76,29 +77,32 @@
     name: str, signature: inspect.Parameter, type_hint: object
 ) -> Parameter[Any]:
     param: Parameter[Any]
 
     # Arguments with a default of None are automatically made optional
     is_optional, type_hint = get_optional_child_type(type_hint)
     type_hint, annotations = get_annotations(type_hint)
-    options = _resolve_options(signature, type_hint, annotations)
+    options = _resolve_options(annotations)
 
-    if isinstance(options, Argument):
+    if options is None:
+        return _resolve_unknown(name, signature, type_hint, annotations, is_optional)
+
+    if isinstance(options, Depends):
+        return _get_depends(name, signature, options)
+
+    elif isinstance(options, Argument):
         param = _resolve_argument(
             name, signature, type_hint, annotations, options, is_optional
         )
 
     elif isinstance(options, Option):
         param = _resolve_option(
             name, signature, type_hint, annotations, options, is_optional
         )
 
-    elif isinstance(options, Depends):
-        return _get_depends(name, signature, options)
-
     else:
         msg = f"Unexpected options type: {options!r}."
         raise TypeError(msg)
 
     if options.default is not MISSING:
         param.default = options.default
 
@@ -126,14 +130,52 @@
 
     if not isinstance(options.metavar, _MISSING_TYPE):
         param.metavar = options.metavar
 
     return param
 
 
+def _resolve_unknown(
+    name: str,
+    signature: inspect.Parameter,
+    type_hint: object,
+    annotations: list[object],
+    is_optional: bool,
+) -> Parameter[Any]:
+    if typing.get_origin(type_hint) is Context:
+        return _get_depends(name, signature, Depends(get_context))
+
+    try:
+        if (
+            signature.kind in (signature.VAR_POSITIONAL, signature.VAR_KEYWORD)
+            or signature.default is not signature.empty
+        ):
+            return _resolve_option(
+                name, signature, type_hint, annotations, Option(), is_optional
+            )
+
+        return _resolve_argument(
+            name, signature, type_hint, annotations, Argument(), is_optional
+        )
+
+    except TypeError:
+        if not callable(type_hint):
+            raise
+        return _get_depends(name, signature, Depends(type_hint))
+
+
+def _get_depends(
+    name: str,
+    signature: inspect.Parameter,
+    options: Depends[Any],
+) -> DependsParameter[Any]:
+    _, kind = _resolve_parameter_kind(signature, AnyType())
+    return DependsParameter(name, kind, options.dependency, use_cache=options.use_cache)
+
+
 def _resolve_argument(
     name: str,
     signature: inspect.Parameter,
     type_hint: object,
     annotations: list[object],
     options: Argument[Any],
     is_optional: bool,
@@ -166,23 +208,14 @@
 
     if not isinstance(options.show_envvar, _MISSING_TYPE):
         option.show_envvar = options.show_envvar
 
     return option
 
 
-def _get_depends(
-    name: str,
-    signature: inspect.Parameter,
-    options: Depends[Any],
-) -> DependsParameter[Any]:
-    _, kind = _resolve_parameter_kind(signature, AnyType())
-    return DependsParameter(name, kind, options.dependency, use_cache=options.use_cache)
-
-
 def _get_argument_type(
     type_hint: object,
     options: Argument[Any],
     is_optional: bool = False,
 ) -> ParameterType[Any]:
     if not isinstance(options.type, _MISSING_TYPE):
         return options.type
@@ -212,22 +245,15 @@
         child_type = _get_argument_type(literal_type, options)
         return ChoicesValidator(child_type, choices)
 
     # Handle bool aruments
     if type_hint is bool:
         return Bool()
 
-    if (result := _resolve_special_types(type_hint)) is not None:
-        return result
-
-    if callable(type_hint):
-        return Scalar(type_hint)
-
-    msg = f"Unexpted type: {type_hint!r}."
-    raise TypeError(msg)
+    return _resolve_type(type_hint)
 
 
 def _resolve_option_type(
     type_hint: object,
     options: Option[Any],
     is_optional: bool = False,
 ) -> ParameterType[Any]:
@@ -259,22 +285,15 @@
         child_type = _resolve_option_type(literal_type, options)
         return ChoicesValidator(child_type, choices)
 
     # Bool options become flags
     if type_hint is bool:
         return Flag()
 
-    if (result := _resolve_special_types(type_hint)) is not None:
-        return result
-
-    if callable(type_hint):
-        return Scalar(type_hint)
-
-    msg = f"Unexpted type: {type_hint!r}."
-    raise TypeError(msg)
+    return _resolve_type(type_hint)
 
 
 def _resolve_parameter_kind(
     signature: inspect.Parameter,
     parameter_type: ParameterType[Any],
     nargs: NArgs | NArgsLiteral | None = None,
 ) -> tuple[ParameterType[Any], ParameterKind]:
@@ -291,27 +310,29 @@
 
     if signature.kind == signature.POSITIONAL_ONLY:
         return parameter_type, ParameterKind.POSITIONAL
 
     if signature.kind == signature.POSITIONAL_OR_KEYWORD:
         return parameter_type, ParameterKind.POSITIONAL_OR_KEYWORD
 
-    msg = f"Unexpted parameter kind: {signature.kind!r}."
+    msg = f"Unexpected parameter kind: {signature.kind!r}."
     raise TypeError(msg)
 
 
-def _resolve_special_types(
-    type_hint: object,
-) -> ParameterType[Any] | None:
+def _resolve_type(type_hint: object) -> ParameterType[Any]:
     base_type = get_base_type(type_hint)
 
     if base_type is pathlib.Path:
         return Path()
 
-    return None
+    if issubclass(base_type, str | bytes | int | float | Secret):
+        return Scalar(cast(Callable[[str], Any], type_hint))
+
+    msg = f"Unexpected type: {type_hint!r}."
+    raise TypeError(msg)
 
 
 def _resolve_validators(
     type_hint: object,
     annotations: list[object],
     parameter_type: ParameterType[Any],
 ) -> ParameterType[Any]:
@@ -320,22 +341,22 @@
             parameter_type = LengthValidator(
                 type=parameter_type,
                 min_length=annotation.min,
                 max_length=annotation.max,
             )
 
         elif isinstance(annotation, Range):
-            cast = get_base_type(type_hint)
-            if cast not in (int, float):
-                msg = f"Cannot use min/max with type {cast!r}."
+            base_type = get_base_type(type_hint)
+            if base_type not in (int, float):
+                msg = f"Cannot use min/max with type {base_type!r}."
                 raise TypeError(msg)
 
             parameter_type = RangeValidator(
                 type=parameter_type,
-                cast=cast,
+                cast=base_type,
                 min=annotation.min,
                 max=annotation.max,
                 min_open=annotation.min_open,
                 max_open=annotation.max_open,
                 clamp=annotation.clamp,
             )
 
@@ -357,23 +378,14 @@
         elif isinstance(annotation, Validate):
             parameter_type = Validator(parameter_type, annotation.validator)
 
     return parameter_type
 
 
 def _resolve_options(
-    signature: inspect.Parameter, type_hint: object, annotations: list[object]
-) -> Argument[Any] | Option[Any] | Depends[Any]:
+    annotations: list[object],
+) -> Argument[Any] | Option[Any] | Depends[Any] | None:
     for annotation in annotations:
         if isinstance(annotation, (Argument | Option | Depends)):
             return annotation
 
-    if typing.get_origin(type_hint) is Context:
-        return Depends(get_context)
-
-    if (
-        signature.kind in (signature.VAR_POSITIONAL, signature.VAR_KEYWORD)
-        or signature.default is not signature.empty
-    ):
-        return Option()
-
-    return Argument()
+    return None
```

### Comparing `tabb-0.3.3/src/tabb/parameter/types.py` & `tabb-0.4.2/src/tabb/parameter/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,20 +758,22 @@
         if self.executable and not os.access(value, os.X_OK):
             self.fail("Path must be executable.")
 
         return True
 
 
 class File(ParameterType[IO[Any]]):
+    _Path: TypeAlias = str | bytes | PathLike[str] | PathLike[bytes]
+
     def __init__(
         self,
         mode: str = "r",
         encoding: str = "utf-8",
         errors: str = "strict",
-        default: int | str | bytes | PathLike[str] | PathLike[bytes] | None = None,
+        default: _Path | None = None,
         allow_overwrite: bool = True,
         close: bool | None = None,
     ) -> None:
         super().__init__()
         self.mode = mode
         self.encoding = encoding
         self.errors = errors
@@ -794,15 +796,15 @@
 
     def has_default(self) -> bool:
         return self.default is not None
 
     def matches(self, arg: ParameterArg) -> bool:
         return arg.value is not None
 
-    def open(self, value: str | None) -> IO[Any]:
+    def open(self, value: _Path | None) -> IO[Any]:
         if value is None:
             self.fail("File path cannot be None.")
 
         if os.fsdecode(value) == "-":
             if any(m in self.mode for m in ["w", "a", "x"]):
                 if "b" in self.mode:
                     return sys.stdout.buffer
```

### Comparing `tabb-0.3.3/src/tabb/parameter/utils.py` & `tabb-0.4.2/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/.gitignore` & `tabb-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/LICENSE.txt` & `tabb-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/README.md` & `tabb-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/pyproject.toml` & `tabb-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabb-0.3.3/PKG-INFO` & `tabb-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.3.3
+Version: 0.4.2
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

