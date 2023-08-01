# Comparing `tmp/mkdocs_include_markdown_plugin-4.0.4.tar.gz` & `tmp/mkdocs_include_markdown_plugin-5.0.0.tar.gz`

## Comparing `mkdocs_include_markdown_plugin-4.0.4.tar` & `mkdocs_include_markdown_plugin-5.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/__init__.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/config.py
--rw-r--r--   0        0        0    25770 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/event.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/files_watcher.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/plugin.py
--rw-r--r--   0        0        0    13050 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/py.typed
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/regexes.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/.gitignore
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/LICENSE
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/README.md
--rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/pyproject.toml
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/__init__.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/cache.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/config.py
+-rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/event.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/files_watcher.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/plugin.py
+-rw-r--r--   0        0        0    13050 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/py.typed
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/regexes.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/.gitignore
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/LICENSE
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/README.md
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/PKG-INFO
```

### Comparing `mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/config.py` & `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'opening_tag': DEFAULT_OPENING_TAG,
     'closing_tag': DEFAULT_CLOSING_TAG,
     'encoding': 'utf-8',
     'preserve_includer_indent': True,
     'dedent': False,
     'trailing_newlines': True,
     'comments': DEFAULT_COMMENTS,
+    'cache': 0,
 }
 
 CONFIG_SCHEME = (
     (
         'opening_tag',
         MkType(str, default=DEFAULT_OPENING_TAG),
     ),
@@ -48,14 +49,18 @@
         'trailing_newlines',
         MkType(bool, default=CONFIG_DEFAULTS['trailing_newlines']),
     ),
     (
         'comments',
         MkType(bool, default=DEFAULT_COMMENTS),
     ),
+    (
+        'cache',
+        MkType(int, default=CONFIG_DEFAULTS['cache']),
+    ),
 )
 
 
 def create_include_tag(
     opening_tag: str, closing_tag: str, tag: str = 'include',
 ) -> re.Pattern[str]:
     """Create a regex pattern to match an inclusion tag directive.
```

### Comparing `mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/event.py` & `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,23 @@
 
 import glob
 import html
 import logging
 import os
 import re
 import textwrap
+import urllib.request
 from collections.abc import MutableMapping
 from typing import TYPE_CHECKING, Any
+from urllib.parse import urlparse
+
+from mkdocs.exceptions import BuildError
 
 from mkdocs_include_markdown_plugin import process
+from mkdocs_include_markdown_plugin.cache import Cache
 from mkdocs_include_markdown_plugin.config import (
     CONFIG_DEFAULTS,
     DEFAULT_CLOSING_TAG,
     DEFAULT_COMMENTS,
     DEFAULT_OPENING_TAG,
     create_include_tag,
 )
@@ -23,20 +28,15 @@
 from mkdocs_include_markdown_plugin.regexes import (
     DOUBLE_QUOTED_STR_RE,
     SINGLE_QUOTED_STR_RE,
 )
 
 
 if TYPE_CHECKING:  # remove this for mypyc compiling
-    import sys
-
-    if sys.version_info >= (3, 8):
-        from typing import TypedDict
-    else:
-        from typing_extensions import TypedDict
+    from typing import TypedDict
 
     from mkdocs.structure.pages import Page
 
     class DirectiveBoolArgument(TypedDict):  # noqa: D101
         value: bool
         regex: re.Pattern[str]
 
@@ -50,14 +50,23 @@
 
 TRUE_FALSE_BOOL_STR = {
     True: 'true',
     False: 'false',
 }
 
 
+def is_url(string: str) -> bool:
+    """Determines if a string is a URL."""
+    try:
+        result = urlparse(string)
+        return all([result.scheme, result.netloc])
+    except ValueError:
+        return False
+
+
 def bool_arg(arg: str) -> re.Pattern[str]:
     """Return a compiled regexp to match a boolean argument."""
     return re.compile(rf'{arg}=(\w+)')
 
 
 def str_arg(arg: str) -> re.Pattern[str]:
     """Return a compiled regexp to match a string argument."""
@@ -120,51 +129,67 @@
 
 def read_file(file_path: str, encoding: str) -> str:
     """Read a file and return its content."""
     with open(file_path, encoding=encoding) as f:
         return f.read()
 
 
+def read_http(target_url: str, http_cache: Cache | None) -> Any:  # noqa: U100
+    """Read an http location and return its content."""
+    if http_cache is not None:
+        cached_content = http_cache.get_(target_url)
+        if cached_content is not None:
+            return cached_content
+    req = urllib.request.Request(target_url)
+    with urllib.request.urlopen(req) as response:
+        content = response.read().decode('UTF-8')
+    if http_cache is not None:
+        http_cache.set_(target_url, content)
+    return content
+
+
 def get_file_content(
     markdown: str,
     page_src_path: str,
     docs_dir: str,
     include_tag_regex: re.Pattern[str],
     include_markdown_tag_regex: re.Pattern[str],
     default_encoding: str,
     default_preserve_includer_indent: bool,
     default_dedent: bool,
     default_trailing_newlines: bool,
     default_comments: bool = DEFAULT_COMMENTS,
     cumulative_heading_offset: int = 0,
     files_watcher: FilesWatcher | None = None,
+    http_cache: Cache | None = None,
 ) -> str:
     """Return the content of the file to include."""
     def found_include_tag(match: re.Match[str]) -> str:
         directive_match_start = match.start()
 
         _includer_indent = match.group('_includer_indent')
 
         filename, raw_filename = parse_filename_argument(match)
         if filename is None:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
-            logger.error(
+            raise BuildError(
                 "Found no path passed including with 'include'"
                 f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
-            return ''
 
         arguments_string = match.group('arguments')
 
         if os.path.isabs(filename):
             file_path_glob = filename
+        elif is_url(filename):
+            file_path_glob = filename
         else:
             file_path_glob = os.path.join(
                 os.path.abspath(os.path.dirname(page_src_path)),
                 filename,
             )
 
         exclude_match = ARGUMENT_REGEXES['exclude'].search(arguments_string)
@@ -173,19 +198,18 @@
         else:
             exclude_string = parse_string_argument(exclude_match)
             if exclude_string is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'exclude' argument in 'include' directive"
                     f' at {os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
-                ignore_paths = []
             else:
 
                 if os.path.isabs(exclude_string):
                     exclude_globstr = exclude_string
                 else:
                     exclude_globstr = os.path.realpath(
                         os.path.join(
@@ -195,28 +219,30 @@
                     )
                 ignore_paths = glob.glob(exclude_globstr)
 
         file_paths_to_include = process.filter_paths(
             glob.iglob(file_path_glob, recursive=True),
             ignore_paths=ignore_paths,
         )
+        if is_url(filename):
+            file_paths_to_include = [file_path_glob]
 
         if not file_paths_to_include:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
-            logger.error(
+            raise BuildError(
                 f"No files found including '{raw_filename}'"
                 f' at {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
-            return ''
         elif files_watcher is not None:
-            files_watcher.included_files.extend(file_paths_to_include)
+            if not is_url(file_path_glob):
+                files_watcher.included_files.extend(file_paths_to_include)
 
         bool_options: dict[str, DirectiveBoolArgument] = {
             'preserve-includer-indent': {
                 'value': default_preserve_includer_indent,
                 'regex': ARGUMENT_REGEXES['preserve-includer-indent'],
             },
             'dedent': {
@@ -240,72 +266,73 @@
                     ) or TRUE_FALSE_BOOL_STR[arg['value']]
                 ]
             except KeyError:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     f"Invalid value for '{arg_name}' argument of 'include'"
                     f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno}. Possible values are true or false.',
                 )
-                return ''
 
         start_match = ARGUMENT_REGEXES['start'].search(arguments_string)
         if start_match:
             start = parse_string_argument(start_match)
             if start is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'start' argument in 'include' directive at "
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
         else:
             start = None
 
         end_match = ARGUMENT_REGEXES['end'].search(arguments_string)
         if end_match:
             end = parse_string_argument(end_match)
             if end is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'end' argument in 'include' directive at "
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
         else:
             end = None
 
         encoding_match = ARGUMENT_REGEXES['encoding'].search(arguments_string)
         if encoding_match:
             encoding = parse_string_argument(encoding_match)
             if encoding is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'encoding' argument in 'include'"
                     ' directive at '
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
-                encoding = 'utf-8'
         else:
             encoding = default_encoding
 
         text_to_include = ''
         expected_but_any_found = [start is not None, end is not None]
         for file_path in file_paths_to_include:
-            new_text_to_include = read_file(file_path, encoding)
+            if is_url(filename):
+                new_text_to_include = read_http(file_path, http_cache)
+            else:
+                new_text_to_include = read_file(file_path, encoding)
 
             if start is not None or end is not None:
                 new_text_to_include, *expected_not_found = (
                     process.filter_inclusions(
                         start,
                         end,
                         new_text_to_include,
@@ -323,14 +350,15 @@
                 include_tag_regex,
                 include_markdown_tag_regex,
                 default_encoding,
                 default_preserve_includer_indent,
                 default_dedent,
                 default_trailing_newlines,
                 files_watcher=files_watcher,
+                http_cache=http_cache,
             )
 
             # trailing newlines right stripping
             if not bool_options['trailing-newlines']['value']:
                 new_text_to_include = process.rstrip_trailing_newlines(
                     new_text_to_include,
                 )
@@ -382,25 +410,26 @@
 
         filename, raw_filename = parse_filename_argument(match)
         if filename is None:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
-            logger.error(
+            raise BuildError(
                 "Found no path passed including with 'include-markdown'"
                 f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
-            return ''
 
         arguments_string = match.group('arguments')
 
         if os.path.isabs(filename):
             file_path_glob = filename
+        elif is_url(filename):
+            file_path_glob = filename
         else:
             file_path_glob = os.path.join(
                 os.path.abspath(os.path.dirname(page_src_path)),
                 filename,
             )
 
         exclude_match = ARGUMENT_REGEXES['exclude'].search(arguments_string)
@@ -409,20 +438,19 @@
         else:
             exclude_string = parse_string_argument(exclude_match)
             if exclude_string is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'exclude' argument in 'include-markdown'"
                     f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno}',
                 )
-                ignore_paths = []
             else:
                 if os.path.isabs(exclude_string):
                     exclude_globstr = exclude_string
                 else:
                     exclude_globstr = os.path.realpath(
                         os.path.join(
                             os.path.abspath(os.path.dirname(page_src_path)),
@@ -432,27 +460,30 @@
                 ignore_paths = glob.glob(exclude_globstr)
 
         file_paths_to_include = process.filter_paths(
             glob.iglob(file_path_glob, recursive=True),
             ignore_paths=ignore_paths,
         )
 
+        if is_url(filename):
+            file_paths_to_include = [file_path_glob]
+
         if not file_paths_to_include:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
-            logger.error(
+            raise BuildError(
                 f"No files found including '{raw_filename}' at"
                 f' {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
-            return ''
         elif files_watcher is not None:
-            files_watcher.included_files.extend(file_paths_to_include)
+            if not is_url(file_path_glob):
+                files_watcher.included_files.extend(file_paths_to_include)
 
         bool_options: dict[str, DirectiveBoolArgument] = {
             'rewrite-relative-urls': {
                 'value': True,
                 'regex': ARGUMENT_REGEXES['rewrite-relative-urls'],
             },
             'comments': {
@@ -484,32 +515,31 @@
                     ) or TRUE_FALSE_BOOL_STR[arg['value']]
                 ]
             except KeyError:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     f"Invalid value for '{arg_name}' argument of"
                     " 'include-markdown' directive at"
                     f' {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno}. Possible values are true or false.',
                 )
-                return ''
 
         # start and end arguments
         start_match = ARGUMENT_REGEXES['start'].search(arguments_string)
         if start_match:
             start = parse_string_argument(start_match)
             if start is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'start' argument in 'include-markdown'"
                     f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno}',
                 )
         else:
             start = None
 
@@ -517,15 +547,15 @@
         if end_match:
             end = parse_string_argument(end_match)
             if end is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'end' argument in 'include-markdown'"
                     f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno}',
                 )
         else:
             end = None
 
@@ -533,15 +563,15 @@
         if encoding_match:
             encoding = parse_string_argument(encoding_match)
             if encoding is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
-                logger.error(
+                raise BuildError(
                     "Invalid empty 'encoding' argument in 'include-markdown'"
                     ' directive at '
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
                 encoding = 'utf-8'
         else:
             encoding = default_encoding
@@ -566,15 +596,18 @@
         #
         # `True` means that no start/end strings have been found in content
         # but they have been specified, so the warning(s) must be raised
         expected_but_any_found = [start is not None, end is not None]
 
         text_to_include = ''
         for file_path in file_paths_to_include:
-            new_text_to_include = read_file(file_path, encoding)
+            if is_url(filename):
+                new_text_to_include = read_http(file_path, http_cache)
+            else:
+                new_text_to_include = read_file(file_path, encoding)
 
             if start is not None or end is not None:
                 new_text_to_include, *expected_not_found = (
                     process.filter_inclusions(
                         start,
                         end,
                         new_text_to_include,
@@ -593,14 +626,15 @@
                 include_markdown_tag_regex,
                 default_encoding,
                 default_preserve_includer_indent,
                 default_dedent,
                 default_trailing_newlines,
                 default_comments=default_comments,
                 files_watcher=files_watcher,
+                http_cache=http_cache,
             )
 
             # trailing newlines right stripping
             if not bool_options['trailing-newlines']['value']:
                 new_text_to_include = process.rstrip_trailing_newlines(
                     new_text_to_include,
                 )
@@ -683,14 +717,15 @@
 
 def on_page_markdown(
     markdown: str,
     page: Page,
     docs_dir: str,
     config: MutableMapping[str, Any] | None = None,
     files_watcher: FilesWatcher | None = None,
+    http_cache: Cache | None = None,
 ) -> str:
     """Process markdown content of a page."""
     if config is None:
         config = {}
 
     return get_file_content(
         markdown,
@@ -716,8 +751,9 @@
             'preserve_includer_indent',
             CONFIG_DEFAULTS['preserve_includer_indent'],
         ),
         config.get('dedent', CONFIG_DEFAULTS['dedent']),
         config.get('trailing_newlines', CONFIG_DEFAULTS['trailing_newlines']),
         default_comments=config.get('comments', CONFIG_DEFAULTS['comments']),
         files_watcher=files_watcher,
+        http_cache=config.get('_cache', http_cache),
     )
```

### Comparing `mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/plugin.py` & `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 """Plugin entry point."""
 
 from __future__ import annotations
 
 from collections.abc import Callable
-from typing import TYPE_CHECKING, Any, TypeVar, cast
+from typing import TYPE_CHECKING, Any, cast
 
+from mkdocs.exceptions import BuildError
 from mkdocs.livereload import LiveReloadServer
-from mkdocs.plugins import BasePlugin
+from mkdocs.plugins import BasePlugin, event_priority
 
 
-try:
-    from mkdocs.plugins import event_priority
-except ImportError:
-    T = TypeVar('T')
-
-    def event_priority(priority: float) -> Callable[[T], T]:  # noqa: D103
-        return lambda f: f
-
 if TYPE_CHECKING:
     from mkdocs.config.defaults import MkDocsConfig
     from mkdocs.structure.files import Files
     from mkdocs.structure.pages import Page
 
+from mkdocs_include_markdown_plugin.cache import initialize_cache
 from mkdocs_include_markdown_plugin.config import (
     CONFIG_SCHEME,
     create_include_tag,
 )
 from mkdocs_include_markdown_plugin.event import (
     on_page_markdown as _on_page_markdown,
 )
@@ -47,14 +41,27 @@
 
         self.config['_include_markdown_tag'] = create_include_tag(
             self.config['opening_tag'],
             self.config['closing_tag'],
             tag='include-markdown',
         )
 
+        if self.config['cache'] > 0:
+            cache = initialize_cache(self.config['cache'])
+            if cache is None:
+                raise BuildError(
+                    'The "platformdirs" package is required to use the'
+                    ' "cache" option. Install'
+                    ' mkdocs-include-markdown-plugin with the "cache"'
+                    ' extra to install it.',
+                )
+            else:
+                cache.clean()
+                self.config['_cache'] = cache
+
         return config
 
     def _watch_included_files(self) -> None:
         global FILES_WATCHER, SERVER
         SERVER = cast(LiveReloadServer, SERVER)
 
         # compatibility with Mkdocs < 1.4.0
```

### Comparing `mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/process.py` & `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/process.py`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-4.0.4/src/mkdocs_include_markdown_plugin/regexes.py` & `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/regexes.py`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-4.0.4/LICENSE` & `mkdocs_include_markdown_plugin-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-4.0.4/README.md` & `mkdocs_include_markdown_plugin-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <!-- mdpo-disable-next-line -->
 
 # mkdocs-include-markdown-plugin
 
-Mkdocs Markdown includer plugin.
-
 <!-- mdpo-disable -->
 
 [![PyPI][pypi-version-badge-link]][pypi-link]
+[![License][license-image]][license-link]
 [![Tests][tests-image]][tests-link]
 [![Coverage status][coverage-image]][coverage-link]
 
 <!-- mdpo-enable -->
 
+Mkdocs Markdown includer plugin.
+
 <!-- mdpo-disable -->
 <!-- mdpo-enable-next-line -->
 
 > Read this document in other languages:
 >
 > - [Español][es-readme-link]
 > - [Français][fr-readme-link]
@@ -35,48 +36,65 @@
 Enable the plugin in your `mkdocs.yml`:
 
 ```yaml
 plugins:
   - include-markdown
 ```
 
-> Make sure that you define `include-markdown` before other plugins that could
-> conflict, like [`mkdocs-macros-plugin`][mkdocs-macros-plugin-link].
-
 ### Configuration
 
 The global behaviour of the plugin can be customized in the configuration.
 
 - <a name="config_tags" href="#config_tags">#</a> **opening_tag** and
   **closing_tag**: The default opening and closing tags. By default are
   `{%` and `%}`.
 
-The rest of the options will define the default values passed to arguments
+Most of the settings will define the default values passed to arguments
 of directives and are documented in the [reference](#reference).
 
 ```yaml
 plugins:
   - include-markdown:
       opening_tag: "{!"
       closing_tag: "!}"
       encoding: ascii
       preserve_includer_indent: false
-      dedent: true
-      trailing_newlines: false
-      comments: false
+      dedent: false
+      trailing_newlines: true
+      comments: true
+```
+
+The `cache` setting defines a expiration time in seconds for HTTP requests
+when including from URLs.
+
+```yaml
+plugins:
+  - include-markdown:
+      cache: 600
+```
+
+In order to use this feature, the dependency [platformdirs] must be installed.
+You can include it in the installation of the plugin adding the `cache` extra:
+
+```txt
+# requirements.txt
+mkdocs-include-markdown-plugin[cache]
 ```
 
 ### Reference
 
 This plugin provides two directives, one to include Markdown files and another
 to include files of any type.
 
-Paths of included files can be absolute or relative to the path of the file
-that includes them. This argument also accept globs, in which case certain
-paths can be ignored using the `exclude` argument.
+Paths of included files can be either:
+
+- Local files with absolute or relative paths to the file that includes them.
+- Globs matching multiples files, in which case certain paths can be ignored
+  using the `exclude` argument.
+- URLs to include remote content.
 
 File paths to include and string arguments can be wrapped by double `"` or
 single `'` quotes, which can be escaped prepending them a `\` character as
 `\"` and `\'`.
 
 The arguments **start** and **end** may contain usual (Python-style) escape
 sequences like `\n` to match against newlines.
@@ -217,16 +235,18 @@
 
 - Joe Rickerby and contributors for
   [giving me the permissions][cibuildwheel-470] to separate this plugin from the
   documentation of [cibuildwheel][cibuildwheel-repo-link].
 
 [pypi-link]: https://pypi.org/project/mkdocs-include-markdown-plugin
 [pypi-version-badge-link]: https://img.shields.io/pypi/v/mkdocs-include-markdown-plugin?logo=pypi&logoColor=white
-[tests-image]: https://img.shields.io/github/actions/workflow/status/mondeja/mkdocs-include-markdown-plugin/ci.yml?branch=master&logo=github&label=tests
+[tests-image]: https://img.shields.io/github/actions/workflow/status/mondeja/mkdocs-include-markdown-plugin/ci.yml?logo=github&label=tests&branch=master
 [tests-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/actions?query=workflow%3ACI
 [coverage-image]: https://img.shields.io/codecov/c/github/mondeja/mkdocs-include-markdown-plugin?logo=codecov&logoColor=white
 [coverage-link]: https://app.codecov.io/gh/mondeja/mkdocs-include-markdown-plugin
+[license-image]: https://img.shields.io/pypi/l/mkdocs-include-markdown-plugin?color=light-green&logo=apache&logoColor=white
+[license-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/blob/master/LICENSE
+[platformdirs]: https://pypi.org/project/platformdirs/
 [cibuildwheel-470]: https://github.com/joerick/cibuildwheel/issues/470
 [cibuildwheel-repo-link]: https://github.com/joerick/cibuildwheel
-[mkdocs-macros-plugin-link]: https://mkdocs-macros-plugin.readthedocs.io
 [es-readme-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/blob/master/locale/es/README.md
 [fr-readme-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/blob/master/locale/fr/README.md
```

### Comparing `mkdocs_include_markdown_plugin-4.0.4/pyproject.toml` & `mkdocs_include_markdown_plugin-5.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [project]
 name = "mkdocs-include-markdown-plugin"
-version = "4.0.4"
+version = "5.0.0"
 description = "Mkdocs Markdown includer plugin."
 readme = "README.md"
 license = "Apache-2.0"
-requires-python = ">=3.7,<3.12"
+requires-python = ">=3.8,<3.13"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Operating System :: OS Independent",
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Topic :: Documentation",
   "Topic :: Software Development :: Documentation",
   "Topic :: Text Processing",
   "Topic :: Text Processing :: Markup :: Markdown",
   "Environment :: Console",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11"
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12"
 ]
 keywords = ["markdown", "mkdocs", "includer", "plugin"]
 
 [[project.authors]]
 name = "Joe Rickerby"
 
 [[project.authors]]
@@ -39,14 +39,17 @@
 Documentation = "https://github.com/mondeja/mkdocs-include-markdown-plugin#documentation"
 "Bug tracker" = "https://github.com/mondeja/mkdocs-include-markdown-plugin/issues"
 Changelog = "https://github.com/mondeja/mkdocs-include-markdown-plugin/releases"
 
 [project.entry-points."mkdocs.plugins"]
 include-markdown = "mkdocs_include_markdown_plugin.plugin:IncludeMarkdownPlugin"
 
+[project.optional-dependencies]
+cache = ["platformdirs"]
+
 [tool.hatch.build]
 include = ["/src"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/mkdocs_include_markdown_plugin"]
 
 [tool.hatch.envs.default]
@@ -59,26 +62,30 @@
 dependencies = ["pre-commit"]
 
 [tool.hatch.envs.style.scripts]
 lint = "pre-commit run -a"
 
 [tool.hatch.envs.tests]
 matrix-name-format = "{variable}-{value}"
-dependencies = ["pytest~=7.0", "coverage~=6.4"]
+dependencies = ["pytest~=7.0", "coverage~=6.4", "covdefaults"]
 
 [[tool.hatch.envs.tests.matrix]]
-python = ["py37", "py38", "py39", "py310", "py311"]
-mkdocs = ["1.2.4", "1.3.1", "1.4.0", "1.4.2"]
+python = ["py38", "py39", "py310", "py311", "py312"]
+mkdocs = ["1.4.0", "1.4.3", "1.5.0", "1.5.1"]
+cache = ["yes", "no"]
 
 [tool.hatch.envs.tests.overrides]
 matrix.mkdocs.dependencies = [
-  { value = "mkdocs==1.2.4", if = ["1.2.4"] },
-  { value = "mkdocs==1.3.1", if = ["1.3.1"] },
   { value = "mkdocs==1.4.0", if = ["1.4.0"] },
-  { value = "mkdocs==1.4.2", if = ["1.4.2"] },
+  { value = "mkdocs==1.4.3", if = ["1.4.3"] },
+  { value = "mkdocs==1.5.0", if = ["1.5.0"] },
+  { value = "mkdocs==1.5.1", if = ["1.5.1"] },
+]
+matrix.cache.dependencies = [
+  { value = "platformdirs", if = ["yes"] },
 ]
 
 [tool.hatch.envs.tests.scripts]
 all = "coverage run -m pytest"
 unit = "coverage run -m pytest tests/test_unit"
 integration = "pytest tests/test_integration --override-ini addopts=-svv"
 cov = [
@@ -90,36 +97,33 @@
 
 [tool.bump]
 targets = [{ file = "pyproject.toml" }]
 
 [tool.project-config]
 cache = "2 days"
 style = [
-  "gh://mondeja/project-config-styles@v4.2/base/pre-commit/md2po2md.json5",
-  "gh://mondeja/project-config-styles@v4.2/python/base.json5",
-  "gh://mondeja/project-config-styles@v4.2/python/single-quotes.json5",
-  "gh://mondeja/project-config-styles@v4.2/python/line-length-80.json5",
-  "gh://mondeja/project-config-styles@v4.2/python/tests.json5",
-  "gh://mondeja/project-config-styles@v4.2/python/google-docstrings.json5",
-  "gh://mondeja/project-config-styles@v4.2/python/mypy.json5",
+  "gh://mondeja/project-config-styles@v4.3/base/pre-commit/md2po2md.json5",
+  "gh://mondeja/project-config-styles@v4.3/python/base.json5",
+  "gh://mondeja/project-config-styles@v4.3/python/single-quotes.json5",
+  "gh://mondeja/project-config-styles@v4.3/python/tests.json5",
+  "gh://mondeja/project-config-styles@v4.3/python/google-docstrings.json5",
+  "gh://mondeja/project-config-styles@v4.3/python/mypy.json5",
 ]
 
 [tool.coverage.run]
 source = ["src"]
 omit = ["src/mkdocs_include_markdown_plugin/plugin.py"]
+plugins = ["covdefaults"]
 
 [tool.coverage.report]
 exclude_lines = [
-  "pragma: no cover",
   "def __repr__\\(",
-  "raise NotImplementedError",
   "@(abc\\.)?abstractmethod",
-  "class .*\\bProtocol\\):",
-  "if TYPE_CHECKING:",
 ]
+fail_under = 1
 
 [tool.flakeheaven]
 inline-quotes = "single"
 max-line-length = 80
 pytest-fixture-no-parentheses = true
 pytest-parametrize-values-type = "tuple"
 docstring-convention = "google"
@@ -179,29 +183,29 @@
   "FUTURE",
   "STDLIB",
   "THIRDPARTY",
   "FIRSTPARTY",
   "TESTS",
   "LOCALFOLDER"
 ]
-py_version = 37
+py_version = 38
 extra_standard_library = [
   "contextvars",
   "dataclasses",
   "importlib.resources",
   "importlib.metadata",
   "zoneinfo",
   "graphlib",
   "tomllib",
   "wsgiref.types"
 ]
 
 [tool.mypy]
 strict = true
-python_version = "3.10"
+python_version = "3.11"
 allow_untyped_calls = true
 allow_any_generics = true
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 # The next object is enough to build the wheel with mypyc, but just
```

### Comparing `mkdocs_include_markdown_plugin-4.0.4/PKG-INFO` & `mkdocs_include_markdown_plugin-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-include-markdown-plugin
-Version: 4.0.4
+Version: 5.0.0
 Summary: Mkdocs Markdown includer plugin.
 Project-URL: Source, https://github.com/mondeja/mkdocs-include-markdown-plugin
 Project-URL: Documentation, https://github.com/mondeja/mkdocs-include-markdown-plugin#documentation
 Project-URL: Bug tracker, https://github.com/mondeja/mkdocs-include-markdown-plugin/issues
 Project-URL: Changelog, https://github.com/mondeja/mkdocs-include-markdown-plugin/releases
 Author: Joe Rickerby
 Author-email: Álvaro Mondéjar Rubio <mondejar1994@gmail.com>
@@ -13,40 +13,43 @@
 License-File: LICENSE
 Keywords: includer,markdown,mkdocs,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: Markdown
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.13,>=3.8
+Provides-Extra: cache
+Requires-Dist: platformdirs; extra == 'cache'
 Description-Content-Type: text/markdown
 
 <!-- mdpo-disable-next-line -->
 
 # mkdocs-include-markdown-plugin
 
-Mkdocs Markdown includer plugin.
-
 <!-- mdpo-disable -->
 
 [![PyPI][pypi-version-badge-link]][pypi-link]
+[![License][license-image]][license-link]
 [![Tests][tests-image]][tests-link]
 [![Coverage status][coverage-image]][coverage-link]
 
 <!-- mdpo-enable -->
 
+Mkdocs Markdown includer plugin.
+
 <!-- mdpo-disable -->
 <!-- mdpo-enable-next-line -->
 
 > Read this document in other languages:
 >
 > - [Español][es-readme-link]
 > - [Français][fr-readme-link]
@@ -66,48 +69,65 @@
 Enable the plugin in your `mkdocs.yml`:
 
 ```yaml
 plugins:
   - include-markdown
 ```
 
-> Make sure that you define `include-markdown` before other plugins that could
-> conflict, like [`mkdocs-macros-plugin`][mkdocs-macros-plugin-link].
-
 ### Configuration
 
 The global behaviour of the plugin can be customized in the configuration.
 
 - <a name="config_tags" href="#config_tags">#</a> **opening_tag** and
   **closing_tag**: The default opening and closing tags. By default are
   `{%` and `%}`.
 
-The rest of the options will define the default values passed to arguments
+Most of the settings will define the default values passed to arguments
 of directives and are documented in the [reference](#reference).
 
 ```yaml
 plugins:
   - include-markdown:
       opening_tag: "{!"
       closing_tag: "!}"
       encoding: ascii
       preserve_includer_indent: false
-      dedent: true
-      trailing_newlines: false
-      comments: false
+      dedent: false
+      trailing_newlines: true
+      comments: true
+```
+
+The `cache` setting defines a expiration time in seconds for HTTP requests
+when including from URLs.
+
+```yaml
+plugins:
+  - include-markdown:
+      cache: 600
+```
+
+In order to use this feature, the dependency [platformdirs] must be installed.
+You can include it in the installation of the plugin adding the `cache` extra:
+
+```txt
+# requirements.txt
+mkdocs-include-markdown-plugin[cache]
 ```
 
 ### Reference
 
 This plugin provides two directives, one to include Markdown files and another
 to include files of any type.
 
-Paths of included files can be absolute or relative to the path of the file
-that includes them. This argument also accept globs, in which case certain
-paths can be ignored using the `exclude` argument.
+Paths of included files can be either:
+
+- Local files with absolute or relative paths to the file that includes them.
+- Globs matching multiples files, in which case certain paths can be ignored
+  using the `exclude` argument.
+- URLs to include remote content.
 
 File paths to include and string arguments can be wrapped by double `"` or
 single `'` quotes, which can be escaped prepending them a `\` character as
 `\"` and `\'`.
 
 The arguments **start** and **end** may contain usual (Python-style) escape
 sequences like `\n` to match against newlines.
@@ -248,16 +268,18 @@
 
 - Joe Rickerby and contributors for
   [giving me the permissions][cibuildwheel-470] to separate this plugin from the
   documentation of [cibuildwheel][cibuildwheel-repo-link].
 
 [pypi-link]: https://pypi.org/project/mkdocs-include-markdown-plugin
 [pypi-version-badge-link]: https://img.shields.io/pypi/v/mkdocs-include-markdown-plugin?logo=pypi&logoColor=white
-[tests-image]: https://img.shields.io/github/actions/workflow/status/mondeja/mkdocs-include-markdown-plugin/ci.yml?branch=master&logo=github&label=tests
+[tests-image]: https://img.shields.io/github/actions/workflow/status/mondeja/mkdocs-include-markdown-plugin/ci.yml?logo=github&label=tests&branch=master
 [tests-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/actions?query=workflow%3ACI
 [coverage-image]: https://img.shields.io/codecov/c/github/mondeja/mkdocs-include-markdown-plugin?logo=codecov&logoColor=white
 [coverage-link]: https://app.codecov.io/gh/mondeja/mkdocs-include-markdown-plugin
+[license-image]: https://img.shields.io/pypi/l/mkdocs-include-markdown-plugin?color=light-green&logo=apache&logoColor=white
+[license-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/blob/master/LICENSE
+[platformdirs]: https://pypi.org/project/platformdirs/
 [cibuildwheel-470]: https://github.com/joerick/cibuildwheel/issues/470
 [cibuildwheel-repo-link]: https://github.com/joerick/cibuildwheel
-[mkdocs-macros-plugin-link]: https://mkdocs-macros-plugin.readthedocs.io
 [es-readme-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/blob/master/locale/es/README.md
 [fr-readme-link]: https://github.com/mondeja/mkdocs-include-markdown-plugin/blob/master/locale/fr/README.md
```

