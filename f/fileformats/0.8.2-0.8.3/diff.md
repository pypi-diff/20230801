# Comparing `tmp/fileformats-0.8.2.tar.gz` & `tmp/fileformats-0.8.3.tar.gz`

## Comparing `fileformats-0.8.2.tar` & `fileformats-0.8.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/archive/__init__.py
--rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/_version.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/converter.py
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/datatype.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/field.py
--rw-r--r--   0        0        0    46180 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/fileset.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/mark.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/mixin.py
--rw-r--r--   0        0        0    10283 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/utils.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_test_extras.py
--rw-r--r--   0        0        0    12335 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/base.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/notclassifiedyet.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/vector.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/misc/medical.py
--rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/misc/unclassified.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/model/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/headers.py
--rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/text/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.2/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.2/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.2/LICENSE
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.2/README.rst
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/converter.py
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/field.py
+-rw-r--r--   0        0        0    46197 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/mark.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/utils.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_test_extras.py
+-rw-r--r--   0        0        0    12335 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/image/base.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/image/notclassifiedyet.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/image/vector.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/misc/medical.py
+-rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/misc/unclassified.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/model/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/text/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.3/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.3/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.3/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.3/LICENSE
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.3/README.rst
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.3/PKG-INFO
```

### Comparing `fileformats-0.8.2/fileformats/archive/__init__.py` & `fileformats-0.8.3/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/audio/__init__.py` & `fileformats-0.8.3/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/converter.py` & `fileformats-0.8.3/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/datatype.py` & `fileformats-0.8.3/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/exceptions.py` & `fileformats-0.8.3/fileformats/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/field.py` & `fileformats-0.8.3/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/fileset.py` & `fileformats-0.8.3/fileformats/core/fileset.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,15 +787,15 @@
 
         Returns
         -------
         FileSet
             a file-set that will pass type-checking as an instance of the given
             fileset class but which doesn't actually point to any FS objects.
         """
-        mock_cls = type(cls.__name__ + "Mock", (MockMixin, cls), {})
+        mock_cls = type(cls.__name__ + "Mock", (MockMixin, cls), {"TRUE_CLASS": cls})
         if not fspaths:
             fspaths = []
             fspath = f"/mock/{cls.__name__.lower()}"
             if cls.ext:
                 fspath += cls.ext
             fspaths.append(fspath)
         return mock_cls(fspaths=fspaths)
```

### Comparing `fileformats-0.8.2/fileformats/core/mark.py` & `fileformats-0.8.3/fileformats/core/mark.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,21 +124,22 @@
     return decorator if task_spec is None else decorator(task_spec)
 
 
 def extra(method: ty.Callable):
     """A decorator which uses singledispatch to facilitate the registering of
     "extra" functionality in external packages (e.g. "fileformats-extras")"""
 
-    functools.wraps(method)
+    dispatch_method = functools.singledispatch(method)
 
+    @functools.wraps(method)
     def decorated(obj, *args, **kwargs):
         cls = type(obj)
         extras_imported, extras_pkg, extras_pypi = import_extras_module(cls)
         try:
-            return method(obj, *args, **kwargs)
+            return dispatch_method(obj, *args, **kwargs)
         except NotImplementedError:
             if extras_imported:
                 msg = f"No implementation for '{method.__name__}' extra for {cls.__name__} types"
             else:
                 try:
                     if check_package_exists_on_pypi(extras_pypi):
                         msg += (
@@ -149,8 +150,9 @@
                 except urllib.error.URLError:
                     msg += (
                         '. Was not able to check whether an "extras" package '
                         f"({extras_pypi}) exists on PyPI or not"
                     )
             raise FileFormatsExtrasError(msg)
 
-    return functools.singledispatch(decorated)
+    decorated.register = dispatch_method.register
+    return decorated
```

### Comparing `fileformats-0.8.2/fileformats/core/mixin.py` & `fileformats-0.8.3/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/utils.py` & `fileformats-0.8.3/fileformats/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,19 @@
     Returns
     -------
     imported : bool
         whether the module was imported or not
     sub_pkg : str
         the name of the sub-package that was attempted to be loaded
     """
-
+    # Check for Mock class
+    try:
+        klass = klass.TRUE_CLASS
+    except AttributeError:
+        pass
     pkg_parts = klass.__module__.split(".")
     if pkg_parts[0] != "fileformats":
         logger.debug(
             "There is no 'extras' module for classes not within the 'fileformats' package, "
             "not %s in %s",
             klass.__name__,
             klass.__module__,
```

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_classifiers.py` & `fileformats-0.8.3/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_converter.py` & `fileformats-0.8.3/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_detection.py` & `fileformats-0.8.3/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_general.py` & `fileformats-0.8.3/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_mime.py` & `fileformats-0.8.3/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_mixin.py` & `fileformats-0.8.3/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_subpackages.py` & `fileformats-0.8.3/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_test_extras.py` & `fileformats-0.8.3/fileformats/core/tests/test_test_extras.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/core/tests/test_utils.py` & `fileformats-0.8.3/fileformats/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/document/__init__.py` & `fileformats-0.8.3/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/field/__init__.py` & `fileformats-0.8.3/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/field/tests/test_fields.py` & `fileformats-0.8.3/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.8.3/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/generic/__init__.py` & `fileformats-0.8.3/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/image/__init__.py` & `fileformats-0.8.3/fileformats/image/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/image/notclassifiedyet.py` & `fileformats-0.8.3/fileformats/image/notclassifiedyet.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/image/raster.py` & `fileformats-0.8.3/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/image/tests/test_image_raster.py` & `fileformats-0.8.3/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/misc/__init__.py` & `fileformats-0.8.3/fileformats/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/misc/unclassified.py` & `fileformats-0.8.3/fileformats/misc/unclassified.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/model/__init__.py` & `fileformats-0.8.3/fileformats/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/serialization/__init__.py` & `fileformats-0.8.3/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/testing/classifiers.py` & `fileformats-0.8.3/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/testing/headers.py` & `fileformats-0.8.3/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/text/__init__.py` & `fileformats-0.8.3/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/fileformats/video/__init__.py` & `fileformats-0.8.3/fileformats/video/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/LICENSE` & `fileformats-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/README.rst` & `fileformats-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/pyproject.toml` & `fileformats-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.2/PKG-INFO` & `fileformats-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.8.2
+Version: 0.8.3
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

