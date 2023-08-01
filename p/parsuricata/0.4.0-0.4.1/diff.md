# Comparing `tmp/parsuricata-0.4.0.tar.gz` & `tmp/parsuricata-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsuricata-0.4.0.tar", max compression
+gzip compressed data, was "parsuricata-0.4.1.tar", max compression
```

## Comparing `parsuricata-0.4.0.tar` & `parsuricata-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3150 2023-08-01 20:06:52.481744 parsuricata-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2021-12-13 17:48:52.294931 parsuricata-0.4.0/LICENSE
--rw-r--r--   0        0        0      801 2021-12-13 17:48:52.294931 parsuricata-0.4.0/README.md
--rw-r--r--   0        0        0      190 2023-08-01 20:06:52.485745 parsuricata-0.4.0/parsuricata/__init__.py
--rw-r--r--   0        0        0     3758 2023-08-01 20:03:42.517925 parsuricata-0.4.0/parsuricata/_parser.py
--rw-r--r--   0        0        0     3090 2023-08-01 19:22:07.060596 parsuricata-0.4.0/parsuricata/rules.py
--rw-r--r--   0        0        0     2397 2023-08-01 19:21:05.899553 parsuricata-0.4.0/parsuricata/transformer.py
--rw-r--r--   0        0        0      852 2023-08-01 20:06:52.177738 parsuricata-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7751 2023-08-01 20:00:31.878069 parsuricata-0.4.0/test_parsuricata.py
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 parsuricata-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3286 2023-08-01 20:16:21.505107 parsuricata-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2021-12-13 17:48:52.294931 parsuricata-0.4.1/LICENSE
+-rw-r--r--   0        0        0      801 2021-12-13 17:48:52.294931 parsuricata-0.4.1/README.md
+-rw-r--r--   0        0        0      190 2023-08-01 20:16:21.509107 parsuricata-0.4.1/parsuricata/__init__.py
+-rw-r--r--   0        0        0     3758 2023-08-01 20:03:42.517925 parsuricata-0.4.1/parsuricata/_parser.py
+-rw-r--r--   0        0        0     3090 2023-08-01 20:14:57.375431 parsuricata-0.4.1/parsuricata/rules.py
+-rw-r--r--   0        0        0     2397 2023-08-01 19:21:05.899553 parsuricata-0.4.1/parsuricata/transformer.py
+-rw-r--r--   0        0        0      852 2023-08-01 20:16:21.249101 parsuricata-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7751 2023-08-01 20:00:31.878069 parsuricata-0.4.1/test_parsuricata.py
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 parsuricata-0.4.1/PKG-INFO
```

### Comparing `parsuricata-0.4.0/CHANGELOG.md` & `parsuricata-0.4.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
 
 
+## [0.4.1] — 2023-08-01
+### Fixed
+ - Resolve minor typing incorrectness (`Option.settings` was referencing removed `KeyValue` type)
+
+
 ## [0.4.0] — 2023-08-01
 ### BREAKING
  - Comma-separated settings now parsed as `Settings` tuple (previously, a `Literal` would be used, or parsing would fail, if some settings were quote-delimited strings)  [GH#15](https://github.com/theY4Kman/parsuricata/issues/15)
 
 ### Added
  - Support parsing of comma-delimited settings
```

### Comparing `parsuricata-0.4.0/LICENSE` & `parsuricata-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parsuricata-0.4.0/README.md` & `parsuricata-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `parsuricata-0.4.0/parsuricata/_parser.py` & `parsuricata-0.4.1/parsuricata/_parser.py`

 * *Files identical despite different names*

### Comparing `parsuricata-0.4.0/parsuricata/rules.py` & `parsuricata-0.4.1/parsuricata/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             body=' \\\n  '.join(str(option) for option in self.options),
         ).strip()
 
 
 @dataclass
 class Option:
     keyword: str
-    settings: Union['Setting', 'KeyValue'] = None
+    settings: Union['Setting', 'Settings'] = None
 
     def __str__(self):
         if self.settings is None:
             return f'{self.keyword};'
         else:
             return f'{self.keyword}: {self.settings!r};'
```

### Comparing `parsuricata-0.4.0/parsuricata/transformer.py` & `parsuricata-0.4.1/parsuricata/transformer.py`

 * *Files identical despite different names*

### Comparing `parsuricata-0.4.0/pyproject.toml` & `parsuricata-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'parsuricata'
-version = "0.4.0"
+version = "0.4.1"
 description = 'Parse Suricata rules'
 authors = ['Zach "theY4Kman" Kanzler <they4kman@gmail.com>']
 license = 'MIT'
 packages = [
   { include = "parsuricata" },
   { include = "test_parsuricata.py", format = "sdist" },
   { include = "LICENSE", format = "sdist" },
```

### Comparing `parsuricata-0.4.0/test_parsuricata.py` & `parsuricata-0.4.1/test_parsuricata.py`

 * *Files identical despite different names*

### Comparing `parsuricata-0.4.0/PKG-INFO` & `parsuricata-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsuricata
-Version: 0.4.0
+Version: 0.4.1
 Summary: Parse Suricata rules
 Home-page: https://github.com/theY4Kman/parsuricata
 License: MIT
 Keywords: suricata,security
 Author: Zach "theY4Kman" Kanzler
 Author-email: they4kman@gmail.com
 Requires-Python: >=3.6,<4.0
```

