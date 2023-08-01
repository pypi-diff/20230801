# Comparing `tmp/blockinfile-2.15.2.tar.gz` & `tmp/blockinfile-2.15.2.1.tar.gz`

## Comparing `blockinfile-2.15.2.tar` & `blockinfile-2.15.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 blockinfile-2.15.2/blockinfile/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 blockinfile-2.15.2/blockinfile/__main__.py
--rwxr-xr-x   0        0        0    15937 2020-02-02 00:00:00.000000 blockinfile-2.15.2/blockinfile/blockinfile.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 blockinfile-2.15.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 blockinfile-2.15.2/COPYING
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 blockinfile-2.15.2/README.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 blockinfile-2.15.2/pyproject.toml
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 blockinfile-2.15.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/blockinfile/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/blockinfile/__main__.py
+-rwxr-xr-x   0        0        0    15966 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/blockinfile/blockinfile.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/COPYING
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/README.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 blockinfile-2.15.2.1/PKG-INFO
```

### Comparing `blockinfile-2.15.2/blockinfile/blockinfile.py` & `blockinfile-2.15.2.1/blockinfile/blockinfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def fail_json(self, msg, rc=1):
         self.parser.exit(rc, msg)
 
     def atomic_move(self, src, dst, unsafe_writes):
         os.rename(src, dst)
 
     def exit_json(self, msg, changed=None, diff=None):
-        self.parser.exit(1, msg)
+        self.parser.exit(int(not changed and bool(msg)), msg)
 
     def boolean(self, v):
         return v
 
     def run_command(self, cmd):
         raise NotImplementedError("run_command")
```

### Comparing `blockinfile-2.15.2/COPYING` & `blockinfile-2.15.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `blockinfile-2.15.2/README.md` & `blockinfile-2.15.2.1/README.md`

 * *Files identical despite different names*

### Comparing `blockinfile-2.15.2/pyproject.toml` & `blockinfile-2.15.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blockinfile-2.15.2/PKG-INFO` & `blockinfile-2.15.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockinfile
-Version: 2.15.2
+Version: 2.15.2.1
 Summary: blockinfile is a tool for editing automatically a text block surrounded by marker lines
 Project-URL: Documentation, https://gitlab.com/hydrargyrum/blockinfile
 Project-URL: Issues, https://gitlab.com/hydrargyrum/blockinfile/issues
 Project-URL: Source, https://gitlab.com/hydrargyrum/blockinfile
 Author-email: Hg <dev@indigo.re>
 License-Expression: MIT
 License-File: COPYING
```

