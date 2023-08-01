# Comparing `tmp/symbolite-0.3.tar.gz` & `tmp/symbolite-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolite-0.3.tar", last modified: Mon Feb 13 12:01:15 2023, max compression
+gzip compressed data, was "symbolite-0.4.tar", last modified: Tue Aug  1 20:17:39 2023, max compression
```

## Comparing `symbolite-0.3.tar` & `symbolite-0.4.tar`

### file list

```diff
@@ -1,38 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.170931 symbolite-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-13 12:01:03.000000 symbolite-0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.162931 symbolite-0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.166931 symbolite-0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-02-13 12:01:03.000000 symbolite-0.3/.github/workflows/lint-autoupdate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-13 12:01:03.000000 symbolite-0.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-13 12:01:03.000000 symbolite-0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-13 12:01:03.000000 symbolite-0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-13 12:01:03.000000 symbolite-0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-13 12:01:03.000000 symbolite-0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-13 12:01:03.000000 symbolite-0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-13 12:01:03.000000 symbolite-0.3/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-13 12:01:03.000000 symbolite-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-02-13 12:01:15.170931 symbolite-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-02-13 12:01:03.000000 symbolite-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-13 12:01:03.000000 symbolite-0.3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-13 12:01:03.000000 symbolite-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-13 12:01:03.000000 symbolite-0.3/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:03.000000 symbolite-0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 12:01:15.170931 symbolite-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.162931 symbolite-0.3/symbolite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.170931 symbolite-0.3/symbolite/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/core/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/core/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/core/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/core/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/core/translators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.170931 symbolite-0.3/symbolite/symbol/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/symbol/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/symbol/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.170931 symbolite-0.3/symbolite/testsuite/
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-02-13 12:01:03.000000 symbolite-0.3/symbolite/testsuite/test_root.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:01:15.170931 symbolite-0.3/symbolite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-02-13 12:01:15.000000 symbolite-0.3/symbolite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-13 12:01:15.000000 symbolite-0.3/symbolite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 12:01:15.000000 symbolite-0.3/symbolite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-13 12:01:15.000000 symbolite-0.3/symbolite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-13 12:01:15.000000 symbolite-0.3/symbolite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.900081 symbolite-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 20:17:30.000000 symbolite-0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.892081 symbolite-0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.892081 symbolite-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 20:17:30.000000 symbolite-0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-01 20:17:30.000000 symbolite-0.4/.github/workflows/lint-autoupdate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-01 20:17:30.000000 symbolite-0.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-01 20:17:30.000000 symbolite-0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 20:17:30.000000 symbolite-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-01 20:17:30.000000 symbolite-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 20:17:30.000000 symbolite-0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-01 20:17:30.000000 symbolite-0.4/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 20:17:30.000000 symbolite-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-08-01 20:17:39.896081 symbolite-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-08-01 20:17:30.000000 symbolite-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-01 20:17:30.000000 symbolite-0.4/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 20:17:30.000000 symbolite-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 20:17:30.000000 symbolite-0.4/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:30.000000 symbolite-0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:17:39.900081 symbolite-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.892081 symbolite-0.4/symbolite/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/abstract/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/abstract/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/abstract/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/core/symbolgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/impl/libjax/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libjax/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libjax/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libjax/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/impl/libnumpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libnumpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libnumpy/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libnumpy/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libnumpy/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/impl/libstd/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libstd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libstd/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libstd/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libstd/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/impl/libsympy/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libsympy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libsympy/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libsympy/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/impl/libsympy/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite/testsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/testsuite/test_scalar_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/testsuite/test_scalar_impls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/testsuite/test_scalar_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/testsuite/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/testsuite/test_symbolgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-01 20:17:30.000000 symbolite-0.4/symbolite/testsuite/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:17:39.896081 symbolite-0.4/symbolite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-08-01 20:17:39.000000 symbolite-0.4/symbolite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-01 20:17:39.000000 symbolite-0.4/symbolite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:17:39.000000 symbolite-0.4/symbolite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 20:17:39.000000 symbolite-0.4/symbolite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 20:17:39.000000 symbolite-0.4/symbolite.egg-info/top_level.txt
```

### Comparing `symbolite-0.3/.github/workflows/lint-autoupdate.yml` & `symbolite-0.4/.github/workflows/lint-autoupdate.yml`

 * *Files identical despite different names*

### Comparing `symbolite-0.3/.github/workflows/test.yml` & `symbolite-0.4/.github/workflows/ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-name: Test with pytest
+name: CI
 
 on: [push]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
@@ -20,13 +20,13 @@
 
       - name: Upgrade pip
         run: python -m pip install --upgrade pip
 
       - name: Install package
         run: pip install --pre .[test]
 
-      - name: Install numpy and sympy (but only for 1 python version)
-        if: ${{ matrix.python-version == '3.11' }}
-        run: pip install sympy numpy
+      - name: Install implementations (but only for 1 python version)
+        # if: ${{ matrix.python-version == '3.11' }}
+        run: pip install sympy numpy jax
 
       - name: Test with pytest
         run: pytest
```

### Comparing `symbolite-0.3/.pre-commit-config.yaml` & `symbolite-0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `symbolite-0.3/LICENSE` & `symbolite-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolite-0.3/conftest.py` & `symbolite-0.4/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def setup_test_readme():
     GENERATED_PATH.mkdir(exist_ok=True)
 
     INDENT = " " * 4
     with TEST_README.open("w") as out, README.open("r") as readme:
         mode = None
         output = []
+
         output.append("def all_tests():\n")
         for i, line in enumerate(readme.readlines()):
             output.append("\n")
             if mode is None and line.strip() == "```python":
                 mode = "first_line"
                 output[i] = INDENT + "# line %04d" % i
                 # output[i] = 'def test_line_%04d():\n' % i
@@ -65,9 +66,10 @@
             rm_tree(child)
     pth.rmdir()
 
 
 def pytest_sessionfinish(session, exitstatus):
     try:
         rm_tree(GENERATED_PATH)
+        pass
     except FileNotFoundError:
         pass
```

### Comparing `symbolite-0.3/pyproject.toml` & `symbolite-0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,23 +8,24 @@
     { name="Hernán E. Grecco", email="hernan.grecco@gmail.com" },
     { name="Mauro Silberberg", email="maurosilber@gmail.com" },
 ]
 description = "A minimalistic symbolic package."
 keywords = ["symbolic"]
 license = { file="LICENSE" }
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dynamic = ["dependencies", "optional-dependencies", "version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [tool.setuptools.packages.find]
@@ -43,12 +44,12 @@
 [tool.pytest.ini_options]
 addopts = "--import-mode=importlib --doctest-modules"
 pythonpath = "."
 testpaths = [
     "symbolite/testsuite"
 ]
 doctest_optionflags = "NUMBER"
-
+filterwarnings = "ignore:No libsl provided, defaulting to Python standard library."
 
 [tool.ruff]
 select = ["E", "F", "I"]
 ignore = ["E501"]
```

### Comparing `symbolite-0.3/symbolite/testsuite/test_root.py` & `symbolite-0.4/symbolite/testsuite/test_symbol.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 import pytest
 
-from symbolite.core.operands import Function
-from symbolite.core.translators import find_libs_in_stack
-from symbolite.symbol.abstract import Symbol
+from symbolite import Function, Symbol
+from symbolite.abstract.symbol import Expression
+from symbolite.impl import find_module_in_stack
 
 x, y, z = map(Symbol, "x y z".split())
 
-F = Function("F", "", 1)
-G = Function("G", "lib", 1)
+F = Function("F", arity=1)
+G = Function("G", arity=1)
+
+
+@pytest.mark.mypy_testing
+# noqa: F821
+def test_typing():
+    reveal_type(x + y)  # R: symbolite.abstract.symbol.Symbol # noqa: F821
+    reveal_type(2 + y)  # R: symbolite.abstract.symbol.Symbol # noqa: F821
+    reveal_type(x + 2)  # R: symbolite.abstract.symbol.Symbol # noqa: F821
 
 
 def test_forward_reverse():
     expr = x + 1
-    assert expr.func.name == "__add__"
-    assert expr.args == (x, 1)
+    assert isinstance(expr.expression, Expression)
+    assert expr.expression.func.name == "add"
+    assert expr.expression.args == (x, 1)
 
     expr = 1 + x
-    assert expr.func.name == "__radd__"
-    assert expr.args == (x, 1)
+    assert isinstance(expr.expression, Expression)
+    assert expr.expression.func.name == "radd"
+    assert expr.expression.args == (x, 1)
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
         (x < y, "(x < y)"),
         (x <= y, "(x <= y)"),
@@ -58,113 +68,109 @@
         (1 & y, "(1 & y)"),
         (1 ^ y, "(1 ^ y)"),
         (1 | y, "(1 | y)"),
         (-x, "(-x)"),
         (+x, "(+x)"),
         (~x, "(~x)"),
         (F(x), "F(x)"),
-        (G(x), "lib.G(x)"),
+        (G(x), "G(x)"),
     ],
 )
-def test_str(expr, result):
+def test_str(expr: Symbol, result: Symbol):
     assert str(expr) == result
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
         (x + 2 * y, x + 2 * z),
         (x + 2 * F(y), x + 2 * F(z)),
     ],
 )
-def test_subs(expr, result):
+def test_subs(expr: Symbol, result: Symbol):
     assert expr.subs({y: z}) == result
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
         (x + 2 * y, x + 2 * z),
         (x + 2 * F(y), x + 2 * F(z)),
     ],
 )
-def test_subs_by_name(expr, result):
+def test_subs_by_name(expr: Symbol, result: Symbol):
     assert expr.subs_by_name(y=z) == result
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
         (x + y, {"x", "y"}),
         (x[z], {"x", "z"}),
         (F(x), {"F", "x"}),
-        (G(x), {"x"}),
+        (G(x), {"G", "x"}),
     ],
 )
-def test_symbol_names(expr, result):
+def test_symbol_names(expr: Symbol, result: set[str]):
     assert expr.symbol_names() == result
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
-        (x + y, {"x", "y", "libsymbol.__add__"}),
-        (x[z], {"x", "z", "libsymbol.__getitem__"}),
+        (x + y, {"x", "y", "symbol.add"}),
+        (x[z], {"x", "z", "symbol.getitem"}),
         (F(x), {"F", "x"}),
-        (G(x), {"x", "lib.G"}),
+        (G(x), {"x", "G"}),
     ],
 )
-def test_symbol_names_ops(expr, result):
+def test_symbol_names_ops(expr: Symbol, result: set[str]):
     assert expr.symbol_names(None) == result
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
         (x + y, set()),
         (x[z], set()),
         (F(x), set()),
         (
             G(x),
-            {
-                "lib.G",
-            },
+            set(),
         ),
     ],
 )
-def test_symbol_names_namespace(expr, result):
+def test_symbol_names_namespace(expr: Symbol, result: Symbol):
     assert expr.symbol_names(namespace="lib") == result
 
 
 class Scalar(Symbol):
     pass
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
         (x + 2 * y, 1 + 2 * 3),
         # (x + 2 * F(y), x + 2 * F(z)),
     ],
 )
-def test_eval_str(expr, result):
+def test_eval_str(expr: Symbol, result: Symbol):
     assert eval(str(expr.subs_by_name(x=1, y=3))) == result
 
 
 @pytest.mark.parametrize(
     "expr,result",
     [
         (x + 2 * y, 1 + 2 * 3),
         # (x + 2 * F(y), x + 2 * F(z)),
     ],
 )
-def test_eval(expr, result):
+def test_eval(expr: Symbol, result: Symbol):
     assert expr.subs_by_name(x=1, y=3).eval() == result
 
 
 def test_find_libs_in_stack():
-    assert "libsymbol" not in find_libs_in_stack()
-    assert "libsymbol" not in find_libs_in_stack(x + y)
-    from symbolite.symbol import default as libsymbol  # noqa: F401
+    assert find_module_in_stack() is None
+    from symbolite.impl import libstd as libsl  # noqa: F401
 
-    assert "libsymbol" in find_libs_in_stack()
-    assert "libsymbol" in find_libs_in_stack(x + y)
+    assert find_module_in_stack()
```

