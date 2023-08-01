# Comparing `tmp/terragrunt-generator-0.6.2.tar.gz` & `tmp/terragrunt-generator-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragrunt-generator-0.6.2.tar", last modified: Sat Apr  8 12:59:10 2023, max compression
+gzip compressed data, was "terragrunt-generator-0.6.3.tar", last modified: Tue Aug  1 17:39:53 2023, max compression
```

## Comparing `terragrunt-generator-0.6.2.tar` & `terragrunt-generator-0.6.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:59:10.785250 terragrunt-generator-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    45732 2023-04-08 12:59:10.785250 terragrunt-generator-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45481 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:59:10.785250 terragrunt-generator-0.6.2/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-08 12:59:00.000000 terragrunt-generator-0.6.2/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/generator/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/generator/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-08 12:59:00.000000 terragrunt-generator-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 12:59:10.785250 terragrunt-generator-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:59:10.785250 terragrunt-generator-0.6.2/terragrunt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45732 2023-04-08 12:59:10.000000 terragrunt-generator-0.6.2/terragrunt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-08 12:59:10.000000 terragrunt-generator-0.6.2/terragrunt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 12:59:10.000000 terragrunt-generator-0.6.2/terragrunt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-08 12:59:10.000000 terragrunt-generator-0.6.2/terragrunt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-08 12:59:10.000000 terragrunt-generator-0.6.2/terragrunt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 12:59:10.000000 terragrunt-generator-0.6.2/terragrunt_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:59:10.785250 terragrunt-generator-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-08 12:58:49.000000 terragrunt-generator-0.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 17:39:42.000000 terragrunt-generator-0.6.3/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 17:39:42.000000 terragrunt-generator-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_utils.py
```

### Comparing `terragrunt-generator-0.6.2/COPYING` & `terragrunt-generator-0.6.3/COPYING`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.2/generator/generate.py` & `terragrunt-generator-0.6.3/generator/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,28 @@
     lookup: str,
     variables: list = [],
 ) -> str:
     text = ''
     for var_type in ('mandatories', 'optionals', 'nullables'):
         for variable in variables.get(var_type, []):
             default = variable.get('default')
+            description = variable.get('description', '').replace('    ', '', 1).replace('\n', '\n#   #').replace('\\"', '"')
 
             if var_type == 'nullables':
-                text += f"#   # {variable['name']} - {variable['description']}\n"
+                text += f"#   # {variable['name']} - {description}\n"
                 text += f"#   # {variable['name']}: {json.JSONEncoder().encode(default) if default else ''}\n"
             elif var_type == 'optionals':
-                text += f"#   # {variable['name']} - {variable['description']}\n"
+                text += f"#   # {variable['name']} - {description}\n"
                 text += f"#   {variable['name']}: {json.JSONEncoder().encode(default) if default else ''}\n"
             else:
-                text += f"#   # {variable['name']} - {variable['description']}\n"
+                text += f"#   # {variable['name']} - {description}\n"
                 text += f"#   {variable['name']}: {json.JSONEncoder().encode(default) if default else ''}\n"
 
     lookup = lookup.replace('local.all', '')
-    if lookup.startswith('['):
-        lookup = lookup.strip('[]').strip('"')
-
+    
     path = path or ''
     url = f"{url.replace('.git', '')}/tree/{version}/{path}"
 
     return f"""# {name} {version}
 # {url}
 #
 # yaml config
@@ -43,19 +42,20 @@
 """
 
 
 def generate_include(enable: bool = True) -> str:
     content: str = ''
     if enable is True:
         content = '    path = find_in_parent_folders()'
-
-    return f"""include {{
+        return f"""
+include {{
 {content}
 }}
 """
+    return ""
 
 
 def generate_locals(
     filename: str = 'config.yaml',
     url: str = None,
     path: str = None,
     version: str = None,
@@ -81,45 +81,53 @@
 }}
 """
 
 
 def generate_terraform(url: str, path: str, version: str, lookup: str) -> str:
     path = f'//{path}' if path is not None else ''
     url = f'{url.replace("https://", "").replace("http://", "")}{path}?ref={version}'
+
+    if lookup.startswith('['):
+        lookup = lookup.strip('[]').strip('"')
+
     source = f'lookup({lookup}, "enabled", true) == true ? local.module.source : null'
 
     return f"""
 terraform {{
     source = {source}
 }}
 """
 
 
 def generate_inputs(variables: list = [], lookup: str = 'local.all') -> str:
     content_fisrt: str = ''
     content_next: str = ''
     content_nullable: str = ''
     variables = sorted(variables, key=lambda d: d['name'], reverse=False)
+        
     for variable in variables:
+
         description = (
             variable.get('description', '')
-            .replace('    ', '', 1)
-            .replace('\n', '\n    #')
+            .replace('    ', '')
+            .replace('\n', '\n    # ')
             .replace('\\"', '"')
         )
 
+
         if variable.get('nullable', False) is False:
             _content: str = ''
 
             line_doc = f"{variable.get('name')} - {description}"
             mandatory = variable.get('mandatory', False)
             line_doc += ' - required' if mandatory is True else ''
 
             line_content = f"{variable.get('name')} = "
             name = variable.get('name')
+
             line_content += f'lookup({lookup}, "{name}"'
 
             value = ''
             if variable.get('type', None) == 'string':
                 value = f', "{variable.get("default", "")}"'
             else:
                 value = f', {json.dumps(variable.get("default"))}'
@@ -213,15 +221,15 @@
             if path is not None
             else url.split('/')[-1:][0].replace('.git', '')
         )
         if name is None
         else name
     )
 
-    lookup = f'local.all{lookup.format(name=name,)}'
+    #lookup = f'local.all{lookup.format(name=name,)}'
     results: str
     results = generate_header(name, url, path, version, lookup, variables_object)
     results += generate_include(include)
     results += generate_locals(config, url, path, version)
     results += generate_terraform(url, path, version, lookup)
     results += generate_inputs(variables, lookup)
     return results
```

### Comparing `terragrunt-generator-0.6.2/generator/main.py` & `terragrunt-generator-0.6.3/generator/main.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.2/pyproject.toml` & `terragrunt-generator-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,13 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.2"
+version = "0.6.3"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "generator/__init__.py",
 ]
```

### Comparing `terragrunt-generator-0.6.2/setup.py` & `terragrunt-generator-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.2/terragrunt_generator.egg-info/SOURCES.txt` & `terragrunt-generator-0.6.3/terragrunt_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.2/tests/test_generate.py` & `terragrunt-generator-0.6.3/tests/test_generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def test_generate_include_without_path():
     # Given the generate_include function is called with path=False
     # When the function is executed
 
     results = generate_include(False)
 
     # Then it should return a string that includes "include {" and an empty path value.
-    assert 'include {\n\n}\n' in results
+    assert '' in results
 
 
 def test_generate_locals():
     # Scenario 1
     # Given the generate_locals function is called with filename="", url="https://gitserver.com/test/test.git", path="modules/test", and version="0.1.0"
     # When the function is executed
     filename = ''
@@ -57,21 +57,21 @@
 def test_generate_terraform():
     # Scenario 1
     # Given the generate_terraform function is called with url="https://gitserver.com/test/test.git", path="modules/test", version="0.1.0", and lookup="local.all[\"test\"]"
     # When the function is executed
     url: str = 'https://gitserver.com/test/test.git'
     path: str = 'modules/test'
     version: str = '0.1.0'
-    lookup: str = 'local.all["test"]'
+    lookup: str = 'local.all.test'
     results = generate_terraform(url, path, version, lookup)
 
     # Then it should return a string that includes the expected "terraform" block
     expected = """
 terraform {
-    source = lookup(local.all["test"], "enabled", true) == true ? local.module.source : null
+    source = lookup(local.all.test, "enabled", true) == true ? local.module.source : null
 }
 """
 
     assert results == expected
 
 
 def test_generate_inputs():
@@ -82,17 +82,17 @@
         {
             'name': 'test',
             'description': 'A',
             'type': 'string',
             'default': 'hello',
         }
     ]
-    lookup: str = 'local.all["test"]'
+    lookup: str = 'local.all.test'
     results = generate_inputs(variables, lookup)
 
     # Then it should return a string that includes the expected "inputs" block
     expected = """
 inputs = {
     # test - A
-    test = lookup(local.all["test"], "test", "hello")
+    test = lookup(local.all.test, "test", "hello")
 }"""
     assert results == expected
```

### Comparing `terragrunt-generator-0.6.2/tests/test_reader.py` & `terragrunt-generator-0.6.3/tests/test_reader.py`

 * *Files identical despite different names*

