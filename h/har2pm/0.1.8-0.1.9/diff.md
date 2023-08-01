# Comparing `tmp/har2pm-0.1.8.tar.gz` & `tmp/har2pm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2pm-0.1.8.tar", max compression
+gzip compressed data, was "har2pm-0.1.9.tar", max compression
```

## Comparing `har2pm-0.1.8.tar` & `har2pm-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.8/har2pm/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.8/har2pm/cli.py
--rw-r--r--   0        0        0     3723 2023-07-18 03:33:17.277795 har2pm-0.1.8/har2pm/common.py
--rw-r--r--   0        0        0     1950 2023-07-27 02:36:24.900740 har2pm-0.1.8/har2pm/har2postman.py
--rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.8/LICENSE
--rw-r--r--   0        0        0      689 2023-07-27 02:36:34.615759 har2pm-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.8/README.md
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.9/har2pm/__init__.py
+-rw-r--r--   0        0        0     1353 2023-08-01 09:27:00.802867 har2pm-0.1.9/har2pm/cli.py
+-rw-r--r--   0        0        0     3723 2023-07-18 03:33:17.277795 har2pm-0.1.9/har2pm/common.py
+-rw-r--r--   0        0        0     2210 2023-08-01 09:16:06.869516 har2pm-0.1.9/har2pm/har2postman.py
+-rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.9/LICENSE
+-rw-r--r--   0        0        0      689 2023-08-01 09:16:38.760967 har2pm-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.9/README.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.9/PKG-INFO
```

### Comparing `har2pm-0.1.8/har2pm/cli.py` & `har2pm-0.1.9/har2pm/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     parser.add_argument(
         '-V', '--version', dest='version', action='store_true',
         help="show version")
     parser.add_argument(
         '--log-level', default='INFO',
         help="Specify logging level, default is INFO.")
     parser.add_argument(
+        '-S', '--skip-same-url', dest='skip_same_url', action='store_true',
+        help="skip same url",
+    )
+    parser.add_argument(
         'har_path', nargs='?',
         help="har file path")
 
     args = parser.parse_args()
 
     log_level = getattr(logging, args.log_level.upper())
     logging.basicConfig(level=log_level)
@@ -26,15 +30,19 @@
         # no argument passed
         parser.print_help()
         return 0
 
     if args.version:
         print("Version:{}".format(__version__))
         return 0
+    
+    skip_same_url = False
+    if args.skip_same_url:
+        skip_same_url = True
 
     har_path = args.har_path
     if not har_path or not har_path.endswith('.har'):
         logging.error('HAR file not specified.')
         sys.exit(1)
-    har2 = Har2Postman(har_path)
+    har2 = Har2Postman(har_path, skip_same_url)
     har2.run()
     return 0
```

### Comparing `har2pm-0.1.8/har2pm/common.py` & `har2pm-0.1.9/har2pm/common.py`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.8/LICENSE` & `har2pm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.8/pyproject.toml` & `har2pm-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "har2pm"
-version = "0.1.8"
+version = "0.1.9"
 description = "Convert HAR(HTTP Archive) to Postman Collection"
 authors = ["ysansan"]
 license = "MIT"
 homepage = "https://github.com/whitexie/Har2Postman"
 repository = "https://github.com/whitexie/Har2Postman"
 keywords = ["har", "postman"]
 readme = "README.md"
```

### Comparing `har2pm-0.1.8/README.md` & `har2pm-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.8/PKG-INFO` & `har2pm-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2pm
-Version: 0.1.8
+Version: 0.1.9
 Summary: Convert HAR(HTTP Archive) to Postman Collection
 Home-page: https://github.com/whitexie/Har2Postman
 License: MIT
 Keywords: har,postman
 Author: ysansan
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

