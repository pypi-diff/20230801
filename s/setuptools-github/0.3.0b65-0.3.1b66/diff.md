# Comparing `tmp/setuptools-github-0.3.0b65.tar.gz` & `tmp/setuptools-github-0.3.1b66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.0b65.tar", last modified: Fri Jul 28 19:42:31 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.1b66.tar", last modified: Tue Aug  1 20:03:07 2023, max compression
```

## Comparing `setuptools-github-0.3.0b65.tar` & `setuptools-github-0.3.1b66.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.502533 setuptools-github-0.3.1b66/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.0b65/LICENSE` & `setuptools-github-0.3.1b66/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/PKG-INFO` & `setuptools-github-0.3.1b66/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b65
+Version: 0.3.1b66
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.0b65/README.md` & `setuptools-github-0.3.1b66/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/pyproject.toml` & `setuptools-github-0.3.1b66/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/setup.py` & `setuptools-github-0.3.1b66/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.1b66/setuptools_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b65
+Version: 0.3.1b66
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.0b65/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.1b66/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/src/setuptools_github/checks.py` & `setuptools-github-0.3.1b66/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/src/setuptools_github/cli.py` & `setuptools-github-0.3.1b66/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/src/setuptools_github/scm.py` & `setuptools-github-0.3.1b66/src/setuptools_github/scm.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,29 +152,34 @@
         ignored: bool = False,
     ) -> dict[str, int]:
         # to update the mapping:
         # pygit2.Repository(self.workdir).status()
         mapper = {
             "??": 128 if untracked_files == "all" else None,
             " D": 512,
+            "D ": 4,
             " M": 256,
             "A ": 1,
         }
-        result = {}
+        result: dict[str, int] = {}
         try:
             txt = self(["status", "--porcelain"])
         except subprocess.CalledProcessError as exc:
             raise GitError("invalid repo") from exc
         for line in txt.split("\n"):
             if not line.strip():
                 continue
             tag, filename = line[:2], line[3:]
+            if tag not in mapper:
+                raise GitError(f"cannot map git status for '{tag}'")
             value = mapper[tag]
             if value:
-                result[filename] = value
+                result[filename] = (
+                    (result[filename] | value) if filename in result else value
+                )
         return result
 
     def commit(
         self,
         paths: ListOfArgs,
         message: str,
     ) -> None:
```

### Comparing `setuptools-github-0.3.0b65/src/setuptools_github/script.py` & `setuptools-github-0.3.1b66/src/setuptools_github/script.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """create a beta branch or release a beta branch
 
 This script will either create a new beta branch:
 
-     setuptools-github beta ./src/setuptools_github/__init__.py
+     setuptools-github make-beta ./src/package_name/__init__.py
 
 Or will release the beta branch and will move inot the next minor
 
-    setuptools-github {major|minor|micro|make-beta} ./src/setuptools_github/__init__.py
+    setuptools-github {major|minor|micro} ./src/package_name/__init__.py
 
 """
 from __future__ import annotations
 
 import argparse
 import logging
 import re
@@ -95,14 +95,28 @@
         for branch in [*options.repo.branches.local, *options.repo.branches.remote]:
             if not branch.endswith(f"beta/{version}"):
                 continue
             options.error(f"branch '{branch}' already present")
         log.info("creating branch '%s'", f"/beta/{version}")
         options.repo.branch(f"beta/{version}", master)
         options.repo(["checkout", master])
+        print(  # noqa: T201
+            tools.indent(
+                f"""
+        The release branch beta/{version} has been created.
+
+        To complete the release:
+            git push origin beta/{version}
+
+        To revert this beta branch:
+            git branch -D beta/{version}
+        """
+            ),
+            file=sys.stderr,
+        )
     elif options.mode in {"micro", "minor", "major"}:
         # we need to be in the beta/N.M.O branch
         expr = re.compile(r"refs/heads/beta/(?P<beta>\d+([.]\d+)*)$")
         if not (match := expr.search(options.repo.head.name)):
             options.error(
                 f"wrong branch '{options.repo.head.shorthand}'",
                 f"expected to be in 'beta/{version}' branch",
@@ -129,18 +143,19 @@
         )
 
         print(  # noqa: T201
             tools.indent(
                 f"""
         The release is almost complete.
 
-        To proceed:
+        To complete the release:
             git push origin release/{version}
+            git push origin master
 
-        To rever this script:
+        To revert this release:
             git reset --hard HEAD~1
             git tag -d release/{version}
         """
             ),
             file=sys.stderr,
         )
     else:
```

### Comparing `setuptools-github-0.3.0b65/src/setuptools_github/tools.py` & `setuptools-github-0.3.1b66/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/tests/conftest.py` & `setuptools-github-0.3.1b66/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/tests/test_checks.py` & `setuptools-github-0.3.1b66/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/tests/test_cli.py` & `setuptools-github-0.3.1b66/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/tests/test_conftest.py` & `setuptools-github-0.3.1b66/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/tests/test_scm.py` & `setuptools-github-0.3.1b66/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/tests/test_script.py` & `setuptools-github-0.3.1b66/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b65/tests/test_tools.py` & `setuptools-github-0.3.1b66/tests/test_tools.py`

 * *Files identical despite different names*

