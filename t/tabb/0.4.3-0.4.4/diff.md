# Comparing `tmp/tabb-0.4.3.tar.gz` & `tmp/tabb-0.4.4.tar.gz`

## Comparing `tabb-0.4.3.tar` & `tabb-0.4.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.3/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.4.3/config.json
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 tabb-0.4.3/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.4.3/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.4.3/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.3/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/__about__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/__init__.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/config.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/context.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/decorators.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/formatter.py
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/missing.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/nargs.py
--rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/py.typed
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/types.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/utils.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    32341 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.4.3/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.4.3/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.4.3/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.4.3/README.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.4/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.4.4/config.json
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 tabb-0.4.4/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.4.4/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.4.4/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.4.4/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/__about__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/config.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/context.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/missing.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/py.typed
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/types.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/utils.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    32341 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.4.4/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.4.4/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.4.4/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.4.4/PKG-INFO
```

### Comparing `tabb-0.4.3/.DS_Store` & `tabb-0.4.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/test.py` & `tabb-0.4.4/test.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/.DS_Store` & `tabb-0.4.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/__init__.py` & `tabb-0.4.4/src/tabb/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/base.py` & `tabb-0.4.4/src/tabb/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/callback.py` & `tabb-0.4.4/src/tabb/callback.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/command.py` & `tabb-0.4.4/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/config.py` & `tabb-0.4.4/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/context.py` & `tabb-0.4.4/src/tabb/context.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/decorators.py` & `tabb-0.4.4/src/tabb/decorators.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/exceptions.py` & `tabb-0.4.4/src/tabb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/formatter.py` & `tabb-0.4.4/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/group.py` & `tabb-0.4.4/src/tabb/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/nargs.py` & `tabb-0.4.4/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parser.py` & `tabb-0.4.4/src/tabb/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/types.py` & `tabb-0.4.4/src/tabb/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/utils.py` & `tabb-0.4.4/src/tabb/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parameter/__init__.py` & `tabb-0.4.4/src/tabb/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parameter/base.py` & `tabb-0.4.4/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parameter/depends.py` & `tabb-0.4.4/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parameter/group.py` & `tabb-0.4.4/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parameter/parser.py` & `tabb-0.4.4/src/tabb/parameter/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,21 +70,24 @@
             return True
 
         if self.default_factory is not MISSING:
             return True
 
         return False
 
+    def get_default_metavar(self, ctx: Context[Any] | None = None) -> str:
+        return self.name.upper()
+
     def get_metavar(self, ctx: Context[Any] | None = None) -> str:
         if self.metavar is not None:
             return self.metavar
 
         metavar = self.type.get_metavar(ctx)
         if metavar is None:
-            metavar = self.name.upper()
+            metavar = self.get_default_metavar(ctx)
 
         return self.nargs.format_metavar(metavar)
 
     def get_config(self, ctx: Context[Any] | None = None) -> list[str]:
         if self.config is not None:
             return self.config
 
@@ -263,14 +266,17 @@
 
     @property
     def nargs(self) -> IntNArgs:
         if isinstance(nargs := self.type.nargs, IntNArgs):
             return nargs
         raise ValueError("nargs for options may not be variadic.")
 
+    def get_default_metavar(self, ctx: Context[Any] | None = None) -> str:
+        return self.type.name.upper()
+
     def get_error_hint(self, ctx: Context[Any] | None = None) -> str:
         return " / ".join(f"'{flag}'" for flag in self.flags)
 
     def get_default_repr(self, ctx: Context[Any] | None = None) -> str | None:
         if isinstance(self.show_default, str):
             return f"({self.show_default})"
```

### Comparing `tabb-0.4.3/src/tabb/parameter/resolve.py` & `tabb-0.4.4/src/tabb/parameter/resolve.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parameter/types.py` & `tabb-0.4.4/src/tabb/parameter/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/src/tabb/parameter/utils.py` & `tabb-0.4.4/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/.gitignore` & `tabb-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/LICENSE.txt` & `tabb-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/README.md` & `tabb-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/pyproject.toml` & `tabb-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabb-0.4.3/PKG-INFO` & `tabb-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

