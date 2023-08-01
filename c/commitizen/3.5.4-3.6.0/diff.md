# Comparing `tmp/commitizen-3.5.4.tar.gz` & `tmp/commitizen-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.5.4.tar", max compression
+gzip compressed data, was "commitizen-3.6.0.tar", max compression
```

## Comparing `commitizen-3.5.4.tar` & `commitizen-3.6.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-07-29 11:26:12.675897 commitizen-3.5.4/LICENSE
--rw-r--r--   0        0        0      609 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/__version__.py
--rw-r--r--   0        0        0     4556 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/bump.py
--rw-r--r--   0        0        0    12112 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    18106 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    14245 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7148 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5208 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/info.py
--rw-r--r--   0        0        0    13053 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7070 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3336 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/factory.py
--rw-r--r--   0        0        0     7295 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/out.py
--rw-r--r--   0        0        0     7134 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9726 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5750 2023-07-29 11:26:12.675897 commitizen-3.5.4/docs/README.md
--rw-r--r--   0        0        0     4308 2023-07-29 11:26:12.687897 commitizen-3.5.4/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-01 01:50:49.770270 commitizen-3.6.0/LICENSE
+-rw-r--r--   0        0        0      609 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/__version__.py
+-rw-r--r--   0        0        0     4770 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/bump.py
+-rw-r--r--   0        0        0    12204 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/changelog.py
+-rw-r--r--   0        0        0     3542 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    18106 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    14333 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7340 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5266 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3559 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/info.py
+-rw-r--r--   0        0        0    13205 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1616 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1758 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1479 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7113 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3164 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2721 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3383 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/factory.py
+-rw-r--r--   0        0        0     7295 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/hooks.py
+-rw-r--r--   0        0        0      913 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/out.py
+-rw-r--r--   0        0        0     7134 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9726 2023-08-01 01:50:49.770270 commitizen-3.6.0/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-08-01 01:50:49.774270 commitizen-3.6.0/docs/README.md
+-rw-r--r--   0        0        0     4308 2023-08-01 01:50:49.786271 commitizen-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.6.0/PKG-INFO
```

### Comparing `commitizen-3.5.4/LICENSE` & `commitizen-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/__init__.py` & `commitizen-3.6.0/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/bump.py` & `commitizen-3.6.0/commitizen/bump.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import os
 import re
 from collections import OrderedDict
 from string import Template
 
-from commitizen.defaults import MAJOR, MINOR, PATCH, bump_message
+from commitizen.defaults import MAJOR, MINOR, PATCH, bump_message, encoding
 from commitizen.exceptions import CurrentVersionNotFoundError
 from commitizen.git import GitCommit, smart_open
-from commitizen.version_schemes import DEFAULT_SCHEME, VersionScheme, Version
+from commitizen.version_schemes import DEFAULT_SCHEME, Version, VersionScheme
 
 
 def find_increment(
     commits: list[GitCommit], regex: str, increments_map: dict | OrderedDict
 ) -> str | None:
     if isinstance(increments_map, dict):
         increments_map = OrderedDict(increments_map)
@@ -41,15 +41,20 @@
                 elif increment == PATCH or increment is None:
                     increment = new_increment
 
     return increment
 
 
 def update_version_in_files(
-    current_version: str, new_version: str, files: list[str], *, check_consistency=False
+    current_version: str,
+    new_version: str,
+    files: list[str],
+    *,
+    check_consistency: bool = False,
+    encoding: str = encoding,
 ) -> None:
     """Change old version to the new one in every file given.
 
     Note that this version is not the tag formatted one.
     So for example, your tag could look like `v1.0.0` while your version in
     the package like `1.0.0`.
     """
@@ -58,36 +63,44 @@
         drive, tail = os.path.splitdrive(location)
         path, _, regex = tail.partition(":")
         filepath = drive + path
         if not regex:
             regex = _version_to_regex(current_version)
 
         current_version_found, version_file = _bump_with_regex(
-            filepath, current_version, new_version, regex
+            filepath,
+            current_version,
+            new_version,
+            regex,
+            encoding=encoding,
         )
 
         if check_consistency and not current_version_found:
             raise CurrentVersionNotFoundError(
                 f"Current version {current_version} is not found in {location}.\n"
                 "The version defined in commitizen configuration and the ones in "
                 "version_files are possibly inconsistent."
             )
 
         # Write the file out again
-        with smart_open(filepath, "w") as file:
+        with smart_open(filepath, "w", encoding=encoding) as file:
             file.write(version_file)
 
 
 def _bump_with_regex(
-    version_filepath: str, current_version: str, new_version: str, regex: str
+    version_filepath: str,
+    current_version: str,
+    new_version: str,
+    regex: str,
+    encoding: str = encoding,
 ) -> tuple[bool, str]:
     current_version_found = False
     lines = []
     pattern = re.compile(regex)
-    with open(version_filepath, "r") as f:
+    with open(version_filepath, "r", encoding=encoding) as f:
         for line in f:
             if pattern.search(line):
                 bumped_line = line.replace(current_version, new_version)
                 if bumped_line != line:
                     current_version_found = True
                 lines.append(bumped_line)
             else:
```

### Comparing `commitizen-3.5.4/commitizen/changelog.py` & `commitizen-3.6.0/commitizen/changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from datetime import date
 from typing import TYPE_CHECKING, Callable, Iterable, Type, cast
 
 from jinja2 import Environment, PackageLoader
 
 from commitizen import out
 from commitizen.bump import normalize_tag
+from commitizen.defaults import encoding
 from commitizen.exceptions import InvalidConfigurationError, NoCommitsFoundError
 from commitizen.git import GitCommit, GitTag
 from commitizen.version_schemes import (
     DEFAULT_SCHEME,
     BaseVersion,
     InvalidVersion,
     Pep440,
@@ -209,29 +210,31 @@
     md_title_parser = r"^(?P<title>#+)"
     m = re.search(md_title_parser, value)
     if not m:
         return None
     return m.groupdict().get("title")
 
 
-def get_metadata(filepath: str, scheme: VersionScheme = Pep440) -> dict:
+def get_metadata(
+    filepath: str, scheme: VersionScheme = Pep440, encoding: str = encoding
+) -> dict:
     unreleased_start: int | None = None
     unreleased_end: int | None = None
     unreleased_title: str | None = None
     latest_version: str | None = None
     latest_version_position: int | None = None
     if not os.path.isfile(filepath):
         return {
             "unreleased_start": None,
             "unreleased_end": None,
             "latest_version": None,
             "latest_version_position": None,
         }
 
-    with open(filepath, "r") as changelog_file:
+    with open(filepath, "r", encoding=encoding) as changelog_file:
         for index, line in enumerate(changelog_file):
             line = line.strip().lower()
 
             unreleased: str | None = None
             if "unreleased" in line:
                 unreleased = parse_title_type_of_line(line)
             # Try to find beginning and end lines of the unreleased block
```

### Comparing `commitizen-3.5.4/commitizen/changelog_parser.py` & `commitizen-3.6.0/commitizen/changelog_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 """
 from __future__ import annotations
 
 import re
 from collections import defaultdict
 from typing import Generator, Iterable
 
+from commitizen.defaults import encoding
+
 MD_VERSION_RE = r"^##\s(?P<version>[a-zA-Z0-9.+]+)\s?\(?(?P<date>[0-9-]+)?\)?"
 MD_CHANGE_TYPE_RE = r"^###\s(?P<change_type>[a-zA-Z0-9.+\s]+)"
 MD_MESSAGE_RE = (
     r"^-\s(\*{2}(?P<scope>[a-zA-Z0-9]+)\*{2}:\s)?(?P<message>.+)(?P<breaking>!)?"
 )
 md_version_c = re.compile(MD_VERSION_RE)
 md_change_type_c = re.compile(MD_CHANGE_TYPE_RE)
@@ -32,15 +34,15 @@
     ("test", "test"),
     ("build", "build"),
     ("ci", "ci"),
     ("chore", "chore"),
 ]
 
 
-def find_version_blocks(filepath: str) -> Generator:
+def find_version_blocks(filepath: str, encoding: str = encoding) -> Generator:
     """Find version block (version block: contains all the information about a version.)
 
     E.g:
     ```
     ## 1.2.1 (2019-07-20)
 
     ### Fix
@@ -49,15 +51,15 @@
 
     ### Feat
 
     - new login system
 
     ```
     """
-    with open(filepath, "r") as f:
+    with open(filepath, "r", encoding=encoding) as f:
         block: list = []
         for line in f:
             line = line.strip("\n")
             if not line:
                 continue
 
             if line.startswith("## "):
```

### Comparing `commitizen-3.5.4/commitizen/cli.py` & `commitizen-3.6.0/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/cmd.py` & `commitizen-3.6.0/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/commands/bump.py` & `commitizen-3.6.0/commitizen/commands/bump.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
-from logging import getLogger
 import warnings
+from logging import getLogger
 
 import questionary
 
 from commitizen import bump, cmd, factory, git, hooks, out
 from commitizen.commands.changelog import Changelog
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
@@ -19,27 +19,28 @@
     NoneIncrementExit,
     NoPatternMapError,
     NotAGitProjectError,
     NotAllowed,
     NoVersionSpecifiedError,
 )
 from commitizen.providers import get_provider
-from commitizen.version_schemes import get_version_scheme, InvalidVersion
+from commitizen.version_schemes import InvalidVersion, get_version_scheme
 
 logger = getLogger("commitizen")
 
 
 class Bump:
     """Show prompt for the user to create a guided commit."""
 
     def __init__(self, config: BaseConfig, arguments: dict):
         if not git.is_git_project():
             raise NotAGitProjectError()
 
         self.config: BaseConfig = config
+        self.encoding = config.settings["encoding"]
         self.arguments: dict = arguments
         self.bump_settings: dict = {
             **config.settings,
             **{
                 key: arguments[key]
                 for key in [
                     "tag_format",
@@ -294,14 +295,15 @@
             raise DryRunExit()
 
         bump.update_version_in_files(
             str(current_version),
             str(new_version),
             version_files,
             check_consistency=self.check_consistency,
+            encoding=self.encoding,
         )
 
         provider.set_version(str(new_version))
 
         if self.pre_bump_hooks:
             hooks.run(
                 self.pre_bump_hooks,
```

### Comparing `commitizen-3.5.4/commitizen/commands/changelog.py` & `commitizen-3.6.0/commitizen/commands/changelog.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     """Generate a changelog based on the commit history."""
 
     def __init__(self, config: BaseConfig, args):
         if not git.is_git_project():
             raise NotAGitProjectError()
 
         self.config: BaseConfig = config
+        self.encoding = self.config.settings["encoding"]
         self.cz = factory.commiter_factory(self.config)
 
         self.start_rev = args.get("start_rev") or self.config.settings.get(
             "changelog_start_rev"
         )
         self.file_name = args.get("file_name") or self.config.settings.get(
             "changelog_file"
@@ -97,15 +98,15 @@
             raise NotAllowed(
                 "Changelog file name is broken.\n"
                 "Check the flag `--file-name` in the terminal "
                 f"or the setting `changelog_file` in {self.config.path}"
             )
 
         changelog_hook: Callable | None = self.cz.changelog_hook
-        with smart_open(self.file_name, "w") as changelog_file:
+        with smart_open(self.file_name, "w", encoding=self.encoding) as changelog_file:
             partial_changelog: str | None = None
             if self.incremental:
                 new_lines = changelog.incremental_build(
                     changelog_out, lines, changelog_meta
                 )
                 changelog_out = "".join(new_lines)
                 partial_changelog = changelog_out
@@ -137,15 +138,19 @@
         # Don't continue if no `file_name` specified.
         assert self.file_name
 
         tags = changelog.get_version_tags(self.scheme, git.get_tags()) or []
 
         end_rev = ""
         if self.incremental:
-            changelog_meta = changelog.get_metadata(self.file_name, self.scheme)
+            changelog_meta = changelog.get_metadata(
+                self.file_name,
+                self.scheme,
+                encoding=self.encoding,
+            )
             latest_version = changelog_meta.get("latest_version")
             if latest_version:
                 latest_tag_version: str = bump.normalize_tag(
                     latest_version,
                     tag_format=self.tag_format,
                     scheme=self.scheme,
                 )
@@ -183,11 +188,11 @@
 
         if self.dry_run:
             out.write(changelog_out)
             raise DryRunExit()
 
         lines = []
         if self.incremental and os.path.isfile(self.file_name):
-            with open(self.file_name, "r") as changelog_file:
+            with open(self.file_name, "r", encoding=self.encoding) as changelog_file:
                 lines = changelog_file.readlines()
 
         self.write_changelog(changelog_out, lines, changelog_meta)
```

### Comparing `commitizen-3.5.4/commitizen/commands/check.py` & `commitizen-3.6.0/commitizen/commands/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             if allowed_prefixes is not None
             else config.settings["allowed_prefixes"]
         )
 
         self._valid_command_argument()
 
         self.config: BaseConfig = config
+        self.encoding = config.settings["encoding"]
         self.cz = factory.commiter_factory(self.config)
 
     def _valid_command_argument(self):
         num_exclusive_args_provided = sum(
             arg is not None
             for arg in (self.commit_msg_file, self.commit_msg, self.rev_range)
         )
@@ -93,15 +94,15 @@
         out.success("Commit validation: successful!")
 
     def _get_commits(self):
         msg = None
         # Get commit message from file (--commit-msg-file)
         if self.commit_msg_file is not None:
             # Enter this branch if commit_msg_file is "".
-            with open(self.commit_msg_file, "r", encoding="utf-8") as commit_file:
+            with open(self.commit_msg_file, "r", encoding=self.encoding) as commit_file:
                 msg = commit_file.read()
         # Get commit message from command line (--message)
         elif self.commit_msg is not None:
             msg = self.commit_msg
         if msg is not None:
             msg = self._filter_comments(msg)
             return [git.GitCommit(rev="", title="", body=msg)]
```

### Comparing `commitizen-3.5.4/commitizen/commands/commit.py` & `commitizen-3.6.0/commitizen/commands/commit.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,29 @@
     """Show prompt for the user to create a guided commit."""
 
     def __init__(self, config: BaseConfig, arguments: dict):
         if not git.is_git_project():
             raise NotAGitProjectError()
 
         self.config: BaseConfig = config
+        self.encoding = config.settings["encoding"]
         self.cz = factory.commiter_factory(self.config)
         self.arguments = arguments
         self.temp_file: str = os.path.join(
             tempfile.gettempdir(),
             "cz.commit{user}.backup".format(user=os.environ.get("USER", "")),
         )
 
     def read_backup_message(self) -> str:
         # Check the commit backup file exists
         if not os.path.isfile(self.temp_file):
             raise NoCommitBackupError()
 
         # Read commit message from backup
-        with open(self.temp_file, "r") as f:
+        with open(self.temp_file, "r", encoding=self.encoding) as f:
             return f.read().strip()
 
     def prompt_commit_questions(self) -> str:
         # Prompt user for the commit message
         cz = self.cz
         questions = cz.questions()
         for question in filter(lambda q: q["type"] == "list", questions):
@@ -78,15 +79,15 @@
             m = self.read_backup_message()
         else:
             m = self.prompt_commit_questions()
 
         out.info(f"\n{m}\n")
 
         if write_message_to_file:
-            with smart_open(write_message_to_file, "w") as file:
+            with smart_open(write_message_to_file, "w", encoding=self.encoding) as file:
                 file.write(m)
 
         if dry_run:
             raise DryRunExit()
 
         signoff: bool = self.arguments.get("signoff")
 
@@ -95,15 +96,15 @@
         else:
             c = git.commit(m)
 
         if c.return_code != 0:
             out.error(c.err)
 
             # Create commit backup
-            with smart_open(self.temp_file, "w") as f:
+            with smart_open(self.temp_file, "w", encoding=self.encoding) as f:
                 f.write(m)
 
             raise CommitError()
 
         if "nothing added" in c.out or "no changes added to commit" in c.out:
             out.error(c.out)
         else:
```

### Comparing `commitizen-3.5.4/commitizen/commands/init.py` & `commitizen-3.6.0/commitizen/commands/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     def is_pre_commit_installed(self) -> bool:
         return bool(shutil.which("pre-commit"))
 
 
 class Init:
     def __init__(self, config: BaseConfig, *args):
         self.config: BaseConfig = config
+        self.encoding = config.settings["encoding"]
         self.cz = factory.commiter_factory(self.config)
         self.project_info = ProjectInfo()
 
     def __call__(self):
         if self.config.path:
             out.line(f"Config file {self.config.path} already exists")
             return
@@ -320,15 +321,17 @@
         }
 
         config_data = {}
         if not self.project_info.has_pre_commit_config:
             # .pre-commit-config.yaml does not exist
             config_data["repos"] = [cz_hook_config]
         else:
-            with open(pre_commit_config_filename) as config_file:
+            with open(
+                pre_commit_config_filename, encoding=self.encoding
+            ) as config_file:
                 yaml_data = yaml.safe_load(config_file)
                 if yaml_data:
                     config_data = yaml_data
 
             if "repos" in config_data:
                 for pre_commit_hook in config_data["repos"]:
                     if "commitizen" in pre_commit_hook["repo"]:
@@ -336,15 +339,17 @@
                         break
                 else:
                     config_data["repos"].append(cz_hook_config)
             else:
                 # .pre-commit-config.yaml exists but there's no "repos" key
                 config_data["repos"] = [cz_hook_config]
 
-        with smart_open(pre_commit_config_filename, "w") as config_file:
+        with smart_open(
+            pre_commit_config_filename, "w", encoding=self.encoding
+        ) as config_file:
             yaml.safe_dump(config_data, stream=config_file)
 
         if not self.project_info.is_pre_commit_installed:
             raise InitFailedError("pre-commit is not installed in current environment.")
         if hook_types is None:
             hook_types = ["commit-msg", "pre-push"]
         self._exec_install_pre_commit_hook(hook_types)
```

### Comparing `commitizen-3.5.4/commitizen/commands/version.py` & `commitizen-3.6.0/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/config/__init__.py` & `commitizen-3.6.0/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/config/base_config.py` & `commitizen-3.6.0/commitizen/config/base_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from commitizen.defaults import DEFAULT_SETTINGS, Settings
 
 
 class BaseConfig:
     def __init__(self):
         self._settings: Settings = DEFAULT_SETTINGS.copy()
+        self.encoding = self.settings["encoding"]
         self._path: Path | None = None
 
     @property
     def settings(self) -> Settings:
         return self._settings
 
     @property
```

### Comparing `commitizen-3.5.4/commitizen/config/json_config.py` & `commitizen-3.6.0/commitizen/config/json_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     def __init__(self, *, data: bytes | str, path: Path | str):
         super(JsonConfig, self).__init__()
         self.is_empty_config = False
         self.add_path(path)
         self._parse_setting(data)
 
     def init_empty_config_content(self):
-        with smart_open(self.path, "a") as json_file:
+        with smart_open(self.path, "a", encoding=self.encoding) as json_file:
             json.dump({"commitizen": {}}, json_file)
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
 
         For now only strings are supported.
         We use to update the version number.
         """
         with open(self.path, "rb") as f:
             parser = json.load(f)
 
         parser["commitizen"][key] = value
-        with smart_open(self.path, "w") as f:
+        with smart_open(self.path, "w", encoding=self.encoding) as f:
             json.dump(parser, f, indent=2)
         return self
 
     def _parse_setting(self, data: bytes | str) -> None:
         """We expect to have a section in .cz.json looking like
 
         ```
```

### Comparing `commitizen-3.5.4/commitizen/config/toml_config.py` & `commitizen-3.6.0/commitizen/config/toml_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,28 +22,28 @@
         else:
             parser = parse("")
 
         with open(self.path, "wb") as output_toml_file:
             if parser.get("tool") is None:
                 parser["tool"] = table()
             parser["tool"]["commitizen"] = table()
-            output_toml_file.write(parser.as_string().encode("utf-8"))
+            output_toml_file.write(parser.as_string().encode(self.encoding))
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
 
         For now only strings are supported.
         We use to update the version number.
         """
         with open(self.path, "rb") as f:
             parser = parse(f.read())
 
         parser["tool"]["commitizen"][key] = value
         with open(self.path, "wb") as f:
-            f.write(parser.as_string().encode("utf-8"))
+            f.write(parser.as_string().encode(self.encoding))
         return self
 
     def _parse_setting(self, data: bytes | str) -> None:
         """We expect to have a section in pyproject looking like
 
         ```
         [tool.commitizen]
```

### Comparing `commitizen-3.5.4/commitizen/config/yaml_config.py` & `commitizen-3.6.0/commitizen/config/yaml_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self, *, data: bytes | str, path: Path | str):
         super(YAMLConfig, self).__init__()
         self.is_empty_config = False
         self._parse_setting(data)
         self.add_path(path)
 
     def init_empty_config_content(self):
-        with smart_open(self.path, "a") as json_file:
+        with smart_open(self.path, "a", encoding=self.encoding) as json_file:
             yaml.dump({"commitizen": {}}, json_file, explicit_start=True)
 
     def _parse_setting(self, data: bytes | str) -> None:
         """We expect to have a section in cz.yaml looking like
 
         ```
         commitizen:
@@ -40,11 +40,11 @@
         For now only strings are supported.
         We use to update the version number.
         """
         with open(self.path, "rb") as yaml_file:
             parser = yaml.load(yaml_file, Loader=yaml.FullLoader)
 
         parser["commitizen"][key] = value
-        with smart_open(self.path, "w") as yaml_file:
+        with smart_open(self.path, "w", encoding=self.encoding) as yaml_file:
             yaml.dump(parser, yaml_file, explicit_start=True)
 
         return self
```

### Comparing `commitizen-3.5.4/commitizen/cz/__init__.py` & `commitizen-3.6.0/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/cz/base.py` & `commitizen-3.6.0/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.6.0/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             r"((\n\n.*)|(\s*))?$"
         )
         return PATTERN
 
     def info(self) -> str:
         dir_path = os.path.dirname(os.path.realpath(__file__))
         filepath = os.path.join(dir_path, "conventional_commits_info.txt")
-        with open(filepath, "r") as f:
+        with open(filepath, "r", encoding=self.config.settings["encoding"]) as f:
             content = f.read()
         return content
 
     def process_commit(self, commit: str) -> str:
         pat = re.compile(self.schema_pattern())
         m = re.match(pat, commit)
         if m is None:
```

### Comparing `commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.6.0/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/cz/customize/customize.py` & `commitizen-3.6.0/commitizen/cz/customize/customize.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,13 +77,13 @@
     def schema(self) -> str | None:
         return self.custom_settings.get("schema")
 
     def info(self) -> str | None:
         info_path = self.custom_settings.get("info_path")
         info = self.custom_settings.get("info")
         if info_path:
-            with open(info_path, "r") as f:
+            with open(info_path, "r", encoding=self.config.settings["encoding"]) as f:
                 content = f.read()
             return content
         elif info:
             return info
         return None
```

### Comparing `commitizen-3.5.4/commitizen/cz/jira/jira.py` & `commitizen-3.6.0/commitizen/cz/jira/jira.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,10 +72,10 @@
 
     def schema_pattern(self) -> str:
         return r".*[A-Z]{2,}\-[0-9]+( #| .* #).+( #.+)*"
 
     def info(self) -> str:
         dir_path = os.path.dirname(os.path.realpath(__file__))
         filepath = os.path.join(dir_path, "jira_info.txt")
-        with open(filepath, "r") as f:
+        with open(filepath, "r", encoding=self.config.settings["encoding"]) as f:
             content = f.read()
         return content
```

### Comparing `commitizen-3.5.4/commitizen/cz/jira/jira_info.txt` & `commitizen-3.6.0/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/defaults.py` & `commitizen-3.6.0/commitizen/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,28 +51,30 @@
     use_shortcuts: bool
     style: list[tuple[str, str]] | None
     customize: CzSettings
     major_version_zero: bool
     pre_bump_hooks: list[str] | None
     post_bump_hooks: list[str] | None
     prerelease_offset: int
+    encoding: str
 
 
 name: str = "cz_conventional_commits"
 config_files: list[str] = [
     "pyproject.toml",
     ".cz.toml",
     ".cz.json",
     "cz.json",
     ".cz.yaml",
     "cz.yaml",
 ]
+encoding: str = "utf-8"
 
 DEFAULT_SETTINGS: Settings = {
-    "name": "cz_conventional_commits",
+    "name": name,
     "version": None,
     "version_files": [],
     "version_provider": "commitizen",
     "version_scheme": None,
     "tag_format": "$version",  # example v$version
     "bump_message": None,  # bumped v$current_version to $new_version
     "allow_abort": False,
@@ -89,14 +91,15 @@
     "changelog_merge_prerelease": False,
     "update_changelog_on_bump": False,
     "use_shortcuts": False,
     "major_version_zero": False,
     "pre_bump_hooks": [],
     "post_bump_hooks": [],
     "prerelease_offset": 0,
+    "encoding": encoding,
 }
 
 MAJOR = "MAJOR"
 MINOR = "MINOR"
 PATCH = "PATCH"
 
 bump_pattern = r"^(((BREAKING[\-\ ]CHANGE|feat|fix|refactor|perf)(\(.+\))?(!)?)|\w+!):"
```

### Comparing `commitizen-3.5.4/commitizen/exceptions.py` & `commitizen-3.6.0/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/factory.py` & `commitizen-3.6.0/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/git.py` & `commitizen-3.6.0/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/hooks.py` & `commitizen-3.6.0/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/out.py` & `commitizen-3.6.0/commitizen/out.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import io
 import sys
 
 from termcolor import colored
 
+if sys.platform == "win32":
+    if isinstance(sys.stdout, io.TextIOWrapper) and sys.version_info >= (3, 7):
+        sys.stdout.reconfigure(encoding="utf-8")
+
 
 def write(value: str, *args) -> None:
     """Intended to be used when value is multiline."""
     print(value, *args)
 
 
 def line(value: str, *args, **kwargs) -> None:
```

### Comparing `commitizen-3.5.4/commitizen/providers.py` & `commitizen-3.6.0/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/commitizen/version_schemes.py` & `commitizen-3.6.0/commitizen/version_schemes.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/docs/README.md` & `commitizen-3.6.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.4/pyproject.toml` & `commitizen-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.5.4"
+version = "3.6.0"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.5.4"
+version = "3.6.0"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
```

### Comparing `commitizen-3.5.4/PKG-INFO` & `commitizen-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.5.4
+Version: 3.6.0
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

