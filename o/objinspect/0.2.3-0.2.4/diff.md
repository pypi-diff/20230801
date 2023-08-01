# Comparing `tmp/objinspect-0.2.3.tar.gz` & `tmp/objinspect-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objinspect-0.2.3.tar", last modified: Wed Jun 28 15:53:43 2023, max compression
+gzip compressed data, was "objinspect-0.2.4.tar", last modified: Tue Aug  1 16:54:59 2023, max compression
```

## Comparing `objinspect-0.2.3.tar` & `objinspect-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:53:43.070666 objinspect-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-28 15:53:32.000000 objinspect-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-28 15:53:43.070666 objinspect-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-28 15:53:32.000000 objinspect-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:53:43.070666 objinspect-0.2.3/objinspect/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-28 15:53:32.000000 objinspect-0.2.3/objinspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-28 15:53:32.000000 objinspect-0.2.3/objinspect/_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-28 15:53:32.000000 objinspect-0.2.3/objinspect/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-28 15:53:32.000000 objinspect-0.2.3/objinspect/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-28 15:53:32.000000 objinspect-0.2.3/objinspect/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-28 15:53:32.000000 objinspect-0.2.3/objinspect/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-28 15:53:32.000000 objinspect-0.2.3/objinspect/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:53:43.070666 objinspect-0.2.3/objinspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-28 15:53:43.000000 objinspect-0.2.3/objinspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-28 15:53:43.000000 objinspect-0.2.3/objinspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:53:43.000000 objinspect-0.2.3/objinspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-28 15:53:43.000000 objinspect-0.2.3/objinspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 15:53:43.000000 objinspect-0.2.3/objinspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-28 15:53:32.000000 objinspect-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:53:43.070666 objinspect-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:53:32.000000 objinspect-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:54:59.906844 objinspect-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 16:54:43.000000 objinspect-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-08-01 16:54:59.906844 objinspect-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-01 16:54:43.000000 objinspect-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:54:59.906844 objinspect-0.2.4/objinspect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 16:54:43.000000 objinspect-0.2.4/objinspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-08-01 16:54:43.000000 objinspect-0.2.4/objinspect/_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-01 16:54:43.000000 objinspect-0.2.4/objinspect/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-08-01 16:54:43.000000 objinspect-0.2.4/objinspect/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-08-01 16:54:43.000000 objinspect-0.2.4/objinspect/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-01 16:54:43.000000 objinspect-0.2.4/objinspect/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-01 16:54:43.000000 objinspect-0.2.4/objinspect/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:54:59.906844 objinspect-0.2.4/objinspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-08-01 16:54:59.000000 objinspect-0.2.4/objinspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 16:54:59.000000 objinspect-0.2.4/objinspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:54:59.000000 objinspect-0.2.4/objinspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 16:54:59.000000 objinspect-0.2.4/objinspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 16:54:59.000000 objinspect-0.2.4/objinspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-01 16:54:43.000000 objinspect-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:54:59.906844 objinspect-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:54:43.000000 objinspect-0.2.4/setup.py
```

### Comparing `objinspect-0.2.3/LICENSE` & `objinspect-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.3/PKG-INFO` & `objinspect-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objinspect
-Version: 0.2.3
+Version: 0.2.4
 Summary: View the structure of Python classes and functions
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
 Project-URL: Repository, https://github.com/zigai/obj-inspect
 Keywords: objinspect,object inspection,code introspection,python inspect
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objinspect-0.2.3/README.md` & `objinspect-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.3/objinspect/__init__.py` & `objinspect-0.2.4/objinspect/__init__.py`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.3/objinspect/_class.py` & `objinspect-0.2.4/objinspect/_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import inspect
 from typing import Any
 
 import docstring_parser
 
 from objinspect.function import _get_docstr_desc, _has_docstr
 from objinspect.method import Method, MethodFilter
+from objinspect.parameter import Parameter
 
 
 class Class:
 
     """
     Class for wrapping a class or class instance and providing information about its methods.
 
@@ -39,55 +40,63 @@
         cls,
         init=True,
         public=True,
         inherited=True,
         static_methods=True,
         protected=False,
         private=False,
+        classmethod=True,
+        skip_self=True,
     ) -> None:
         self.cls = cls
         self.is_initialized = False
+        self.skip_self = skip_self
+
         try:
             self.name: str = self.cls.__name__
         except AttributeError:
             self.name = f"{self.cls.__class__.__name__} instance"
             self.is_initialized = True
+
         self.instance = None if not self.is_initialized else self.cls
         self.docstring = inspect.getdoc(self.cls)
         self.has_docstring = _has_docstr(self.docstring)
         self.extractor_kwargs = {
             "init": init,
             "public": public,
             "inherited": inherited,
             "static_methods": static_methods,
             "protected": protected,
             "private": private,
+            "classmethod": classmethod,
         }
         self._methods = self._find_methods()
         self.has_init = "__init__" in self._methods
         self._parsed_docstring = (
             docstring_parser.parse(self.docstring) if self.has_docstring else None  # type: ignore
         )
         self.description = _get_docstr_desc(self._parsed_docstring)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name='{self.name}', methods={len(self._methods)}, has_init={self.has_init}, description={self.description})"
 
     @functools.cached_property
-    def _get_class_base(self):
+    def _class_base(self):
         if self.is_initialized:
             return self.cls.__class__
         return self.cls
 
-    def _find_methods(self):
+    def _find_methods(self) -> dict[str, Method]:
         method_filter = MethodFilter(**self.extractor_kwargs)
         members = inspect.getmembers(self.cls, inspect.isfunction)
         methods = {}
-        for i in method_filter.extract([Method(i[1], self._get_class_base) for i in members]):
-            methods[i.name] = i
+        for method in method_filter.extract(
+            [Method(i[1], self._class_base, skip_self=self.skip_self) for i in members]
+        ):
+            methods[method.name] = method
         return methods
 
     def init(self, *args, **kwargs) -> None:
         """
         Initializes the class as an instance using the provided arguments.
 
         Raises:
@@ -134,25 +143,38 @@
                 return self._methods[method]
             case int():
                 return self.methods[method]
             case _:
                 raise TypeError(type(method))
 
     @property
+    def init_method(self):
+        try:
+            return self.get_method("__init__")
+        except KeyError:
+            return None
+
+    @property
+    def init_args(self) -> list[Parameter] | None:
+        if self.init_method is None:
+            return None
+        return self.init_method.params
+
+    @property
     def methods(self) -> list[Method]:
         """
         Returns the list of methods of the class or instance as a list of :class:`Function` objects.
         """
         return list(self._methods.values())
 
     @property
     def dict(self) -> dict[str, Any]:
         return {
             "name": self.name,
-            "methods": [i.dict for i in self.methods],
+            "methods": [method.dict for method in self.methods],
             "description": self.description,
             "initialized": self.is_initialized,
             "docstring": self.docstring,
         }
 
 
 __all__ = ["Class"]
```

### Comparing `objinspect-0.2.3/objinspect/function.py` & `objinspect-0.2.4/objinspect/function.py`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.3/objinspect/method.py` & `objinspect-0.2.4/objinspect/method.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,28 +72,31 @@
         self,
         init=True,
         public=True,
         inherited=True,
         static_methods=True,
         protected=False,
         private=False,
+        classmethod=False,
     ) -> None:
         self.checks = []
         if not init:
             self.checks.append(lambda method: method.name == "__init__")
         if not static_methods:
             self.checks.append(lambda method: method.is_static)
         if not inherited:
             self.checks.append(lambda method: method.is_inherited)
         if not private:
             self.checks.append(lambda method: method.is_private)
         if not protected:
             self.checks.append(lambda method: method.is_protected)
         if not public:
             self.checks.append(lambda method: method.is_public)
+        if not classmethod:
+            self.checks.append(lambda method: method.is_classmethod)
 
     def check(self, method: Method) -> bool:
         for check_func in self.checks:
             if check_func(method):
                 return False
         return True
```

### Comparing `objinspect-0.2.3/objinspect/parameter.py` & `objinspect-0.2.4/objinspect/parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,21 +32,21 @@
         """
         self.name = name
         self.type = type
         self.default = default
         self.description = description
         self.kind = kind
         if infer_type and not self.is_typed:
-            self.type = self._get_infered_type()
+            self.type = self.get_infered_type()
 
     def __repr__(self):
         data = f"name='{self.name}', kind={str(self.kind)}, type={self.type}, default={self.default}, description='{self.description}'"
         return f"{self.__class__.__name__}({data})"
 
-    def _get_infered_type(self):
+    def get_infered_type(self):
         """Infer the type of the parameter based on its default value."""
         if self.default is EMPTY:
             return EMPTY
         return type(self.default)
 
     @property
     def is_typed(self) -> bool:
```

### Comparing `objinspect-0.2.3/objinspect/util.py` & `objinspect-0.2.4/objinspect/util.py`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.3/objinspect.egg-info/PKG-INFO` & `objinspect-0.2.4/objinspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objinspect
-Version: 0.2.3
+Version: 0.2.4
 Summary: View the structure of Python classes and functions
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
 Project-URL: Repository, https://github.com/zigai/obj-inspect
 Keywords: objinspect,object inspection,code introspection,python inspect
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objinspect-0.2.3/pyproject.toml` & `objinspect-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "objinspect"
-version = "0.2.3"
+version = "0.2.4"
 description = "View the structure of Python classes and functions"
 authors = [{ name = "Žiga Ivanšek", email = "ziga.ivansek@gmail.com" }]
 license = { file = "LICENSE.txt" }
 readme = "README.md"
 requires-python = ">=3.10"
 
 classifiers = [
```

