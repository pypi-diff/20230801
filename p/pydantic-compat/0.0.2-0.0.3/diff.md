# Comparing `tmp/pydantic_compat-0.0.2.tar.gz` & `tmp/pydantic_compat-0.0.3.tar.gz`

## Comparing `pydantic_compat-0.0.2.tar` & `pydantic_compat-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/__init__.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_shared.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v1_decorators.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v1_mixin.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v2_decorators.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v2_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/py.typed
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/tests/test_base_model.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/tests/test_decorators.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/.gitignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/LICENSE
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/README.md
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/__init__.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_shared.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v1_decorators.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v1_mixin.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v2_decorators.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v2_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/py.typed
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/tests/test_base_model.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/tests/test_decorators.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/README.md
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/PKG-INFO
```

### Comparing `pydantic_compat-0.0.2/src/pydantic_compat/__init__.py` & `pydantic_compat-0.0.3/src/pydantic_compat/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 ]
 
 from ._shared import PYDANTIC2
 
 if TYPE_CHECKING:
     from pydantic import field_validator, model_validator, root_validator, validator
 
-    from ._v2_mixin import PydanticCompatMixin
+    # using this to avoid breaking pydantic mypy plugin
+    # not that it will be hard to provide proper names AND proper signatures for
+    # both versions of pydantic without a ton of potentially outdated signatures
+    PydanticCompatMixin = type
 
 elif PYDANTIC2:
     from pydantic import field_validator, model_validator
 
     from ._v2_decorators import root_validator, validator
     from ._v2_mixin import PydanticCompatMixin
```

### Comparing `pydantic_compat-0.0.2/src/pydantic_compat/_shared.py` & `pydantic_compat-0.0.3/src/pydantic_compat/_shared.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/src/pydantic_compat/_v1_decorators.py` & `pydantic_compat-0.0.3/src/pydantic_compat/_v1_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/src/pydantic_compat/_v1_mixin.py` & `pydantic_compat-0.0.3/src/pydantic_compat/_v1_mixin.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/src/pydantic_compat/_v2_decorators.py` & `pydantic_compat-0.0.3/src/pydantic_compat/_v2_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/src/pydantic_compat/_v2_mixin.py` & `pydantic_compat-0.0.3/src/pydantic_compat/_v2_mixin.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/tests/test_base_model.py` & `pydantic_compat-0.0.3/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/tests/test_decorators.py` & `pydantic_compat-0.0.3/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/.gitignore` & `pydantic_compat-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/LICENSE` & `pydantic_compat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/README.md` & `pydantic_compat-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/pyproject.toml` & `pydantic_compat-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.2/PKG-INFO` & `pydantic_compat-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-compat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compatibility layer for pydantic v1/v2
 Project-URL: homepage, https://github.com/tlambert03/pydantic-compat
 Project-URL: repository, https://github.com/tlambert03/pydantic-compat
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

