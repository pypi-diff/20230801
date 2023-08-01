# Comparing `tmp/blockinfile-2.14.2.1.tar.gz` & `tmp/blockinfile-2.15.2.tar.gz`

## Comparing `blockinfile-2.14.2.1.tar` & `blockinfile-2.15.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/blockinfile/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/blockinfile/__main__.py
--rwxr-xr-x   0        0        0    15623 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/blockinfile/blockinfile.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/COPYING
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/README.md
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/pyproject.toml
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 blockinfile-2.14.2.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 blockinfile-2.15.2/blockinfile/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 blockinfile-2.15.2/blockinfile/__main__.py
+-rwxr-xr-x   0        0        0    15937 2020-02-02 00:00:00.000000 blockinfile-2.15.2/blockinfile/blockinfile.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 blockinfile-2.15.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 blockinfile-2.15.2/COPYING
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 blockinfile-2.15.2/README.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 blockinfile-2.15.2/pyproject.toml
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 blockinfile-2.15.2/PKG-INFO
```

### Comparing `blockinfile-2.14.2.1/blockinfile/blockinfile.py` & `blockinfile-2.15.2/blockinfile/blockinfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #!/usr/bin/env python3
+# SPDX-License-Identifier: GPL-3.0-only
 # this file has been generated from ansible sources + injected code
 # manual edits might be lost
 # license: GPLv3+, same as ansible
 
 import argparse
 from pathlib import Path
 from functools import cache
 
+import yaml
+
 
 def to_bytes(s):
     if isinstance(s, str):
         return s.encode()
     assert isinstance(s, bytes)
     return s
 
@@ -31,24 +34,31 @@
         if v.lower() in ("y", "yes", "1", "true"):
             return True
         if v.lower() in ("n", "no", "0", "false"):
             return False
         raise ValueError(f"{v!r} not recognized as bool")
 
     def __init__(self, argument_spec, mutually_exclusive=(), add_file_common_args=None, supports_check_mode=None):
-        self.parser = argparse.ArgumentParser()
+        module_doc = yaml.safe_load(DOCUMENTATION)
+
+        self.parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
         for name, spec in argument_spec.items():
             kwargs = {}
             if spec["type"] == "str":
                 pass
             elif spec["type"] == "bool":
                 kwargs["type"] = self.parse_bool
             elif spec["type"] == "path":
                 kwargs["type"] = Path
 
+            try:
+                kwargs["help"] = "\n".join(module_doc["options"][name]["description"])
+            except KeyError:
+                pass
+
             for copy in ("choices", "required", "default"):
                 if copy in spec:
                     kwargs[copy] = spec[copy]
 
             self.parser.add_argument(f"--{name.replace('_', '-')}", **kwargs)
 
         self.parser.add_argument("--unsafe-writes", type=self.parse_bool, default=True)
```

### Comparing `blockinfile-2.14.2.1/COPYING` & `blockinfile-2.15.2/COPYING`

 * *Files identical despite different names*

### Comparing `blockinfile-2.14.2.1/README.md` & `blockinfile-2.15.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # blockinfile
 
 `blockinfile` is a tool for editing automatically a text block surrounded by marker lines. It's an automated port of ansible's [blockinfile module](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/blockinfile_module.html).
 
+Basically, it can overwrite a part of a file that's well delimited so it doesn't overwrite the whole file.
+
 ## Usage
 
 ```
-blockinfile --path FILE_TO_PATCH --block CONTENT_TO_INSERT [--marker NAME] [--marker-begin START_STRING] [--marker-end END_STRING] [MORE_OPTIONS]
+blockinfile --path FILE_TO_PATCH --block CONTENT_TO_INSERT [--marker MARKER_TEMPLATE] [--marker-begin START_STRING] [--marker-end END_STRING] [MORE_OPTIONS]
 ```
 
 Options are the same as in [Ansible documentation](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/blockinfile_module.html).
 
 ## Sample
 
 #### If `myfile.conf` initially contains:
```

### Comparing `blockinfile-2.14.2.1/pyproject.toml` & `blockinfile-2.15.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Code Generators",
   "Topic :: Software Development :: Pre-processors",
   "Topic :: System :: Systems Administration",
   "Topic :: Text Processing :: General",
   "Topic :: Utilities",
 ]
-dependencies = []
+dependencies = ["PyYAML"]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://gitlab.com/hydrargyrum/blockinfile"
 Issues = "https://gitlab.com/hydrargyrum/blockinfile/issues"
 Source = "https://gitlab.com/hydrargyrum/blockinfile"
```

### Comparing `blockinfile-2.14.2.1/PKG-INFO` & `blockinfile-2.15.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockinfile
-Version: 2.14.2.1
+Version: 2.15.2
 Summary: blockinfile is a tool for editing automatically a text block surrounded by marker lines
 Project-URL: Documentation, https://gitlab.com/hydrargyrum/blockinfile
 Project-URL: Issues, https://gitlab.com/hydrargyrum/blockinfile/issues
 Project-URL: Source, https://gitlab.com/hydrargyrum/blockinfile
 Author-email: Hg <dev@indigo.re>
 License-Expression: MIT
 License-File: COPYING
@@ -22,24 +22,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
+Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 # blockinfile
 
 `blockinfile` is a tool for editing automatically a text block surrounded by marker lines. It's an automated port of ansible's [blockinfile module](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/blockinfile_module.html).
 
+Basically, it can overwrite a part of a file that's well delimited so it doesn't overwrite the whole file.
+
 ## Usage
 
 ```
-blockinfile --path FILE_TO_PATCH --block CONTENT_TO_INSERT [--marker NAME] [--marker-begin START_STRING] [--marker-end END_STRING] [MORE_OPTIONS]
+blockinfile --path FILE_TO_PATCH --block CONTENT_TO_INSERT [--marker MARKER_TEMPLATE] [--marker-begin START_STRING] [--marker-end END_STRING] [MORE_OPTIONS]
 ```
 
 Options are the same as in [Ansible documentation](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/blockinfile_module.html).
 
 ## Sample
 
 #### If `myfile.conf` initially contains:
```

