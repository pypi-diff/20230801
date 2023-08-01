# Comparing `tmp/dude-0.1.2.tar.gz` & `tmp/dude-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dude-0.1.2.tar", last modified: Thu Dec 10 18:26:55 2020, max compression
+gzip compressed data, was "dude-0.1.3.tar", max compression
```

## Comparing `dude-0.1.2.tar` & `dude-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,3 @@
--rw-r--r--   0        0        0     1317 2020-12-10 18:26:31.805008 dude-0.1.2/dude.py
--rw-r--r--   0        0        0      916 2020-12-10 18:26:10.967537 dude-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      718 2020-12-10 18:26:55.051792 dude-0.1.2/setup.py
--rw-r--r--   0        0        0      775 2020-12-10 18:26:55.051911 dude-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1351 2023-08-01 20:19:38.628615 dude-0.1.3/dude.py
+-rw-r--r--   0        0        0      965 2023-08-01 20:23:02.673856 dude-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 dude-0.1.3/PKG-INFO
```

### Comparing `dude-0.1.2/dude.py` & `dude-0.1.3/dude.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     parser = ArgumentParser()
     parser.add_argument("top", type=Path, nargs="?", default=Path("."))
     parser.add_argument("-f", "--tablefmt", default="plain")
     args = parser.parse_args()
 
     sizes = walk(args.top)
     table = []
-    for path, size in sorted(sizes.items(), key=lambda v: (v[1], v[0])):
+    for path, size in sorted(
+        sizes.items(), key=lambda v: (v[1], -len(v[0].parents), v[0])
+    ):
         if args.top in path.parents or args.top == path:
             end = "/" if path.is_dir() and not path.as_posix().endswith("/") else ""
             table.append(
                 (*naturalsize(size, binary=True).split(), path.as_posix() + end)
             )
 
     print(tabulate(table, tablefmt=args.tablefmt))
```

### Comparing `dude-0.1.2/pyproject.toml` & `dude-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [tool.poetry]
 name = "dude"
-version = "0.1.2"
+version = "0.1.3"
 description = "tool similar to du but a little fancier i guess"
-authors = ["Andrew Herbig <notandrewherbig@gmail.com>"]
+authors = ["Hannah Herbig <nothannahherbig@gmail.com>"]
 license = "MIT"
-repository = "https://github.com/andrew12/dude"
+repository = "https://github.com/hannahherbig/dude"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-humanize = "^3.1.0"
-tabulate = "^0.8.7"
+humanize = ">=3.1,<5.0"
+tabulate = ">=0.8.7,<0.10.0"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^2.9.3"
-isort = "^5.6.4"
-black = "^20.8b1"
-coverage = "^5.3"
+pre-commit = "^2.21.0"
+isort = "^5.11.5"
+black = "^23.3"
+coverage = "^7.2"
 
 [tool.poetry.scripts]
 dude = "dude:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
```

### Comparing `dude-0.1.2/PKG-INFO` & `dude-0.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: dude
-Version: 0.1.2
+Version: 0.1.3
 Summary: tool similar to du but a little fancier i guess
-Home-page: https://github.com/andrew12/dude
+Home-page: https://github.com/hannahherbig/dude
 License: MIT
-Author: Andrew Herbig
-Author-email: notandrewherbig@gmail.com
+Author: Hannah Herbig
+Author-email: nothannahherbig@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: humanize (>=3.1.0,<4.0.0)
-Requires-Dist: tabulate (>=0.8.7,<0.9.0)
-Project-URL: Repository, https://github.com/andrew12/dude
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: humanize (>=3.1,<5.0)
+Requires-Dist: tabulate (>=0.8.7,<0.10.0)
+Project-URL: Repository, https://github.com/hannahherbig/dude
```

