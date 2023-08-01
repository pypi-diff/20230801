# Comparing `tmp/shell_whiz-0.2.5rc2.tar.gz` & `tmp/shell_whiz-0.2.5rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.2.5rc2.tar", max compression
+gzip compressed data, was "shell_whiz-0.2.5rc3.tar", max compression
```

## Comparing `shell_whiz-0.2.5rc2.tar` & `shell_whiz-0.2.5rc3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-08-01 19:19:52.554443 shell_whiz-0.2.5rc2/LICENSE
--rw-r--r--   0        0        0     3141 2023-08-01 19:19:52.554443 shell_whiz-0.2.5rc2/README.md
--rw-r--r--   0        0        0      542 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/pyproject.toml
--rw-r--r--   0        0        0      510 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/argparse.py
--rw-r--r--   0        0        0     6761 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/cli.py
--rw-r--r--   0        0        0     1686 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/config.py
--rw-r--r--   0        0        0       54 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/console.py
--rw-r--r--   0        0        0      207 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/constants.py
--rw-r--r--   0        0        0      152 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/exceptions.py
--rw-r--r--   0        0        0    10011 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/openai.py
--rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 shell_whiz-0.2.5rc2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 19:31:55.693470 shell_whiz-0.2.5rc3/LICENSE
+-rw-r--r--   0        0        0     3141 2023-08-01 19:31:55.693470 shell_whiz-0.2.5rc3/README.md
+-rw-r--r--   0        0        0      542 2023-08-01 19:31:55.697470 shell_whiz-0.2.5rc3/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/argparse.py
+-rw-r--r--   0        0        0     6780 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/cli.py
+-rw-r--r--   0        0        0     1686 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/config.py
+-rw-r--r--   0        0        0       54 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/console.py
+-rw-r--r--   0        0        0      207 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/constants.py
+-rw-r--r--   0        0        0      152 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0    10011 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 shell_whiz-0.2.5rc3/PKG-INFO
```

### Comparing `shell_whiz-0.2.5rc2/LICENSE` & `shell_whiz-0.2.5rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc2/README.md` & `shell_whiz-0.2.5rc3/README.md`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc2/pyproject.toml` & `shell_whiz-0.2.5rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.2.5rc2"
+version = "0.2.5rc3"
 description = "Shell Whiz: AI assistant right in your terminal"
 license = "GPL-3.0-only"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shell_whiz-0.2.5rc2/shell_whiz/cli.py` & `shell_whiz-0.2.5rc3/shell_whiz/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
             edit_prompt = inquirer.text(message="Revise query")
         elif choice == "Edit manually":
             shell_command = inquirer.text(
                 message="Edit command", default=shell_command
             )
         elif choice == "Run this command":
             subprocess.run(shell_command, shell=True)
+            return
 
 
 async def run_ai_assistant(args):
     shell_whiz_config()
 
     if args.sw_command == "ask":
         shell_command = " ".join(args.prompt).strip()
```

### Comparing `shell_whiz-0.2.5rc2/shell_whiz/config.py` & `shell_whiz-0.2.5rc3/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc2/shell_whiz/openai.py` & `shell_whiz-0.2.5rc3/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc2/PKG-INFO` & `shell_whiz-0.2.5rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.2.5rc2
+Version: 0.2.5rc3
 Summary: Shell Whiz: AI assistant right in your terminal
 License: GPL-3.0-only
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

