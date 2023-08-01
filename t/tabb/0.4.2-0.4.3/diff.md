# Comparing `tmp/tabb-0.4.2.tar.gz` & `tmp/tabb-0.4.3.tar.gz`

## Comparing `tabb-0.4.2.tar` & `tabb-0.4.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.2/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.4.2/config.json
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 tabb-0.4.2/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.4.2/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.4.2/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.2/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/__about__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/__init__.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/config.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/context.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/decorators.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/formatter.py
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/missing.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/nargs.py
--rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/py.typed
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/types.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/utils.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    32341 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.4.2/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.4.2/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.4.2/README.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.3/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.4.3/config.json
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 tabb-0.4.3/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.4.3/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.4.3/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.3/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/__about__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/config.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/context.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/missing.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/py.typed
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/types.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/utils.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    32341 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.4.3/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.4.3/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.4.3/PKG-INFO
```

### Comparing `tabb-0.4.2/.DS_Store` & `tabb-0.4.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/test.py` & `tabb-0.4.3/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,19 @@
     def decorator(fn: Callable[P, T]) -> Callable[P, T]:
         register_callback(fn, update_config, localns=localns)
         return fn
 
     return decorator
 
 
+breakpoint()
+
+
 @group()
-@load_json_config()
+# @load_json_config()
 def cli(foo: bool | None = None) -> None:
     print(f"{foo=}")
 
 
 @cli.command
 def cp(
     src: Annotated[
```

### Comparing `tabb-0.4.2/src/.DS_Store` & `tabb-0.4.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/__init__.py` & `tabb-0.4.3/src/tabb/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/base.py` & `tabb-0.4.3/src/tabb/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/callback.py` & `tabb-0.4.3/src/tabb/callback.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/command.py` & `tabb-0.4.3/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/config.py` & `tabb-0.4.3/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/context.py` & `tabb-0.4.3/src/tabb/context.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/decorators.py` & `tabb-0.4.3/src/tabb/decorators.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/exceptions.py` & `tabb-0.4.3/src/tabb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/formatter.py` & `tabb-0.4.3/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/group.py` & `tabb-0.4.3/src/tabb/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/nargs.py` & `tabb-0.4.3/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parser.py` & `tabb-0.4.3/src/tabb/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/types.py` & `tabb-0.4.3/src/tabb/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/utils.py` & `tabb-0.4.3/src/tabb/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parameter/__init__.py` & `tabb-0.4.3/src/tabb/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parameter/base.py` & `tabb-0.4.3/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parameter/depends.py` & `tabb-0.4.3/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parameter/group.py` & `tabb-0.4.3/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parameter/parser.py` & `tabb-0.4.3/src/tabb/parameter/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parameter/resolve.py` & `tabb-0.4.3/src/tabb/parameter/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,35 +137,42 @@
 def _resolve_unknown(
     name: str,
     signature: inspect.Parameter,
     type_hint: object,
     annotations: list[object],
     is_optional: bool,
 ) -> Parameter[Any]:
+    param: ArgumentParameter[Any] | OptionParameter[Any]
+
     if typing.get_origin(type_hint) is Context:
         return _get_depends(name, signature, Depends(get_context))
 
     try:
         if (
             signature.kind in (signature.VAR_POSITIONAL, signature.VAR_KEYWORD)
             or signature.default is not signature.empty
         ):
-            return _resolve_option(
+            param = _resolve_option(
                 name, signature, type_hint, annotations, Option(), is_optional
             )
-
-        return _resolve_argument(
-            name, signature, type_hint, annotations, Argument(), is_optional
-        )
+        else:
+            param = _resolve_argument(
+                name, signature, type_hint, annotations, Argument(), is_optional
+            )
 
     except TypeError:
         if not callable(type_hint):
             raise
         return _get_depends(name, signature, Depends(type_hint))
 
+    if signature.default is not signature.empty:
+        param.default = signature.default
+
+    return param
+
 
 def _get_depends(
     name: str,
     signature: inspect.Parameter,
     options: Depends[Any],
 ) -> DependsParameter[Any]:
     _, kind = _resolve_parameter_kind(signature, AnyType())
```

### Comparing `tabb-0.4.2/src/tabb/parameter/types.py` & `tabb-0.4.3/src/tabb/parameter/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/src/tabb/parameter/utils.py` & `tabb-0.4.3/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/.gitignore` & `tabb-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/LICENSE.txt` & `tabb-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/README.md` & `tabb-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/pyproject.toml` & `tabb-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabb-0.4.2/PKG-INFO` & `tabb-0.4.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.4.2
+Version: 0.4.3
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

