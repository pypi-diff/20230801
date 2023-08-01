# Comparing `tmp/satori_ci-1.2.9.tar.gz` & `tmp/satori_ci-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.2.9.tar", last modified: Mon May 15 23:24:34 2023, max compression
+gzip compressed data, was "satori_ci-1.3.1.tar", last modified: Tue Aug  1 14:45:56 2023, max compression
```

## Comparing `satori_ci-1.2.9.tar` & `satori_ci-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.9/LICENSE
--rw-r--r--   0        0        0     4984 2023-05-15 15:49:56.139568 satori_ci-1.2.9/README.md
--rw-r--r--   0        0        0      646 2023-05-15 23:24:34.356210 satori_ci-1.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.9/src/satorici/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.9/src/satorici/classes/__init__.py
--rw-r--r--   0        0        0     4066 2023-05-15 12:33:16.870027 satori_ci-1.2.9/src/satorici/classes/api.py
--rw-r--r--   0        0        0     1770 2023-05-15 12:33:16.870199 satori_ci-1.2.9/src/satorici/classes/bundler.py
--rw-r--r--   0        0        0     2807 2023-05-15 12:33:16.870273 satori_ci-1.2.9/src/satorici/classes/playbooks.py
--rw-r--r--   0        0        0    20716 2023-05-15 22:14:04.481522 satori_ci-1.2.9/src/satorici/classes/satori.py
--rw-r--r--   0        0        0    10150 2023-05-15 23:24:06.860593 satori_ci-1.2.9/src/satorici/classes/utils.py
--rw-r--r--   0        0        0     1440 2023-05-15 12:33:16.870721 satori_ci-1.2.9/src/satorici/classes/validations.py
--rwxr-xr-x   0        0        0     6027 2023-05-15 12:33:16.870846 satori_ci-1.2.9/src/satorici/satori_module.py
--rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 14:45:33.791812 satori_ci-1.3.1/LICENSE
+-rw-r--r--   0        0        0     7140 2023-08-01 14:45:33.791812 satori_ci-1.3.1/README.md
+-rw-r--r--   0        0        0      755 2023-08-01 14:45:56.007913 satori_ci-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/__main__.py
+-rw-r--r--   0        0        0     4558 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/api.py
+-rw-r--r--   0        0        0     1633 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/bundler.py
+-rw-r--r--   0        0        0      468 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/models.py
+-rw-r--r--   0        0        0     3345 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/playbooks.py
+-rw-r--r--   0        0        0    28020 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/satori.py
+-rw-r--r--   0        0        0    12442 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/utils.py
+-rw-r--r--   0        0        0     1194 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/validations.py
+-rwxr-xr-x   0        0        0     8966 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/cli/parser.py
+-rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.1/PKG-INFO
```

### Comparing `satori_ci-1.2.9/LICENSE` & `satori_ci-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.9/pyproject.toml` & `satori_ci-1.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 [project]
 name = "satori-ci"
-version = "1.2.9"
+version = "1.3.1"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
-    "tqdm>=4.64.1",
     "colorama>=0.4.6",
     "flatdict>=4.0.1",
     "rich>=13.0",
     "gitpython>=3.1.31",
+    "satori-playbook-validator>=3.0.0",
+    "textual>=0.26.0",
+    "packaging>=23.1",
+    "setuptools>=67.8.0",
+    "satori-docs",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://www.satori-ci.com"
 
 [project.scripts]
-satori-cli = "satorici.satori_module:main"
+satori-cli = "satoricli.cli.parser:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `satori_ci-1.2.9/src/satorici/classes/api.py` & `satori_ci-1.3.1/src/satoricli/classes/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import requests
 import sys
 from requests import Response
 from requests.exceptions import HTTPError
-from typing import Union, Any
-from argparse import Namespace
+from typing import Union, Any, Optional
 
-from satorici.classes.utils import FAIL_COLOR, puts, autoformat, log, argument
+from .utils import FAIL_COLOR, autoformat, log, console
+from .models import arguments
 
 HOST = "https://api.satori-ci.com"
+ERROR_MESSAGE = "An error occurred"
 
 
 class SatoriAPI:
-    def __init__(
-        self, token: str, server: Union[str, None], cli_args: Union[Namespace, argument]
-    ):
+    def __init__(self, token: str, server: Union[str, None], cli_args: arguments):
         self.__session__ = requests.Session()
         self.__session__.headers.update(
             Authorization=f"Bearer {token}",
         )
         self.timeout = cli_args.timeout
         self.debug = cli_args.debug
         if self.debug:
@@ -48,44 +47,41 @@
             try:
                 status = res.json()
             except Exception:
                 status = res.text
             if self.debug:
                 autoformat(status, capitalize=True, color=FAIL_COLOR, jsonfmt=self.json)
             else:
-                msg = "Error"
+                msg = ERROR_MESSAGE
                 if isinstance(status, dict) and "detail" in status:
-                    msg += f": {status['detail']}"
-                puts(FAIL_COLOR, msg)
+                    msg += f":[/] {status['detail']}"
+                console.print("[error]" + msg)
         except Exception as e:
-            puts(FAIL_COLOR, "Error")
+            console.print("[error]" + ERROR_MESSAGE)
             log.debug(e)
         else:  # response is 20x
             return resp
         sys.exit(1)
 
-    def runs(self, run_type: str, secrets: str) -> Any:
-        res = self.request("POST", f"runs/{run_type}", json={"secrets": secrets})
+    def runs(self, run_type: str, data: dict) -> Any:
+        res = self.request("POST", f"runs/{run_type}", json=data)
         return res.json()
 
     def repos(self, method: str, repo: str, action: str, **kwargs) -> Any:
         res = self.request(method, f"repos/{repo}/{action}", **kwargs)
         return res.json()
 
     def repos_scan(self, method: str, repo: str, action: str, **kwargs) -> Any:
         res = self.request(method, f"repos/scan/{repo}/{action}", **kwargs)
         return res.json()
 
     def monitors(self, method: str, monitor_id: str, action: str, **kwargs) -> Any:
         res = self.request(method, f"monitors/{monitor_id}/{action}", **kwargs)
         return res.json()
 
-    def monitor_delete(self, parameters: dict) -> None:
-        self.request("DELETE", f"monitors/{parameters['id']}")
-
     def reports(
         self,
         method: str,
         report_id: str,
         action: str,
         raise_error: bool = False,
         **kwargs,
@@ -95,24 +91,40 @@
         )
         report = res.json()
         if isinstance(report, dict) and report.get("json"):
             for e in report["json"]:
                 e.pop("gfx", None)
         return report
 
+    def get_report_output(self, report_id: str):
+        r = self.request("GET", f"reports/{report_id}/output", stream=True)
+        return r.iter_lines()
+
+    def get_report_files(self, report_id: str):
+        return self.request("GET", f"reports/{report_id}/files", stream=True)
+
     def report_delete(self, parameters: dict) -> None:
         self.request("DELETE", f"reports/{parameters['id']}")
 
     def dashboard(self):
         res = self.request("GET", "dashboard")
         return res.json()
 
-    def playbook_get(self, parameters: dict) -> Any:
-        res = self.request("GET", "playbooks", params=parameters)
-        return res.json()
-
-    def playbook_delete(self, parameters: dict) -> None:
-        self.request("DELETE", "playbooks", params=parameters)
+    def playbook(
+        self, method: str, obj_id: str, params: Optional[dict] = None
+    ) -> Union[dict, str, None]:
+        res = self.request(method, f"playbooks/{obj_id}", params=params)
+        if obj_id != "":
+            return res.text
+        if method != "DELETE":
+            return res.json()
 
     def teams(self, method: str, name: str, action: str, **kwargs) -> Any:
         res = self.request(method, f"teams/{name}/{action}", **kwargs)
+        if "application/json" in res.headers["content-type"]:
+            return res.json()
+        else:
+            return res.text
+
+    def users(self, method: str, user: str, action: str, **kwargs) -> Any:
+        res = self.request(method, f"users/{user}/{action}", **kwargs)
         return res.json()
```

### Comparing `satori_ci-1.2.9/src/satorici/classes/bundler.py` & `satori_ci-1.3.1/src/satoricli/classes/bundler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 import io
 import os
-import re
 from pathlib import Path
 from zipfile import ZipFile
 
 import yaml
-
-
-IMPORT_REGEX = re.compile(r"(satori|file):\/(\/[\w-]+)+\.ya?ml")
-
-
-def is_import(value):
-    return isinstance(value, list) and (
-        all(isinstance(e, str) and IMPORT_REGEX.fullmatch(e) for e in value)
-    )
-
-
-def is_input(value):
-    return isinstance(value, list) and (all(isinstance(e, (str, dict)) for e in value))
+from satorici.validator import is_import_group, is_input_group, is_test
 
 
 def get_local_files(config: dict):
     paths = {"imports": set(), "inputs": set()}
     for value in config.values():
-        if is_import(value):
+        if is_import_group(value):
             paths["imports"].update([p[7:] for p in value if p.startswith("file")])
-        elif is_input(value):
+        elif is_input_group(value):
             paths["inputs"].update(
                 [p.get("file") for p in value if isinstance(p, dict) and p.get("file")]
             )
-        elif isinstance(value, dict):
-            paths.update(get_local_files(value))
+        elif is_test(value):
+            subtest_files = get_local_files(value)
+            paths["imports"].update(subtest_files["imports"])
+            paths["inputs"].update(subtest_files["inputs"])
     return paths
 
 
 def get_references(stream, dir):
     file_list = get_local_files(yaml.safe_load(stream))
 
     for key, files in file_list.items():
```

### Comparing `satori_ci-1.2.9/src/satorici/classes/satori.py` & `satori_ci-1.3.1/src/satoricli/classes/satori.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import ast
 import json
 import os
 import shutil
 import sys
 import tempfile
+import time
 import uuid
+import warnings
+from argparse import Namespace
+from base64 import b64decode
 from pathlib import Path
-import time
+
 import requests
 import yaml
-from typing import Union
-from tqdm import tqdm
-from tqdm.utils import CallbackIOWrapper
 from colorama import Fore
-from argparse import Namespace
-
-from satorici.classes.api import SatoriAPI
-from satorici.classes.bundler import make_bundle
-from satorici.classes.utils import (
-    dict_formatter,
-    filter_params,
-    autoformat,
-    check_monitor,
+from rich.progress import open as progress_open, Progress
+from rich.table import Table
+from satorici.validator import validate_playbook
+from satorici.validator.exceptions import PlaybookValidationError, PlaybookVariableError
+from satorici.validator.warnings import NoLogMonitorWarning
+
+from .api import SatoriAPI
+from .bundler import get_local_files, make_bundle
+from .models import arguments
+from .playbooks import display_public_playbooks
+from .utils import (
     FAIL_COLOR,
     KEYNAME_COLOR,
     SATORIURL_COLOR,
-    VALUE_COLOR,
     UUID4_REGEX,
+    VALUE_COLOR,
     autocolor,
-    puts,
-    argument,
-    log,
+    autoformat,
     autotable,
+    check_monitor,
     console,
+    filter_params,
+    log,
+    puts,
 )
-from satorici.classes.validations import get_parameters, validate_parameters
-from satorici.classes.playbooks import display_public_playbooks
+from .validations import get_parameters, validate_parameters
 
 
 class Satori:
     """Have some class"""
 
-    def __init__(self, args: Union[Namespace, argument], config=False) -> None:
+    def __init__(self, args: arguments, config=False) -> None:
         """Turn on the engines"""
         self.profile = args.profile
         self.config_paths = [
             f"{Path.home()}/.satori_credentials.yml",
             ".satori_credentials.yml",
         ]
         self.verbose = False
@@ -106,21 +110,33 @@
                     puts(FAIL_COLOR, "Invalid config format")
                     sys.exit(1)
         else:
             config = {}
             config_file = self.config_paths[0]
 
         config.setdefault(self.profile, {})[key] = value
-
-        with open(config_file, "w") as f:
-            f.write(yaml.safe_dump(config))
-
+        try:
+            with open(config_file, "w") as f:
+                os.chmod(config_file, 0o600)
+                f.write(yaml.safe_dump(config))
+        except Exception:
+            puts(
+                FAIL_COLOR,
+                "Could not write to home directory, writing into current directory",
+            )
+            config_file = self.config_paths[1]
+            with open(config_file, "w") as f:
+                os.chmod(config_file, 0o600)
+                f.write(yaml.safe_dump(config))
         puts(Fore.LIGHTGREEN_EX, key.capitalize() + " saved")
 
-    def run(self, args: Union[Namespace, argument]):
+    def run(self, args: arguments):
+        if args.path.startswith("satori://"):
+            self.run_url(args)
+
         path = Path(args.path)
         params = set()
 
         if getattr(args, "data", False):
             try:
                 data = ast.literal_eval(args.data)
 
@@ -133,130 +149,133 @@
                 sys.exit(1)
 
         if path.is_dir():
             playbook = path / ".satori.yml"
         elif path.is_file():
             playbook = path
         else:
-            puts(FAIL_COLOR, "Satori can not access to file/folder")
+            puts(FAIL_COLOR, "Playbook file or folder not found")
             sys.exit(1)
 
         playbook_text = playbook.read_text()
+        config = None
+
         try:
-            variables = get_parameters(yaml.safe_load(playbook_text))
+            config = yaml.safe_load(playbook_text)
+
+            with warnings.catch_warnings(record=True) as w:
+                validate_playbook(config)
+
+            for warning in w:
+                if warning.category == NoLogMonitorWarning:
+                    console.print(
+                        "[warning]WARNING:[/] No notifications (log, onLogFail or onLogPass) were defined for the Monitor"
+                    )
         except yaml.YAMLError as e:
-            console.log(
-                f"Error parsing the playbook [bold]{playbook.name}[/bold]:\n", e
+            console.print(f"Error parsing the playbook [bold]{playbook.name}[/]:\n", e)
+            sys.exit(1)
+        except PlaybookVariableError:
+            pass
+        except PlaybookValidationError as e:
+            console.print(
+                f"Validation error on playbook [bold]{playbook.name}[/]:\n", e
             )
             sys.exit(1)
+
+        if not isinstance(config, dict):
+            console.print("[error]Failed to load the playbook")
+            sys.exit(1)
+
+        variables = get_parameters(config)
+
         if variables - params:
-            puts(FAIL_COLOR, f"Required parameters: {variables - params}")
+            console.print(f"[error]Required parameters: {variables - params}")
             sys.exit(1)
 
         if path.is_dir():
             exec_data = self.run_folder(args)
         else:  # is file
             exec_data = self.run_file(args)
-        if args.sync and exec_data:
-            self.run_sync(exec_data)
+        if (args.sync or args.output or args.report or args.files) and exec_data:
+            self.run_sync(exec_data, args)
 
-    def run_file(self, args: Union[Namespace, argument]) -> dict:
+    def run_file(self, args: arguments) -> dict:
         """Just run"""
         playbook = args.path
-        if playbook is None:
-            print(
-                f"Define the Satori playbook file:\n{sys.argv[0]} run -p playbook.yml"
-            )
-            sys.exit(1)
-
-        if not os.path.isfile(playbook):
-            puts(FAIL_COLOR, f"Playbook not found: {playbook}")
-            sys.exit(1)
-
         bundle = make_bundle(playbook)
         is_monitor = check_monitor(playbook)
-        url = self.api.runs("bundle", args.data)
+        url = self.api.runs("bundle", {"secrets": args.data})
         log.debug(url)
-        res = requests.post(
+        res = requests.post(  # nosec
             url["url"], url["fields"], files={"file": bundle}, timeout=None
         )
         log.debug(res.text)
         if not res.ok:
             puts(FAIL_COLOR, "File upload failed")
             sys.exit(1)
         if is_monitor:
             exec_type = "monitor"
             exec_id = url["monitor"]
             print(KEYNAME_COLOR + "Monitor ID: " + VALUE_COLOR + f"{exec_id}")
             print(autocolor(f"Status: https://www.satori-ci.com/status?id={exec_id}"))
         else:
             exec_type = "report"
             exec_id = url["fields"]["key"].split("/")[1]
-            print(KEYNAME_COLOR + "UUID: " + VALUE_COLOR + f"{exec_id}")
+            print(KEYNAME_COLOR + "Report ID: " + VALUE_COLOR + f"{exec_id}")
             print(
                 KEYNAME_COLOR
                 + "Report: "
                 + SATORIURL_COLOR
                 + f"https://www.satori-ci.com/report_details/?n={exec_id}"
             )
         return {"type": exec_type, "id": exec_id}
 
-    def run_folder(self, args: Union[Namespace, argument]) -> dict:
+    def run_folder(self, args: arguments) -> dict:
         """Upload directory and run"""
         directory = args.path
-        if directory is None:
-            print(
-                "Define the directory with the Satori playbook:"
-                f"\n{sys.argv[0]} run -p ./directory_with_playbook"
-            )
-            sys.exit(1)
-
-        if not os.path.isdir(directory):
-            puts(FAIL_COLOR, f"Directory not found: {directory}")
-            sys.exit(1)
-
         satori_yml = Path(directory, ".satori.yml")
         bundle = make_bundle(str(satori_yml), from_dir=True)
         is_monitor = check_monitor(satori_yml)
         temp_file = Path(tempfile.gettempdir(), str(uuid.uuid4()))
-        full_path = f"{temp_file}.zip"
+        full_path = f"{temp_file}.tar.gz"
+
+        local_ymls = list(
+            filter(lambda p: p.is_file(), Path(args.path).rglob(".satori.yml"))
+        )
+
+        imported = get_local_files(yaml.safe_load(satori_yml.read_text()))["imports"]
+
+        if len(local_ymls) > 1 and len(local_ymls) - 1 > len(imported):
+            console.print("[warning]WARNING:[/] There are some .satori.yml outside the root folder that have not been imported.")
 
         try:
-            shutil.make_archive(str(temp_file), "zip", directory)
+            shutil.make_archive(str(temp_file), "gztar", directory)
         except Exception as e:
             puts(FAIL_COLOR, f"Could not compress directory: {e}")
             sys.exit(1)
 
-        res = self.api.runs("archive", args.data)
+        res = self.api.runs("archive", {"secrets": args.data})
         log.debug(res)
         arc = res["archive"]
         bun = res["bundle"]
         mon = res["monitor"]
 
         try:
-            bar_params = {
-                "total": os.stat(full_path).st_size,
-                "unit": "B",
-                "desc": "Archive upload",
-                "unit_scale": True,
-            }
-            with tqdm(**bar_params) as t, open(full_path, "rb") as f:
-                w = CallbackIOWrapper(t.update, f, "read")
-                file = {"file": w}
-                res = requests.post(
-                    arc["url"], arc["fields"], files=file, timeout=None  # type: ignore
+            with progress_open(full_path, "rb", description="Uploading...") as f:
+                res = requests.post(  # nosec
+                    arc["url"], arc["fields"], files={"file": f}, timeout=None
                 )
         finally:
             os.remove(full_path)
 
         if not res.ok:
             print("Archive upload failed")
             sys.exit(1)
 
-        res = requests.post(
+        res = requests.post(  # nosec
             bun["url"], bun["fields"], files={"file": bundle}, timeout=None
         )
         log.debug(res.text)
         if not res.ok:
             print("Bundle upload failed")
             sys.exit(1)
 
@@ -264,24 +283,37 @@
             exec_type = "monitor"
             exec_id = mon
             print(KEYNAME_COLOR + "Monitor ID: " + VALUE_COLOR + f"{mon}")
             print(autocolor(f"Status: https://www.satori-ci.com/status?id={mon}"))
         else:
             exec_type = "report"
             exec_id = bun["fields"]["key"].split("/")[1]
-            print(KEYNAME_COLOR + "UUID: " + VALUE_COLOR + f"{exec_id}")
+            print(KEYNAME_COLOR + "Report ID: " + VALUE_COLOR + f"{exec_id}")
             print(
                 autocolor(
                     f"Report: https://www.satori-ci.com/report_details/?n={exec_id}"
                 )
             )
         return {"type": exec_type, "id": exec_id}
 
-    def run_sync(self, exec_data: dict) -> None:
-        puts(KEYNAME_COLOR, "Fetching data...", end="\r")
+    def run_url(self, args: arguments):
+        info = self.api.runs("url", {"secrets": args.data, "url": args.path})
+        autoformat({"Running with the ID": info.get("report_id")}, jsonfmt=args.json)
+        if args.sync or args.output or args.report:
+            exec_data = {"type": "report", "id": info["report_id"]}
+            self.run_sync(exec_data, args)
+        sys.exit(0)
+
+    def run_sync(self, exec_data: dict, args: arguments) -> None:
+        if exec_data["type"] == "monitor":
+            console.print(
+                "[warning]WARNING:[/] Sync mode is not supported for monitors"
+            )
+            sys.exit(0)
+        console.print("[key]Fetching data...", end="\r")
         start_time = time.time()
         spin = "-\\|/"
         pos = 0
         while True:
             pos += 1
             if pos >= len(spin):
                 pos = 0
@@ -299,59 +331,70 @@
                         autocolor(
                             f"{spin[pos]} Report status: Unknown | {elapsed_text}"
                         ),
                         end="\r",
                     )
                     continue
                 else:
-                    puts(FAIL_COLOR, f"Failed to get data\nStatus code: {code}")
+                    console.print(f"[error]Failed to get data\n[/]Status code: {code}")
                     sys.exit(1)
 
             status = report_data.get("status", "Unknown")
             if status in ("Completed", "Undefined"):
                 fails = report_data["fails"]
-                if fails is None:
-                    result = "Unknown"
-                else:
+                if isinstance(fails, int):
                     result = "Pass" if fails == 0 else f"Fail({fails})"
+                else:
+                    result = "Unknown"
                 print(
                     autocolor(
                         f"- Report status: {status} | Result: {result} | {elapsed_text}"
                     ),
                     end="\r\n",
                 )
-                report_out = []
-                # Remove keys
-                json_data = report_data.get("json") or []
-                for report in json_data:
-                    report.pop("gfx", None)
-                    report_out.append(report)
-                    asserts = []
-                    for asrt in report["asserts"]:
-                        asrt.pop("count", None)
-                        asrt.pop("description", None)
-                        if len(asrt.get("data", [])) == 0:
-                            asrt.pop("data", None)
-                        asserts.append(asrt)
-                autoformat(report_out, list_separator="- " * 20)
+                if args.report:  # --report or -r
+                    report_out = []
+                    # Remove keys
+                    json_data = report_data.get("json") or []
+                    for report in json_data:
+                        report.pop("gfx", None)
+                        report_out.append(report)
+                        asserts = []
+                        for asrt in report["asserts"]:
+                            asrt.pop("count", None)
+                            asrt.pop("description", None)
+                            if len(asrt.get("data", [])) == 0:
+                                asrt.pop("data", None)
+                            asserts.append(asrt)
+                    autoformat(report_out, list_separator="- " * 20)
+                elif args.output:
+                    out_args = Namespace(
+                        id=exec_data["id"], action="output", json=args.json
+                    )
+                    self.output(out_args.id)
+                elif args.files:
+                    self.output_files(exec_data["id"])
+                else:  # --sync or -s
+                    # TODO: print something else?
+                    pass  # already printed
                 if status == "Undefined":
                     comments = report_data.get("comments")
                     if comments:
                         puts(FAIL_COLOR, f"Error: {comments}")
                     sys.exit(1)
-                else:
+                else:  # Completed
                     # Return code 0 if report status==pass else 1
                     sys.exit(0 if report_data["fails"] == 0 else 1)
             else:
                 print(
                     autocolor(f"{spin[pos]} Report status: {status} | {elapsed_text}"),
                     end="\r",
                 )
 
-    def repo(self, args: Union[Namespace, argument]):
+    def repo(self, args: arguments):
         """Run Satori on multiple commits"""
         params = filter_params(args, ("id",))
         if args.playbook:
             playbook = Path(args.playbook)
             if playbook.is_file():
                 args.playbook = playbook.read_text()
         if args.action == "scan":
@@ -363,16 +406,24 @@
         elif args.action == "clean":
             params = filter_params(args, ("id", "delete_commits"))
             info = self.api.repos("GET", args.id, args.action, params=params)
         elif args.action == "tests":
             params = filter_params(args, ("id", "filter", "all", "limit", "fail"))
             info = self.api.repos("GET", args.id, args.action, params=params)
         elif args.action == "run":
-            params = filter_params(args, ("id", "data", "playbook"))
-            info = self.api.repos_scan("GET", args.id, "last", params=params)
+            params = filter_params(args, ("data", "playbook"))
+            params["url"] = args.id
+            info = self.api.repos_scan("GET", "", "last", params=params)
+            if args.sync:
+                if len(info) == 1:
+                    console.print(
+                        "Report: [link]https://www.satori-ci.com/report_details/?n="
+                        + info[0]["status"].replace("Report running ", "")
+                    )
+                self.sync_reports_list(info)
         elif args.action == "scan-stop":
             info = self.api.repos_scan("GET", args.id, "stop", params=params)
         elif args.action == "scan-status":
             info = self.api.repos_scan("GET", args.id, "status", params=params)
         elif args.action == "check-forks":
             info = self.api.repos_scan("GET", args.id, args.action, params=params)
         elif args.action == "check-commits":
@@ -384,165 +435,275 @@
             puts(FAIL_COLOR, "Unknown subcommand")
             sys.exit(1)
 
         if args.id != "" or args.action != "" or args.json:
             autoformat(info, jsonfmt=args.json, list_separator="-" * 48)
         else:  # Default command (satori-cli repo)
             if len(info["pending"]) > 1:
-                print("Pending actions:")
-                autotable(info["pending"], "bold red")
-            print("\nRepos:")
-            autotable(info["list"], "bold blue")
+                console.rule("[b red]Pending actions", style="red")
+                autotable(info["pending"], "bold red", widths=(50, 50))
+            console.rule("[b green]GitHub Repositories", style="green")
+            autotable(info["list"], "bold blue", widths=(None, 10, 12, 20, 10, 40))
         if args.action == "run" and args.sync:
             if isinstance(info, list):
                 info = info[0]
             report = info.get("status", "")
             match = UUID4_REGEX.findall(report)
             if match:
-                self.run_sync({"type": "report", "id": match[0]})
+                self.run_sync({"type": "report", "id": match[0]}, args)
 
-    def report(self, args: Union[Namespace, argument]):
+    def report(self, args: arguments):
         """Show a list of reports"""
         params = filter_params(args, ("id",))
-        if args.action == "":
+        if args.action == "":  # default: print reports
             params = filter_params(args, ("id", "page", "limit", "filter"))
             res = self.api.reports("GET", args.id, "", params=params)
-            if isinstance(res, list) and not args.json:
-                for commit in res:
-                    dict_formatter(commit)
-                    puts(Fore.LIGHTBLACK_EX, ("_" * 48) + "\n")
-            else:
+            if args.id == "" and not args.json:  # default: print list
+                autoformat(res["list"])
+                console.print(
+                    f"[b]Page:[/] {res['current_page']} of {res['total_pages']}"
+                )
+            else:  # single report or json output
                 autoformat(res, jsonfmt=args.json)
-            if not args.json:
-                print(f"Current page: {args.page}")
         elif args.action == "output":
-            self.output(args, params)
+            self.output(args.id)
+        elif args.action == "files":
+            self.output_files(args.id)
         elif args.action == "stop":
             res = self.api.reports("GET", args.id, "stop")
             autoformat(res, jsonfmt=args.json)
         elif args.action == "delete":
             self.api.report_delete(params)
             print("Report deleted")
         else:
             print("Unknown subcommand")
             sys.exit(1)
 
-    def monitor(self, args: Union[Namespace, argument]):
+    def monitor(self, args: arguments):
         """Get information about the"""
         params = filter_params(args, ("id",))
         if args.action == "delete":
-            self.api.monitor_delete(params)
+            params = filter_params(args, ("clean",))
+            self.api.request("DELETE", f"monitors/{args.id}", params=params)
             print("Monitor deleted")
             sys.exit(0)
         elif args.action == "":
-            info = self.api.monitors("GET", args.id, "")
+            params = filter_params(args, ("id", "deleted"))
+            info = self.api.monitors("GET", args.id, "", params=params)
         elif args.action in ("start", "stop"):
             info = self.api.monitors("PATCH", args.id, args.action)
         else:
             print("Unknown subcommand")
             sys.exit(1)
         if args.id != "" or args.action != "" or args.json:
             autoformat(info, jsonfmt=args.json, list_separator="*" * 48)
         else:  # Default command (satori-cli monitor)
             if len(info["pending"]) > 1:
-                print("Pending actions:")
-                autotable(info["pending"], "bold red")
-            print("\nMonitors:")
-            autotable(info["list"], "bold blue")
+                console.rule("[b red]Pending actions", style="red")
+                autotable(info["pending"], "b red")
+            console.rule("[b blue]Monitors", style="blue")
+            autotable(info["list"], "b blue")
 
-    def output(self, args, params):
+    def output(self, report_id: str):
         """Returns commands output"""
-        try:
-            uuid.UUID(args.id)
-        except ValueError:
-            puts(FAIL_COLOR, f"{args.id} is not a valid report ID")
-            sys.exit(1)
-        data = self.api.reports("GET", args.id, args.action, params=params)
-
-        if not args.json:  # default output
-            outputs = data.pop("output", [])
-            for key, value in data.items():
-                print(f"{key}: {value}")
-
-            for row in outputs:
-                puts(Fore.LIGHTBLACK_EX, "-" * 48)
-                puts(Fore.CYAN, f"test_name: {row['test_name']}")
-                puts(KEYNAME_COLOR, "command: ", Fore.LIGHTBLUE_EX, row["command"])
-                for key, value in row.items():
-                    if key in ("test_name", "command"):
-                        continue
-                    val_color = VALUE_COLOR
-                    if key == "stdout":
-                        val_color = Fore.LIGHTGREEN_EX
-                    elif key == "stderr":
-                        val_color = Fore.LIGHTRED_EX
-                    elif key == "return_code":
-                        val_color = Fore.YELLOW
-                    puts(KEYNAME_COLOR, f"{key}: ", val_color, str(value))
-        else:
-            print(json.dumps(data, indent=2))
+        current_path = ""
+
+        for line in self.api.get_report_output(report_id):
+            output = json.loads(line)
+
+            if current_path != output["path"]:
+                console.rule(f"[b]{output['path']}[/b]")
+                current_path = output["path"]
+
+            console.print(f"[b][green]Command:[/green] {output['original']}[/b]")
+
+            if output["testcase"]:
+                testcase = Table(show_header=False, show_edge=False)
 
-    def dashboard(self, args: Union[Namespace, argument]):
+                testcase.add_column(style="b")
+                testcase.add_column()
+
+                for key, value in output["testcase"].items():
+                    testcase.add_row(key, b64decode(value).decode(errors="ignore"))
+
+                console.print("[blue]Testcase:[/blue]")
+                console.print(testcase)
+
+            console.print("[blue]Return code:[/blue]", output["output"]["return_code"])
+            console.print("[blue]Stdout:[/blue]")
+            if output["output"]["stdout"]:
+                console.out(
+                    b64decode(output["output"]["stdout"])
+                    .decode(errors="ignore")
+                    .strip()
+                )
+            console.print("[blue]Stderr:[/blue]")
+            if output["output"]["stderr"]:
+                console.out(
+                    b64decode(output["output"]["stderr"])
+                    .decode(errors="ignore")
+                    .strip()
+                )
+
+    def output_files(self, report_id: str):
+        r = self.api.get_report_files(report_id)
+        total = int(r.headers["Content-Length"])
+
+        with Progress() as progress:
+            task = progress.add_task("Downloading...", total=total)
+
+            with open(f"satorici-files-{report_id}.tar.gz", "wb") as f:
+                for chunk in r.iter_content():
+                    progress.update(task, advance=len(chunk))
+                    f.write(chunk)
+
+    def dashboard(self, args: arguments):
         """Get user dashboard"""
         info = self.api.dashboard()
         if args.json:
             autoformat(info, jsonfmt=True)
         else:
             len_mon = len(info["monitors"]["pending"])
             len_rep = len(info["repos"]["pending"])
             if len_mon > 0 or len_rep > 0:
                 # print pending actions
                 if len_mon > 0:
-                    print("Monitors(Actions required):")
-                    autotable(info["monitors"]["pending"], "bold green")
+                    console.rule(
+                        "[b][blue]Monitors[/blue] (Actions required)", style="white"
+                    )
+                    autotable(
+                        info["monitors"]["pending"], "b blue", widths=(20, 20, None)
+                    )
                 if len_rep > 0:
-                    print("Repos(Actions required):")
-                    autotable(info["repos"]["pending"], "bold green")
+                    console.rule(
+                        "[b][green]GitHub Repositories[/green] (Actions required)",
+                        style="white",
+                    )
+                    autotable(info["repos"]["pending"], "b green", widths=(50, 50))
             if len(info["monitors"]["list"]) == 0:
-                print("\nMonitors: no active monitors defined")
+                console.print("[b]Monitors:[red] no active monitors defined")
             else:
-                print("Monitors:")
-                autotable(info["monitors"]["list"], "bold blue", True)
+                console.rule("[b blue]Monitors", style="blue")
+                autotable(info["monitors"]["list"], "b blue", True)
             if len(info["repos"]["list"]) > 0:
-                print("Repos:")
-                autotable(info["repos"]["list"], "bold blue", True)
+                console.rule("[b green]Github Repositories", style="green")
+                autotable(
+                    info["repos"]["list"],
+                    "b green",
+                    True,
+                    widths=(3, None, 10, 12, 20, 10, 40),
+                )
 
-    def playbook(self, args: Union[Namespace, argument]):
+    def playbook(self, args: arguments):
         """Get playbooks"""
-        if args.public:
-            display_public_playbooks()
+        if args.public or args.id.startswith("satori://"):
+            display_public_playbooks(args.id)
 
         if args.action == "":
-            params = filter_params(args, ("id", "limit", "page"))
-            data = self.api.playbook_get(params)
-            if args.json:
-                autoformat(data, jsonfmt=True)
-                sys.exit(1)
+            if args.id == "":
+                # Default: get list of user playbooks
+                params = filter_params(args, ("limit", "page"))
+                data = self.api.playbook("GET", "", params)
+            else:
+                data = self.api.playbook("GET", args.id)
         elif args.action == "delete":
-            params = filter_params(args, ("id",))
-            data = self.api.playbook_delete(params)
+            data = self.api.playbook("DELETE", args.id)
+            print("Playbook Deleted")
+            sys.exit(0)
         else:
             print("Unknown subcommand")
             sys.exit(1)
         autoformat(data, jsonfmt=args.json, list_separator="-" * 48)
 
-    def team(self, args: Union[Namespace, argument]):
+    def team(self, args: arguments):
         """Get information about the"""
         params = filter_params(args, ("id",))
         if args.action == "":
-            info = self.api.teams("GET", "", "", params=params)
+            info = self.api.teams("GET", args.id, "", params=params)
         elif args.action == "create":
-            info = self.api.teams("PUT", args.id, "", data=params)
+            info = self.api.teams("POST", args.id, "", json=params)
         elif args.action == "members":
             info = self.api.teams("GET", args.id, "members", params=params)
         elif args.action == "add_member":
             params = filter_params(args, ("id", "email", "role"))
-            info = self.api.teams("PUT", args.id, "members", data=params)
+            info = self.api.teams("POST", args.id, "members", json=params)
         elif args.action == "repos":
-            info = self.api.teams("PUT", args.id, "repos", data=params)
+            info = self.api.teams("GET", args.id, "repos", data=params)
         elif args.action == "add_repo":
             params = filter_params(args, ("id", "repo"))
-            info = self.api.teams("PUT", args.id, "repos", data=params)
+            info = self.api.teams("POST", args.id, "repos", json=params)
+        elif args.action == "get_config":
+            info = self.api.teams("GET", args.id, f"config/{args.config_name}")
+        elif args.action == "set_config":
+            info = self.api.teams(
+                "PUT",
+                args.id,
+                "config",
+                json={"name": args.config_name, "value": args.config_value},
+            )
+        elif args.action == "get_token":
+            info = self.api.teams("GET", args.id, "token")
+        elif args.action == "refresh_token":
+            info = self.api.teams("PUT", args.id, "token")
+        elif args.action == "delete":
+            self.api.request("DELETE", f"teams/{args.id}")
+            console.print("Team deleted")
+            sys.exit(0)
+        elif args.action == "del_member":
+            self.api.request(
+                "DELETE", f"teams/{args.id}/members", json={"email": args.email}
+            )
+            console.print("Team member deleted")
+            sys.exit(0)
         else:
             print("Unknown subcommand")
             sys.exit(1)
         autoformat(info, jsonfmt=args.json, list_separator="*" * 48, table=True)
+
+    def sync_reports_list(self, report_list: list[dict]) -> None:
+        completed = []
+        n = 0
+        with console.status("[bold cyan]Getting results...") as report:
+            while len(completed) < len(report_list):
+                report = report_list[n]["status"].replace("Report running ", "")
+                repo = report_list[n]["repo"]
+                if repo not in completed:
+                    if report == "Failed to scan commit":
+                        console.print(f"[bold]{repo}[/bold] [red]Failed to start")
+                        completed.append(repo)
+                    try:
+                        report_data = self.api.reports(
+                            "GET", report, "", raise_error=True
+                        )
+                    except requests.HTTPError as e:
+                        code = e.response.status_code
+                        if code not in (404, 403):
+                            console.print(
+                                f"[red]Failed to get data\nStatus code: {code}"
+                            )
+                            sys.exit(1)
+                    else:
+                        report_status = report_data.get("status", "Unknown")
+                        if report_status in ("Completed", "Undefined"):
+                            fails = report_data["fails"]
+                            if fails is None:
+                                result = "[yellow]Unknown"
+                            else:
+                                result = (
+                                    "[green]Pass"
+                                    if fails == 0
+                                    else f"[red]Fail({fails})"
+                                )
+                            console.print(
+                                f"[bold]{repo}[/bold] Completed | Result: {result}"
+                            )
+                            completed.append(repo)
+                time.sleep(0.5)
+                n += 1
+                if n >= len(report_list):
+                    n = 0
+        sys.exit(0)
+
+    def user(self, args: arguments):
+        """Get information about the"""
+        info = self.api.users("GET", args.action, args.id)
+        autoformat(info, jsonfmt=args.json, table=True)
```

### Comparing `satori_ci-1.2.9/src/satorici/classes/utils.py` & `satori_ci-1.3.1/src/satoricli/classes/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,95 @@
-from typing import Union
+from typing import Union, Optional
 import json
 import yaml
 import re
 from typing import Any
 from colorama import Fore, Style
 from rich.logging import RichHandler
 import logging
 from rich import print_json
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
+from rich.theme import Theme
+from rich.highlighter import RegexHighlighter
 import random
-from dataclasses import dataclass
 
 __decorations = "▢•○░"
 __random_colors = ["green", "blue", "red"]
 # IDs
 UUID4_REGEX = re.compile(
     r"[0-9a-f]{8}-[0-9a-f]{4}-4[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}",
     re.I,
 )
 # Regex
-PASS_REGEX = re.compile(r"(pass|completed)", re.IGNORECASE)
+PASS_REGEX = re.compile(r"(pass|completed|^yes$)", re.IGNORECASE)
 RUNNING_REGEX = re.compile(r"(pending|running)", re.IGNORECASE)
-FAIL_REGEX = re.compile(r"(fail(\(\d+\))?|error)", re.IGNORECASE)
+FAIL_REGEX = re.compile(r"(fail(\(\d+\))?|(?<!\w)error(?!\w)|^no$)", re.IGNORECASE)
 UNKNOWN_REGEX = re.compile(r"(unknown|undefined)", re.IGNORECASE)
 SATORIURL_REGEX = re.compile(r"(https?:\/\/(www\.)satori-ci\.com\S+)")
 KEYNAME_REGEX = re.compile(r"(([^\w]|^)\w[\w\s]*:\s*)(?!\/\/)")  # ex: "key: "
-# Colors outputs
+
+# Colors outputs | TODO: remove this
 PASS_COLOR = Fore.LIGHTGREEN_EX
 FAIL_COLOR = Fore.LIGHTRED_EX
 UNKNOWN_COLOR = Fore.LIGHTYELLOW_EX
 RUNNING_COLOR = Fore.LIGHTBLUE_EX
 KEYNAME_COLOR = Fore.WHITE
 SATORIURL_COLOR = Fore.LIGHTBLUE_EX
 VALUE_COLOR = Fore.CYAN
 MULTILINE_COLOR = Fore.YELLOW
 
+# Set rich theme and console
+# https://rich.readthedocs.io/en/latest/appendix/colors.html#appendix-colors
+class SatoriHighlighter(RegexHighlighter):
+    base_style = "satori."
+    highlights = [
+        r"(?P<value>(?<=:\s)\w+$)",
+        r"(?P<email>[\w-]+@([\w-]+\.)+[\w-]+)",
+        r"(?P<pass>(?<!\w)(pass|completed|yes|true)(?!\w))",
+        r"(?P<pending>(?<!\w)(pending|running)(?!\w))",
+        r"(?P<fail>(?<!\w)(fail(\(\d+\))?|error|no|false)(?!\w))",
+        r"(?P<unknown>(?<!\w)(unknown|undefined|null|None)(?!\w))",
+        r"(?P<satori_com>https?:\/\/(www\.)satori-ci\.com\S+)",
+        r"(?P<key>([^\w]|^)\w[\w\s]*:\s*)(?!\/\/)",
+        r"(?P<number>(?<!\w)\-?[0-9]+\.?[0-9]*(e[-+]?\d+?)?\b|0x[0-9a-fA-F]*)",
+        r"(?P<uuid>[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12})",
+    ]
+
+
+satori_theme = Theme(
+    {
+        "debug": "dim blue",
+        "info": "dim cyan",
+        "warning": "yellow",
+        "danger": "bold red",
+        "error": "red",
+        "critical": "on red",
+        "multiline": "yellow",
+        "satori.email": "cyan",
+        "satori.pass": "chartreuse1",
+        "satori.pending": "dark_slate_gray3",
+        "satori.fail": "bright_red",
+        "satori.unknown": "bright_yellow",
+        "satori.satori_com": "turquoise2",
+        "satori.key": "white b",
+        "satori.value": "cyan1",
+        "satori.number": "deep_sky_blue1",
+        "satori.uuid": "purple",
+    }
+)
+console = Console(highlighter=SatoriHighlighter(), theme=satori_theme, log_path=False)
+
 logging.basicConfig(
     level="CRITICAL",
     format="%(message)s",
     handlers=[RichHandler(rich_tracebacks=True, show_time=False)],
 )
 log = logging.getLogger()
-console = Console(log_path=False, log_time=False)
 
 
 def get_decoration(indent):
     return (
         Style.DIM
         + "  " * indent
         + __decorations[indent % len(__decorations)]
@@ -68,38 +110,39 @@
         if isinstance(obj[key], dict):
             print(indent_text + KEYNAME_COLOR + f"{key_text}:" + Style.RESET_ALL)
             dict_formatter(obj[key], capitalize, indent + 1, list_separator)
         elif isinstance(obj[key], list):
             print(indent_text + KEYNAME_COLOR + f"{key_text}:" + Style.RESET_ALL)
             list_formatter(obj[key], capitalize, indent + 1, list_separator)
         else:
-            item = str(obj[key])
+            item = str(obj[key]).strip()
             color = get_value_color(item)
             print(indent_text + KEYNAME_COLOR + f"{key_text}: ", end="")
             if item.count("\n") > 0:
+                print()#add empty line
                 if autosyntax(item, indent + 2):
                     continue
             # Not JSON or YAML
             print(color + item + Style.RESET_ALL)
 
 
 def list_formatter(
     obj: list,
     capitalize: bool = False,
     indent: int = 0,
-    list_separator: Union[str, None] = None,
+    list_separator: Optional[str] = None,
 ):
     for item in obj:
         indent_text = get_decoration(indent)
         if isinstance(item, dict):
             dict_formatter(item, capitalize, indent + 1, list_separator)
         elif isinstance(item, list):
             list_formatter(item, capitalize, indent + 1, list_separator)
         else:
-            item = str(item)
+            item = str(item).strip()
             print(indent_text + get_value_color(item) + item + Style.RESET_ALL)
         if list_separator:
             print(
                 "  " * (indent + 1)
                 + Fore.LIGHTBLACK_EX
                 + list_separator
                 + Style.RESET_ALL
@@ -107,15 +150,15 @@
 
 
 def autoformat(
     obj: Any,
     capitalize: bool = False,
     indent: int = 0,
     jsonfmt: bool = False,
-    list_separator: Union[str, None] = None,
+    list_separator: Optional[str] = None,
     color: str = "",
     table: bool = False,
 ) -> None:
     """Format and print a dict, list or other var
 
     Parameters
     ----------
@@ -138,17 +181,19 @@
         elif isinstance(obj, list):
             if table and len(obj) > 0 and isinstance(obj[0], dict):
                 head_color = random.choice(__random_colors)  # nosec
                 autotable(obj, f"bold {head_color}")
                 return None
             list_formatter(obj, capitalize, indent, list_separator)
         elif isinstance(obj, str):
-            if obj.count("\n") > 0:
-                if not autosyntax(obj, indent):
+            if obj.count("\n") > 0:  # multiline
+                if not autosyntax(obj, indent):  # autodetect syntax and print
                     print(obj)
+            else:  # singleline
+                print(obj)
         else:
             print(color + str(obj) + Style.RESET_ALL)
 
 
 def filter_params(params: Any, filter_keys: Union[tuple, list]) -> dict:
     """Filter elements of a dict/namespace according to a list of keys
 
@@ -174,15 +219,16 @@
     with open(playbook) as stream:
         config = yaml.safe_load(stream)
         settings = config.get("settings", {})
         return set() != {"rate", "cron"} & settings.keys()
 
 
 def puts(color: str = Style.NORMAL, *args, **kargs):
-    """Print with colors, resets the color after printing
+    """[deprecated] Print with colors, resets the color after printing.
+    Use console.print(str) or console.log(object) instead
 
     Parameters
     ----------
     color : Any, optional
         Color of the text, by default Style.NORMAL
     """
     # color, args adds an empty space??
@@ -218,49 +264,63 @@
     txt = RUNNING_REGEX.sub(rf"{RUNNING_COLOR}\1{rst}", txt)
     txt = FAIL_REGEX.sub(rf"{FAIL_COLOR}\1{rst}", txt)
     txt = UNKNOWN_REGEX.sub(rf"{UNKNOWN_COLOR}\1{rst}", txt)
     txt = SATORIURL_REGEX.sub(rf"{SATORIURL_COLOR}\1{rst}", txt)
     return txt
 
 
-def autosyntax(item: str, indent: int) -> bool:
+def autosyntax(item: str, indent: int = 0, lexer: Optional[str] = None) -> bool:
     ind = (indent) * 2
-    try:
-        json.loads(item)
-    except Exception:
+    lang = None
+    if lexer is None:
         try:
-            yaml.safe_load(item)
-        except Exception:  # Not YAML/JSON
-            return False
-        else:  # Is YAML
-            yml = Syntax(item, "YAML", padding=(0, ind), theme="fruity", word_wrap=True)
-            print()
-            console.log(yml)
-            return True
-    else:  # Is JSON
-        print()
-        print_json(item, indent=ind)
-        return True
-
-
-def table_generator(headers: list[str], items: list[list], header_style=None):
+            json.loads(item)
+        except Exception:
+            try:
+                yaml.safe_load(item)
+            except Exception:  # Not YAML/JSON
+                return False
+            else:  # Is YAML
+                lang = "YAML"
+        else:  # Is JSON
+            lang = "JSON"
+    final_lexer = lexer or lang
+    if final_lexer is None:
+        return False
+    yml = Syntax(item, final_lexer, padding=(0, ind), theme="ansi_dark", word_wrap=True)
+    console.print(yml)
+    return True
+
+
+def table_generator(
+    headers: list[str],
+    items: list[list],
+    header_style: Optional[str] = None,
+    widths: Union[tuple, list] = [None],
+):
     """Print a rich table
 
     Parameters
     ----------
     headers : list
         A list of the headers names, ex: ["header1","header2"]
     items : list
         A list of rows with cells, ex: [["row1-1","row1-2"],["row2-1","row2-2"]]
-    header_style : _type_, optional
+    header_style : str, optional
         Rich Table header style, by default None
     """
-    table = Table(show_header=True, header_style=header_style)
+    widths_iter = iter_loop(widths)
+    table = Table(
+        show_header=True,
+        header_style=header_style,
+        row_styles=["on #222222", "on black"],
+        expand=True,
+    )
     for header in headers:
-        table.add_column(header)
+        table.add_column(header, width=next(widths_iter))
     for item in items:
         cells = []
         for raw_i in item:
             i = str(raw_i)
             if PASS_REGEX.search(i):
                 styled = "[green]" + i
             elif FAIL_REGEX.search(i):
@@ -269,49 +329,41 @@
                 styled = "[yellow]" + i
             elif RUNNING_REGEX.search(i):
                 styled = "[blue]" + i
             else:
                 styled = i
             cells.append(styled)
         table.add_row(*cells)
-    console.log(table)
-
-
-@dataclass
-class argument:
-    id: str
-    action: str
-    profile: str
-    debug: bool
-    json: bool
-    path: str
-    data: Any
-    sync: bool
-    timeout: int
-    playbook: str
-    page: int
-    public: bool
+    console.print(table)
 
 
-def autotable(items: list[dict], header_style=None, numerate=False) -> None:
+def autotable(
+    items: list[dict],
+    header_style: Optional[str] = None,
+    numerate: Optional[bool] = False,
+    widths: Union[tuple, list] = [None],
+) -> None:
     """Print a list of dictionaries like a table
 
     Parameters
     ----------
     items : list[dict]
         The list, ex: [{"id":1,"name":"one"},{"id":2,"name":"two"}]
-    header_style : _type_, optional
+    header_style : str, optional
         Rich Table header style, by default None
     numerate : bool, optional
         Add numeration, by default False
     """
+    if len(items) == 0:
+        console.print("No items found")
+        return
     h = get_headers(items)
     headers = ["N°", *h] if numerate else h
     rows = get_rows(items, headers)
-    table_generator(capitalize_list(headers), rows, header_style)
+    table_generator(capitalize_list(headers), rows, header_style, widths)
 
 
 def get_headers(items: list[dict]) -> list[str]:
     headers = []
     for i in items:
         for h in i.keys():
             h = str(h)
@@ -336,7 +388,16 @@
         rows.append(row)
     return rows
 
 
 def capitalize_list(items: list[str]) -> list[str]:
     new_list = map(lambda x: x.capitalize() if len(x) > 2 else x.upper(), items)
     return list(new_list)
+
+
+def iter_loop(data: Union[tuple[Any], list[Any]]):
+    i = 0
+    while True:
+        yield data[i]
+        i += 1
+        if i >= len(data):
+            i = 0
```

### Comparing `satori_ci-1.2.9/src/satorici/classes/validations.py` & `satori_ci-1.3.1/src/satoricli/classes/validations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-import re
-
 from flatdict import FlatDict
-
-INPUT_REGEX = re.compile(r"\$\(([\w-]+)\)")
-
-
-def is_command_block(value):
-    if isinstance(value, list):
-        if all(
-            (
-                isinstance(v, list) and len(v) == 1 and isinstance(v[0], str)
-                for v in value
-            )
-        ):
-            return True
+from satorici.validator import INPUT_REGEX, is_command_group
 
 
 def get_unbound(commands: list[list[str]], key: str, flat_config: dict[str]):
     variables = set()
 
     for command in commands:
         variables.update(INPUT_REGEX.findall(command[0]))
@@ -39,15 +25,15 @@
 def get_parameters(config: dict):
     """Returns the needed parameters from the yaml loaded config"""
 
     flat_config = FlatDict(config)
     parameters: set[str] = set()
 
     for key, value in flat_config.items():
-        if is_command_block(value):
+        if is_command_group(value):
             parameters.update(get_unbound(value, key, flat_config))
 
     return parameters
 
 
 def validate_parameters(params: dict):
     if isinstance(params, dict):
```

### Comparing `satori_ci-1.2.9/PKG-INFO` & `satori_ci-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.2.9
+Version: 1.3.1
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,204 +677,258 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://www.satori-ci.com
 Requires-Python: >=3.9
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pyyaml>=6.0
-Requires-Dist: tqdm>=4.64.1
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: flatdict>=4.0.1
 Requires-Dist: rich>=13.0
 Requires-Dist: gitpython>=3.1.31
+Requires-Dist: satori-playbook-validator>=3.0.0
+Requires-Dist: textual>=0.26.0
+Requires-Dist: packaging>=23.1
+Requires-Dist: setuptools>=67.8.0
+Requires-Dist: satori-docs
 Description-Content-Type: text/markdown
 
-# 1. Five Ws (and one H)
+# What is Satori CI?
 
-## 1.1 What is Satori CI?
+Satori allows you to assert how systems and software behave. Automatize software and system testing using three different approaches:
+- On demand: you need to execute the test one time (ie, Security Testing, Stress Testing, etc)
+- Scheduled: you need to know on a regular basis what is the status of something (ie, Monitoring live systems every five minutes, Auditing weekly/monthly/yearly systems, etc)
+- CI/CD: you need to execute it every time you are pushing new code (ie, Security Testing, System Testing, etc)
 
-Satori CI is an automated software testing as a service. It asserts what the outputs of the programs will be. Consider the following example "Hello World" program in Python:
+## Setup Satori CLI
+Three steps:
+1. Execute on your command line terminal:
 
-```py
-print("Hello World")
+```console 
+pip3 install satori-ci
 ```
 
-If we execute this program, we will see the following:
+2. With Satori CLI installed, now we need to get a Satori Token to use it:
 
-```py
-$ ./hello_world.py
-Hello World
-```
+ * Log in the Satori website using Github credentials: https://www.satori-ci.com/login
+ * On the Satori website go to User Settings 
+ * Copy your User API Token
 
-We can assert that the return code will be 0 and the standard output of this program will be Hello World:
+3. Replace the string YOUR_TOKEN with your clipboard on the next command: 
 
-```yml
-test:
-    assertReturnCode: 0
-    assertStdoutEqual: Hello World
-    python:
-    - [ ./hello_world.py ]
+```console 
+satori-cli config token YOUR_TOKEN`
 ```
 
-## 1.2 Why
-
-This no code testing language will help you test your software throughout different stages of its development lifecycle. Playbooks can look both at source code and execution (more examples of this in the "CI: Import" section)
+## Actions
 
-## 1.3 Who
+You can take actions on:
 
-Test engineers, software developers and security testers.
+  * **run**: whenever you are launching on demand scans for playbook files or directories
+  * **repo**: whenever you are taking actions on repositories
+  * **monitor**: visualize your scheduled playbooks
+  * **team**: actions related to your team settings
 
-## 1.4 When
+Now, lets test software.
 
-You can attach it to your CI process (Satori CI), you can launch them manually (Satori Run), and you can launch them periodically (Satori Monitor)
+## satori-cli run
 
-## 1.5 Where
+Consider the following example "Hello World" program written in Python:
 
-Satori can be used on your continuous integration, deployment and delivery tests.
+```py
+print("Hello World")
+```
 
-## 1.6 How to use it?
+If save that into a file named `hello_world.py` and we execute this program, we would see the following on the console:
 
-First, login at https://www.satori-ci.com using your Github account to be able to use our CI cappabilities. Github will ask for confirmation for us to access to your repositories of choice. After accepting the conditions, you can get a token fromus at https://www.satori-ci.com/user-settings/ 
+```console 
+foo@bar:~$ python hello_world.py
+Hello World
+```
 
-You will use that token to setup your account with our CLI tool
+How can you test aumatically that that piece of software behaves according to specification? You can write a Satori Playbook using a simple and practical notation:
 
-```sh
-git clone git@github.com:satorici/satori-cli.git
-cd satori-cli/
-apt install python3.10
-pip3 install -f requirements.txt
-# TBD: pip3 install satori-cli
-satori-cli config default YOUR_TOKEN
+```console
+foo@bar:~$ cat .satori.yml
+test:
+    assertStdoutEqual: Hello World
+    python:
+    - [ python hello_world.py ]
 ```
 
-# 2. Playbooks
+Lets test the code with the playbook
+```console
+foo@bar:~$ satori-cli run ./ --sync
+Satori CI 1.2.3 - Automated Software Testing Platform 
+Uploading... ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 331/331 bytes 0:00:00
+UUID: AOQxDWDkXpZp
+Report: https://www.satori-ci.com/report_details/?n=AOQxDWDkXpZp
+- Report status: Completed | Result: Pass | Elapsed time: 62.6s
+  • test: test > python
+  • asserts:
+      ░ assert: assertStdoutEqual
+      ░ status: Pass
+      ░ expected: Hello World
+      - - - - - - - - - - - - - - - - - - - - 
+  • testcases: 1
+  • test_status: Pass
+  • total_fails: 0
+  - - - - - - - - - - - - - - - - - - - - 
+```
+
+The code and the Satori playbook instructions were executed on a new Docker instance hosted by AWS. Satori asserts that this piece of software output "Hello World". You can assert several things:
+  
+  * **assertStdout**: True|False 
+  
+  Is output produced? 
+  
+  * **assertStdoutEquals**: String*
+  
+  Is the output equal to the String?
+  
+  * **assertStdoutNotEquals**: String 
+  
+  Is the output different than String?
+  
+  * **assertStdoutContains**: String 
+  
+  Does the output contains the String?
+  
+  * **assertStdoutNotContains**: String 
+  
+  Does the output not contain the String?
+  * **assertStdoutSHA256**: SHA256Checksum
+  
+  Is the output equal to this SHA256 hash?
+  
+  * **assertStdoutRegex**: Regex
+  
+  Does the output matches your regexp?
+  
+  * **assertStdoutNotRegex**: Regex
+  
+  Does the output not match your regexp?
+  
+The previos can also be applied to *assertStderr*. Finally, you can assert the return code of your the execution using **assertReturnCode**. 
+
+Please let us know if you need to assert something else that we is not covered by them.
+
+## Setup Satori CI Github App
+
+We tested on demand. Now let's do it as part of your regular Github CI process. 
+
+1. Go to https://github.com/apps/satorici
 
-Are used to assert software behaviors, wether they are source code files or live systems.
+2. Click on Install
 
-## 2.1 Playbooks: Hello World
+3. Select the repositories where you will be installing it or select all repositories
 
-TBC
+By default you can get notifications via email and Github issues. If you want to get notified in slack, discord or telegram go to https://www.satori-ci.com/user-settings/ to define their details. 
 
-## 2.2 Playbooks: Import
 
-Playbooks can import other local or remote playbooks. We keep at TBC a list of playbooks that can be referenced with the
+If you want to detail in your playbook to be notified when the scans are ready, add the following to them:
 
 ```yml
-import:
-    - satori://code/trufflehog.yml
+settings:
+  log|logOnFail|logOnPass: slack|email|issue|discord|telegram
+```
 
+For example:
+```yml
+settings:
+    logOnFail: slack
+  
 test:
-    assertStdoutEqual: "Hello World"
-    bash:
-    - [ echo "Hello World" ]
+    assertStdoutEqual: Hello World
+    python:
+    - [ python hello_world.py ]
 ```
 
-Is there a playbook that you would like us to incluide? Drop us a line at support@satori-ci.com
 
-# 3. CI
+and put it on a file named .satori.yml inside your repository. 
+  
+## satori-cli repo
 
-Check how your repositories are connected to our CI with. This command will show you what is our visibility on your repositories. We will tell you which ones are connected, if they have a playbook associated and what is their status.
-Example output:
+You can check which repositories you connected with a playbook by running 
 
-```sh
-$ satori-cli ci
-TBC
 ```
-
-## 2.1 CI: Add a playbook file
-Adding a file named .satori.yml in your root directory, we will be used by your Github pushes to test your code. Lets suppose for example that you created a Hello World application, and you want to know that that will be the output every time you push new code:
-
-- .satori.yml:
-
-```yml
-test:
-    assertStdoutEqual: "Hello World"
-    bash:
-    - [ echo "Hello World" ]
+foo@bar:~$ satori-cli repo
 ```
 
-# Monitor
-
-Check that your assets are correctly monitored. This command will check on the playbooks that are running with a crontab to monitor resources:
-`satori-cli monitor`
-Example output:
+You can scan all your commits from your repository to see if there were any discrepancies at some point:
 
-```sh
-TBC
+```console
+foo@bar:~$ satori-cli repo githubusername/repository scan -c 100 --sync
 ```
 
-## Monitor: add a playbook to be executed at a certain rate
+## satori-cli playbook
 
-Playbook that define a rate are automatically included within the monitor functionality:
+Are used to assert software behaviors, wether they are source code files or live systems. You can see a list of public playbooks by running 
 
-- MonitorBlog.yml
 
-```yml
-settings:
-  - name: Monitor Blog
-  - rate: TBC
+#### Public playbooks
 
-test:
-  assertStdout: "Hello World"
-  blog:
-  - [ curl -s https://www.satori-ci.com/hello-world/ ]
+They can be imported by playbooks that you have in your CI or on assets being Monitored.
+
+```console
+foo@bar:~$ satori-cli playbook --public
+URI                          | Name                                            
+satori://code/trufflehog.yml | Trufflehog will search for secrets in your code 
+satori://code/semgrep.yml    | Static source code analysis with semgrep
+  
+...
 ```
 
-This will be checked every X minutes once you execute it. Example:
+You can check your private playbooks executed just by running `satori-cli playbook`
 
-```sh
-$ satori-cli run MonitorBlog.yml`
-TBC
-```
+#### Import Playbooks
 
-## Monitor: stopping and running again a playbook
+Playbooks can import other local or remote playbooks. We keep at TBC a list of playbooks that can be referenced with the 
 
-You will get a list with the `satori-cli monitor`, from where you will take the UUID. You can use that UUID with the `stop` and `run` subcommands
+```yml
+import:
+    - satori://code/trufflehog.yml
+    - satori://code/semgrep.yml
 
-```sh
-$ satori-cli stop UUID
-TBC
+test:
+    assertStdoutEqual: Hello World
+    python:
+    - [ python hello_world.py ]
 ```
 
-# Scan 
-TBC
+#### Private Playbooks
 
-### Scan all your commits
+We will store a copy of the playbooks that you have executed and show them to you whenever you execute the command:
 
-```sh
-$ satori-cli scan GithubAccount/Repository -c 100
-TBC
+```console
+foo@bar:~$ satori-cli playbooks private
+Type    | URI                                                     | Name           | Imports
+CI      | github://satorici/satori-cli/.satori.yml                |                |
+Monitor | github://satorici/playbooks/test/satori/monitor.yml     | Monitor Assets | monitorBlog.yml
+Run     | github://satorici/playbooks/test/satori/monitorBlog.yml | Monitor Blog   |
+...
 ```
 
-# Playbooks:
+Is there a playbook that you would like us to add? Drop us a line at support@satori-ci.com
 
-You can see a list of public playbooks when at https://github.com/satorici/playbooks/
 
-```sh
-$ satori-cli playbook
-Private playbooks:
-Public Playbooks:
-```
-
-## Public playbooks:
+## satori-cli monitor
 
-They can be imported by playbooks that you have in your CI or on assets being Monitored.
+Assert that your systems are running as expected by setting a schedule for your playbook. Playbooks that define a schedule can be monitored with:
 
-```sh
-$ satori-cli playbook --public
-URI                          | Name                                            
-satori://code/trufflehog.yml | Trufflehog will search for secrets in your code 
-...
+```console
+satori-cli monitor
 ```
 
-## Private Playbooks:
+For example, you can define schedule a crontab rate to a playbook just as in the following exmaple to verify the Hello World website from Satori every hour:
 
-We will store a copy of the playbooks that you have executed and show them to you whenever you execute the command:
+```yml
+settings:
+  - name: Monitor Blog
+  - schedule: "0 * * * *"
+  - logOnFail: slack
 
-```sh
-$ satori-cli playbooks private
-Type    | URI                                                     | Name           | Imports
-CI      | github://satorici/satori-cli/.satori.yml                |                |
-Monitor | github://satorici/playbooks/test/satori/monitor.yml     | Monitor Assets | monitorBlog.yml
-Run     | github://satorici/playbooks/test/satori/monitorBlog.yml | Monitor Blog   |
-...
+test:
+  assertStdout: "Hello World"
+  blog:
+  - [ curl -s https://www.satori-ci.com/hello-world/ ]
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

