# Comparing `tmp/zulip_doc-0.1.0.tar.gz` & `tmp/zulip_doc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zulip_doc-0.1.0.tar", last modified: Tue Aug  1 21:33:09 2023, max compression
+gzip compressed data, was "zulip_doc-0.2.0.tar", last modified: Tue Aug  1 21:40:48 2023, max compression
```

## Comparing `zulip_doc-0.1.0.tar` & `zulip_doc-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-08-01 15:22:12.948824 zulip_doc-0.1.0/LICENSE
--rw-r--r--   0        0        0      777 2023-08-01 21:23:46.534445 zulip_doc-0.1.0/README.md
--rw-r--r--   0        0        0      698 2023-08-01 21:33:09.179093 zulip_doc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 18:53:34.217481 zulip_doc-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 21:15:31.360705 zulip_doc-0.1.0/zdoc/__init__.py
--rwxr-xr-x   0        0        0     1835 2023-08-01 21:07:05.610539 zulip_doc-0.1.0/zdoc/main.py
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 zulip_doc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-01 15:22:12.948824 zulip_doc-0.2.0/LICENSE
+-rw-r--r--   0        0        0      783 2023-08-01 21:34:35.557954 zulip_doc-0.2.0/README.md
+-rw-r--r--   0        0        0      697 2023-08-01 21:40:48.472943 zulip_doc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 18:53:34.217481 zulip_doc-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:15:31.360705 zulip_doc-0.2.0/zdoc/__init__.py
+-rwxr-xr-x   0        0        0     1835 2023-08-01 21:07:05.610539 zulip_doc-0.2.0/zdoc/main.py
+-rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 zulip_doc-0.2.0/PKG-INFO
```

### Comparing `zulip_doc-0.1.0/LICENSE` & `zulip_doc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zulip_doc-0.1.0/README.md` & `zulip_doc-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
 Options:
   --max-idle INTEGER              [env var: MAX_IDLE; default: 86400]
   --ignore-weekends / --no-ignore-weekends
                                   [env var: IGNORE_WEEKENDS; default: ignore-
                                   weekends]
   --config-file FILE              [env var: CONFIG_FILE; default:
-                                  /home/paul/.zuliprc]
+                                  /home/{username}/.zuliprc]
   --help                          Show this message and exit.
 ```
 
 Example: `zdoc 12 22`
```

### Comparing `zulip_doc-0.1.0/pyproject.toml` & `zulip_doc-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "zulip-doc"
-version = "0.1.0"
+version = "0.2.0"
 description = "Zulip service that checks user presence for Duty of Care responsibilities for remote teams"
 authors = [
     { name = "Paul Bailey", email = "paul@neutron.studio" },
 ]
 dependencies = [
     "zulip>=0.8.2",
     "typer>=0.9.0",
     "humanize>=4.7.0",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 zdoc = "zdoc.main:app"
```

### Comparing `zulip_doc-0.1.0/zdoc/main.py` & `zulip_doc-0.2.0/zdoc/main.py`

 * *Files identical despite different names*

### Comparing `zulip_doc-0.1.0/PKG-INFO` & `zulip_doc-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: zulip-doc
-Version: 0.1.0
+Version: 0.2.0
 Summary: Zulip service that checks user presence for Duty of Care responsibilities for remote teams
 Author-Email: Paul Bailey <paul@neutron.studio>
 License: MIT
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: zulip>=0.8.2
 Requires-Dist: typer>=0.9.0
 Requires-Dist: humanize>=4.7.0
 Description-Content-Type: text/markdown
 
 # Zulip Duty of Care Service
 
@@ -28,12 +28,12 @@
 
 Options:
   --max-idle INTEGER              [env var: MAX_IDLE; default: 86400]
   --ignore-weekends / --no-ignore-weekends
                                   [env var: IGNORE_WEEKENDS; default: ignore-
                                   weekends]
   --config-file FILE              [env var: CONFIG_FILE; default:
-                                  /home/paul/.zuliprc]
+                                  /home/{username}/.zuliprc]
   --help                          Show this message and exit.
 ```
 
 Example: `zdoc 12 22`
```

