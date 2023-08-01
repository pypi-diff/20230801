# Comparing `tmp/semv-1.1.0.tar.gz` & `tmp/semv-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semv-1.1.0.tar", last modified: Tue Aug  1 08:01:28 2023, max compression
+gzip compressed data, was "semv-1.2.0.tar", last modified: Tue Aug  1 11:30:23 2023, max compression
```

## Comparing `semv-1.1.0.tar` & `semv-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-01 08:00:28.000000 semv-1.1.0/.github/workflows/attempt-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 08:00:28.000000 semv-1.1.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 08:00:28.000000 semv-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 08:00:28.000000 semv-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-01 08:01:28.570065 semv-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-01 08:00:28.000000 semv-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 08:00:28.000000 semv-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:01:28.570065 semv-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/src/semv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/increment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/version_control_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/src/semv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/tests/cram/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/test_config.t
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/test_multiple_branches.t
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/test_normal_usage.t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_commit_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_version_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 08:00:28.000000 semv-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.422209 semv-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-01 11:29:32.000000 semv-1.2.0/.github/workflows/attempt-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 11:29:32.000000 semv-1.2.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 11:29:32.000000 semv-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 11:29:32.000000 semv-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 11:30:23.422209 semv-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-01 11:29:32.000000 semv-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 11:29:32.000000 semv-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:30:23.422209 semv-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/src/semv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 11:29:32.000000 semv-1.2.0/src/semv/version_control_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/src/semv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 11:30:23.000000 semv-1.2.0/src/semv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.414209 semv-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/tests/cram/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_config.t
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_config2.t
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_multiple_branches.t
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-01 11:29:32.000000 semv-1.2.0/tests/cram/test_normal_usage.t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:23.418209 semv-1.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_commit_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 11:29:32.000000 semv-1.2.0/tests/unit/test_version_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 11:29:32.000000 semv-1.2.0/tox.ini
```

### Comparing `semv-1.1.0/.github/workflows/attempt-release.yml` & `semv-1.2.0/.github/workflows/attempt-release.yml`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/.github/workflows/run-tests.yml` & `semv-1.2.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/.gitignore` & `semv-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/LICENSE` & `semv-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/PKG-INFO` & `semv-1.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: semv
-Version: 1.1.0
-Summary: A read-only semantic version commit parsing and validation tool
-Author-email: Ingo Fruend <github@ingofruend.net>
-License: BSD-3-Clause
-Keywords: Semantic Versioning
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # semv - A read-only semantic version commit parsing and validation tool
 
 This package is inspired by a talk by [Stephan
 Bönnemann](https://www.youtube.com/watch?v=tc2UgG5L7WM) as well as the package
 [python semantic
 release](https://python-semantic-release.readthedocs.io/en/latest/).
 Both suggest parsing commit message to automatically create a new version number.
@@ -31,7 +21,26 @@
 
 If you are inside a git repository, you can use semv to print the semantic version that the current commit *should* recieve. E.g.
 
   $ semv
   v1.0.5 (no-eol)
 
 Note that this will have not change anything about your repository. It is up to you to use the printed version. An example for using the printed version is given in semv's own [release workflow](https://github.com/igordertigor/semv/blob/master/.github/workflows/attempt-release.yml).
+
+## Configuration
+
+You can configure semv via the `pyproject.toml` config file. Here are the defaults:
+```toml
+[tool.semv]
+invalid_commit_action = "warning"  # Could also be "error" or "skip"
+
+[tool.types]
+feat = "minor"
+fix = "patch"
+perf = "patch"
+chore = "valid"
+test = "valid"
+docs = "valid"
+ci = "valid"
+refactor = "valid"
+style = "valid"
+```
```

### Comparing `semv-1.1.0/pyproject.toml` & `semv-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/src/semv/commands.py` & `semv-1.2.0/src/semv/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,19 @@
         InvalidCommitType
     """
     pyproject = Path('pyproject.toml')
     if pyproject.exists():
         config = Config.parse(pyproject.read_text())
     else:
         config = Config()
+
+    if len(sys.argv) > 1 and sys.argv[1] == '--list-types':
+        print(config.format_types())
+        sys.exit(0)
+
     vcs = Git()
     cp = AngularCommitParser(config.invalid_commit_action)
     vi = DefaultIncrementer(
         config.commit_types_minor,
         config.commit_types_patch,
         config.commit_types_skip,
         config.invalid_commit_action,
```

### Comparing `semv-1.1.0/src/semv/increment.py` & `semv-1.2.0/src/semv/increment.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/src/semv/interface.py` & `semv-1.2.0/src/semv/interface.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/src/semv/parse.py` & `semv-1.2.0/src/semv/parse.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/src/semv/types.py` & `semv-1.2.0/src/semv/types.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/src/semv/version_control_system.py` & `semv-1.2.0/src/semv/version_control_system.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/src/semv.egg-info/PKG-INFO` & `semv-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semv
-Version: 1.1.0
+Version: 1.2.0
 Summary: A read-only semantic version commit parsing and validation tool
 Author-email: Ingo Fruend <github@ingofruend.net>
 License: BSD-3-Clause
 Keywords: Semantic Versioning
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -31,7 +31,26 @@
 
 If you are inside a git repository, you can use semv to print the semantic version that the current commit *should* recieve. E.g.
 
   $ semv
   v1.0.5 (no-eol)
 
 Note that this will have not change anything about your repository. It is up to you to use the printed version. An example for using the printed version is given in semv's own [release workflow](https://github.com/igordertigor/semv/blob/master/.github/workflows/attempt-release.yml).
+
+## Configuration
+
+You can configure semv via the `pyproject.toml` config file. Here are the defaults:
+```toml
+[tool.semv]
+invalid_commit_action = "warning"  # Could also be "error" or "skip"
+
+[tool.types]
+feat = "minor"
+fix = "patch"
+perf = "patch"
+chore = "valid"
+test = "valid"
+docs = "valid"
+ci = "valid"
+refactor = "valid"
+style = "valid"
+```
```

### Comparing `semv-1.1.0/src/semv.egg-info/SOURCES.txt` & `semv-1.2.0/src/semv.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/semv.egg-info/SOURCES.txt
 src/semv.egg-info/dependency_links.txt
 src/semv.egg-info/entry_points.txt
 src/semv.egg-info/requires.txt
 src/semv.egg-info/top_level.txt
 tests/cram/setup.sh
 tests/cram/test_config.t
+tests/cram/test_config2.t
 tests/cram/test_multiple_branches.t
 tests/cram/test_normal_usage.t
 tests/unit/test_commit_parsing.py
 tests/unit/test_config.py
 tests/unit/test_git.py
 tests/unit/test_version.py
 tests/unit/test_version_incrementer.py
```

### Comparing `semv-1.1.0/tests/cram/test_config.t` & `semv-1.2.0/tests/cram/test_config.t`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tests/cram/test_multiple_branches.t` & `semv-1.2.0/tests/cram/test_multiple_branches.t`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tests/cram/test_normal_usage.t` & `semv-1.2.0/tests/cram/test_normal_usage.t`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tests/unit/test_commit_parsing.py` & `semv-1.2.0/tests/unit/test_commit_parsing.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tests/unit/test_config.py` & `semv-1.2.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tests/unit/test_git.py` & `semv-1.2.0/tests/unit/test_git.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tests/unit/test_version.py` & `semv-1.2.0/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tests/unit/test_version_incrementer.py` & `semv-1.2.0/tests/unit/test_version_incrementer.py`

 * *Files identical despite different names*

### Comparing `semv-1.1.0/tox.ini` & `semv-1.2.0/tox.ini`

 * *Files identical despite different names*

