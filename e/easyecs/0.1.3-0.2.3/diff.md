# Comparing `tmp/easyecs-0.1.3.tar.gz` & `tmp/easyecs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.1.3.tar", max compression
+gzip compressed data, was "easyecs-0.2.3.tar", max compression
```

## Comparing `easyecs-0.1.3.tar` & `easyecs-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     2230 2023-07-31 20:04:45.575575 easyecs-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8375 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0     3390 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0     3511 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     7949 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0      468 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/template/verify.py
--rw-r--r--   0        0        0    12418 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1459 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2043 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2360 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     1666 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/model/ecs.py
--rw-r--r--   0        0        0      505 2023-07-31 20:04:45.599577 easyecs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-01 15:28:41.778321 easyecs-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     7382 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0     3390 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1872 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     2770 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     7949 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12418 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1459 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     2360 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2398 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-01 15:28:41.798321 easyecs-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.2.3/PKG-INFO
```

### Comparing `easyecs-0.1.3/README.md` & `easyecs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/easyecs/cli.py` & `easyecs-0.2.3/easyecs/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 #!python
 
 import time
-import inotify.adapters
 import boto3
 import click
+from easyecs.cloudformation.stack.create import create_stack
+from easyecs.cloudformation.stack.delete import delete_stack
+from easyecs.cloudformation.stack.update import update_stack
 from easyecs.cloudformation.template import create_template
 from easyecs.cloudformation.fetch import (
     fetch_containers,
     fetch_is_stack_created,
 )
-from easyecs.cloudformation.stack import (
-    create_stack,
-    delete_stack,
-    update_stack,
-)
-from easyecs.cloudformation.template.verify import verify_ecs_manifest
 from easyecs.command import (
     run_nc_commands,
     create_port_forwards,
     execute_command,
     run_sync_thread,
     popen_procs_port_forward,
     popen_procs_exec_command,
@@ -27,45 +23,39 @@
 from easyecs.docker import build_docker_image
 from easyecs.helpers.common import check_credentials
 from easyecs.helpers.loader import Loader
 
 from easyecs.helpers.settings import load_settings, read_ecs_file
 
 
-def action_run(no_docker_build, force_redeployment):
-    aws_account = boto3.client("iam").list_account_aliases()["AccountAliases"][0]
-    cache_settings = load_settings(aws_account)
-    aws_region = cache_settings["aws_region"]
-    aws_account_id = cache_settings["aws_account_id"]
-    vpc_id = cache_settings["vpc_id"]
-    subnet_ids = cache_settings["subnet_ids"]
-    azs = cache_settings["azs"]
-
-    ecs_manifest = read_ecs_file()
-    app_name = ecs_manifest.metadata.appname
-    user = ecs_manifest.metadata.user
-    stack_name = f"{user}-{app_name}"
-
-    verify_ecs_manifest(ecs_manifest)
-
-    print()
-
+def step_import_aws_cdk():
     loader_import = Loader(
         "Importing CloudFormation:",
         "Importing CloudFormation: \u2705",
         "Importing CloudFormation: \u274c",
         0.05,
     )
-
     loader_import.start()
     # It takes time to import CDK so we show it to the user!
     import aws_cdk  # noqa: F401
 
     loader_import.stop()
 
+
+def step_docker_build_and_push(
+    no_docker_build,
+    ecs_manifest,
+    stack_name,
+    aws_account_id,
+    aws_region,
+    vpc_id,
+    subnet_ids,
+    azs,
+    run,
+):
     if not no_docker_build:
         loader_docker = Loader(
             "Building and pushing docker images:",
             "Building and pushing docker images: \u2705",
             "Building and pushing docker images: \u274c",
             0.05,
         )
@@ -84,173 +74,144 @@
         stack_name,
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
         ecs_manifest,
-        run=True,
+        run,
     )
     loader.stop()
 
+
+def step_create_or_update_stack(stack_name, force_redeployment):
     if not fetch_is_stack_created(stack_name):
         create_stack(stack_name)
     else:
         update_stack(stack_name, force_redeployment)
 
-    print()
-
-    parsed_containers = fetch_containers(user, app_name)
-
-    create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
 
+def step_idle_keyboard():
     try:
         while True:
             time.sleep(1)
     except KeyboardInterrupt:
         print("Quitting...")
         pass
 
+
+def step_clean_exit():
     for popen_proc in popen_procs_port_forward:
         popen_proc.kill()
 
     for thread in threads:
         thread.stop()
 
-    exit(0)
+    for popen_proc in popen_procs_exec_command:
+        popen_proc.stdin.write("exit\x03\x04".encode("utf8"))
+        popen_proc.stdin.flush()
+        popen_proc.wait()
 
 
-def action_dev(no_docker_build, force_redeployment):
+def action_run(ctx):
+    no_docker_build = ctx.obj["no_docker_build"]
+    force_redeployment = ctx.obj["force_redeployment"]
     aws_account = boto3.client("iam").list_account_aliases()["AccountAliases"][0]
     cache_settings = load_settings(aws_account)
+    ecs_manifest = read_ecs_file()
+    app_name = ecs_manifest.metadata.appname
+    user = ecs_manifest.metadata.user
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
     vpc_id = cache_settings["vpc_id"]
     subnet_ids = cache_settings["subnet_ids"]
     azs = cache_settings["azs"]
-
-    ecs_manifest = read_ecs_file()
-    app_name = ecs_manifest.metadata.appname
-    user = ecs_manifest.metadata.user
     stack_name = f"{user}-{app_name}"
 
-    verify_ecs_manifest(ecs_manifest)
-
     print()
-
-    loader_import = Loader(
-        "Importing CloudFormation:",
-        "Importing CloudFormation: \u2705",
-        "Importing CloudFormation: \u274c",
-        0.05,
+    step_import_aws_cdk()
+    step_docker_build_and_push(
+        no_docker_build,
+        ecs_manifest,
+        stack_name,
+        aws_account_id,
+        aws_region,
+        vpc_id,
+        subnet_ids,
+        azs,
+        True,
     )
+    step_create_or_update_stack(stack_name, force_redeployment)
+    parsed_containers = fetch_containers(user, app_name)
+    print()
+    create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
+    step_idle_keyboard()
 
-    loader_import.start()
-    # It takes time to import CDK so we show it to the user!
-    import aws_cdk  # noqa: F401
+    step_clean_exit()
 
-    loader_import.stop()
+    exit(0)
 
-    if not no_docker_build:
-        loader_docker = Loader(
-            "Building and pushing docker images:",
-            "Building and pushing docker images: \u2705",
-            "Building and pushing docker images: \u274c",
-            0.05,
-        )
-        loader_docker.start()
-        build_docker_image(ecs_manifest)
-        loader_docker.stop()
 
-    loader = Loader(
-        "Creating CloudFormation template:",
-        "Creating CloudFormation template: \u2705",
-        "Creating CloudFormation template: \u274c",
-        0.05,
-    )
-    loader.start()
-    create_template(
+def action_dev(ctx):
+    no_docker_build = ctx.obj["no_docker_build"]
+    force_redeployment = ctx.obj["force_redeployment"]
+    aws_account = boto3.client("iam").list_account_aliases()["AccountAliases"][0]
+    cache_settings = load_settings(aws_account)
+    ecs_manifest = read_ecs_file()
+    app_name = ecs_manifest.metadata.appname
+    user = ecs_manifest.metadata.user
+    aws_region = cache_settings["aws_region"]
+    aws_account_id = cache_settings["aws_account_id"]
+    vpc_id = cache_settings["vpc_id"]
+    subnet_ids = cache_settings["subnet_ids"]
+    azs = cache_settings["azs"]
+    stack_name = f"{user}-{app_name}"
+
+    print()
+    step_import_aws_cdk()
+    step_docker_build_and_push(
+        no_docker_build,
+        ecs_manifest,
         stack_name,
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
-        ecs_manifest,
+        False,
     )
-    loader.stop()
-
-    if not fetch_is_stack_created(stack_name):
-        create_stack(stack_name)
-    else:
-        update_stack(stack_name, force_redeployment)
-
-    print()
-
+    step_create_or_update_stack(stack_name, force_redeployment)
     parsed_containers = fetch_containers(user, app_name)
-
+    print()
     create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
-
     run_nc_commands(parsed_containers, aws_region, aws_account, ecs_manifest)
-
     run_sync_thread(parsed_containers, ecs_manifest)
-
     print()
 
     found_tty = execute_command(
         ecs_manifest,
         parsed_containers,
         aws_region,
         aws_account,
     )
 
     if not found_tty:
-        try:
-            while True:
-                time.sleep(1)
-        except KeyboardInterrupt:
-            print("Quitting...")
-            pass
-
-    for popen_proc in popen_procs_port_forward:
-        popen_proc.kill()
-
-    for popen_proc in popen_procs_exec_command:
-        popen_proc.stdin.write("exit\x03\x04".encode("utf8"))
-        popen_proc.stdin.flush()
-        popen_proc.wait()
-
-    for thread in threads:
-        thread.stop()
-
+        step_idle_keyboard()
+    step_clean_exit()
     exit(0)
 
 
-def action_delete():
+def action_delete(_):
     ecs_manifest = read_ecs_file()
     app_name = ecs_manifest.metadata.appname
     user = ecs_manifest.metadata.user
     stack_name = f"{user}-{app_name}"
     delete_stack(stack_name)
 
 
-def action_debug():
-    sync_events = set(["IN_CLOSE_WRITE"])
-    i = inotify.adapters.Inotify()
-    i.add_watch(".")
-    for event in i.event_gen(yield_nones=False):
-        (_, type_names, path, filename) = event
-        if set(type_names).issubset(sync_events):
-            print(
-                "PATH=[{}] FILENAME=[{}] EVENT_TYPES={}".format(
-                    path, filename, type_names
-                )
-            )
-
-
 @click.group()
 @click.pass_context
 def entrypoint(ctx):
     ctx.ensure_object(dict)
     check_credentials()
 
 
@@ -273,15 +234,17 @@
     help=(
         "If used, and only when there's no update on the cloudformation stack, easyecs"
         " will force a new deployment of the task."
     ),
 )
 @click.pass_context
 def click_run(ctx, no_docker_build, force_redeployment):
-    action_run(no_docker_build, force_redeployment)
+    ctx.obj["no_docker_build"] = no_docker_build
+    ctx.obj["force_redeployment"] = force_redeployment
+    action_run(ctx)
 
 
 @entrypoint.command(name="dev", help="Run a stack in development mode")
 @click.option(
     "--no-docker-build",
     is_flag=True,
     default=False,
@@ -299,28 +262,20 @@
     help=(
         "If used, and only when there's no update on the cloudformation stack, easyecs"
         " will force a new deployment of the task."
     ),
 )
 @click.pass_context
 def click_dev(ctx, no_docker_build, force_redeployment):
-    action_dev(no_docker_build, force_redeployment)
+    ctx.obj["no_docker_build"] = no_docker_build
+    ctx.obj["force_redeployment"] = force_redeployment
+    action_dev(ctx)
 
 
 @entrypoint.command(name="delete", help="Delete a stack")
-@click.option(
-    "--force-redeployment",
-    is_flag=True,
-    default=False,
-    show_default=True,
-    help=(
-        "If used, and only when there's no update on the cloudformation stack, easyecs"
-        " will force a new deployment of the task."
-    ),
-)
 @click.pass_context
-def click_delete(ctx, force_redeployment):
-    action_delete()
+def click_delete(ctx):
+    action_delete(ctx)
 
 
 if __name__ == "__main__":
     entrypoint()
```

### Comparing `easyecs-0.1.3/easyecs/cloudformation/fetch.py` & `easyecs-0.2.3/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/easyecs/cloudformation/template/__init__.py` & `easyecs-0.2.3/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/easyecs/command/__init__.py` & `easyecs-0.2.3/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/easyecs/docker/__init__.py` & `easyecs-0.2.3/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/easyecs/helpers/common.py` & `easyecs-0.2.3/easyecs/helpers/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+import json
 import os
 import random
 import time
+from typing import Dict
 import boto3
 import socket
 from botocore.exceptions import UnauthorizedSSOTokenError
 
 from easyecs.helpers.color import Color
 
 
+def load_template(stack_name: str) -> Dict:
+    """
+    Loads the CloudFormation template from a JSON file.
+    """
+    with open(f".cloudformation/{stack_name}.template.json") as f:
+        return json.load(f)
+
+
 def parse_dict_with_env_var(build_args):
     for key, value in build_args.items():
         if value.startswith("{{.") and value.endswith("}}"):
             env_var_name = value[3:][:-2]
             new_value = os.environ.get(env_var_name)
             if new_value is None:
                 print(
```

### Comparing `easyecs-0.1.3/easyecs/helpers/loader.py` & `easyecs-0.2.3/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/easyecs/helpers/selector.py` & `easyecs-0.2.3/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/easyecs/helpers/settings.py` & `easyecs-0.2.3/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.3/PKG-INFO` & `easyecs-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.1.3
+Version: 0.2.3
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

