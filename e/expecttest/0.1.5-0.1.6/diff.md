# Comparing `tmp/expecttest-0.1.5.tar.gz` & `tmp/expecttest-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expecttest-0.1.5.tar", max compression
+gzip compressed data, was "expecttest-0.1.6.tar", max compression
```

## Comparing `expecttest-0.1.5.tar` & `expecttest-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2022-05-26 13:25:48.952145 expecttest-0.1.5/LICENSE
--rw-r--r--   0        0        0     1832 2022-05-26 13:25:48.952540 expecttest-0.1.5/README.md
--rw-r--r--   0        0        0    10734 2023-07-31 16:10:01.285123 expecttest-0.1.5/expecttest/__init__.py
--rw-r--r--   0        0        0        0 2022-05-26 13:25:48.953543 expecttest-0.1.5/expecttest/py.typed
--rw-r--r--   0        0        0     1197 2023-07-31 16:10:01.288931 expecttest-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2402 2023-07-31 16:10:18.020267 expecttest-0.1.5/setup.py
--rw-r--r--   0        0        0     2538 2023-07-31 16:10:18.020430 expecttest-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-05-26 13:25:48.952145 expecttest-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1832 2022-05-26 13:25:48.952540 expecttest-0.1.6/README.md
+-rw-r--r--   0        0        0    10615 2023-08-01 12:10:45.580458 expecttest-0.1.6/expecttest/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-26 13:25:48.953543 expecttest-0.1.6/expecttest/py.typed
+-rw-r--r--   0        0        0     1197 2023-08-01 12:10:45.581232 expecttest-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2402 2023-08-01 12:10:48.185297 expecttest-0.1.6/setup.py
+-rw-r--r--   0        0        0     2538 2023-08-01 12:10:48.185487 expecttest-0.1.6/PKG-INFO
```

### Comparing `expecttest-0.1.5/LICENSE` & `expecttest-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `expecttest-0.1.5/README.md` & `expecttest-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `expecttest-0.1.5/expecttest/__init__.py` & `expecttest-0.1.6/expecttest/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -281,20 +281,19 @@
         except exc_type as e:
             self.assertExpectedInline(str(e), expect, skip=1)
             return
         # Don't put this in the try block; the AssertionError will catch it
         self.fail(msg="Did not raise when expected to")
 
     def assertMultiLineEqualMaybeCppStack(self, expect: str, actual: str, *args: Any, **kwargs: Any) -> None:
+        cpp_stack_header = "\nException raised from"
+        if cpp_stack_header in actual:
+            actual = actual.rsplit(cpp_stack_header, maxsplit=1)[0]
         if hasattr(self, "assertMultiLineEqual"):
-            self.assertMultiLineEqual(expect, actual[:len(expect)], *args, **kwargs)
+            self.assertMultiLineEqual(expect, actual, *args, **kwargs)
         else:
-            self.assertEqual(expect, actual[:len(expect)], *args, **kwargs)
-        if len(actual) > len(expect):
-            cpp_stacktrace_header = "\nException raised from"
-            end_header = len(expect) + len(cpp_stacktrace_header)
-            self.assertEqual(actual[len(expect): end_header], cpp_stacktrace_header)
+            self.assertEqual(expect, actual, *args, **kwargs)
 
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `expecttest-0.1.5/pyproject.toml` & `expecttest-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "expecttest"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 readme = "README.md"
 repository = "https://github.com/ezyang/expecttest"
 authors = ["Edward Z. Yang <ezyang@mit.edu>"]
 include = ["expecttest/py.typed"]
 license = "MIT"
 classifiers = [
```

### Comparing `expecttest-0.1.5/setup.py` & `expecttest-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['expecttest']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'expecttest',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': '# expecttest [![PyPI version](https://badge.fury.io/py/expecttest.svg)](https://badge.fury.io/py/expecttest)\n\nThis library implements expect tests (also known as "golden" tests). Expect\ntests are a method of writing tests where instead of hard-coding the expected\noutput of a test, you run the test to get the output, and the test framework\nautomatically populates the expected output.  If the output of the test changes,\nyou can rerun the test with the environment variable `EXPECTTEST_ACCEPT=1` to\nautomatically update the expected output.\n\nSomewhat unusually, this library implements *inline* expect tests: that is to\nsay, the expected output isn\'t saved to an external file, it is saved directly\nin the Python file (and we modify your Python file when updating the expect\ntest.)\n\nThe general recipe for how to use this is as follows:\n\n  1. Write your test and use `assertExpectedInline()` instead of a normal\n     `assertEqual`.  Leave the expected argument blank with an empty string:\n     ```py\n     self.assertExpectedInline(some_func(), "")\n     ```\n\n  2. Run your test.  It should fail, and you get an error message about\n     accepting the output with `EXPECTTEST_ACCEPT=1`\n\n  3. Rerun the test with `EXPECTTEST_ACCEPT=1`.  Now the previously blank string\n     literal will contain the expected value of the test.\n     ```py\n     self.assertExpectedInline(some_func(), "my_value")\n     ```\n\nSome tips and tricks:\n\n  - Often, you will want to expect test on a multiline string.  This framework\n    understands triple-quoted strings, so you can just write `"""my_value"""`\n    and it will turn into triple-quoted strings.\n\n  - Take some time thinking about how exactly you want to design the output\n    format of the expect test.  It is often profitable to design an output\n    representation specifically for expect tests.\n',
     'author': 'Edward Z. Yang',
     'author_email': 'ezyang@mit.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ezyang/expecttest',
```

### Comparing `expecttest-0.1.5/PKG-INFO` & `expecttest-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expecttest
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/ezyang/expecttest
 License: MIT
 Author: Edward Z. Yang
 Author-email: ezyang@mit.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

