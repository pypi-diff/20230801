# Comparing `tmp/tabb-0.4.5.tar.gz` & `tmp/tabb-0.4.6.tar.gz`

## Comparing `tabb-0.4.5.tar` & `tabb-0.4.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.5/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.4.5/config.json
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 tabb-0.4.5/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.4.5/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.4.5/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.5/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/__about__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/__init__.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/config.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/context.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/decorators.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/formatter.py
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/missing.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/nargs.py
--rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/py.typed
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/types.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/utils.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    31544 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.4.5/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.4.5/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.4.5/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.4.5/README.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.6/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.4.6/config.json
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 tabb-0.4.6/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.4.6/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.4.6/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.6/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/__about__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/config.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/context.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/missing.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/py.typed
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/types.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/utils.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.4.6/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.4.6/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.4.6/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.4.6/PKG-INFO
```

### Comparing `tabb-0.4.5/.DS_Store` & `tabb-0.4.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/test.py` & `tabb-0.4.6/test.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/.DS_Store` & `tabb-0.4.6/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/__init__.py` & `tabb-0.4.6/src/tabb/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/base.py` & `tabb-0.4.6/src/tabb/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/callback.py` & `tabb-0.4.6/src/tabb/callback.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/command.py` & `tabb-0.4.6/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/config.py` & `tabb-0.4.6/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/context.py` & `tabb-0.4.6/src/tabb/context.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/decorators.py` & `tabb-0.4.6/src/tabb/decorators.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/exceptions.py` & `tabb-0.4.6/src/tabb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/formatter.py` & `tabb-0.4.6/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/group.py` & `tabb-0.4.6/src/tabb/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/nargs.py` & `tabb-0.4.6/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parser.py` & `tabb-0.4.6/src/tabb/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/types.py` & `tabb-0.4.6/src/tabb/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/utils.py` & `tabb-0.4.6/src/tabb/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parameter/__init__.py` & `tabb-0.4.6/src/tabb/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parameter/base.py` & `tabb-0.4.6/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parameter/depends.py` & `tabb-0.4.6/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parameter/group.py` & `tabb-0.4.6/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parameter/parser.py` & `tabb-0.4.6/src/tabb/parameter/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parameter/resolve.py` & `tabb-0.4.6/src/tabb/parameter/resolve.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/src/tabb/parameter/types.py` & `tabb-0.4.6/src/tabb/parameter/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         """Returns the metavar default for this param if it provides one."""
         return None
 
     def parse_flags(self, flags: Sequence[str]) -> tuple[list[str], list[str]]:
         return list(flags), []
 
     def format_value(self, value: ValueType) -> str:
-        return repr(value)
+        return str(value)
 
     def fail(
         self,
         message: str,
         ctx: Context[Any] | None = None,
         param: ParserParameter[Any] | None = None,
     ) -> NoReturn:
@@ -488,17 +488,14 @@
         return super().validate(value)
 
 
 class Tuple(SequenceType[ValueType], ParameterType[list[ValueType]]):
     def _cast(self, value: Sequence[ValueType]) -> tuple[ValueType, ...]:
         return tuple(value)
 
-    def format_value(self, value: Sequence[ValueType]) -> str:
-        return f"[{super().format_value(value)}]"
-
     def process_args(self, args: list[ParameterArg]) -> tuple[ValueType, ...]:
         return self._cast(super().process_args(args))
 
     def process_config(self, value: object) -> object:
         value = super().process_config(value)
         if isinstance(value, Sequence):
             return self._cast(value)
```

### Comparing `tabb-0.4.5/src/tabb/parameter/utils.py` & `tabb-0.4.6/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/.gitignore` & `tabb-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/LICENSE.txt` & `tabb-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/README.md` & `tabb-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/pyproject.toml` & `tabb-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabb-0.4.5/PKG-INFO` & `tabb-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.4.5
+Version: 0.4.6
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

