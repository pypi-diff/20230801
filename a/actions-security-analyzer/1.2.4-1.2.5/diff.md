# Comparing `tmp/actions_security_analyzer-1.2.4.tar.gz` & `tmp/actions_security_analyzer-1.2.5.tar.gz`

## Comparing `actions_security_analyzer-1.2.4.tar` & `actions_security_analyzer-1.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/__about__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/colors.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/requirements.txt
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/.github/workflows/asa-scan.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-that-creates-or-approves-pr.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/analyzer/__init__.py
--rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/analyzer/analyzer.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/analyzer/analyzer_test.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/images/asa-stdout.png
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/LICENSE
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/README.md
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/__about__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/colors.py
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/.github/workflows/asa-scan.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-that-creates-or-approves-pr.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/analyzer/__init__.py
+-rw-r--r--   0        0        0    12497 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/analyzer/analyzer.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/images/asa-stdout.png
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/LICENSE
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/README.md
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.5/PKG-INFO
```

### Comparing `actions_security_analyzer-1.2.4/action.yml` & `actions_security_analyzer-1.2.5/action.yml`

 * *Files 26% similar despite different names*

```diff
@@ -27,22 +27,28 @@
   - uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1 # v4.7.0
     with:
       python-version: '3.11' 
   - run: |
       pip install actions-security-analyzer
       args=()
 
-      [ ! -z ${{ inputs.dir }} ] && args+=('--dir', ${{ inputs.dir }})
-      [ ! -z ${{ inputs.ignore-warnings }} ] && args+=('--ignore-warnings')
-      [ ! -z ${{ inputs.no-summary }} ] && args+=('--no-summary')
-      [ ! -z ${{ inputs.verbose }} ] && args+=('--verbose')
+      dir=$( echo ${{ inputs.dir }} | tr '[:upper:]' '[:lower:]')
+      ignore_warnings=$( echo ${{ inputs.ignore-warnings }} | tr '[:upper:]' '[:lower:]')
+      ignore_checks=$( echo ${{ inputs.ignore-checks }} | tr '[:upper:]' '[:lower:]')
+      no_summary=$( echo ${{ inputs.no-summary }} | tr '[:upper:]' '[:lower:]')
+      verbose=$( echo ${{ inputs.verbose }} | tr '[:upper:]' '[:lower:]')
 
-      if [[ ! -z "${{ inputs.ignore-checks }}" ]]; then
+      [ ! -z $dir ] && args+=('--dir', ${{ inputs.dir }})
+      [ ! -z $ignore_warnings ] && [[ $ignore_warnings != "false" ]] && args+=('--ignore-warnings')
+      [ ! -z $no_summary ] && [[ $no_summary != "false" ]] && args+=('--no-summary')
+      [ ! -z $verbose ] && [[ $verbose != "false" ]] && args+=('--verbose')
+
+      if [[ ! -z "$ignore_checks" ]]; then
         checks=()
-        for check in $(echo ${{ inputs.ignore-checks }} )
+        for check in $(echo $ignore_checks)
         do
           checks+=("$check")
         done
         args+=('--ignore-checks', ${checks[@]/,/ })
       fi
 
       echo "ARGS: ${args[@]/,/ }"
```

### Comparing `actions_security_analyzer-1.2.4/colors.py` & `actions_security_analyzer-1.2.5/colors.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.4/main.py` & `actions_security_analyzer-1.2.5/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from yaml import safe_load, YAMLError
 from sys import exit
 
 FAILED = 1
 SUCCESS = 0
 
 
+# reference: https://stackoverflow.com/a/36470466
 def _rewrite_pyyaml_boolean_recognition_rules():
     for ch in "OoYyNn":
         if len(Resolver.yaml_implicit_resolvers[ch]) == 1:
             del Resolver.yaml_implicit_resolvers[ch]
         else:
             Resolver.yaml_implicit_resolvers[ch] = [
                 x for x in Resolver.yaml_implicit_resolvers[ch] if x[0] != "tag:yaml.org,2002:bool"
```

### Comparing `actions_security_analyzer-1.2.4/.github/workflows/asa-scan.yml` & `actions_security_analyzer-1.2.5/.github/workflows/asa-scan.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-name: 'RunActionsSecurityAnalzyer'
+name: "RunActionsSecurityAnalzyer"
 on:
   push:
     branches:
       - main
       - dev
     paths:
-      - '.github/workflows/**'
+      - ".github/workflows/**"
 jobs:
   RunAsa:
     runs-on: ubuntu-latest
     steps:
-    - name: "Checkout repo"
-      uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
-    - name: "Run asa scanner"
-      uses: "bin3xish477/asa@a6f5eb8c20e936c07326a1eb6aa6427b25494045"
-      with:
-        dir: "./actions/"
-        verbose: true
-        no-summary: true
-        ignore-checks: 'check_for_inline_script check_for_cache_action_usage'
-      continue-on-error: true # adding this since this workflow is always expected to fail
+      - name: "Checkout repo"
+        uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
+      - name: "Run asa scanner"
+        uses: "bin3xish477/asa@ee733379e314d44f1a960a70339ee5e5d19e404d"
+        with:
+          dir: "./actions/"
+          verbose: true
+          #no-summary: true
+          #ignore-checks: ''
+          #ignore-warnings: true
+        continue-on-error: true # adding this since this workflow is always expected to fail
```

### Comparing `actions_security_analyzer-1.2.4/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `actions_security_analyzer-1.2.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.4/analyzer/analyzer.py` & `actions_security_analyzer-1.2.5/analyzer/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """analyzer.py contains all the INFOic related to analyzing GitHub Actions"""
 from colors import Colors
 from re import search
+from pathlib import Path
 
 
 class Analyzer:
     """Analyzer contains all the checks that will run
     against a specified GitHub Action parsed into a Python
     dictionary.
     """
@@ -72,17 +73,21 @@
     def _check_for_inline_script(self) -> bool:
         passed = True
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "run" in step:
                     if self.verbose:
-                        print(
-                            f"{Colors.LIGHT_GRAY}INFO{Colors.END} found inline script in job('{job}').step('{step['name']}')"
-                        )
+                        # NOTE: name is not required according to GitHub Docs: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#name
+                        if 'name' in step:
+                            print(
+                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} found inline script in job('{job}').step('{step['name']}')"
+                            )
+                        else:
+                            print(f"{Colors.LIGHT_GRAY}INFO{Colors.END} found step with inline script in job('{job}')")
                     passed = False
         return passed
 
     def _check_for_script_injection(self) -> bool:
         passed = True
         DANGEROUS_GITHUB_CONTEXT_VARIABLE_REGEX = r"\$\{\{.*github.+\}\}"
         for job in self.jobs.keys():
@@ -187,14 +192,15 @@
             "macos-latest",
             "macos-12",
             "macos-latest-xl",
             "macos-12-xl",
             "macos-11",
         ]
         for job in self.jobs.keys():
+            # TODO: Add verbosity to print which self-hosted runners were found.
             if "strategy" in self.jobs[job] and "matrix" in self.jobs[job]["strategy"]:
                 matrix = self.jobs[job]["strategy"]["matrix"]
                 if "runner" in matrix:
                     if type(matrix["runner"]) == list:
                         if any(runner not in default_runners for runner in matrix["runner"]):
                             passed = False
                             break
@@ -280,8 +286,9 @@
                     continue
                 if not Analyzer.__dict__[check](self):
                     fail_checks.append(check)
                     if passed_all_checks:
                         passed_all_checks = False
             for check in fail_checks:
                 self._print_failed_check_msg(check, self.checks[check]["level"])
+
         return passed_all_checks
```

### Comparing `actions_security_analyzer-1.2.4/analyzer/analyzer_test.py` & `actions_security_analyzer-1.2.5/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.4/images/asa-stdout.png` & `actions_security_analyzer-1.2.5/images/asa-stdout.png`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.4/.gitignore` & `actions_security_analyzer-1.2.5/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.vscode
```

### Comparing `actions_security_analyzer-1.2.4/LICENSE` & `actions_security_analyzer-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.4/README.md` & `actions_security_analyzer-1.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 jobs:
   RunAsa:
     runs-on: ubuntu-latest
     steps:
     - name: "Checkout repo"
       uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
     - name: "Run asa scanner"
-      uses: "bin3xish477/asa@a6f5eb8c20e936c07326a1eb6aa6427b25494045"
+      uses: "bin3xish477/asa@ee733379e314d44f1a960a70339ee5e5d19e404d"
       with:
         dir: "./actions/"
         verbose: true
         no-summary: true
         ignore-checks: 'check_for_inline_script check_for_cache_action_usage'
 ```
```

### Comparing `actions_security_analyzer-1.2.4/pyproject.toml` & `actions_security_analyzer-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.2.4/PKG-INFO` & `actions_security_analyzer-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actions-security-analyzer
-Version: 1.2.4
+Version: 1.2.5
 Summary: Analyze the security posture of one or more GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/asa#readme
 Project-URL: Issues, https://github.com/bin3xish477/asa/issues
 Project-URL: Source, https://github.com/bin3xish477/asa
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -63,15 +63,15 @@
 jobs:
   RunAsa:
     runs-on: ubuntu-latest
     steps:
     - name: "Checkout repo"
       uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
     - name: "Run asa scanner"
-      uses: "bin3xish477/asa@a6f5eb8c20e936c07326a1eb6aa6427b25494045"
+      uses: "bin3xish477/asa@ee733379e314d44f1a960a70339ee5e5d19e404d"
       with:
         dir: "./actions/"
         verbose: true
         no-summary: true
         ignore-checks: 'check_for_inline_script check_for_cache_action_usage'
 ```
```

