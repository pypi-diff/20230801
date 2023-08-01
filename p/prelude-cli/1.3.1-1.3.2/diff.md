# Comparing `tmp/prelude-cli-1.3.1.tar.gz` & `tmp/prelude-cli-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.3.1.tar", last modified: Mon Jul 17 19:33:02 2023, max compression
+gzip compressed data, was "prelude-cli-1.3.2.tar", last modified: Tue Aug  1 18:22:30 2023, max compression
```

## Comparing `prelude-cli-1.3.1.tar` & `prelude-cli-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.275609 prelude-cli-1.3.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-07-17 19:33:02.275701 prelude-cli-1.3.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.3.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.272566 prelude-cli-1.3.1/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.3.1/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.3.1/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.273384 prelude-cli-1.3.1/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      263 2023-06-27 14:52:45.000000 prelude-cli-1.3.1/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.275391 prelude-cli-1.3.1/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4543 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.3.1/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     8431 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     4138 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     3041 2023-07-17 19:18:31.000000 prelude-cli-1.3.1/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      658 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.273204 prelude-cli-1.3.1/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-07-17 19:33:02.275965 prelude-cli-1.3.1/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.960707 prelude-cli-1.3.2/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-08-01 18:22:30.960753 prelude-cli-1.3.2/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.3.2/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.956825 prelude-cli-1.3.2/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.3.2/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.3.2/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.957646 prelude-cli-1.3.2/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      263 2023-06-27 14:52:45.000000 prelude-cli-1.3.2/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.959254 prelude-cli-1.3.2/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     4512 2023-07-26 15:41:33.000000 prelude-cli-1.3.2/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.3.2/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     8536 2023-07-31 17:07:15.000000 prelude-cli-1.3.2/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     4204 2023-07-26 15:41:33.000000 prelude-cli-1.3.2/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     3074 2023-07-26 15:41:33.000000 prelude-cli-1.3.2/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      658 2023-07-17 14:47:48.000000 prelude-cli-1.3.2/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 18:22:30.957455 prelude-cli-1.3.2/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-08-01 18:22:30.000000 prelude-cli-1.3.2/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.3.2/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-08-01 18:22:30.960968 prelude-cli-1.3.2/setup.cfg
```

### Comparing `prelude-cli-1.3.1/LICENSE` & `prelude-cli-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.1/PKG-INFO` & `prelude-cli-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.3.1
+Version: 1.3.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.3.1/prelude_cli/cli.py` & `prelude-cli-1.3.2/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.1/prelude_cli/views/build.py` & `prelude-cli-1.3.2/prelude_cli/views/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,34 +69,34 @@
 @click.option('-q', '--techniques', help='comma-separated list of valid MITRE ATT&CK codes [e.g. T1557,T1040]', default=None, type=str)
 @click.option('-a', '--advisory', help='alert identifier [CVE ID, Advisory ID, etc]', default=None, hidden=True, type=str)
 @click.pass_obj
 @handle_api_error
 def update_test(controller, test, name, unit, techniques, advisory):
     """ Create or update a security test """
     with Spinner(description='Updating test'):
-        test = controller.update_test(
+        data = controller.update_test(
             test_id=test,
             name=name,
             unit=unit,
             techniques=techniques,
             advisory=advisory
         )
-    print_json(data=test)
+    print_json(data=data)
 
 
 @build.command('delete-test')
 @click.argument('test')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def delete_test(controller, test):
     """ Delete a test """
     with Spinner(description='Removing test'):
-        controller.delete_test(test_id=test)
-    click.secho(f'Deleted {test}', fg='green')
+        data = controller.delete_test(test_id=test)
+    print_json(data=data)
 
 
 @build.command('upload')
 @click.argument('path', type=click.Path(exists=True))
 @click.option('-t', '--test', help='test identifier', default=None, type=str)
 @click.pass_obj
 @handle_api_error
@@ -107,21 +107,21 @@
         if match:
             return match.group(0)
         raise FileNotFoundError('You must supply a test ID or include it in the path')
 
     def upload(p: Path):
         with open(p, 'rb') as data:
             with Spinner(description='Uploading to test'):
-                controller.upload(
+                data = controller.upload(
                     test_id=identifier, 
                     filename=p.name, 
                     data=data.read(), 
                     binary=True
                 )
-            click.secho(f'Uploaded {p.name}', fg='green')
+            print_json(data=data)
 
     identifier = test or test_id()
     
     if Path(path).is_file():
         upload(p=Path(path))
     else:
         for obj in Path(path).rglob('*'):
```

### Comparing `prelude-cli-1.3.1/prelude_cli/views/configure.py` & `prelude-cli-1.3.2/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.1/prelude_cli/views/detect.py` & `prelude-cli-1.3.2/prelude_cli/views/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,23 @@
 @click.argument('endpoint_id')
 @click.option('-h', '--host', help='hostname of this machine', type=str, default=None)
 @click.option('-e', '--edr_id', help='EDR id', type=str, default=None)
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default=None)
 @click.pass_obj
 @handle_api_error
 def update_endpoint(controller, endpoint_id, host, edr_id, tags):
-    """ Register a new endpoint """
+    """ Update an existing endpoint """
     with Spinner(description='Updating endpoint'):
-        ep = controller.update_endpoint(
+        data = controller.update_endpoint(
             endpoint_id=endpoint_id,
             host=host,
             edr_id=edr_id,
             tags=tags
         )
-    print_json(data=ep)
+    print_json(data=data)
 
 
 @detect.command('tests')
 @click.pass_obj
 @handle_api_error
 def list_tests(controller):
     """ List all security tests """
@@ -103,27 +103,29 @@
               default=RunCode.DAILY.name, show_default=True,
               type=click.Choice([r.name for r in RunCode], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
 def enable_test(controller, test, run_code, tags):
     """ Add test to your queue """
     with Spinner(description='Enabling test'):
-        controller.enable_test(ident=test, run_code=RunCode[run_code.upper()].value, tags=tags)
+        data = controller.enable_test(ident=test, run_code=RunCode[run_code.upper()].value, tags=tags)
+    print_json(data=data)
 
 
 @detect.command('disable-test')
 @click.argument('test')
 @click.option('-t', '--tags', help='only disable for these tags (comma-separated list)', type=str, default='')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def disable_test(controller, test, tags):
     """ Remove test from your queue """
     with Spinner(description='Disabling test'):
-        controller.disable_test(ident=test, tags=tags)
+        data = controller.disable_test(ident=test, tags=tags)
+    print_json(data=data)
 
 
 @detect.command('social-stats')
 @click.argument('test')
 @click.option('-d', '--days', help='days to look back', default=30, type=int, show_default=True)
 @click.pass_obj
 @handle_api_error
@@ -138,26 +140,27 @@
 @click.argument('endpoint_id')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def delete_endpoint(controller, endpoint_id):
     """Delete a probe/endpoint"""
     with Spinner(description='Deleting endpoint'):
-        controller.delete_endpoint(ident=endpoint_id)
+        data = controller.delete_endpoint(ident=endpoint_id)
+    print_json(data=data)
 
 
 @detect.command('queue')
 @click.pass_obj
 @handle_api_error
 def queue(controller):
     """ List all tests in your active queue """
     with Spinner(description='Fetching active tests from queue'):
         iam = IAMController(account=controller.account)
-        queue = iam.get_account().get('queue')
-    print_json(data=queue)
+        data = iam.get_account().get('queue')
+    print_json(data=data)
 
 
 @detect.command('endpoints')
 @click.option('-d', '--days', help='only show endpoints that have run at least once in the past DAYS days', default=90, type=int)
 @click.pass_obj
 @handle_api_error
 def endpoints(controller, days):
```

### Comparing `prelude-cli-1.3.1/prelude_cli/views/iam.py` & `prelude-cli-1.3.2/prelude_cli/views/iam.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,16 @@
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('handle')
 @click.pass_obj
 @handle_api_error
 def delete_user(controller, handle):
     """ Remove a user from your account """
     with Spinner(description='Deleting user'):
-        controller.delete_user(handle=handle)
+        data = controller.delete_user(handle=handle)
+    print_json(data=data)
 
 
 @iam.command('logs')
 @click.option('-d', '--days', help='days back to search from today', default=7, type=int)
 @click.option('-l', '--limit', help='limit the number of results', default=1000, type=int)
 @click.pass_obj
 @handle_api_error
@@ -110,8 +111,9 @@
 @iam.command('purge')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def purge(controller):
     """ Delete your account """
     with Spinner(description='Purging account from existence'):
-        controller.purge_account()
+        data = controller.purge_account()
+    print_json(data=data)
```

### Comparing `prelude-cli-1.3.1/prelude_cli/views/partner.py` & `prelude-cli-1.3.2/prelude_cli/views/partner.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 @click.argument('partner',
               type=click.Choice([c.name for c in Control if c != Control.INVALID], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
 def detach_partner(controller, partner):
     """ Detach an existing partner from your account """
     with Spinner(description='Detaching partner'):
-        controller.detach(partner_code=Control[partner.upper()].value)
+        data = controller.detach(partner_code=Control[partner.upper()].value)
+    print_json(data=data)
 
 
 @partner.command('endpoints')
 @click.argument('partner',
               type=click.Choice([c.name for c in Control if c != Control.INVALID], case_sensitive=False))
 @click.option('--platform', required=True, help='platform name (e.g. "windows")', type=click.Choice(['windows', 'linux', 'darwin'], case_sensitive=False))
 @click.option('--hostname', default='', help='hostname pattern (e.g. "mycompany-c24oi444")')
```

### Comparing `prelude-cli-1.3.1/prelude_cli/views/shared.py` & `prelude-cli-1.3.2/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.1/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.3.2/prelude_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.3.1
+Version: 1.3.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.3.1/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.3.2/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.1/setup.cfg` & `prelude-cli-1.3.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.3.1
+version = 1.3.2
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.3.1
+	prelude-sdk == 1.3.4
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

