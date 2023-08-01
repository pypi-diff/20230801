# Comparing `tmp/jinjanator_plugins-23.2.1.tar.gz` & `tmp/jinjanator_plugins-23.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 31 13:23:07 2023, max compression
+gzip compressed data, last modified: Tue Aug  1 13:10:12 2023, max compression
```

## Comparing `jinjanator_plugins-23.2.1.tar` & `jinjanator_plugins-23.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1645 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/CHANGELOG.md
--rw-r--r--   0        0        0    10862 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/README.md
--rw-r--r--   0        0        0     1684 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/jinjanator_plugin_example.py
--rw-r--r--   0        0        0      599 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/pyproject.toml
--rw-r--r--   0        0        0     1144 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin.py
--rw-r--r--   0        0        0     1296 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery.py
--rw-r--r--   0        0        0     1321 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery_entrypoint.py
--rw-r--r--   0        0        0     3066 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/src/jinjanator_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/src/jinjanator_plugins/py.typed
--rw-r--r--   0        0        0       32 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/LICENSE
--rw-r--r--   0        0        0     6351 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/pyproject.toml
--rw-r--r--   0        0        0     9723 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11409 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/README.md
+-rw-r--r--   0        0        0     2063 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/jinjanator_plugin_example.py
+-rw-r--r--   0        0        0      599 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/pyproject.toml
+-rw-r--r--   0        0        0     1198 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin.py
+-rw-r--r--   0        0        0     1434 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin_discovery.py
+-rw-r--r--   0        0        0     1459 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin_discovery_entrypoint.py
+-rw-r--r--   0        0        0     4210 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/src/jinjanator_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/src/jinjanator_plugins/py.typed
+-rw-r--r--   0        0        0       32 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/LICENSE
+-rw-r--r--   0        0        0     6733 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10315 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/PKG-INFO
```

### Comparing `jinjanator_plugins-23.2.1/CHANGELOG.md` & `jinjanator_plugins-23.3.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator-plugins/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.3.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.3.0) - 2023-08-01
+
+### Changes
+
+- Improved format option exceptions to accept details and messages, and provide their own formatted output.
+
+
 ## [23.2.1](https://github.com/kpfleming/jinjanator-plugins/tree/23.2.1) - 2023-07-31
 
 ### Additions
 
 - Add documentation for features added in version 23.2.0.
```

### Comparing `jinjanator_plugins-23.2.1/README.md` & `jinjanator_plugins-23.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   "setuptools>=61",
 ]
 
 [project]
 name = "jinjanator-plugin-example"
 version = "0.0.0"
 dependencies = [
-  "jinjanator-plugins==23.1.0",
+  "jinjanator-plugins==23.3.0",
 ]
 
 [tool.setuptools]
 py-modules = ["jinjanator_plugin_example"]
 
 [project.entry-points.jinjanator]
 example = "jinjanator_plugin_example"
@@ -100,17 +100,17 @@
 
 The `name` and `version` are required to build a package containing
 the plugin. Note the *specific version dependency* on the
 `jinjanator-plugins` package.
 
 #### tool.setuptools
 
-This section tells `setuptools` to include a single source file (not a package
-directory) into the distribution. Note that this is a *module name*,
-not a *file name*, so there is no `.py` extension.
+This section tells `setuptools` to include a single source file (not a
+package directory) into the distribution. Note that this is a *module
+name*, not a *file name*, so there is no `.py` extension.
 
 #### project.entry-points.jinjanator
 
 This is the first part of the 'magic' mechanism which allows
 Jinjanator to find the plugin. The entry here (which can use any name,
 but should be related to the project name in order to avoid conflicts)
 creates an 'entry point' which Jinjanator can use to find the plugin;
@@ -139,36 +139,38 @@
     return codecs.encode(value, "rot13")
 
 
 def is_len12_test(value):
     return len(value) == 12
 
 
-def spam_format(data_string, options):
-    ham = False
+class SpamFormat:
+    @staticmethod
+    def parser(data_string, options):
+        ham = False
+
+        if options:
+            for option in options:
+                if option == "ham":
+                    ham = True
+
+        if ham:
+            return {
+                "ham": "ham",
+                "cheese": "ham and cheese",
+                "potatoes": "ham and potatoes",
+            }
 
-    if options:
-        for option in options:
-            if option == "ham":
-                ham = True
-            else:
-                raise FormatOptionUnknownError(option)
-
-    if ham:
         return {
-            "ham": "ham",
-            "cheese": "ham and cheese",
-            "potatoes": "ham and potatoes",
+            "spam": "spam",
+            "cheese": "spam and cheese",
+            "potatoes": "spam and potatoes",
         }
 
-    return {
-        "spam": "spam",
-        "cheese": "spam and cheese",
-        "potatoes": "spam and potatoes",
-    }
+    fmt = Format(name="spam", parser=parser, suffixes=[".spam"], options=["ham"])
 
 
 @plugin_identity_hook
 def plugin_identities():
     return "example"
 
 
@@ -180,43 +182,48 @@
 @plugin_tests_hook
 def plugin_tests():
     return {"len12": is_len12_test}
 
 
 @plugin_formats_hook
 def plugin_formats():
-    return {"spam": Format(parser=spam_format, suffixes=[".spam"])}
+    return {SpamFormat.fmt.name: SpamFormat.fmt}
 ```
 
 Note that the real example makes use of type annotations, but they
 have been removed here for simplicity.
 
 #### Imports
 
 The imports from `jinjanator_plugins` are necessary for the plugin to:
 * Mark the hooks it wishes to use to provide additional features.
-* Construct one (or more) `Format` objects to describe the formats it supports, if any.
+* Construct one (or more) `Format` objects to describe the formats it
+  supports, if any.
 * Raise option-related exceptions from its format function, if any.
 
 #### rot13_filter
 
 A simple filter function which applies the `rot13` transformation to
 the string value it receives.
 
 #### is_len12_test
 
 A simple test function which returns `True` if the value it receives
 has length 12.
 
-#### spam_format
+#### SpamFormat
 
-A simple format function which ignores the content provided (which
-Jinjanator would have read from a data file), and instead returns one
-of two canned responses based on whether the `ham` option has been
-provided by the user.
+A class providing a simple format function which ignores the content
+provided (which Jinjanator would have read from a data file), and
+instead returns one of two canned responses based on whether the `ham`
+option has been provided by the user.
+
+The `parser` static method is the function which does the work, and
+the `fmt` class variable is a `Format` object providing the details of
+the format.
 
 #### plugin_identities
 
 The hook function which will be called by Jinjanator to allow this
 plugin to identify itself; the `@plugin_identities_hook` decorator
 marks the function so that it will be found.
 
@@ -225,14 +232,17 @@
 and version, and can include versions of any packages on which it
 depends.
 
 This string will be included in the output generated by `jinjanate
 --version`, so it should not include any newlines or other formatting
 characters.
 
+Note that the function *must* be named `plugin_identities`; it is the
+second part of the 'magic' mechanism mentioned above.
+
 #### plugin_filters
 
 The hook function which will be called by Jinjanator to allow this
 plugin to register any filter functions it provides; the
 `@plugin_filters_hook` decorator marks the function so that it will be
 found.
 
@@ -265,33 +275,35 @@
 plugin to register any format functions it provides; the
 `@plugin_formats_hook` decorator marks the function so that it will be
 found.
 
 The function must return a dictionary, with each key being a format
 function name (the name which will be used in the `--format` argument
 to Jinjanator, if needed) and the corresponding value being a Format
-object containing a reference to the format function itself and an
-optional list of file suffixes which can be matched to this format
-during format auto-detection.
+object. That object contains the name of the format (for use in error
+messages), a reference to the format parser function, a (possibly
+empty) list of file suffixes which can be matched to this format
+during format auto-detection, and a (possibly empty) list of options
+which the user can provide to modify the parser's behavior.
 
 Note that the function *must* be named `plugin_formats`; it is the
 second part of the 'magic' mechanism mentioned above.
 
 Format functions can accept 'options' to modify their behavior, and
-should raise the exceptions listed below when needed to inform the
+should raise the exceptions listed below, when needed, to inform the
 user if one of the provided options does not meet the format's
 requirements.
 
-* `FormatOptionUnknownError` should be raised when a provided option
-  name is not valid.
+* `FormatOptionUnknownError` will be raised automatically by the
+  Jinjanator CLI based on the content of the `options` attribute of
+  the `Format` object.
 
 * `FormatOptionUnsupportedError` should be raised when a provided
   option is not supported in combination with the other provided
-  options; it should also be raised when options are provided to a
-  format which does not support options.
+  options or with the parsed data.
 
 * `FormatOptionValueError` should be raised when a provided option has
   a value that is not valid.
 <!-- fancy-readme end -->
 
 ## Chat
```

### Comparing `jinjanator_plugins-23.2.1/plugin_example/jinjanator_plugin_example.py` & `jinjanator_plugins-23.3.0/plugin_example/jinjanator_plugin_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,43 +24,51 @@
     return codecs.encode(value, "rot13")
 
 
 def is_len12_test(value: str) -> bool:
     return len(value) == 12  # noqa: PLR2004
 
 
-def spam_format(
-    data_string: str,  # noqa: ARG001
-    options: list[str] | None = None,
-) -> Mapping[str, str]:
-    ham = False
-
-    if options:
-        for option in options:
-            if option == "ham":
-                ham = True
-            elif option == "uns":
-                raise FormatOptionUnsupportedError(option)
-            elif option == "val":
-                raise FormatOptionValueError(option)
-            else:
-                raise FormatOptionUnknownError(option)
+class SpamFormat:
+    @staticmethod
+    def parser(
+        data_string: str,  # noqa: ARG004
+        options: list[str] | None = None,
+    ) -> Mapping[str, str]:
+        ham = False
+
+        if options:
+            for option in options:
+                if option == "ham":
+                    ham = True
+                elif option == "uns":
+                    raise FormatOptionUnsupportedError(
+                        SpamFormat.fmt, option, "is not supported"
+                    )
+                elif option == "val":
+                    raise FormatOptionValueError(
+                        SpamFormat.fmt, option, "", "is not valid"
+                    )
+                else:
+                    raise FormatOptionUnknownError(SpamFormat.fmt, option)
+
+        if ham:
+            return {
+                "ham": "ham",
+                "cheese": "ham and cheese",
+                "potatoes": "ham and potatoes",
+            }
 
-    if ham:
         return {
-            "ham": "ham",
-            "cheese": "ham and cheese",
-            "potatoes": "ham and potatoes",
+            "spam": "spam",
+            "cheese": "spam and cheese",
+            "potatoes": "spam and potatoes",
         }
 
-    return {
-        "spam": "spam",
-        "cheese": "spam and cheese",
-        "potatoes": "spam and potatoes",
-    }
+    fmt = Format(name="spam", parser=parser, suffixes=[".spam"], options=["ham"])
 
 
 @plugin_identity_hook
 def plugin_identities() -> Identity:
     return "example"
 
 
@@ -72,8 +80,8 @@
 @plugin_tests_hook
 def plugin_tests() -> Tests:
     return {"len12": is_len12_test}
 
 
 @plugin_formats_hook
 def plugin_formats() -> Formats:
-    return {"spam": Format(parser=spam_format, suffixes=[".spam"])}
+    return {f.name: f for f in [SpamFormat.fmt]}
```

### Comparing `jinjanator_plugins-23.2.1/plugin_example/pyproject.toml` & `jinjanator_plugins-23.3.0/plugin_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin.py` & `jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import jinjanator_plugin_example as plugin
+import jinjanator_plugin_example as plugin  # type: ignore[import]
 import pytest
 
 from jinjanator_plugins import (
     FormatOptionUnknownError,
     FormatOptionUnsupportedError,
     FormatOptionValueError,
 )
@@ -16,31 +16,31 @@
 
 def test_test() -> None:
     assert True is plugin.is_len12_test("Bartholomew1")
     assert False is plugin.is_len12_test("Bart")
 
 
 def test_format() -> None:
-    result = plugin.spam_format("", [])
+    result = plugin.SpamFormat.parser("", [])
     assert "cheese" in result
     assert "spam and cheese" == result["cheese"]
 
 
 def test_format_option() -> None:
-    result = plugin.spam_format("", ["ham"])
+    result = plugin.SpamFormat.parser("", ["ham"])
     assert "cheese" in result
     assert "ham and cheese" == result["cheese"]
 
 
 def test_format_option_unknown() -> None:
     with pytest.raises(FormatOptionUnknownError):
-        plugin.spam_format("", ["unk"])
+        plugin.SpamFormat.parser("", ["unk"])
 
 
 def test_format_option_unsupported() -> None:
     with pytest.raises(FormatOptionUnsupportedError):
-        plugin.spam_format("", ["uns"])
+        plugin.SpamFormat.parser("", ["uns"])
 
 
 def test_format_option_value() -> None:
     with pytest.raises(FormatOptionValueError):
-        plugin.spam_format("", ["val"])
+        plugin.SpamFormat.parser("", ["val"])
```

### Comparing `jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery.py` & `jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import cast
 
-import jinjanator_plugin_example as plugin
+import jinjanator_plugin_example as plugin  # type: ignore[import]
 import pluggy  # type: ignore[import]
 import pytest
 
 from jinjanator_plugins import (
     PluginHookCallers,
     PluginHooks,
 )
@@ -16,34 +16,35 @@
 def hook_callers() -> PluginHookCallers:
     pm = pluggy.PluginManager("jinjanator")
     pm.add_hookspecs(PluginHooks)
     pm.register(plugin)
     return cast(PluginHookCallers, pm.hook)
 
 
-def test_identity(hook_callers) -> None:
+def test_identity(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_identities()
     assert len(result) == 1
     assert "example" == result[0]
 
 
-def test_filter(hook_callers) -> None:
+def test_filter(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_filters()
     assert len(result) == 1
     assert "rot13" in result[0]
     assert plugin.rot13_filter == result[0]["rot13"]
 
 
-def test_test(hook_callers) -> None:
+def test_test(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_tests()
     assert len(result) == 1
     assert "len12" in result[0]
     assert plugin.is_len12_test == result[0]["len12"]
 
 
-def test_format(hook_callers) -> None:
+def test_format(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_formats()
     assert len(result) == 1
     assert "spam" in result[0]
-    assert plugin.spam_format == result[0]["spam"].parser
     assert len(result[0]["spam"].suffixes) == 1
     assert ".spam" == result[0]["spam"].suffixes[0]
+    assert len(result[0]["spam"].options) == 1
+    assert "ham" == result[0]["spam"].options[0]
```

### Comparing `jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery_entrypoint.py` & `jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin_discovery_entrypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import cast
 
-import jinjanator_plugin_example as plugin
+import jinjanator_plugin_example as plugin  # type: ignore[import]
 import pluggy  # type: ignore[import]
 import pytest
 
 from jinjanator_plugins import (
     PluginHookCallers,
     PluginHooks,
 )
@@ -16,34 +16,35 @@
 def hook_callers() -> PluginHookCallers:
     pm = pluggy.PluginManager("jinjanator")
     pm.add_hookspecs(PluginHooks)
     pm.load_setuptools_entrypoints("jinjanator")
     return cast(PluginHookCallers, pm.hook)
 
 
-def test_identity(hook_callers) -> None:
+def test_identity(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_identities()
     assert len(result) == 1
     assert "example" == result[0]
 
 
-def test_filter(hook_callers) -> None:
+def test_filter(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_filters()
     assert len(result) == 1
     assert "rot13" in result[0]
     assert plugin.rot13_filter == result[0]["rot13"]
 
 
-def test_test(hook_callers) -> None:
+def test_test(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_tests()
     assert len(result) == 1
     assert "len12" in result[0]
     assert plugin.is_len12_test == result[0]["len12"]
 
 
-def test_format(hook_callers) -> None:
+def test_format(hook_callers: PluginHookCallers) -> None:
     result = hook_callers.plugin_formats()
     assert len(result) == 1
     assert "spam" in result[0]
-    assert plugin.spam_format == result[0]["spam"].parser
     assert len(result[0]["spam"].suffixes) == 1
     assert ".spam" == result[0]["spam"].suffixes[0]
+    assert len(result[0]["spam"].options) == 1
+    assert "ham" == result[0]["spam"].options[0]
```

### Comparing `jinjanator_plugins-23.2.1/LICENSE` & `jinjanator_plugins-23.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.1/pyproject.toml` & `jinjanator_plugins-23.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -44,17 +44,19 @@
 skip-install = true
 dependencies = [
   "towncrier",
 ]
 
 [tool.hatch.envs.changelog.scripts]
 draft = [
+  "rm -f changelog.d/*~",
   "towncrier build --version main --draft",
 ]
 release = [
+  "rm -f changelog.d/*~",
   "towncrier build --yes --version {args}",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build]
@@ -84,26 +86,28 @@
     "ruff",
     "mypy",
     "pytest", # needed for type-checking plugin_example
 ]
 
 [tool.hatch.envs.lint.scripts]
 lint = [
-     "black --preview src plugin_example",
-     "ruff check --fix -- src plugin_example",
-     "mypy --package jinjanator_plugins",
-     "mypy plugin_example/*.py",
-     "shellcheck workflow-support/*.sh",
+    "black --preview src tests plugin_example",
+    "ruff check --fix -- src tests plugin_example",
+    "mypy --package jinjanator_plugins",
+    "mypy tests",
+    "mypy plugin_example",
+    "shellcheck workflow-support/*.sh",
 ]
 lint-action = [
-     "black --check --diff --preview src plugin_example",
-     "ruff check --format=github -- src plugin_example",
-     "mypy --package jinjanator_plugins",
-     "mypy plugin_example/*.py",
-     "shellcheck workflow-support/*.sh",
+    "black --check --diff --preview src tests plugin_example",
+    "ruff check --format=github -- src tests plugin_example",
+    "mypy --package jinjanator_plugins",
+    "mypy tests",
+    "mypy plugin_example",
+    "shellcheck workflow-support/*.sh",
 ]
 
 [tool.hatch.envs.ci]
 dependencies = [
     "coverage[toml]",
     "pytest",
     "pytest-cov",
@@ -130,15 +134,15 @@
 ]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
-# *jinjanator-plugins*: An API package for Jinjanator plugins
+# *jinjanator-plugins*: API package for Jinjanator plugins
 
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 start-after = "<!-- fancy-readme start -->"
 end-before = "<!-- fancy-readme end -->"
@@ -184,14 +188,21 @@
   "E501",     # leave line-length enforcement to Black
   "PLR0912",  # Leave complexity to me.
   "TRY301",   # Raise in try blocks can totally make sense.
 ]
 unfixable = ["F401"]
 
 [tool.ruff.per-file-ignores]
+"tests/*" = [
+  "INP001",  # we don't care that these are in implicit namespace packages
+  "PLC1901", # empty strings are falsey, but are less specific in tests
+  "PT005",   # we use always underscores and explicit names
+  "S101",    # assert
+  "SIM300",  # Yoda rocks in tests
+]
 "plugin_example/*" = [
   "INP001",  # we don't care that these are in implicit namespace packages
 ]
 "plugin_example/tests/*" = [
   "PLC1901", # empty strings are falsey, but are less specific in tests
   "PT005",   # we use always underscores and explicit names
   "S101",    # assert
@@ -202,14 +213,15 @@
 lines-between-types = 1
 lines-after-imports = 2
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 xfail_strict = true
 testpaths = [
+    "tests",
     "plugin_example/tests",
 ]
 addopts = [
     "-ra",
     "--strict-markers",
 ]
```

### Comparing `jinjanator_plugins-23.2.1/PKG-INFO` & `jinjanator_plugins-23.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator-plugins
-Version: 23.2.1
+Version: 23.3.0
 Summary: Package which provides the plugin API for the Jinjanator tool
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugins/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugins
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: pluggy
 Description-Content-Type: text/markdown
 
-# *jinjanator-plugins*: An API package for Jinjanator plugins
+# *jinjanator-plugins*: API package for Jinjanator plugins
 
 
 
 Jinjanator can be extended through the use of plugins; these are
 Python packages installed into the same environment as the tool
 itself, which use special markers to 'hook' into various
 features. There is a minimal example in the
@@ -86,15 +86,15 @@
   "setuptools>=61",
 ]
 
 [project]
 name = "jinjanator-plugin-example"
 version = "0.0.0"
 dependencies = [
-  "jinjanator-plugins==23.1.0",
+  "jinjanator-plugins==23.3.0",
 ]
 
 [tool.setuptools]
 py-modules = ["jinjanator_plugin_example"]
 
 [project.entry-points.jinjanator]
 example = "jinjanator_plugin_example"
@@ -109,17 +109,17 @@
 
 The `name` and `version` are required to build a package containing
 the plugin. Note the *specific version dependency* on the
 `jinjanator-plugins` package.
 
 #### tool.setuptools
 
-This section tells `setuptools` to include a single source file (not a package
-directory) into the distribution. Note that this is a *module name*,
-not a *file name*, so there is no `.py` extension.
+This section tells `setuptools` to include a single source file (not a
+package directory) into the distribution. Note that this is a *module
+name*, not a *file name*, so there is no `.py` extension.
 
 #### project.entry-points.jinjanator
 
 This is the first part of the 'magic' mechanism which allows
 Jinjanator to find the plugin. The entry here (which can use any name,
 but should be related to the project name in order to avoid conflicts)
 creates an 'entry point' which Jinjanator can use to find the plugin;
@@ -148,36 +148,38 @@
     return codecs.encode(value, "rot13")
 
 
 def is_len12_test(value):
     return len(value) == 12
 
 
-def spam_format(data_string, options):
-    ham = False
+class SpamFormat:
+    @staticmethod
+    def parser(data_string, options):
+        ham = False
+
+        if options:
+            for option in options:
+                if option == "ham":
+                    ham = True
+
+        if ham:
+            return {
+                "ham": "ham",
+                "cheese": "ham and cheese",
+                "potatoes": "ham and potatoes",
+            }
 
-    if options:
-        for option in options:
-            if option == "ham":
-                ham = True
-            else:
-                raise FormatOptionUnknownError(option)
-
-    if ham:
         return {
-            "ham": "ham",
-            "cheese": "ham and cheese",
-            "potatoes": "ham and potatoes",
+            "spam": "spam",
+            "cheese": "spam and cheese",
+            "potatoes": "spam and potatoes",
         }
 
-    return {
-        "spam": "spam",
-        "cheese": "spam and cheese",
-        "potatoes": "spam and potatoes",
-    }
+    fmt = Format(name="spam", parser=parser, suffixes=[".spam"], options=["ham"])
 
 
 @plugin_identity_hook
 def plugin_identities():
     return "example"
 
 
@@ -189,43 +191,48 @@
 @plugin_tests_hook
 def plugin_tests():
     return {"len12": is_len12_test}
 
 
 @plugin_formats_hook
 def plugin_formats():
-    return {"spam": Format(parser=spam_format, suffixes=[".spam"])}
+    return {SpamFormat.fmt.name: SpamFormat.fmt}
 ```
 
 Note that the real example makes use of type annotations, but they
 have been removed here for simplicity.
 
 #### Imports
 
 The imports from `jinjanator_plugins` are necessary for the plugin to:
 * Mark the hooks it wishes to use to provide additional features.
-* Construct one (or more) `Format` objects to describe the formats it supports, if any.
+* Construct one (or more) `Format` objects to describe the formats it
+  supports, if any.
 * Raise option-related exceptions from its format function, if any.
 
 #### rot13_filter
 
 A simple filter function which applies the `rot13` transformation to
 the string value it receives.
 
 #### is_len12_test
 
 A simple test function which returns `True` if the value it receives
 has length 12.
 
-#### spam_format
+#### SpamFormat
 
-A simple format function which ignores the content provided (which
-Jinjanator would have read from a data file), and instead returns one
-of two canned responses based on whether the `ham` option has been
-provided by the user.
+A class providing a simple format function which ignores the content
+provided (which Jinjanator would have read from a data file), and
+instead returns one of two canned responses based on whether the `ham`
+option has been provided by the user.
+
+The `parser` static method is the function which does the work, and
+the `fmt` class variable is a `Format` object providing the details of
+the format.
 
 #### plugin_identities
 
 The hook function which will be called by Jinjanator to allow this
 plugin to identify itself; the `@plugin_identities_hook` decorator
 marks the function so that it will be found.
 
@@ -234,14 +241,17 @@
 and version, and can include versions of any packages on which it
 depends.
 
 This string will be included in the output generated by `jinjanate
 --version`, so it should not include any newlines or other formatting
 characters.
 
+Note that the function *must* be named `plugin_identities`; it is the
+second part of the 'magic' mechanism mentioned above.
+
 #### plugin_filters
 
 The hook function which will be called by Jinjanator to allow this
 plugin to register any filter functions it provides; the
 `@plugin_filters_hook` decorator marks the function so that it will be
 found.
 
@@ -274,37 +284,39 @@
 plugin to register any format functions it provides; the
 `@plugin_formats_hook` decorator marks the function so that it will be
 found.
 
 The function must return a dictionary, with each key being a format
 function name (the name which will be used in the `--format` argument
 to Jinjanator, if needed) and the corresponding value being a Format
-object containing a reference to the format function itself and an
-optional list of file suffixes which can be matched to this format
-during format auto-detection.
+object. That object contains the name of the format (for use in error
+messages), a reference to the format parser function, a (possibly
+empty) list of file suffixes which can be matched to this format
+during format auto-detection, and a (possibly empty) list of options
+which the user can provide to modify the parser's behavior.
 
 Note that the function *must* be named `plugin_formats`; it is the
 second part of the 'magic' mechanism mentioned above.
 
 Format functions can accept 'options' to modify their behavior, and
-should raise the exceptions listed below when needed to inform the
+should raise the exceptions listed below, when needed, to inform the
 user if one of the provided options does not meet the format's
 requirements.
 
-* `FormatOptionUnknownError` should be raised when a provided option
-  name is not valid.
+* `FormatOptionUnknownError` will be raised automatically by the
+  Jinjanator CLI based on the content of the `options` attribute of
+  the `Format` object.
 
 * `FormatOptionUnsupportedError` should be raised when a provided
   option is not supported in combination with the other provided
-  options; it should also be raised when options are provided to a
-  format which does not support options.
+  options or with the parsed data.
 
 * `FormatOptionValueError` should be raised when a provided option has
   a value that is not valid.
 ## Release Information
-### Additions
+### Changes
 
-- Add documentation for features added in version 23.2.0.
+- Improved format option exceptions to accept details and messages, and provide their own formatted output.
 
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugins/blob/main/CHANGELOG.md)
```

