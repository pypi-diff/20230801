# Comparing `tmp/jinjanator_plugins-23.3.0.tar.gz` & `tmp/jinjanator_plugins-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Aug  1 13:10:12 2023, max compression
+gzip compressed data, last modified: Tue Aug  1 19:40:18 2023, max compression
```

## Comparing `jinjanator_plugins-23.3.0.tar` & `jinjanator_plugins-23.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1855 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    11409 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/README.md
--rw-r--r--   0        0        0     2063 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/jinjanator_plugin_example.py
--rw-r--r--   0        0        0      599 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/pyproject.toml
--rw-r--r--   0        0        0     1198 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin.py
--rw-r--r--   0        0        0     1434 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin_discovery.py
--rw-r--r--   0        0        0     1459 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin_discovery_entrypoint.py
--rw-r--r--   0        0        0     4210 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/src/jinjanator_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/src/jinjanator_plugins/py.typed
--rw-r--r--   0        0        0       32 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/LICENSE
--rw-r--r--   0        0        0     6733 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/pyproject.toml
--rw-r--r--   0        0        0    10315 2023-08-01 13:10:12.000000 jinjanator_plugins-23.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2144 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    12087 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/README.md
+-rw-r--r--   0        0        0     1996 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/plugin_example/jinjanator_plugin_example.py
+-rw-r--r--   0        0        0      599 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/plugin_example/pyproject.toml
+-rw-r--r--   0        0        0     1163 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/plugin_example/tests/test_plugin.py
+-rw-r--r--   0        0        0     1887 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/plugin_example/tests/test_plugin_discovery.py
+-rw-r--r--   0        0        0     1845 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/plugin_example/tests/test_plugin_discovery_entrypoint.py
+-rw-r--r--   0        0        0     4405 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/src/jinjanator_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/src/jinjanator_plugins/py.typed
+-rw-r--r--   0        0        0       32 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/LICENSE
+-rw-r--r--   0        0        0     6697 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11190 2023-08-01 19:40:18.000000 jinjanator_plugins-23.4.0/PKG-INFO
```

### Comparing `jinjanator_plugins-23.3.0/CHANGELOG.md` & `jinjanator_plugins-23.4.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator-plugins/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.4.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.4.0) - 2023-08-01
+
+### Backwards-incompatible Changes
+
+- Major redesign of the 'formats' API; formats are now classes and can store data for their needs.
+  [#4](https://github.com/kpfleming/jinjanator-plugins/issues/4)
+
+
 ## [23.3.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.3.0) - 2023-08-01
 
 ### Changes
 
 - Improved format option exceptions to accept details and messages, and provide their own formatted output.
```

### Comparing `jinjanator_plugins-23.3.0/README.md` & `jinjanator_plugins-23.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -120,15 +120,14 @@
 
 ### jinjanator_plugin_example.py
 
 ```python
 import codecs
 
 from jinjanator_plugins import (
-    Format,
     FormatOptionUnknownError,
     FormatOptionUnsupportedError,
     FormatOptionValueError,
     plugin_filters_hook,
     plugin_formats_hook,
     plugin_identity_hook,
     plugin_tests_hook,
@@ -140,38 +139,40 @@
 
 
 def is_len12_test(value):
     return len(value) == 12
 
 
 class SpamFormat:
-    @staticmethod
-    def parser(data_string, options):
-        ham = False
+    name = "spam"
+    suffixes = (".spam",)
+    option_names = ("ham",)
+
+    def __init__(self, options):
+        self.ham = False
 
         if options:
             for option in options:
                 if option == "ham":
-                    ham = True
+                    self.ham = True
 
-        if ham:
+    def parse(self, data_string):
+        if self.ham:
             return {
                 "ham": "ham",
                 "cheese": "ham and cheese",
                 "potatoes": "ham and potatoes",
             }
 
         return {
             "spam": "spam",
             "cheese": "spam and cheese",
             "potatoes": "spam and potatoes",
         }
 
-    fmt = Format(name="spam", parser=parser, suffixes=[".spam"], options=["ham"])
-
 
 @plugin_identity_hook
 def plugin_identities():
     return "example"
 
 
 @plugin_filters_hook
@@ -182,15 +183,15 @@
 @plugin_tests_hook
 def plugin_tests():
     return {"len12": is_len12_test}
 
 
 @plugin_formats_hook
 def plugin_formats():
-    return {SpamFormat.fmt.name: SpamFormat.fmt}
+    return {SpamFormat.name: SpamFormat}
 ```
 
 Note that the real example makes use of type annotations, but they
 have been removed here for simplicity.
 
 #### Imports
 
@@ -213,17 +214,17 @@
 #### SpamFormat
 
 A class providing a simple format function which ignores the content
 provided (which Jinjanator would have read from a data file), and
 instead returns one of two canned responses based on whether the `ham`
 option has been provided by the user.
 
-The `parser` static method is the function which does the work, and
-the `fmt` class variable is a `Format` object providing the details of
-the format.
+The `parse` method is the function which does the work; the `__init__`
+method handles options provided by the user; the class attributes
+provide details of the format.
 
 #### plugin_identities
 
 The hook function which will be called by Jinjanator to allow this
 plugin to identify itself; the `@plugin_identities_hook` decorator
 marks the function so that it will be found.
 
@@ -274,32 +275,50 @@
 The hook function which will be called by Jinjanator to allow this
 plugin to register any format functions it provides; the
 `@plugin_formats_hook` decorator marks the function so that it will be
 found.
 
 The function must return a dictionary, with each key being a format
 function name (the name which will be used in the `--format` argument
-to Jinjanator, if needed) and the corresponding value being a Format
-object. That object contains the name of the format (for use in error
-messages), a reference to the format parser function, a (possibly
-empty) list of file suffixes which can be matched to this format
-during format auto-detection, and a (possibly empty) list of options
-which the user can provide to modify the parser's behavior.
+to Jinjanator, if needed) and the corresponding value being a class
+which implements the requirements of the `Format` protocol (defined in
+[__init__.py](src/jinjanator-plugins/__init__.py)).
+
+In particular these requirements include:
+
+* a class attribute called `name` which contains the name of the
+  format (for use in error messages)
+
+* a class attribute called 'suffixes' which contains a (possibly
+  empty) list of file suffixes which can be matched to this format
+  during format auto-detection
+
+* a class attribute called 'option_names' which contains a (possibly
+  empty) list of options which the user can provide to modify the
+  parser's behavior
+
+* a constructor method (`__init__`) which accepts a (possibly empty)
+  list of options provided by the user, and performs any validation
+  needed on them, storing the results in the `self` object
+
+* a `parse` method which accepts a (possibly empty) string containing
+  the input data, and parses it according to the format's needs, using
+  any previously-validated options stored in the `self` object
 
-Note that the function *must* be named `plugin_formats`; it is the
+Note that the hook function *must* be named `plugin_formats`; it is the
 second part of the 'magic' mechanism mentioned above.
 
-Format functions can accept 'options' to modify their behavior, and
+Format classes can accept 'options' to modify their behavior, and
 should raise the exceptions listed below, when needed, to inform the
 user if one of the provided options does not meet the format's
 requirements.
 
 * `FormatOptionUnknownError` will be raised automatically by the
-  Jinjanator CLI based on the content of the `options` attribute of
-  the `Format` object.
+  Jinjanator CLI based on the content of the `option_names` attribute of
+  the format class.
 
 * `FormatOptionUnsupportedError` should be raised when a provided
   option is not supported in combination with the other provided
   options or with the parsed data.
 
 * `FormatOptionValueError` should be raised when a provided option has
   a value that is not valid.
```

### Comparing `jinjanator_plugins-23.3.0/plugin_example/jinjanator_plugin_example.py` & `jinjanator_plugins-23.4.0/plugin_example/jinjanator_plugin_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import codecs
 
-from typing import Mapping
+from typing import Iterable, Mapping
 
 from jinjanator_plugins import (
     Filters,
-    Format,
     FormatOptionUnknownError,
     FormatOptionUnsupportedError,
     FormatOptionValueError,
     Formats,
     Identity,
     Tests,
     plugin_filters_hook,
@@ -25,51 +24,49 @@
 
 
 def is_len12_test(value: str) -> bool:
     return len(value) == 12  # noqa: PLR2004
 
 
 class SpamFormat:
-    @staticmethod
-    def parser(
-        data_string: str,  # noqa: ARG004
-        options: list[str] | None = None,
-    ) -> Mapping[str, str]:
-        ham = False
+    name = "spam"
+    suffixes: Iterable[str] | None = (".spam",)
+    option_names: Iterable[str] | None = ("ham",)
+
+    def __init__(self, options: Iterable[str] | None) -> None:
+        self.ham = False
 
         if options:
             for option in options:
                 if option == "ham":
-                    ham = True
+                    self.ham = True
                 elif option == "uns":
-                    raise FormatOptionUnsupportedError(
-                        SpamFormat.fmt, option, "is not supported"
-                    )
+                    raise FormatOptionUnsupportedError(self, option, "is not supported")
                 elif option == "val":
-                    raise FormatOptionValueError(
-                        SpamFormat.fmt, option, "", "is not valid"
-                    )
+                    raise FormatOptionValueError(self, option, "", "is not valid")
                 else:
-                    raise FormatOptionUnknownError(SpamFormat.fmt, option)
+                    raise FormatOptionUnknownError(self, option)
 
-        if ham:
+    def parse(
+        self,
+        data_string: str,  # noqa: ARG002
+    ) -> Mapping[str, str]:
+        if self.ham:
             return {
                 "ham": "ham",
                 "cheese": "ham and cheese",
                 "potatoes": "ham and potatoes",
             }
 
         return {
             "spam": "spam",
             "cheese": "spam and cheese",
             "potatoes": "spam and potatoes",
         }
 
-    fmt = Format(name="spam", parser=parser, suffixes=[".spam"], options=["ham"])
-
 
 @plugin_identity_hook
 def plugin_identities() -> Identity:
     return "example"
 
 
 @plugin_filters_hook
@@ -80,8 +77,8 @@
 @plugin_tests_hook
 def plugin_tests() -> Tests:
     return {"len12": is_len12_test}
 
 
 @plugin_formats_hook
 def plugin_formats() -> Formats:
-    return {f.name: f for f in [SpamFormat.fmt]}
+    return {SpamFormat.name: SpamFormat}
```

### Comparing `jinjanator_plugins-23.3.0/plugin_example/pyproject.toml` & `jinjanator_plugins-23.4.0/plugin_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.3.0/plugin_example/tests/test_plugin.py` & `jinjanator_plugins-23.4.0/plugin_example/tests/test_plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 
 def test_test() -> None:
     assert True is plugin.is_len12_test("Bartholomew1")
     assert False is plugin.is_len12_test("Bart")
 
 
 def test_format() -> None:
-    result = plugin.SpamFormat.parser("", [])
+    result = plugin.SpamFormat([]).parse("")
     assert "cheese" in result
     assert "spam and cheese" == result["cheese"]
 
 
 def test_format_option() -> None:
-    result = plugin.SpamFormat.parser("", ["ham"])
+    result = plugin.SpamFormat(["ham"]).parse("")
     assert "cheese" in result
     assert "ham and cheese" == result["cheese"]
 
 
 def test_format_option_unknown() -> None:
     with pytest.raises(FormatOptionUnknownError):
-        plugin.SpamFormat.parser("", ["unk"])
+        plugin.SpamFormat(["unk"])
 
 
 def test_format_option_unsupported() -> None:
     with pytest.raises(FormatOptionUnsupportedError):
-        plugin.SpamFormat.parser("", ["uns"])
+        plugin.SpamFormat(["uns"])
 
 
 def test_format_option_value() -> None:
     with pytest.raises(FormatOptionValueError):
-        plugin.SpamFormat.parser("", ["val"])
+        plugin.SpamFormat(["val"])
```

### Comparing `jinjanator_plugins-23.3.0/src/jinjanator_plugins/__init__.py` & `jinjanator_plugins-23.4.0/src/jinjanator_plugins/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Iterable,
     Mapping,
     Protocol,
-    Sequence,
+    Type,
     TypeVar,
     cast,
 )
 
 import pluggy  # type: ignore[import]
 
-from attrs import define
-
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing_extensions import TypeAlias
 
 
-@define(kw_only=True)
-class Format:
+class Format(Protocol):
     name: str
-    parser: Callable[[str, list[str] | None], Mapping[str, Any]]
-    suffixes: list[str]
-    options: list[str]
+    suffixes: Iterable[str] | None
+    option_names: Iterable[str] | None
+
+    def __init__(self, options: Iterable[str] | None) -> None:
+        ...  # pragma: no cover
+
+    def parse(self, data_string: str) -> Mapping[str, Any]:
+        ...  # pragma: no cover
 
 
 class FormatOptionUnknownError(Exception):
-    def __init__(self, fmt: Format, option: str):
+    def __init__(self, fmt: type[Format] | Format, option: str):
         self.fmt = fmt
         self.option = option
 
     def __str__(self) -> str:
-        if len(self.fmt.options) > 0:
+        if self.fmt.option_names:
             return (
                 f"Format {self.fmt.name}: option '{self.option}' is not valid; valid"
-                f" options are '{', '.join(self.fmt.options)}'"
+                f" options are '{', '.join(self.fmt.option_names)}'"
             )
 
         return (
             f"Format {self.fmt.name}: option '{self.option}' is not valid; this format"
             " does not accept any options."
         )
 
 
 class FormatOptionUnsupportedError(Exception):
-    def __init__(self, fmt: Format, option: str, message: str):
+    def __init__(self, fmt: type[Format] | Format, option: str, message: str):
         self.fmt = fmt
         self.option = option
         self.message = message
 
     def __str__(self) -> str:
         return f"Format {self.fmt.name}: option '{self.option}' {self.message}."
 
 
 class FormatOptionValueError(Exception):
-    def __init__(self, fmt: Format, option: str, value: str, message: str):
+    def __init__(self, fmt: type[Format] | Format, option: str, value: str, message: str):
         self.fmt = fmt
         self.option = option
         self.message = message
         self.value = value
 
     def __str__(self) -> str:
         return (
@@ -70,15 +73,15 @@
         )
 
 
 F = TypeVar("F", bound=Callable[..., Any])
 hookspec = cast(Callable[[F], F], pluggy.HookspecMarker("jinjanator"))
 
 Identity: TypeAlias = str
-Formats: TypeAlias = Mapping[str, Format]
+Formats: TypeAlias = Mapping[str, Type[Format]]
 Filters: TypeAlias = Mapping[str, Callable[..., Any]]
 Globals: TypeAlias = Mapping[str, Callable[..., Any]]
 Tests: TypeAlias = Mapping[str, Callable[..., Any]]
 
 PluginIdentityHook: TypeAlias = Callable[[], Identity]
 PluginFormatsHook: TypeAlias = Callable[[], Formats]
 PluginFiltersHook: TypeAlias = Callable[[], Filters]
@@ -132,25 +135,25 @@
     @hookspec
     def plugin_tests() -> Tests:
         """Returns dict of test functions"""
 
 
 class PluginHookCallers(Protocol):
     @staticmethod
-    def plugin_identities() -> Sequence[Identity]:
-        """Returns list of strings of identities"""
+    def plugin_identities() -> Iterable[Identity]:
+        """Returns iterable of strings of identities"""
 
     @staticmethod
-    def plugin_formats() -> Sequence[Formats]:
-        """Returns list of dicts of formats"""
+    def plugin_formats() -> Iterable[Formats]:
+        """Returns iterable of dicts of formats"""
 
     @staticmethod
-    def plugin_filters() -> Sequence[Filters]:
-        """Returns list of dicts of filter functions"""
+    def plugin_filters() -> Iterable[Filters]:
+        """Returns iterable of dicts of filter functions"""
 
     @staticmethod
-    def plugin_globals() -> Sequence[Globals]:
-        """Returns list of dicts of global functions"""
+    def plugin_globals() -> Iterable[Globals]:
+        """Returns iterable of dicts of global functions"""
 
     @staticmethod
-    def plugin_tests() -> Sequence[Tests]:
-        """Returns list of dicts of test functions"""
+    def plugin_tests() -> Iterable[Tests]:
+        """Returns iterable of dicts of test functions"""
```

### Comparing `jinjanator_plugins-23.3.0/LICENSE` & `jinjanator_plugins-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.3.0/pyproject.toml` & `jinjanator_plugins-23.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -123,18 +123,16 @@
 "3.12",
 ]
 
 [tool.hatch.envs.ci.scripts]
 ci = [
     "pip install ./plugin_example",
     "rm -f .coverage",
-    # run tests
-    "pytest --verbose --cov-append  --cov-branch --cov-fail-under=100 --cov=jinjanator_plugins",
-    # produce a coverage report with 'missing' lines indicated
-    "coverage report -m",
+    "pytest --verbose --cov-append  --cov-branch --cov=jinjanator_plugins",
+    "coverage report --show-missing --fail-under=100",
 ]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
@@ -239,14 +237,15 @@
 follow_imports = "normal"
 no_implicit_optional = true
 strict_equality = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_ignores = true
+exclude = ['plugin_example/build']
 
 [tool.towncrier]
 name = "jinjanator-plugins"
 package = "jinjanator_plugins"
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
```

### Comparing `jinjanator_plugins-23.3.0/PKG-INFO` & `jinjanator_plugins-23.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator-plugins
-Version: 23.3.0
+Version: 23.4.0
 Summary: Package which provides the plugin API for the Jinjanator tool
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugins/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugins
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -129,15 +129,14 @@
 
 ### jinjanator_plugin_example.py
 
 ```python
 import codecs
 
 from jinjanator_plugins import (
-    Format,
     FormatOptionUnknownError,
     FormatOptionUnsupportedError,
     FormatOptionValueError,
     plugin_filters_hook,
     plugin_formats_hook,
     plugin_identity_hook,
     plugin_tests_hook,
@@ -149,38 +148,40 @@
 
 
 def is_len12_test(value):
     return len(value) == 12
 
 
 class SpamFormat:
-    @staticmethod
-    def parser(data_string, options):
-        ham = False
+    name = "spam"
+    suffixes = (".spam",)
+    option_names = ("ham",)
+
+    def __init__(self, options):
+        self.ham = False
 
         if options:
             for option in options:
                 if option == "ham":
-                    ham = True
+                    self.ham = True
 
-        if ham:
+    def parse(self, data_string):
+        if self.ham:
             return {
                 "ham": "ham",
                 "cheese": "ham and cheese",
                 "potatoes": "ham and potatoes",
             }
 
         return {
             "spam": "spam",
             "cheese": "spam and cheese",
             "potatoes": "spam and potatoes",
         }
 
-    fmt = Format(name="spam", parser=parser, suffixes=[".spam"], options=["ham"])
-
 
 @plugin_identity_hook
 def plugin_identities():
     return "example"
 
 
 @plugin_filters_hook
@@ -191,15 +192,15 @@
 @plugin_tests_hook
 def plugin_tests():
     return {"len12": is_len12_test}
 
 
 @plugin_formats_hook
 def plugin_formats():
-    return {SpamFormat.fmt.name: SpamFormat.fmt}
+    return {SpamFormat.name: SpamFormat}
 ```
 
 Note that the real example makes use of type annotations, but they
 have been removed here for simplicity.
 
 #### Imports
 
@@ -222,17 +223,17 @@
 #### SpamFormat
 
 A class providing a simple format function which ignores the content
 provided (which Jinjanator would have read from a data file), and
 instead returns one of two canned responses based on whether the `ham`
 option has been provided by the user.
 
-The `parser` static method is the function which does the work, and
-the `fmt` class variable is a `Format` object providing the details of
-the format.
+The `parse` method is the function which does the work; the `__init__`
+method handles options provided by the user; the class attributes
+provide details of the format.
 
 #### plugin_identities
 
 The hook function which will be called by Jinjanator to allow this
 plugin to identify itself; the `@plugin_identities_hook` decorator
 marks the function so that it will be found.
 
@@ -283,40 +284,59 @@
 The hook function which will be called by Jinjanator to allow this
 plugin to register any format functions it provides; the
 `@plugin_formats_hook` decorator marks the function so that it will be
 found.
 
 The function must return a dictionary, with each key being a format
 function name (the name which will be used in the `--format` argument
-to Jinjanator, if needed) and the corresponding value being a Format
-object. That object contains the name of the format (for use in error
-messages), a reference to the format parser function, a (possibly
-empty) list of file suffixes which can be matched to this format
-during format auto-detection, and a (possibly empty) list of options
-which the user can provide to modify the parser's behavior.
+to Jinjanator, if needed) and the corresponding value being a class
+which implements the requirements of the `Format` protocol (defined in
+[__init__.py](https://github.com/kpfleming/jinjanator-plugins/tree/main/src/jinjanator-plugins/__init__.py)).
+
+In particular these requirements include:
+
+* a class attribute called `name` which contains the name of the
+  format (for use in error messages)
+
+* a class attribute called 'suffixes' which contains a (possibly
+  empty) list of file suffixes which can be matched to this format
+  during format auto-detection
+
+* a class attribute called 'option_names' which contains a (possibly
+  empty) list of options which the user can provide to modify the
+  parser's behavior
+
+* a constructor method (`__init__`) which accepts a (possibly empty)
+  list of options provided by the user, and performs any validation
+  needed on them, storing the results in the `self` object
+
+* a `parse` method which accepts a (possibly empty) string containing
+  the input data, and parses it according to the format's needs, using
+  any previously-validated options stored in the `self` object
 
-Note that the function *must* be named `plugin_formats`; it is the
+Note that the hook function *must* be named `plugin_formats`; it is the
 second part of the 'magic' mechanism mentioned above.
 
-Format functions can accept 'options' to modify their behavior, and
+Format classes can accept 'options' to modify their behavior, and
 should raise the exceptions listed below, when needed, to inform the
 user if one of the provided options does not meet the format's
 requirements.
 
 * `FormatOptionUnknownError` will be raised automatically by the
-  Jinjanator CLI based on the content of the `options` attribute of
-  the `Format` object.
+  Jinjanator CLI based on the content of the `option_names` attribute of
+  the format class.
 
 * `FormatOptionUnsupportedError` should be raised when a provided
   option is not supported in combination with the other provided
   options or with the parsed data.
 
 * `FormatOptionValueError` should be raised when a provided option has
   a value that is not valid.
 ## Release Information
-### Changes
+### Backwards-incompatible Changes
 
-- Improved format option exceptions to accept details and messages, and provide their own formatted output.
+- Major redesign of the 'formats' API; formats are now classes and can store data for their needs.
+  [[#4](https://github.com/kpfleming/jinjanator-plugins/issues/4)](https://github.com/kpfleming/jinjanator-plugins/issues/4)
 
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugins/blob/main/CHANGELOG.md)
```

