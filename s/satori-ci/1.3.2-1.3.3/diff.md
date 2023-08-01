# Comparing `tmp/satori_ci-1.3.2.tar.gz` & `tmp/satori_ci-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.3.2.tar", last modified: Tue Aug  1 14:58:54 2023, max compression
+gzip compressed data, was "satori_ci-1.3.3.tar", last modified: Tue Aug  1 21:01:39 2023, max compression
```

## Comparing `satori_ci-1.3.2.tar` & `satori_ci-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-08-01 14:58:39.148381 satori_ci-1.3.2/LICENSE
--rw-r--r--   0        0        0     7140 2023-08-01 14:58:39.148381 satori_ci-1.3.2/README.md
--rw-r--r--   0        0        0      755 2023-08-01 14:58:54.964747 satori_ci-1.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/__init__.py
--rw-r--r--   0        0        0       37 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/__main__.py
--rw-r--r--   0        0        0     4558 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/api.py
--rw-r--r--   0        0        0     1633 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/bundler.py
--rw-r--r--   0        0        0      468 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/models.py
--rw-r--r--   0        0        0     3345 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/playbooks.py
--rw-r--r--   0        0        0    28020 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/satori.py
--rw-r--r--   0        0        0    12442 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/utils.py
--rw-r--r--   0        0        0     1194 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/validations.py
--rwxr-xr-x   0        0        0     8991 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/cli/parser.py
--rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 21:01:19.555182 satori_ci-1.3.3/LICENSE
+-rw-r--r--   0        0        0     7140 2023-08-01 21:01:19.555182 satori_ci-1.3.3/README.md
+-rw-r--r--   0        0        0      755 2023-08-01 21:01:39.360215 satori_ci-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/__main__.py
+-rw-r--r--   0        0        0     4558 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/api.py
+-rw-r--r--   0        0        0     1633 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/bundler.py
+-rw-r--r--   0        0        0      484 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/models.py
+-rw-r--r--   0        0        0     3345 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/playbooks.py
+-rw-r--r--   0        0        0    28045 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/satori.py
+-rw-r--r--   0        0        0    12410 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/utils.py
+-rw-r--r--   0        0        0     1194 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/validations.py
+-rwxr-xr-x   0        0        0     8991 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/cli/parser.py
+-rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.3/PKG-INFO
```

### Comparing `satori_ci-1.3.2/LICENSE` & `satori_ci-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.2/README.md` & `satori_ci-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.2/pyproject.toml` & `satori_ci-1.3.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.3.2"
+version = "1.3.3"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.3.2/src/satoricli/classes/api.py` & `satori_ci-1.3.3/src/satoricli/classes/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.2/src/satoricli/classes/bundler.py` & `satori_ci-1.3.3/src/satoricli/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.2/src/satoricli/classes/playbooks.py` & `satori_ci-1.3.3/src/satoricli/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.2/src/satoricli/classes/satori.py` & `satori_ci-1.3.3/src/satoricli/classes/satori.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,15 +454,15 @@
     def report(self, args: arguments):
         """Show a list of reports"""
         params = filter_params(args, ("id",))
         if args.action == "":  # default: print reports
             params = filter_params(args, ("id", "page", "limit", "filter"))
             res = self.api.reports("GET", args.id, "", params=params)
             if args.id == "" and not args.json:  # default: print list
-                autoformat(res["list"])
+                autoformat(res["list"], list_separator="-" * 48)
                 console.print(
                     f"[b]Page:[/] {res['current_page']} of {res['total_pages']}"
                 )
             else:  # single report or json output
                 autoformat(res, jsonfmt=args.json)
         elif args.action == "output":
             self.output(args.id)
```

### Comparing `satori_ci-1.3.2/src/satoricli/classes/utils.py` & `satori_ci-1.3.3/src/satoricli/classes/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,17 @@
     capitalize: bool = False,
     indent: int = 0,
     list_separator: Optional[str] = None,
 ):
     for item in obj:
         indent_text = get_decoration(indent)
         if isinstance(item, dict):
-            dict_formatter(item, capitalize, indent + 1, list_separator)
+            dict_formatter(item, capitalize, indent + 1)
         elif isinstance(item, list):
-            list_formatter(item, capitalize, indent + 1, list_separator)
+            list_formatter(item, capitalize, indent + 1)
         else:
             item = str(item).strip()
             print(indent_text + get_value_color(item) + item + Style.RESET_ALL)
         if list_separator:
             print(
                 "  " * (indent + 1)
                 + Fore.LIGHTBLACK_EX
```

### Comparing `satori_ci-1.3.2/src/satoricli/classes/validations.py` & `satori_ci-1.3.3/src/satoricli/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.2/src/satoricli/cli/parser.py` & `satori_ci-1.3.3/src/satoricli/cli/parser.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.2/PKG-INFO` & `satori_ci-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.3.2
+Version: 1.3.3
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

