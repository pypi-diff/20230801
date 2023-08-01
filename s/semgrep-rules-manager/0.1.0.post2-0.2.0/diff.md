# Comparing `tmp/semgrep_rules_manager-0.1.0.post2.tar.gz` & `tmp/semgrep_rules_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semgrep_rules_manager-0.1.0.post2.tar", max compression
+gzip compressed data, was "semgrep_rules_manager-0.2.0.tar", max compression
```

## Comparing `semgrep_rules_manager-0.1.0.post2.tar` & `semgrep_rules_manager-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.1.0.post2/LICENSE
--rw-r--r--   0        0        0     1711 2023-08-01 08:02:36.011149 semgrep_rules_manager-0.1.0.post2/README.pypi.md
--rw-r--r--   0        0        0     1443 2023-08-01 08:00:26.082746 semgrep_rules_manager-0.1.0.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/__init__.py
--rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/cli.py
--rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/core.py
--rw-r--r--   0        0        0     1426 2023-07-28 07:44:40.423516 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/data/sources.yaml
--rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/exception.py
--rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/sources.py
--rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.1.0.post2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1818 2023-08-01 08:51:28.710258 semgrep_rules_manager-0.2.0/README.pypi.md
+-rw-r--r--   0        0        0     1437 2023-08-01 08:59:07.269003 semgrep_rules_manager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.2.0/semgrep_rules_manager/__init__.py
+-rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.2.0/semgrep_rules_manager/cli.py
+-rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.2.0/semgrep_rules_manager/core.py
+-rw-r--r--   0        0        0     1590 2023-08-01 08:51:22.410389 semgrep_rules_manager-0.2.0/semgrep_rules_manager/data/sources.yaml
+-rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.2.0/semgrep_rules_manager/exception.py
+-rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.2.0/semgrep_rules_manager/sources.py
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.2.0/PKG-INFO
```

### Comparing `semgrep_rules_manager-0.1.0.post2/LICENSE` & `semgrep_rules_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post2/README.pypi.md` & `semgrep_rules_manager-0.2.0/README.pypi.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 |---------------|------------------------------------------------------------|---------------|-----------|
 | `community`   | https://github.com/returntocorp/semgrep-rules              | Semgrep       | LGPL 2.1  |
 | `gitlab`      | https://gitlab.com/gitlab-org/security-products/sast-rules | GitLab        | MIT       |
 | `trailofbits` | https://github.com/trailofbits/semgrep-rules               | Trail of Bits | AGPL-3.0  |
 | `0xdea`       | https://github.com/0xdea/semgrep-rules                     | Marco Ivaldi  | MIT       |
 | `elttam`      | https://github.com/elttam/semgrep-rules                    | elttam        | MIT       |
 | `kondukto`    | https://github.com/kondukto-io/semgrep-rules               | Kondukto      |           |
+| `dgryski`     | https://github.com/dgryski/semgrep-go                      | Damian Gryski | MIT       |
 
 ## Read Further
 
 This is only an excerpt from the [`README.md` hosted on GitHub](https://github.com/iosifache/semgrep-rules-manager#readme).
```

### Comparing `semgrep_rules_manager-0.1.0.post2/pyproject.toml` & `semgrep_rules_manager-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semgrep_rules_manager"
-version = "0.1.0.post2"
+version = "0.2.0"
 description = "Manager of third-party Semgrep rules"
 keywords = ["semgrep", "semgrep-rules", "semgrep-rules-manager", "sast"]
 authors = ["George-Andrei Iosif <andrei.iosif@canonical.com>"]
 readme = "README.pypi.md"
 license = "MIT"
 packages = [{include = "semgrep_rules_manager"}]
 repository = "https://github.com/iosifache/semgrep-rules-manager"
```

### Comparing `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/cli.py` & `semgrep_rules_manager-0.2.0/semgrep_rules_manager/cli.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/core.py` & `semgrep_rules_manager-0.2.0/semgrep_rules_manager/core.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/data/sources.yaml` & `semgrep_rules_manager-0.2.0/semgrep_rules_manager/data/sources.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -44,7 +44,13 @@
   license: MIT
 kondukto:
   description: Custom rules used in Kondukto
   repository_url: https://github.com/kondukto-io/semgrep-rules
   repository_branch: master
   author: Kondukto
   license: 
+dgryski:
+  description: Custom Go rules
+  repository_url: https://github.com/dgryski/semgrep-go
+  repository_branch: master
+  author: Damian Gryski 
+  license: MIT
```

### Comparing `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/sources.py` & `semgrep_rules_manager-0.2.0/semgrep_rules_manager/sources.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post2/PKG-INFO` & `semgrep_rules_manager-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semgrep-rules-manager
-Version: 0.1.0.post2
+Version: 0.2.0
 Summary: Manager of third-party Semgrep rules
 Home-page: https://github.com/iosifache/semgrep-rules-manager
 License: MIT
 Keywords: semgrep,semgrep-rules,semgrep-rules-manager,sast
 Author: George-Andrei Iosif
 Author-email: andrei.iosif@canonical.com
 Requires-Python: >=3.10,<4.0
@@ -41,12 +41,13 @@
 |---------------|------------------------------------------------------------|---------------|-----------|
 | `community`   | https://github.com/returntocorp/semgrep-rules              | Semgrep       | LGPL 2.1  |
 | `gitlab`      | https://gitlab.com/gitlab-org/security-products/sast-rules | GitLab        | MIT       |
 | `trailofbits` | https://github.com/trailofbits/semgrep-rules               | Trail of Bits | AGPL-3.0  |
 | `0xdea`       | https://github.com/0xdea/semgrep-rules                     | Marco Ivaldi  | MIT       |
 | `elttam`      | https://github.com/elttam/semgrep-rules                    | elttam        | MIT       |
 | `kondukto`    | https://github.com/kondukto-io/semgrep-rules               | Kondukto      |           |
+| `dgryski`     | https://github.com/dgryski/semgrep-go                      | Damian Gryski | MIT       |
 
 ## Read Further
 
 This is only an excerpt from the [`README.md` hosted on GitHub](https://github.com/iosifache/semgrep-rules-manager#readme).
```

