# Comparing `tmp/semv-1.2.0.tar.gz` & `tmp/semv-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semv-1.2.0.tar", last modified: Tue Aug  1 11:30:23 2023, max compression
+gzip compressed data, was "semv-1.3.0.tar", last modified: Tue Aug  1 20:36:57 2023, max compression
```

## Comparing `semv-1.2.0.tar` & `semv-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.422209 semv-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-01 11:29:32.000000 semv-1.2.0/.github/workflows/attempt-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 11:29:32.000000 semv-1.2.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 11:29:32.000000 semv-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 11:29:32.000000 semv-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 11:30:23.422209 semv-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-01 11:29:32.000000 semv-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 11:29:32.000000 semv-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:30:23.422209 semv-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/src/semv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/increment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/version_control_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/src/semv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/tests/cram/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_config.t
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_config2.t
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_multiple_branches.t
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_normal_usage.t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_commit_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_version_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 11:29:32.000000 semv-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.398315 semv-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.386315 semv-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.386315 semv-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-01 20:36:08.000000 semv-1.3.0/.github/workflows/attempt-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 20:36:08.000000 semv-1.3.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 20:36:08.000000 semv-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 20:36:08.000000 semv-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 20:36:57.398315 semv-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-01 20:36:08.000000 semv-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 20:36:08.000000 semv-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:36:57.398315 semv-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.386315 semv-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.394315 semv-1.3.0/src/semv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 20:36:08.000000 semv-1.3.0/src/semv/version_control_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.394315 semv-1.3.0/src/semv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 20:36:57.000000 semv-1.3.0/src/semv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-01 20:36:57.000000 semv-1.3.0/src/semv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:36:57.000000 semv-1.3.0/src/semv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 20:36:57.000000 semv-1.3.0/src/semv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 20:36:57.000000 semv-1.3.0/src/semv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 20:36:57.000000 semv-1.3.0/src/semv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.386315 semv-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.394315 semv-1.3.0/tests/cram/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 20:36:08.000000 semv-1.3.0/tests/cram/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 20:36:08.000000 semv-1.3.0/tests/cram/test_config.t
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 20:36:08.000000 semv-1.3.0/tests/cram/test_config2.t
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-01 20:36:08.000000 semv-1.3.0/tests/cram/test_hooks.t
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-01 20:36:08.000000 semv-1.3.0/tests/cram/test_multiple_branches.t
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-01 20:36:08.000000 semv-1.3.0/tests/cram/test_normal_usage.t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:57.398315 semv-1.3.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 20:36:08.000000 semv-1.3.0/tests/unit/test_commit_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 20:36:08.000000 semv-1.3.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-01 20:36:08.000000 semv-1.3.0/tests/unit/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 20:36:08.000000 semv-1.3.0/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 20:36:08.000000 semv-1.3.0/tests/unit/test_version_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 20:36:08.000000 semv-1.3.0/tox.ini
```

### Comparing `semv-1.2.0/.github/workflows/attempt-release.yml` & `semv-1.3.0/.github/workflows/attempt-release.yml`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/.github/workflows/run-tests.yml` & `semv-1.3.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/.gitignore` & `semv-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/LICENSE` & `semv-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/PKG-INFO` & `semv-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semv
-Version: 1.2.0
+Version: 1.3.0
 Summary: A read-only semantic version commit parsing and validation tool
 Author-email: Ingo Fruend <github@ingofruend.net>
 License: BSD-3-Clause
 Keywords: Semantic Versioning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `semv-1.2.0/README.md` & `semv-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/pyproject.toml` & `semv-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/src/semv/config.py` & `semv-1.3.0/src/semv/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
             'docs',
             'ci',
             'refactor',
             'style',
         }
     )
     invalid_commit_action: InvalidCommitAction = InvalidCommitAction.warning
+    checks: Set[str] = field(default_factory=set)
 
     @classmethod
     def parse(cls, text: str):
         cfg = parse_toml_section(text)
         if 'invalid_commit_action' in cfg:
             cfg['invalid_commit_action'] = InvalidCommitAction(
                 cfg['invalid_commit_action']
```

### Comparing `semv-1.2.0/src/semv/increment.py` & `semv-1.3.0/src/semv/increment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Iterator, Set
-import sys
+from operator import attrgetter
 from .interface import VersionIncrementer
 from . import errors
 from .types import VersionIncrement, Commit, InvalidCommitAction
 from .utils import warn_or_raise
 
 
 class DefaultIncrementer(VersionIncrementer):
@@ -24,15 +24,17 @@
         self.commit_types_skip = commit_types_skip
         self.invalid_commit_action = invalid_commit_action
 
     def get_version_increment(
         self, commits: Iterator[Commit]
     ) -> VersionIncrement:
         return min(
-            (self._commit_to_inc(c) for c in commits), key=lambda vi: vi.value
+            (self._commit_to_inc(c) for c in commits),
+            key=attrgetter('value'),
+            default=VersionIncrement.skip,
         )
 
     def _commit_to_inc(self, commit: Commit) -> VersionIncrement:
         if commit.breaking:
             return VersionIncrement.major
         elif commit.type in self.commit_types_minor:
             return VersionIncrement.minor
```

### Comparing `semv-1.2.0/src/semv/interface.py` & `semv-1.3.0/src/semv/interface.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/src/semv/parse.py` & `semv-1.3.0/src/semv/parse.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/src/semv/types.py` & `semv-1.3.0/src/semv/types.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/src/semv/version_control_system.py` & `semv-1.3.0/src/semv/version_control_system.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/src/semv.egg-info/PKG-INFO` & `semv-1.3.0/src/semv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semv
-Version: 1.2.0
+Version: 1.3.0
 Summary: A read-only semantic version commit parsing and validation tool
 Author-email: Ingo Fruend <github@ingofruend.net>
 License: BSD-3-Clause
 Keywords: Semantic Versioning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `semv-1.2.0/src/semv.egg-info/SOURCES.txt` & `semv-1.3.0/src/semv.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 tox.ini
 .github/workflows/attempt-release.yml
 .github/workflows/run-tests.yml
 src/semv/__init__.py
 src/semv/commands.py
 src/semv/config.py
 src/semv/errors.py
+src/semv/hooks.py
 src/semv/increment.py
 src/semv/interface.py
 src/semv/main.py
 src/semv/parse.py
 src/semv/py.typed
 src/semv/types.py
 src/semv/utils.py
@@ -22,14 +23,15 @@
 src/semv.egg-info/dependency_links.txt
 src/semv.egg-info/entry_points.txt
 src/semv.egg-info/requires.txt
 src/semv.egg-info/top_level.txt
 tests/cram/setup.sh
 tests/cram/test_config.t
 tests/cram/test_config2.t
+tests/cram/test_hooks.t
 tests/cram/test_multiple_branches.t
 tests/cram/test_normal_usage.t
 tests/unit/test_commit_parsing.py
 tests/unit/test_config.py
 tests/unit/test_git.py
 tests/unit/test_version.py
 tests/unit/test_version_incrementer.py
```

### Comparing `semv-1.2.0/tests/cram/test_config.t` & `semv-1.3.0/tests/cram/test_config.t`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/cram/test_config2.t` & `semv-1.3.0/tests/cram/test_config2.t`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/cram/test_multiple_branches.t` & `semv-1.3.0/tests/cram/test_multiple_branches.t`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/cram/test_normal_usage.t` & `semv-1.3.0/tests/cram/test_normal_usage.t`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/unit/test_commit_parsing.py` & `semv-1.3.0/tests/unit/test_commit_parsing.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/unit/test_config.py` & `semv-1.3.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/unit/test_git.py` & `semv-1.3.0/tests/unit/test_git.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/unit/test_version.py` & `semv-1.3.0/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tests/unit/test_version_incrementer.py` & `semv-1.3.0/tests/unit/test_version_incrementer.py`

 * *Files identical despite different names*

### Comparing `semv-1.2.0/tox.ini` & `semv-1.3.0/tox.ini`

 * *Files identical despite different names*

