# Comparing `tmp/mgmt-0.7.0.tar.gz` & `tmp/mgmt-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgmt-0.7.0.tar", max compression
+gzip compressed data, was "mgmt-0.7.2.tar", max compression
```

## Comparing `mgmt-0.7.0.tar` & `mgmt-0.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-17 02:33:10.918450 mgmt-0.7.0/LICENSE
--rw-r--r--   0        0        0     4773 2023-07-17 02:33:10.918450 mgmt-0.7.0/README.md
--rw-r--r--   0        0        0      553 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/__init__.py
--rw-r--r--   0        0        0       44 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/__main__.py
--rw-r--r--   0        0        0     7759 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/app.py
--rw-r--r--   0        0        0     6839 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/aws.py
--rw-r--r--   0        0        0     2315 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/config.py
--rw-r--r--   0        0        0     4287 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/files.py
--rw-r--r--   0        0        0     1744 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/log.py
--rw-r--r--   0        0        0      338 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/utils.py
--rw-r--r--   0        0        0     2304 2023-07-17 02:33:10.918450 mgmt-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 mgmt-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 09:17:51.774593 mgmt-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4773 2023-08-01 09:17:51.774593 mgmt-0.7.2/README.md
+-rw-r--r--   0        0        0       50 2023-08-01 09:17:51.774593 mgmt-0.7.2/mgmt/__init__.py
+-rw-r--r--   0        0        0       44 2023-08-01 09:17:51.774593 mgmt-0.7.2/mgmt/__main__.py
+-rw-r--r--   0        0        0     8309 2023-08-01 09:17:51.774593 mgmt-0.7.2/mgmt/app.py
+-rw-r--r--   0        0        0     6839 2023-08-01 09:17:51.774593 mgmt-0.7.2/mgmt/aws.py
+-rw-r--r--   0        0        0     2315 2023-08-01 09:17:51.774593 mgmt-0.7.2/mgmt/config.py
+-rw-r--r--   0        0        0     4293 2023-08-01 09:17:51.774593 mgmt-0.7.2/mgmt/files.py
+-rw-r--r--   0        0        0     1744 2023-08-01 09:17:51.774593 mgmt-0.7.2/mgmt/log.py
+-rw-r--r--   0        0        0      338 2023-08-01 09:17:51.778593 mgmt-0.7.2/mgmt/utils.py
+-rw-r--r--   0        0        0     2321 2023-08-01 09:17:51.778593 mgmt-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6327 1970-01-01 00:00:00.000000 mgmt-0.7.2/PKG-INFO
```

### Comparing `mgmt-0.7.0/LICENSE` & `mgmt-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mgmt-0.7.0/README.md` & `mgmt-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mgmt-0.7.0/mgmt/app.py` & `mgmt-0.7.2/mgmt/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import json
 from typing import Optional
 from pathlib import Path
 
+import toml
 import typer
 from rich import box
 from typer import echo
 from rich.table import Table
 from rich.console import Console
 
 from mgmt.aws import AwsStorageMgmt
@@ -14,14 +15,35 @@
 from mgmt.utils import check_selection
 from mgmt.config import Config
 
 app = typer.Typer(add_completion=False)
 aws = AwsStorageMgmt()
 
 
+def get_version():
+    pyproject = toml.load("pyproject.toml")
+    return pyproject["tool"]["poetry"]["version"]
+
+
+def version_callback(value: bool):
+    if value:
+        print(f"Media MGMT CLI Version: {get_version()}")
+        raise typer.Exit()
+
+
+@app.callback()
+def common(
+    ctx: typer.Context,
+    version: bool = typer.Option(
+        None, "--version", callback=version_callback, help="Show the version and exit.", is_eager=True
+    ),
+):
+    pass
+
+
 @app.command()
 def upload(filename: str, compression: Optional[str] = "gzip") -> None:
     """
     Uploads the specified file to S3
 
     Args:
         filename (str): The name of the file or directory to upload.
@@ -71,14 +93,15 @@
     location = "global"
     file_mgmt = FileManager()
     local_files, s3_keys = aws.get_files(location=location)
     echo(f"\nSearching `{location}` for keyword `{keyword}`...")
     local_matches = [file for file in local_files if file_mgmt.keyword_in_string(keyword, file)]
     s3_matches = [file for file in s3_keys if file_mgmt.keyword_in_string(keyword, file)]
 
+    echo(f"total matches found = {str(len(local_matches)+len(s3_matches))}")
     if len(local_matches + s3_matches) >= 1:
         echo("at least one match found\n")
         echo("Local File Matches")
         echo("\n".join(local_matches))
         console = Console()
         table = Table(title="AWS S3 Search Matches", box=box.SIMPLE)
         table.add_column("Option #", style="cyan", no_wrap=True)
```

### Comparing `mgmt-0.7.0/mgmt/aws.py` & `mgmt-0.7.2/mgmt/aws.py`

 * *Files identical despite different names*

### Comparing `mgmt-0.7.0/mgmt/config.py` & `mgmt-0.7.2/mgmt/config.py`

 * *Files identical despite different names*

### Comparing `mgmt-0.7.0/mgmt/files.py` & `mgmt-0.7.2/mgmt/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class FileManager:
     def __init__(self, base_path=None):
         self.logger = Log(debug=False)
         if base_path:
             self.base_path = Path(base_path)
         else:
             config = Config()
-            self.base_path = config.configs.get("MGMT_LOCAL_DIR")
+            self.base_path = Path(config.configs.get("MGMT_LOCAL_DIR"))
         if not self.base_path.exists():
             self.logger.error(f"-- ValueError -- Path {str(self.base_path)} is not a valid path from root")
             self.logger.error("rerun `mgmt config`")
 
     def zip_single_file(self, filename: str) -> str:
         zip_file = filename.split(".")[0] + ".zip"
         with ZipFile(zip_file, "w") as zipf:
```

### Comparing `mgmt-0.7.0/mgmt/log.py` & `mgmt-0.7.2/mgmt/log.py`

 * *Files identical despite different names*

### Comparing `mgmt-0.7.0/pyproject.toml` & `mgmt-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "mgmt"
-version = "0.7.0"
+version = "0.7.2"
 description = ""
 readme = "README.md"
 authors = ["Will Wright <willwright@example.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/will-wright-eng/media-mgmt-cli"
 homepage = "https://github.com/will-wright-eng/media-mgmt-cli"
 
@@ -35,14 +35,15 @@
 six = "^1.16.0"
 urllib3 = "^1.26.14"
 pytest = "^7.2.1"
 typer = "^0.9.0"
 rich = "^13.3.5"
 python-dotenv = "^1.0.0"
 rarfile = "^4.0"
+toml = "^0.10.2"
 
 [package.optional-dependencies]
 test = [
     "pytest >= 7.2.2, < 8.0.0",
     "requests-mock[fixture] >= 1.10.0, < 2.0.0",
     "isort >= 5.12.0, < 6.0.0",
     "black == 23.1.0",
```

### Comparing `mgmt-0.7.0/PKG-INFO` & `mgmt-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgmt
-Version: 0.7.0
+Version: 0.7.2
 Summary: 
 Home-page: https://github.com/will-wright-eng/media-mgmt-cli
 License: GNU GPL v3.0
 Author: Will Wright
 Author-email: willwright@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,15 @@
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: s3transfer (>=0.6.0,<0.7.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
 Project-URL: Repository, https://github.com/will-wright-eng/media-mgmt-cli
 Description-Content-Type: text/markdown
 
 # Media Management Command Line Interface
```

