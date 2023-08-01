# Comparing `tmp/pydantic_compat-0.0.1.tar.gz` & `tmp/pydantic_compat-0.0.2.tar.gz`

## Comparing `pydantic_compat-0.0.1.tar` & `pydantic_compat-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/src/pydantic_compat/__init__.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/src/pydantic_compat/_shared.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/src/pydantic_compat/_v1_decorators.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/src/pydantic_compat/_v1_mixin.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/src/pydantic_compat/_v2_decorators.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/src/pydantic_compat/_v2_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/src/pydantic_compat/py.typed
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/tests/test_base_model.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/tests/test_decorators.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/.gitignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/LICENSE
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/README.md
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7317 2020-02-02 00:00:00.000000 pydantic_compat-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/__init__.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_shared.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v1_decorators.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v1_mixin.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v2_decorators.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/_v2_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/src/pydantic_compat/py.typed
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/tests/test_base_model.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/tests/test_decorators.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/README.md
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pydantic_compat-0.0.2/PKG-INFO
```

### Comparing `pydantic_compat-0.0.1/src/pydantic_compat/__init__.py` & `pydantic_compat-0.0.2/src/pydantic_compat/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """CompatibilityMixin for pydantic v1/1/v2."""
 
-from importlib.metadata import PackageNotFoundError, version
+try:
+    from importlib.metadata import PackageNotFoundError, version
+except ImportError:
+    from importlib_metadata import PackageNotFoundError, version
+
 from typing import TYPE_CHECKING
 
 try:
     __version__ = version("pydantic-compat")
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "uninstalled"
```

### Comparing `pydantic_compat-0.0.1/src/pydantic_compat/_shared.py` & `pydantic_compat-0.0.2/src/pydantic_compat/_shared.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/src/pydantic_compat/_v1_decorators.py` & `pydantic_compat-0.0.2/src/pydantic_compat/_v1_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/src/pydantic_compat/_v1_mixin.py` & `pydantic_compat-0.0.2/src/pydantic_compat/_v1_mixin.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/src/pydantic_compat/_v2_decorators.py` & `pydantic_compat-0.0.2/src/pydantic_compat/_v2_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/src/pydantic_compat/_v2_mixin.py` & `pydantic_compat-0.0.2/src/pydantic_compat/_v2_mixin.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/tests/test_base_model.py` & `pydantic_compat-0.0.2/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/tests/test_decorators.py` & `pydantic_compat-0.0.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/.gitignore` & `pydantic_compat-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/LICENSE` & `pydantic_compat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.1/README.md` & `pydantic_compat-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Pydantic 2 was a major release that completely changed the pydantic API.
 
 For applications, this is not a big deal, as they can pin to whatever version of
 pydantic they need. But for libraries that want to exist in a broader
 environment, pinning to a specific version of pydantic is not always an option
 (as it limits the ability to co-exist with other libraries).
 
-This package provides compatibility mixins and function adaptors for pydantic
+This package provides (unofficial) compatibility mixins and function adaptors for pydantic
 v1-v2 cross compatibility. It allows you to use either v1 or v2 API names,
 regardless of the pydantic version installed. (Prefer using v2 names when possible)
 
 The API conversion is not exhaustive, but suffices for many of the use cases
 I have come across. I will be using it in:
 
 - [ome-types](https://github.com/tlambert03/ome-types)
```

### Comparing `pydantic_compat-0.0.1/pyproject.toml` & `pydantic_compat-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,52 +4,61 @@
 build-backend = "hatchling.build"
 
 # https://peps.python.org/pep-0621/
 [project]
 name = "pydantic-compat"
 description = "Compatibility layer for pydantic v1/v2"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 license = { text = "BSD 3-Clause License" }
 authors = [{ email = "talley.lambert@gmail.com", name = "Talley Lambert" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Framework :: Pydantic",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic"]
+dependencies = ["pydantic", "importlib_metadata; python_version<'3.8'"]
 
 [tool.hatch.envs.default]
-dependencies = ["pytest", "pytest-cov", "pdbpp", "rich"]
+dependencies = [
+    "pytest",
+    "pytest-cov",
+    "pdbpp",
+    "rich",
+    "importlib_metadata; python_version<'3.8'",
+]
 
 [tool.hatch.envs.test]
 
 [tool.hatch.envs.test.scripts]
 test = "pytest -v"
 test-cov = "pytest -v --cov --cov-report=term-missing"
 test-cov-xml = "pytest -v --color=yes --cov --cov-report=xml --cov-append"
 
 [[tool.hatch.envs.test.matrix]]
-# python = ["3.8", "3.11"] # good for local, too verbose for CI
-pydantic = ["v1", "v2"]
+# python = ["3.7", "3.11"] # good for local, too verbose for CI
+pydantic = ["v1.8", "v1", "v2"]
 
 [tool.hatch.envs.test.overrides]
 matrix.pydantic.extra-dependencies = [
+    { value = "pydantic==1.8.0", if = ["v1.8"] },
     { value = "pydantic<2.0", if = ["v1"] },
     { value = "pydantic>=2.0", if = ["v2"] },
 ]
 
 
+
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 test = ["pytest>=6.0", "pytest-cov"]
 dev = [
     "black",
     "ipython",
     "mypy",
@@ -76,15 +85,15 @@
 [tool.hatch.build.targets.wheel]
 only-include = ["src"]
 sources = ["src"]
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
-target-version = "py38"
+target-version = "py37"
 src = ["src"]
 # https://beta.ruff.rs/docs/rules/
 select = [
     "E",    # style errors
     "W",    # style warnings
     "F",    # flakes
     "I",    # isort
```

### Comparing `pydantic_compat-0.0.1/PKG-INFO` & `pydantic_compat-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pydantic-compat
-Version: 0.0.1
+Version: 0.0.2
 Summary: Compatibility layer for pydantic v1/v2
 Project-URL: homepage, https://github.com/tlambert03/pydantic-compat
 Project-URL: repository, https://github.com/tlambert03/pydantic-compat
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
+Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: pydantic
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
@@ -47,15 +49,15 @@
 Pydantic 2 was a major release that completely changed the pydantic API.
 
 For applications, this is not a big deal, as they can pin to whatever version of
 pydantic they need. But for libraries that want to exist in a broader
 environment, pinning to a specific version of pydantic is not always an option
 (as it limits the ability to co-exist with other libraries).
 
-This package provides compatibility mixins and function adaptors for pydantic
+This package provides (unofficial) compatibility mixins and function adaptors for pydantic
 v1-v2 cross compatibility. It allows you to use either v1 or v2 API names,
 regardless of the pydantic version installed. (Prefer using v2 names when possible)
 
 The API conversion is not exhaustive, but suffices for many of the use cases
 I have come across. I will be using it in:
 
 - [ome-types](https://github.com/tlambert03/ome-types)
```

