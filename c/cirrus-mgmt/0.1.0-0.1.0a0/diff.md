# Comparing `tmp/cirrus-mgmt-0.1.0.tar.gz` & `tmp/cirrus-mgmt-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirrus-mgmt-0.1.0.tar", last modified: Tue Aug  1 20:16:54 2023, max compression
+gzip compressed data, was "cirrus-mgmt-0.1.0a0.tar", last modified: Thu Nov 10 05:29:23 2022, max compression
```

## Comparing `cirrus-mgmt-0.1.0.tar` & `cirrus-mgmt-0.1.0a0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.192600 cirrus-mgmt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-01 20:16:54.192600 cirrus-mgmt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:16:54.192600 cirrus-mgmt-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.188600 cirrus-mgmt-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.188600 cirrus-mgmt-0.1.0/src/cirrus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.188600 cirrus-mgmt-0.1.0/src/cirrus/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.192600 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.192600 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.192600 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/utils/boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-01 20:16:43.000000 cirrus-mgmt-0.1.0/src/cirrus/plugins/management/utils/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:16:54.192600 cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-01 20:16:54.000000 cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-01 20:16:54.000000 cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 20:16:54.000000 cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 20:16:54.000000 cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 20:16:54.000000 cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 20:16:54.000000 cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.392634 cirrus-mgmt-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11341 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-11-10 05:29:23.392634 cirrus-mgmt-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 05:29:23.392634 cirrus-mgmt-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.388634 cirrus-mgmt-0.1.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.388634 cirrus-mgmt-0.1.0a0/src/cirrus/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.388634 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.392634 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.392634 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6459 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8946 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.392634 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/utils/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-11-10 05:29:11.000000 cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/utils/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:29:23.392634 cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-11-10 05:29:23.000000 cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-10 05:29:23.000000 cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-10 05:29:23.000000 cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-10 05:29:23.000000 cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 05:29:23.000000 cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-10 05:29:23.000000 cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/top_level.txt
```

### Comparing `cirrus-mgmt-0.1.0/LICENSE` & `cirrus-mgmt-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cirrus-mgmt-0.1.0/PKG-INFO` & `cirrus-mgmt-0.1.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirrus-mgmt
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: cirrus-geo plugin providing deployment management commands
 Home-page: https://github.com/cirrus-geo/cirrus-mgmt
 Author: Jarrett Keifer (jkeifer), Element 84
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cirrus-mgmt-0.1.0/README.md` & `cirrus-mgmt-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `cirrus-mgmt-0.1.0/setup.py` & `cirrus-mgmt-0.1.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/deployments.py` & `cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/deployments.py`

 * *Files identical despite different names*

### Comparing `cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/manage.py` & `cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/manage.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from functools import wraps
 
 import click
 from cirrus.cli.utils import click as utils_click
 from click_option_group import RequiredMutuallyExclusiveOptionGroup, optgroup
 
-from cirrus.plugins.management.deployment import WORKFLOW_POLL_INTERVAL, Deployment
+from cirrus.plugins.management.deployment import Deployment
 from cirrus.plugins.management.utils.click import (
     additional_variables,
     silence_templating_errors,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -107,44 +107,14 @@
 def refresh(deployment, stackname=None, profile=None):
     """Refresh the environment values from the AWS deployment,
     optionally changing the stackname or profile.
     """
     deployment.refresh(stackname=stackname, profile=profile)
 
 
-@manage.command("run-workflow")
-@click.option(
-    "-t",
-    "--timeout",
-    type=int,
-    default=3600,
-    help="Maximum time (seconds) to allow for the workflow to complete",
-)
-@click.option(
-    "-p",
-    "--poll-interval",
-    type=int,
-    default=WORKFLOW_POLL_INTERVAL,
-    help="Maximum time (seconds) to allow for the workflow to complete",
-)
-@raw_option
-@pass_deployment
-def run_workflow(deployment, timeout, raw, poll_interval):
-    """Pass a payload (from stdin) off to a deployment, wait for the workflow to finish,
-    retrieve and return its output payload"""
-    payload = json.load(sys.stdin.read())
-
-    output = deployment.run_workflow(
-        payload=payload,
-        timeout=timeout,
-        poll_interval=poll_interval,
-    )
-    click.echo(json.dump(output, sys.stdout, indent=4 if not raw else None))
-
-
 @manage.command("get-payload")
 @click.argument(
     "payload-id",
 )
 @raw_option
 @pass_deployment
 def get_payload(deployment, payload_id, raw):
@@ -229,30 +199,30 @@
 @manage.command()
 @pass_deployment
 def process(deployment):
     """Enqueue a payload (from stdin) for processing"""
     click.echo(json.dumps(deployment.process_payload(sys.stdin), indent=4))
 
 
-@manage.command()
-@click.argument(
-    "lambda-name",
-)
-@pass_deployment
-def invoke_lambda(deployment, lambda_name):
-    """Invoke lambda with event (from stdin)"""
-    click.echo(
-        json.dumps(deployment.invoke_lambda(sys.stdin.read(), lambda_name), indent=4)
-    )
-
-
 @manage.command("template-payload")
 @additional_variables
 @silence_templating_errors
 @include_user_vars
+@click.option(
+    "-x",
+    "--var",
+    "additional_vars",
+    nargs=2,
+    multiple=True,
+    help="Additional templating variables",
+)
+@click.option(
+    "--silence-templating-errors",
+    is_flag=True,
+)
 @pass_deployment
 def template_payload(
     deployment,
     additional_variables,
     silence_templating_errors,
     include_user_vars,
 ):
@@ -283,43 +253,11 @@
 def _exec(ctx, deployment, command, include_user_vars):
     """Run an executable with the deployment environment vars loaded"""
     if not command:
         return
     deployment.exec(command, include_user_vars=include_user_vars)
 
 
-@manage.command(
-    "call",
-    context_settings={
-        "ignore_unknown_options": True,
-    },
-)
-@click.argument(
-    "command",
-    nargs=-1,
-)
-@include_user_vars
-@pass_deployment
-@click.pass_context
-def _call(ctx, deployment, command, include_user_vars):
-    """Run an executable, in a new process, with the deployment environment vars loaded"""
-    if not command:
-        return
-    deployment.call(command, include_user_vars=include_user_vars)
-
-
-@manage.command()
-@pass_deployment
-@click.pass_context
-def list_lambdas(ctx, deployment):
-    """List lambda functions"""
-    click.echo(
-        json.dumps(
-            {"Functions": deployment.get_lambda_functions()}, indent=4, default=str
-        )
-    )
-
-
 # check-pipeline
 #   - this is like failmgr check
 #   - not sure how to reconcile with cache above
 #   - maybe need subcommand for everything it can do
```

### Comparing `cirrus-mgmt-0.1.0/src/cirrus/plugins/management/commands/payload.py` & `cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/commands/payload.py`

 * *Files identical despite different names*

### Comparing `cirrus-mgmt-0.1.0/src/cirrus/plugins/management/deployment.py` & `cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/deployment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import dataclasses
 import json
 import logging
 import os
 from datetime import datetime, timezone
 from pathlib import Path
-from subprocess import check_call
-from time import sleep, time
-
-import backoff
-from cirrus.lib2.process_payload import ProcessPayload
 
 from . import exceptions
 from .utils.boto3 import get_mfa_session, validate_session
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_DEPLOYMENTS_DIR_NAME = "deployments"
 MAX_SQS_MESSAGE_LENGTH = 2**18  # max length of SQS message
 CONFIG_VERSION = 0
 
-WORKFLOW_POLL_INTERVAL = 15  # seconds between state checks
-
 
 def deployments_dir_from_project(project):
     _dir = project.dot_dir.joinpath(DEFAULT_DEPLOYMENTS_DIR_NAME)
     _dir.mkdir(exist_ok=True)
     return _dir
 
 
@@ -75,15 +68,14 @@
 class Deployment(DeploymentMeta):
     def __init__(self, path: Path, *args, **kwargs):
         self.path = path
 
         super().__init__(*args, **kwargs)
 
         self._session = None
-        self._functions = None
 
     @classmethod
     def create(cls, name: str, project, stackname: str = None, profile: str = None):
         if not stackname:
             stackname = project.config.get_stackname(name)
 
         env = cls.get_env_from_lambda(stackname, cls._get_session(profile))
@@ -156,32 +148,14 @@
             )
         except aws_lambda.exceptions.ResourceNotFoundException:
             # TODO: fatal error bad lambda name, needs better handling
             raise
 
         return process_conf["Environment"]["Variables"]
 
-    def get_lambda_functions(self):
-        if self._functions is None:
-            aws_lambda = self.get_session().client("lambda")
-
-            def deployment_functions_filter(response):
-                return [
-                    f["FunctionName"].replace(f"{self.stackname}-", "")
-                    for f in response["Functions"]
-                    if f["FunctionName"].startswith(self.stackname)
-                ]
-
-            resp = aws_lambda.list_functions()
-            self._functions = deployment_functions_filter(resp)
-            while "NextMarker" in resp:
-                resp = aws_lambda.list_functions(Marker=resp["NextMarker"])
-                self._functions += deployment_functions_filter(resp)
-        return self._functions
-
     def get_session(self):
         if not self._session:
             self._session = self._get_session(profile=self.profile)
         return self._session
 
     def reload(self):
         self.__dict__.update(DeploymentMeta.load(self.path).asdict())
@@ -193,16 +167,15 @@
         self.updated = now_isoformat()
         self.save()
 
     def set_env(self, include_user_vars=False):
         os.environ.update(self.environment)
         if include_user_vars:
             os.environ.update(self.user_vars)
-        if self.profile:
-            os.environ["AWS_PROFILE"] = self.profile
+        os.environ["AWS_PROFILE"] = self.profile
 
     def add_user_vars(self, _vars, save=False):
         self.user_vars.update(_vars)
         if save:
             self.save()
 
     def del_user_var(self, name, save=False):
@@ -221,38 +194,22 @@
             if include_user_vars:
                 env.update(self.user_vars)
             os.execlpe(command[0], *command, env)
 
         self.set_env(include_user_vars=include_user_vars)
         os.execlp(command[0], *command)
 
-    def call(self, command, include_user_vars=True, isolated=False):
-        if isolated:
-            env = self.environment.copy()
-            if include_user_vars:
-                env.update(self.user_vars)
-            check_call(command, env=env)
-        else:
-            self.set_env(include_user_vars=include_user_vars)
-            check_call(command)
-
     def get_payload_state(self, payload_id):
         from cirrus.lib2.statedb import StateDB
 
         statedb = StateDB(
             table_name=self.environment["CIRRUS_STATE_DB"],
             session=self.get_session(),
         )
-
-        @backoff.on_predicate(backoff.expo, lambda x: x is None, max_time=60)
-        def _get_payload_item_from_statedb(statedb, payload_id):
-            return statedb.get_dbitem(payload_id)
-
-        state = _get_payload_item_from_statedb(statedb, payload_id)
-
+        state = statedb.get_dbitem(payload_id)
         if not state:
             raise exceptions.PayloadNotFoundError(payload_id)
         return state
 
     def process_payload(self, payload):
         stream = None
 
@@ -304,75 +261,14 @@
         try:
             exec_arn = execs[0]
         except IndexError:
             raise exceptions.NoExecutionsError(payload_id)
 
         return self.get_execution(exec_arn)
 
-    def invoke_lambda(self, event, function_name):
-        aws_lambda = self.get_session().client("lambda")
-        if function_name not in self.get_lambda_functions():
-            raise ValueError(
-                f"lambda named '{function_name}' not found in deployment '{self.name}'"
-            )
-        full_name = f"{self.stackname}-{function_name}"
-        response = aws_lambda.invoke(FunctionName=full_name, Payload=event)
-        if response["StatusCode"] < 200 or response["StatusCode"] > 299:
-            raise RuntimeError(response)
-
-        return json.load(response["Payload"])
-
-    def run_workflow(
-        self,
-        payload: dict,
-        timeout: int = 3600,
-        poll_interval: int = WORKFLOW_POLL_INTERVAL,
-    ) -> dict:
-        """
-
-        Args:
-            deployment (Deployment): where the workflow will be run.
-
-            payload (str): payload to pass to the deployment to kick off the workflow.
-
-            timeout (Optional[int]): - upper bound on the number of seconds to poll the
-                                       deployment before considering the test failed.
-
-            poll_interval (Optional[int]): - seconds to delay between checks of the
-                                             workflow status.
-
-        Returns:
-            dict containing output payload or error message
-
-        """
-        payload = ProcessPayload(payload)
-        wf_id = payload["id"]
-        logger.info("Submitting %s to %s", wf_id, self.name)
-        resp = self.process_payload(json.dumps(payload))
-        logger.debug(resp)
-
-        state = "PROCESSING"
-        end_time = time() + timeout - poll_interval
-        while state == "PROCESSING" and time() < end_time:
-            sleep(poll_interval)
-            resp = self.get_payload_state(wf_id)
-            state = resp["state_updated"].split("_")[0]
-            logger.debug({"state": state})
-
-        execution = self.get_execution_by_payload_id(wf_id)
-
-        if state == "COMPLETED":
-            output = dict(ProcessPayload.from_event(json.loads(execution["output"])))
-        elif state == "PROCESSING":
-            output = {"last_error": "Unkonwn: cirrus-mgmt polling timeout exceeded"}
-        else:
-            output = {"last_error": resp.get("last_error", "last error not recorded")}
-
-        return output
-
     def template_payload(
         self,
         payload: str,
         additional_vars: dict = None,
         silence_templating_errors: bool = False,
         include_user_vars: bool = True,
     ):
```

### Comparing `cirrus-mgmt-0.1.0/src/cirrus/plugins/management/exceptions.py` & `cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `cirrus-mgmt-0.1.0/src/cirrus/plugins/management/utils/boto3.py` & `cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/utils/boto3.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,26 +21,22 @@
             the session is created.
 
         session_vars: A dictionary that is used to override some or all
             of the environment variables associated with this session.  The
             key/value pairs defined in this dictionary will override the
             corresponding variables defined in ``SESSION_VARIABLES``.
     """
-    profile = kwargs.get("profile", None)
+    # Change the cache path from the default of
+    # ~/.aws/boto/cache to the one used by awscli
+    working_dir = os.path.join(os.path.expanduser("~"), ".aws/cli/cache")
 
     # Construct botocore session with cache
     session = botocore.session.Session(**kwargs)
     provider = session.get_component("credential_provider").get_provider("assume-role")
-    if profile:
-        # If ``profile`` is provided, then we need to
-        # change the cache path from the default of
-        # ~/.aws/boto/cache to the one used by awscli.
-        # Without ``profile``, we defer to normal boto operations.
-        working_dir = os.path.join(os.path.expanduser("~"), ".aws/cli/cache")
-        provider.cache = credentials.JSONFileCache(working_dir)
+    provider.cache = credentials.JSONFileCache(working_dir)
 
     return boto3.Session(botocore_session=session)
 
 
 def validate_session(session, profile):
     try:
         session.client("sts").get_caller_identity()
```

### Comparing `cirrus-mgmt-0.1.0/src/cirrus/plugins/management/utils/click.py` & `cirrus-mgmt-0.1.0a0/src/cirrus/plugins/management/utils/click.py`

 * *Files identical despite different names*

### Comparing `cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/PKG-INFO` & `cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirrus-mgmt
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: cirrus-geo plugin providing deployment management commands
 Home-page: https://github.com/cirrus-geo/cirrus-mgmt
 Author: Jarrett Keifer (jkeifer), Element 84
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cirrus-mgmt-0.1.0/src/cirrus_mgmt.egg-info/SOURCES.txt` & `cirrus-mgmt-0.1.0a0/src/cirrus_mgmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

