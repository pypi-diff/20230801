# Comparing `tmp/frigobar-3.tar.gz` & `tmp/frigobar-4.tar.gz`

## Comparing `frigobar-3.tar` & `frigobar-4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 frigobar-3/frigobar/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 frigobar-3/frigobar/__main__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 frigobar-3/frigobar/cli.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 frigobar-3/frigobar/frigobar.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 frigobar-3/frigobar/downloaders/download_deps.ps1
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 frigobar-3/frigobar/downloaders/download_pip.ps1
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 frigobar-3/frigobar/downloaders/download_python.ps1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-3/tests/__init__.py
--rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 frigobar-3/tests/test_frigobar.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/another_script.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/requirements.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/data/data
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 frigobar-3/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 frigobar-3/license
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 frigobar-3/pyproject.toml
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 frigobar-3/readme.md
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 frigobar-3/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 frigobar-4/frigobar/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 frigobar-4/frigobar/__main__.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 frigobar-4/frigobar/cli.py
+-rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 frigobar-4/frigobar/frigobar.py
+-rw-r--r--   0        0        0    55296 2020-02-02 00:00:00.000000 frigobar-4/frigobar/_tkinter/_tkinter.pyd
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 frigobar-4/frigobar/downloaders/download_deps.ps1
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 frigobar-4/frigobar/downloaders/download_pip.ps1
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 frigobar-4/frigobar/downloaders/download_python.ps1
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 frigobar-4/frigobar/downloaders/download_tkinter.ps1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-4/tests/__init__.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 frigobar-4/tests/test_frigobar.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-4/tests/script_folder/another_script.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 frigobar-4/tests/script_folder/requirements.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-4/tests/script_folder/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-4/tests/script_folder/data/data
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 frigobar-4/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 frigobar-4/license
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 frigobar-4/pyproject.toml
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 frigobar-4/readme.md
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 frigobar-4/PKG-INFO
```

### Comparing `frigobar-3/frigobar/cli.py` & `frigobar-4/frigobar/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 def create_frigobar(args):
     frigobar.create_frigobar(
         script_path=args.script_path,
         target_directory=args.target_directory,
         requirements_file=args.requirements_file,
         python_version=args.python_version,
         copy_directory=args.copy_directory,
+        tkinter=args.tkinter,
     )
 
 
 def main():
     parser = argparse.ArgumentParser(
         description=(
             "Distribute Python apps to Windows machines without freezing them. The "
@@ -50,13 +51,18 @@
         ),
     )
     parser.add_argument(
         "--copy-directory",
         action="store_true",
         help="Copy the contents of the script directory to the distribution.",
     )
+    parser.add_argument(
+        "--tkinter",
+        action="store_true",
+        help="Include Tkinter in the distribution.",
+    )
     args = parser.parse_args()
     create_frigobar(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `frigobar-3/frigobar/frigobar.py` & `frigobar-4/frigobar/frigobar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import glob
 import os
 import shutil
 from subprocess import Popen
 
-BAT_TEMPLATE = '''powershell Unblock-File -Path '%~dp0downloaders\download_python.ps1'
-powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version {python_version} -TargetDirectory "{rel_target_directory}"
-powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_pip.ps1" -TargetDirectory "{rel_python_directory}"
-powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_deps.ps1" -RequirementsFile "{rel_requirements_file}" -PipPath "{rel_pip_path}"
-"%~dp0/python-{python_version}-embed-amd64/python.exe" "{rel_script_path}"'''
-BAT_TEMPLATE_NO_REQ = '''powershell Unblock-File -Path '%~dp0downloaders\download_python.ps1'
-powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version {python_version} -TargetDirectory "{rel_target_directory}"
-"%~dp0/python-{python_version}-embed-amd64/python.exe" "{rel_script_path}"'''
+unblock_cmd = "powershell Unblock-File -Path '%~dp0downloaders\download_python.ps1'"
+download_python_cmd = 'powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version {python_version} -TargetDirectory "{rel_target_directory}"'
+download_pip_cmd = 'powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_pip.ps1" -TargetDirectory "{rel_python_directory}"'
+download_deps_cmd = 'powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_deps.ps1" -RequirementsFile "{rel_requirements_file}" -PipPath "{rel_pip_path}"'
+download_tkinter_cmd = 'powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_tkinter.ps1" -TargetDirectory "{rel_target_directory}" -PythonVersion {python_version} -MoveFiles -PythonDirectory "{rel_python_directory}"'
+run_script_cmd = (
+    '"%~dp0/python-{python_version}-embed-amd64/python.exe" "{rel_script_path}"'
+)
 
 
 def create_frigobar(
     script_path: str,
     target_directory: str = "frigobar",
     python_version: str = "3.11.4",
     requirements_file: str = None,
     copy_directory: bool = False,
+    tkinter: bool = False,
 ):
     script_path = os.path.abspath(script_path)
     if not os.path.exists(target_directory):
         os.mkdir(target_directory)
     elif not os.path.isdir(target_directory):
         raise Exception("Target directory must be a directory")
     elif os.listdir(target_directory):
@@ -59,25 +60,24 @@
 
     # Add a copy of the requirements file to frigobar
     if requirements_file:
         shutil.copy(requirements_file, script_dir)
 
     # Add a copy of the downloaders to frigobar
     downloaders_dir = os.path.join(os.path.dirname(__file__), "downloaders")
-    downloader_scripts = (
-        [
-            os.path.join(downloaders_dir, "download_python.ps1"),
+    downloader_scripts = [os.path.join(downloaders_dir, "download_python.ps1")]
+    if requirements_file:
+        downloader_scripts += [
             os.path.join(downloaders_dir, "download_pip.ps1"),
             os.path.join(downloaders_dir, "download_deps.ps1"),
         ]
-        if requirements_file
-        else [
-            os.path.join(downloaders_dir, "download_python.ps1"),
+    if tkinter:
+        downloader_scripts += [
+            os.path.join(downloaders_dir, "download_tkinter.ps1"),
         ]
-    )
     downloaders_dir = os.path.join(target_directory, "downloaders")
     os.mkdir(downloaders_dir)
     for script in downloader_scripts:
         if not os.path.exists(script):
             raise Exception(f"Missing script: {script}")
         shutil.copy(script, downloaders_dir)
 
@@ -94,37 +94,44 @@
         os.path.join(script_dir, os.path.basename(script_path)), target_directory
     )
     if requirements_file:
         rel_requirements_file = os.path.relpath(
             os.path.join(script_dir, os.path.basename(requirements_file)),
             target_directory,
         )
+    else:
+        rel_requirements_file = ""
     script_basename = os.path.splitext(os.path.basename(script_path))[0]
     bat_file = os.path.join(target_directory, f"{script_basename}.bat")
     with open(bat_file, "w") as f:
+        template_list = [unblock_cmd, download_python_cmd]
         if requirements_file:
-            f.write(
-                BAT_TEMPLATE.format(
-                    python_version=python_version,
-                    rel_target_directory=rel_target_directory,
-                    rel_python_directory=rel_python_directory,
-                    rel_requirements_file=rel_requirements_file,
-                    rel_pip_path=rel_pip_path,
-                    rel_script_path=rel_script_path,
-                )
-            )
-        else:
-            f.write(
-                BAT_TEMPLATE_NO_REQ.format(
-                    python_version=python_version,
-                    rel_target_directory=rel_target_directory,
-                    rel_python_directory=rel_python_directory,
-                    rel_script_path=rel_script_path,
-                )
+            template_list.append(download_pip_cmd)
+            template_list.append(download_deps_cmd)
+        if tkinter:
+            template_list.append(download_tkinter_cmd)
+        template_list.append(run_script_cmd)
+        template = "\n".join(template_list)
+        f.write(
+            template.format(
+                python_version=python_version,
+                rel_target_directory=rel_target_directory,
+                rel_python_directory=rel_python_directory,
+                rel_requirements_file=rel_requirements_file,
+                rel_pip_path=rel_pip_path,
+                rel_script_path=rel_script_path,
             )
+        )
+
+    # Add _tkinter.pyd to frigobar
+    if tkinter:
+        tkinter_pyd_path = os.path.join(
+            os.path.dirname(__file__), "_tkinter", "_tkinter.pyd"
+        )
+        shutil.copy(tkinter_pyd_path, target_directory)
 
 
 def fill_frigobar(frigobar_path: str):
     bat_pattern = os.path.join(frigobar_path, "*.bat")
     bat_file = glob.glob(bat_pattern)[0]
     p = Popen(bat_file)
     stdout, stderr = p.communicate()
```

### Comparing `frigobar-3/frigobar/downloaders/download_pip.ps1` & `frigobar-4/frigobar/downloaders/download_pip.ps1`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 if (Test-Path $PipExe) {
     Write-Host "Pip already downloaded"
     exit 0
 }
 
 Write-Host "Downloading get-pip.py"
-# Checking if there is a proxy
 $Proxy = [System.Net.WebRequest]::GetSystemWebproxy()
 $ProxyBypassed = $Proxy.IsBypassed($PipUrl)
 if ($ProxyBypassed){
     Invoke-WebRequest -Uri $PipUrl -OutFile $PipFile 
 } else {
     $ProxyUrl = $Proxy.GetProxy($PipUrl)
     Invoke-WebRequest -Uri $PipUrl -OutFile $PipFile -Proxy $ProxyUrl -ProxyUseDefaultCredentials
```

### Comparing `frigobar-3/frigobar/downloaders/download_python.ps1` & `frigobar-4/frigobar/downloaders/download_python.ps1`

 * *Files 18% similar despite different names*

```diff
@@ -17,39 +17,45 @@
 
 if (Test-Path $PythonExe) {
     Write-Host "Python $version already downloaded"
     exit 0
 }
 
 Write-Host "Downloading Python $Version"
-# Checking if there is a proxy
 $Proxy = [System.Net.WebRequest]::GetSystemWebproxy()
 $ProxyBypassed = $Proxy.IsBypassed($PythonUrl)
 if ($ProxyBypassed){
     Invoke-WebRequest -Uri $PythonUrl -OutFile $PythonZip
 } else {
     $ProxyUrl = $Proxy.GetProxy($PythonUrl)
     Invoke-WebRequest -Uri $PythonUrl -OutFile $PythonZip -Proxy $ProxyUrl -ProxyUseDefaultCredentials
 }
 
 Write-Host "Extracting Python $version"
 Expand-Archive -Path $PythonZip -DestinationPath "$PythonDir"
 
-# Modify _pht file to allow pip in embedabble Python
-# See https://stackoverflow.com/a/48906746
+# Modify _pht file to add custom configurations to embedabble Python
 $PthFile = Get-ChildItem -Path $PythonDir -Filter "python*_pth" | Select-Object -Last 1
 
 if ($PthFile) {
     # Read the content of the file into an array
     $Lines = Get-Content $PthFile.FullName
 
+    # Insert the script path at the beginning of the content
+    # This allows embeddable Python to find modules in the script folder
+    # See https://stackoverflow.com/a/61976910
+    $ScriptPath = "..\script"
+    $Lines = @($ScriptPath) + $Lines
+
     # Find the last line of the file
     $LastLineIndex = $Lines.Count - 1
 
     # Uncomment the last line by removing the leading '#'
+    # This allows embeddable Python to use pip
+    # See https://stackoverflow.com/a/48906746
     $Lines[$LastLineIndex] = $Lines[$LastLineIndex] -replace '^#', ''
 
     # Write the updated content back to the file
     $Lines | Set-Content $PthFile.FullName
 
     Write-Host "Uncommented the last line in $($file.FullName)."
 } else {
```

### Comparing `frigobar-3/tests/test_frigobar.py` & `frigobar-4/tests/test_frigobar.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,25 +192,49 @@
         script_path=script_path,
         target_directory=target_dir,
         requirements_file=None,
         python_version=python_version,
     )
 
     assert path.exists(path.join(target_dir, "script", "script.py"))
-    assert path.exists(path.join(target_dir, "downloaders", "download_python.ps1"))
     assert path.exists(path.join(target_dir, "script.bat"))
     assert not path.exists(path.join(target_dir, "script", "requirements.txt"))
     assert not path.exists(path.join(target_dir, "downloaders", "download_pip.ps1"))
     assert not path.exists(path.join(target_dir, "downloaders", "download_deps.ps1"))
+    assert not path.exists(path.join(target_dir, "downloaders", "download_tkinter.ps1"))
+
+    with open(path.join(target_dir, "script.bat"), "r") as f:
+        assert (
+            f.read()
+            == r'''powershell Unblock-File -Path '%~dp0downloaders\download_python.ps1'
+powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version 3.8.5 -TargetDirectory "."
+"%~dp0/python-3.8.5-embed-amd64/python.exe" "script\script.py"'''
+        )
+
+
+def test_create_frigobar_with_tkinter():
+    frigobar.create_frigobar(
+        script_path=script_path,
+        target_directory=target_dir,
+        python_version=python_version,
+        tkinter=True,
+    )
+
+    assert path.exists(path.join(target_dir, "script", "script.py"))
+    assert path.exists(path.join(target_dir, "downloaders", "download_python.ps1"))
+    assert path.exists(path.join(target_dir, "downloaders", "download_tkinter.ps1"))
+    assert path.exists(path.join(target_dir, "script.bat"))
+    assert not path.exists(path.join(target_dir, "python-3.8.5-amd64.zip"))
 
     with open(path.join(target_dir, "script.bat"), "r") as f:
         assert (
             f.read()
             == r'''powershell Unblock-File -Path '%~dp0downloaders\download_python.ps1'
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version 3.8.5 -TargetDirectory "."
+powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_tkinter.ps1" -TargetDirectory "." -PythonVersion 3.8.5 -MoveFiles -PythonDirectory "python-3.8.5-embed-amd64"
 "%~dp0/python-3.8.5-embed-amd64/python.exe" "script\script.py"'''
         )
 
 
 def test_fill_frigobar():
     frigobar.create_frigobar(
         script_path=script_path,
```

### Comparing `frigobar-3/.gitignore` & `frigobar-4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
+!frigobar/_tkinter/_tkinter.pyd
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `frigobar-3/license` & `frigobar-4/license`

 * *Files identical despite different names*

### Comparing `frigobar-3/pyproject.toml` & `frigobar-4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "frigobar"
-version = "3"
+version = "4"
 description = "Distribute Python apps to Windows machines without freezing them."
 authors = [
     {name="ubalklen", email="42127323+ubalklen@users.noreply.github.com"},
 ]
 readme = "readme.md"
 
 [project.urls]
```

### Comparing `frigobar-3/readme.md` & `frigobar-4/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
   -h, --help            show this help message and exit
   -r REQUIREMENTS_FILE, --requirements-file REQUIREMENTS_FILE
                         Path to a requirements file that lists the dependencies of the script.
   -p PYTHON_VERSION, --python-version PYTHON_VERSION, --python PYTHON_VERSION
                         Python version, in X.Y.Z format, that the distribution should use.The version must be available as  
                         an embeddable package on https://www.python.org/downloads/windows/. Defaults to 3.11.4.
   --copy-directory      Copy the contents of the script directory to the distribution.
+  --tkinter             Include Tkinter in the distribution.
 ```
 
 ## Rationale
 A common technique to distribute Python apps is to "freeze" them using tools like [PyInstaller](https://pyinstaller.org/) or [cx_Freeze](https://cx-freeze.readthedocs.io/). These freezers create a standalone executable that contains your app and all its dependencies. This is a workable solution, but it has two main drawbacks:
 
 1. The resulting frozen app is often huge. It's not uncommon to see a simple app taking MBs of space.
 2. Because dependence resolution is hard, the frozen app may contain more or less dependencies than it needs. Less dependencies lead to dread "working-app-that-stop-working-when-you-freeze-it" situations. Unnecessary dependencies lead to bloated apps.
```

### Comparing `frigobar-3/PKG-INFO` & `frigobar-4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frigobar
-Version: 3
+Version: 4
 Summary: Distribute Python apps to Windows machines without freezing them.
 Project-URL: Homepage, https://github.com/ubalklen/my_package
 Project-URL: Bug Tracker, https://github.com/ubalklen/my_package/issues
 Author-email: ubalklen <42127323+ubalklen@users.noreply.github.com>
 License-File: license
 Description-Content-Type: text/markdown
 
@@ -39,14 +39,15 @@
   -h, --help            show this help message and exit
   -r REQUIREMENTS_FILE, --requirements-file REQUIREMENTS_FILE
                         Path to a requirements file that lists the dependencies of the script.
   -p PYTHON_VERSION, --python-version PYTHON_VERSION, --python PYTHON_VERSION
                         Python version, in X.Y.Z format, that the distribution should use.The version must be available as  
                         an embeddable package on https://www.python.org/downloads/windows/. Defaults to 3.11.4.
   --copy-directory      Copy the contents of the script directory to the distribution.
+  --tkinter             Include Tkinter in the distribution.
 ```
 
 ## Rationale
 A common technique to distribute Python apps is to "freeze" them using tools like [PyInstaller](https://pyinstaller.org/) or [cx_Freeze](https://cx-freeze.readthedocs.io/). These freezers create a standalone executable that contains your app and all its dependencies. This is a workable solution, but it has two main drawbacks:
 
 1. The resulting frozen app is often huge. It's not uncommon to see a simple app taking MBs of space.
 2. Because dependence resolution is hard, the frozen app may contain more or less dependencies than it needs. Less dependencies lead to dread "working-app-that-stop-working-when-you-freeze-it" situations. Unnecessary dependencies lead to bloated apps.
```

