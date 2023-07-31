# Comparing `tmp/dfsync-0.3.8.tar.gz` & `tmp/dfsync-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsync-0.3.8.tar", last modified: Mon Aug  9 17:21:41 2021, max compression
+gzip compressed data, was "dfsync-0.4.0.tar", max compression
```

## Comparing `dfsync-0.3.8.tar` & `dfsync-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,35 @@
--rw-r--r--   0        0        0       22 2021-03-27 05:46:27.532800 dfsync-0.3.8/dfsync/__init__.py
--rw-r--r--   0        0        0       64 2021-04-06 10:05:47.667270 dfsync-0.3.8/dfsync/backends/__init__.py
--rw-r--r--   0        0        0    21420 2021-08-09 17:18:08.988648 dfsync-0.3.8/dfsync/backends/kube.py
--rwxr-xr-x   0        0        0     1600 2021-08-09 16:54:53.225674 dfsync-0.3.8/dfsync/backends/kube_exec.py
--rw-r--r--   0        0        0     4780 2021-07-15 05:23:26.792307 dfsync-0.3.8/dfsync/backends/rsync.py
--rw-r--r--   0        0        0      475 2021-05-23 23:31:09.551867 dfsync-0.3.8/dfsync/char_ui.py
--rw-r--r--   0        0        0      125 2021-03-17 16:28:00.884270 dfsync-0.3.8/dfsync/cli.py
--rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.393669 dfsync-0.3.8/dfsync/exp.py
--rw-r--r--   0        0        0     5225 2021-05-24 01:03:50.413273 dfsync-0.3.8/dfsync/filters.py
--rw-r--r--   0        0        0     6610 2021-08-09 17:19:30.466837 dfsync-0.3.8/dfsync/monitor.py
--rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.3.8/dfsync/transactions.py
--rw-r--r--   0        0        0      436 2021-08-09 17:20:34.624075 dfsync-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      785 2021-08-09 17:21:42.324396 dfsync-0.3.8/setup.py
--rw-r--r--   0        0        0      503 2021-08-09 17:21:42.324673 dfsync-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 08:22:13.656849 dfsync-0.4.0/dfsync/__init__.py
+-rw-r--r--   0        0        0       64 2021-04-06 10:05:47.000000 dfsync-0.4.0/dfsync/backends/__init__.py
+-rw-r--r--   0        0        0    23995 2023-04-03 16:24:42.000000 dfsync-0.4.0/dfsync/backends/kube.py
+-rwxr-xr-x   0        0        0     1928 2022-09-10 10:08:34.000000 dfsync-0.4.0/dfsync/backends/kube_exec.py
+-rw-r--r--   0        0        0     5473 2023-07-31 21:29:22.099082 dfsync-0.4.0/dfsync/backends/rsync.py
+-rw-r--r--   0        0        0     3617 2023-07-31 19:01:18.508583 dfsync-0.4.0/dfsync/char_ui.py
+-rw-r--r--   0        0        0     1334 2022-10-21 04:03:26.000000 dfsync-0.4.0/dfsync/chcli.py
+-rw-r--r--   0        0        0      582 2023-07-25 16:18:24.031315 dfsync-0.4.0/dfsync/check_dns.py
+-rw-r--r--   0        0        0      148 2023-06-17 21:12:04.987300 dfsync-0.4.0/dfsync/cli.py
+-rw-r--r--   0        0        0     2381 2023-06-19 07:28:44.923993 dfsync-0.4.0/dfsync/config.py
+-rw-r--r--   0        0        0     2389 2023-07-31 22:35:43.410956 dfsync-0.4.0/dfsync/distribution.py
+-rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.000000 dfsync-0.4.0/dfsync/exp.py
+-rw-r--r--   0        0        0     7025 2023-07-31 22:24:18.258289 dfsync-0.4.0/dfsync/filters.py
+-rw-r--r--   0        0        0     1094 2023-05-20 11:19:56.000000 dfsync-0.4.0/dfsync/generate.py
+-rw-r--r--   0        0        0     4543 2023-06-17 23:21:49.780512 dfsync-0.4.0/dfsync/kube_credentials.py
+-rw-r--r--   0        0        0      679 2023-07-31 20:23:04.492784 dfsync-0.4.0/dfsync/lib.py
+-rw-r--r--   0        0        0    10870 2023-07-31 20:25:25.957594 dfsync-0.4.0/dfsync/monitor.py
+-rw-r--r--   0        0        0      725 2023-07-08 13:02:10.410286 dfsync-0.4.0/dfsync/pycode/__init__.py
+-rw-r--r--   0        0        0     4421 2023-05-20 10:16:55.000000 dfsync-0.4.0/dfsync/pycode/bpe.py
+-rw-r--r--   0        0        0     3641 2023-05-18 09:12:53.000000 dfsync-0.4.0/dfsync/pycode/generate_data.py
+-rw-r--r--   0        0        0     2121 2023-05-20 11:12:31.000000 dfsync-0.4.0/dfsync/pycode/generate_docstring.py
+-rw-r--r--   0        0        0     5869 2023-05-20 13:52:38.000000 dfsync-0.4.0/dfsync/pycode/generate_expansion.py
+-rw-r--r--   0        0        0     3088 2023-05-20 11:12:48.000000 dfsync-0.4.0/dfsync/pycode/generate_func.py
+-rw-r--r--   0        0        0      540 2023-05-16 17:24:44.000000 dfsync-0.4.0/dfsync/pycode/generate_pytest.py
+-rw-r--r--   0        0        0     1822 2023-07-08 13:05:08.349161 dfsync-0.4.0/dfsync/pycode/oai.py
+-rw-r--r--   0        0        0     2674 2023-06-02 11:17:40.000000 dfsync-0.4.0/dfsync/pycode/prompts.py
+-rw-r--r--   0        0        0      212 2023-07-08 13:05:57.874746 dfsync-0.4.0/dfsync/pycode/search.py
+-rw-r--r--   0        0        0     1830 2023-05-18 09:18:10.000000 dfsync-0.4.0/dfsync/pycode/test_generate_data.py
+-rw-r--r--   0        0        0     4879 2023-05-20 08:26:16.000000 dfsync-0.4.0/dfsync/pycode/tokens.py
+-rw-r--r--   0        0        0     3193 2023-05-20 11:11:17.000000 dfsync-0.4.0/dfsync/pycode/util.py
+-rw-r--r--   0        0        0     4269 2023-07-26 02:24:53.086605 dfsync-0.4.0/dfsync/scrape_anm.py
+-rw-r--r--   0        0        0      982 2023-07-26 01:41:23.893303 dfsync-0.4.0/dfsync/scrape_reord.py
+-rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.4.0/dfsync/transactions.py
+-rw-r--r--   0        0        0      630 2023-07-31 22:31:34.135533 dfsync-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 dfsync-0.4.0/PKG-INFO
```

### Comparing `dfsync-0.3.8/dfsync/backends/kube.py` & `dfsync-0.4.0/dfsync/backends/kube.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,123 +2,129 @@
 import os
 import os.path
 import json
 
 from urllib.parse import urlparse
 from kubernetes import client, config, watch
 from kubernetes.stream import stream
+from kubernetes.client.exceptions import ApiException
+from tenacity import retry, retry_if_exception_type, wait_exponential, stop_after_attempt
 
 from dfsync.filters import GIT_FILTER
 from .rsync import rsync_backend
 
 DEFAULT_COMMAND = []
 DEFAULT_PULL_POLICY = "Always"
 
 
 class Alpine:
     @classmethod
     def name(cls):
         return "Alpine linux (or apk-based Alpine clone)"
 
     @classmethod
-    def get_supervise_command(cls):
+    def get_supervise_command(cls, container_command):
+        container_command = container_command or "while true; do sleep 1; done"
         return [
             "/bin/sh",
             "-c",
-            "echo dfsync && apk --no-cache add rsync; while true; do sleep 1; done",
+            f"echo dfsync && apk --no-cache add rsync; {container_command}",
         ]
 
     @classmethod
     def install_rsync(cls):
         return ["apk", "--no-cache", "add", "rsync"]
 
     @classmethod
     def check_rsync(cls):
-        return ["rsync", "--version"]
+        return ["/bin/sh", "-c", "rsync --version"]
 
     @classmethod
     def check_package_manager(cls):
-        return ["apk", "--version"]
+        return ["/bin/sh", "-c", "apk --version"]
 
     @classmethod
     def check_can_exec(cls):
         return ["true"]
 
 
-class CentOS:
+class ELinuxOS:
     @classmethod
     def name(cls):
-        return "CentOS linux (or dnf-based CentOS clone)"
+        return "Enterprise Linux (or rpm/dnf-based Enterprise Linux clone)"
 
     @classmethod
-    def get_supervise_command(cls):
+    def get_supervise_command(cls, container_command):
+        container_command = container_command or "while true; do sleep 1; done"
         return [
             "/bin/bash",
             "-c",
-            "echo dfsync && dnf install -y rsync; while true; do sleep 1; done",
+            f"echo dfsync && dnf install -y rsync; {container_command}",
         ]
 
     @classmethod
     def install_rsync(cls):
         return ["dnf", "install", "-y", "rsync"]
 
     @classmethod
     def check_rsync(cls):
-        return ["rsync", "--version"]
+        return ["/bin/sh", "-c", "rsync --version"]
 
     @classmethod
     def check_package_manager(cls):
-        return ["dnf", "--version"]
+        return ["/bin/sh", "-c", "dnf --version"]
 
     @classmethod
     def check_can_exec(cls):
         return ["true"]
 
 
 class Ubuntu:
     @classmethod
     def name(cls):
         return "Ubuntu/Debian linux (or apt-based Debian clone)"
 
     @classmethod
-    def get_supervise_command(cls):
+    def get_supervise_command(cls, container_command):
+        container_command = container_command or "while true; do sleep 1; done"
         return [
             "/bin/bash",
             "-c",
-            "echo dfsync && apt install -y rsync; while true; do sleep 1; done",
+            f"echo dfsync && apt install -y rsync; {container_command}",
         ]
 
     @classmethod
     def install_rsync(cls):
         return ["apt", "install", "-y", "rsync"]
 
     @classmethod
     def check_rsync(cls):
-        return ["rsync", "--version"]
+        return ["/bin/sh", "-c", "rsync --version"]
 
     @classmethod
     def check_package_manager(cls):
-        return ["apt", "--version"]
+        return ["/bin/sh", "-c", "apt --version"]
 
     @classmethod
     def check_can_exec(cls):
         return ["true"]
 
 
 class Generic:
     @classmethod
     def name(cls):
         return "Generic linux (with bash, rsync and supervisor installed)"
 
     @classmethod
-    def get_supervise_command(cls):
+    def get_supervise_command(cls, container_command):
+        container_command = container_command or "while true; do sleep 1; done"
         return [
             "/bin/sh",
             "-c",
-            "echo dfsync && while true; do sleep 1; done",
+            f"echo dfsync && {container_command}",
         ]
 
     @classmethod
     def install_rsync(cls):
         return ["true"]
 
     @classmethod
@@ -196,34 +202,37 @@
     if selected_context is None:
         selected_context = active_context
         selected_context_api = active_context_api
     return selected_context, selected_context_api
 
 
 class KubeReDeployer:
-    def __init__(self, kube_host=None, pod_timeout=30, **kwargs):
+    def __init__(self, kube_host=None, pod_timeout=30, container_command=None, full_sync=True, **kwargs):
         config.load_kube_config()
 
         selected_context, selected_context_api = get_selected_kubernetes(kube_host)
 
         self.context_name = selected_context["name"]
         self.api = selected_context_api
         self.apps_api = client.AppsV1Api(api_client=config.new_client_from_config(context=self.context_name))
 
         print(f"Using cluster: {self.context_name} on {self.api.api_client.configuration.host}")
         self.rsync_backend_instance = rsync_backend()
         self._image_distro = None
         self.pod_timeout = pod_timeout
+        self.container_command = container_command
+        self._full_sync = full_sync
 
     def supervisor_install(self, pod, spec, status):
         if self._is_supervised(pod, spec, status):
             return
 
-        command = self._image_distro.get_supervise_command()
-        deployments = self._set_deployment_command(pod, spec, status, command)
+        command = self._image_distro.get_supervise_command(self.container_command)
+        deployments = self._edit_deployment(pod, spec, status, command=command, image_pull_policy="Never")
+
         print("Supervisor installing on {}".format(" ".join(deployments)))
 
     def supervisor_uninstall(self, pod, spec, status):
         if not self._is_supervised(pod, spec, status):
             return
 
         deployments = self._reset_deployment_command(pod, spec, status)
@@ -236,42 +245,54 @@
         return annotations
 
     def _get_dfsync_annotation(self, deployment):
         anno_key = "dfsync.localgrid.io"
         annotations_str = deployment.metadata.annotations.get(anno_key, "{}")
         return json.loads(annotations_str)
 
-    def _set_deployment_command(self, pod, spec, status, command):
-        # image_pull_policy="IfNotPresent",
-        return self._edit_deployment(pod, spec, status, command=command, image_pull_policy="Never")
-
     def _reset_deployment_command(self, pod, spec, status):
         return self._edit_deployment(pod, spec, status)
 
+    @retry(
+        stop=stop_after_attempt(5),
+        wait=wait_exponential(multiplier=1, min=4, max=10),
+        retry=retry_if_exception_type(ApiException),
+        reraise=True,
+    )
     def _edit_deployment(self, pod, spec, status, **kwargs):
         namespace = pod.metadata.namespace
         deployments = {}
         is_undo = len(kwargs) == 0
         for deployment, container_spec in self.list_deployments(namespace, spec.image):
             if spec.name != container_spec.name:
                 continue
 
             if is_undo:
-                kwargs = self._get_dfsync_annotation(deployment) or {}
+                kwargs = self._get_dfsync_annotation(deployment) or {"command": None}
             else:
-                self._set_dfsync_annotation(deployment, {k: getattr(container_spec, k) for k, v in kwargs.items()})
+                self._set_dfsync_annotation(deployment, marshall_dfsync_annotation(container_spec, kwargs.keys()))
 
             for k, v in kwargs.items():
                 if is_undo and k == "command" and self._is_dfsync_command(v):
                     print("Clearing dfsync metadata annotations")
                     container_spec.image_pull_policy = DEFAULT_PULL_POLICY
                     container_spec.command = DEFAULT_COMMAND
-                elif k == "command":
+                    container_spec.resources.limits = {}
+                    container_spec.resources.requests = {}
+                elif k in ["command"]:
                     # Yeah, None seems to be a special value that does not work as well as the empty list
                     container_spec.command = v or []
+                elif k == "resources":
+                    existing_limits = container_spec.resources.limits or {}
+                    new_limits = v.get("limits") or {}
+                    container_spec.resources.limits = {**existing_limits, **new_limits}
+
+                    existing_requests = container_spec.resources.requests or {}
+                    new_requests = v.get("requests") or {}
+                    container_spec.resources.requests = {**existing_requests, **new_requests}
                 else:
                     setattr(container_spec, k, v)
 
             deployments[deployment.metadata.uid] = deployment
 
         for _, deployment in deployments.items():
             patch = client.V1Deployment(
@@ -310,24 +331,28 @@
     def _is_uncrashed(self, pod, spec, status):
         return self._is_dfsync_command(spec.command, markers=["echo uncrash"])
 
     def status(self, image_base):
         ready_map = {False: "🔴  ", True: "🟢  ", "dev": "🟠  "}
         # print("Pods using image: {}".format(image_base))
         for pod, spec, status in self.generate_matching_containers(image_base):
-            icon = ready_map[status.ready]
-            status_msg = status.ready
-            if not status.ready and status.state.waiting:
-                status_msg = "{} - {}".format(status.ready, status.state.waiting.reason)
-            elif not status.ready and status.last_state.waiting:
-                status_msg = "{} - {}".format(status.ready, status.last_state.waiting.reason)
-            elif status.ready and self._is_supervised(pod, spec, status):
+            waiting = None
+            is_ready = False
+            if status:
+                waiting = status.state.waiting or status.last_state.waiting
+                is_ready = status.ready
+
+            icon = ready_map[is_ready]
+            status_msg = is_ready
+            if not is_ready and waiting:
+                status_msg = "{} - {}".format(is_ready, waiting.reason)
+            elif is_ready and self._is_supervised(pod, spec, status):
                 icon = ready_map["dev"]
                 status_msg = "supervisor is running"
-            elif status.ready and self._is_uncrashed(pod, spec, status):
+            elif is_ready and self._is_uncrashed(pod, spec, status):
                 icon = ready_map["dev"]
                 status_msg = "still sleeping, having recovered from crashed state"
 
             print("{}{} - ready: {}".format(icon, pod.metadata.name, status_msg))
         print("")
 
     def split_destination(self, destination):
@@ -373,19 +398,18 @@
                 yield deployment, container_spec
 
     def generate_matching_containers(self, image_base):
         result = self.api.list_pod_for_all_namespaces(watch=False)
 
         for pod in result.items:
             for spec, status in self.list_containers(pod):
-                if not status:
-                    continue
-
-                parsed = urlparse(status.image_id)
-                pod_images = [status.image, f"{parsed.netloc}{parsed.path}"]
+                pod_images = [spec.image]
+                if status:
+                    parsed = urlparse(status.image_id)
+                    pod_images = [*pod_images, status.image, f"{parsed.netloc}{parsed.path}"]
 
                 if not any(i.startswith(image_base) for i in pod_images):
                     continue
                 yield pod, spec, status
 
     def list_containers(self, pod):
         containers = {}
@@ -416,17 +440,21 @@
                 )
                 continue
 
             if not self.dry_run_exec(pod, spec, status):
                 print("{} failed to rsync into {}".format(src_file_path, pod.metadata.name))
                 continue
 
-            container_dir = self.get_container_destination_dir(pod, status, destination_dir)
-            rsh_command, rsh_env = self.get_exec_command(pod.metadata.namespace, pod.metadata.name, status.name)
-            self.sync_files(rsh_command, src_file_path, container_dir, rsh_env=rsh_env, **kwargs)
+            if self._full_sync is not False:
+                container_dir = self.get_container_destination_dir(pod, status, destination_dir)
+                rsh_command, rsh_env = self.get_exec_command(pod.metadata.namespace, pod.metadata.name, status.name)
+                self.sync_files(rsh_command, src_file_path, container_dir, rsh_env=rsh_env, **kwargs)
+            else:
+                self._full_sync = None
+                print("Full Sync skipped")
 
     def sync_files(self, rsh_command, src_file, destination_dir: str = None, **kwargs):
         rsh_destination = ":{}".format(destination_dir)
         rsync_args = {
             **kwargs,
             "destination_dir": rsh_destination,
             "rsh": rsh_command,
@@ -436,34 +464,45 @@
             self.rsync_backend_instance.sync_project(src_file, **rsync_args)
         elif src_file == "./":
             self.rsync_backend_instance.sync_project([src_file], **rsync_args)
         else:
             self.rsync_backend_instance.sync(src_file, **rsync_args)
 
     def _exec(self, pod, spec, status, command: list):
+        if not status:
+            raise ValueError(f"Pod {spec.name} does not have a container")
+
         return stream(
             self.api.connect_get_namespaced_pod_exec,
             pod.metadata.name,
             pod.metadata.namespace,
             container=status.name,
             command=command,
             stdin=False,
             stdout=True,
             stderr=True,
             tty=False,
         )
 
     def _uncrash(self, pod, spec, status):
-        if status.ready:
+        if status and status.ready:
             return
-        if not status.state.waiting and not status.state.terminated:
+        if status and not status.state.waiting and not status.state.terminated:
             return
 
         print("Pod {}, is crashing, attempting deployment recovery".format(pod.metadata.name))
-        deployments = self._set_deployment_command(pod, spec, status, command=Generic.get_uncrash_command())
+        resources = {"limits": {"memory": "16Gi", "cpu": "5000m"}, "requests": {"memory": "1Mi", "cpu": "1m"}}
+        deployments = self._edit_deployment(
+            pod,
+            spec,
+            status,
+            command=Generic.get_uncrash_command(),
+            image_pull_policy="IfNotPresent",
+            resources=resources,
+        )
 
         please_wait()
         w = watch.Watch()
         for event in w.stream(self.api.list_pod_for_all_namespaces, timeout_seconds=30):
             event_pod = event["object"]
             if pod.metadata.name != event_pod.metadata.name:
                 continue
@@ -482,36 +521,35 @@
         try:
             resp = self._exec(pod, spec, status, Generic.check_can_exec())
             return
         except:
             self._uncrash(pod, spec, status)
 
     def _sniff_image_distro(self, pod, spec, status):
-        for distro in [Alpine, CentOS, Ubuntu]:
+        for distro in [Alpine, ELinuxOS, Ubuntu]:
             try:
                 resp = self._exec(pod, spec, status, distro.check_package_manager())
-                if resp and "runtime exec failed" in resp:
+                if resp and "command not found" in resp:
                     continue
 
                 return distro
-            except:
+            except Exception as e:
                 pass
 
         print("Failed to detect container image OS variant. Assuming bash, rsync and supervisor are already installed")
         return Generic
 
     def dry_run_exec(self, pod, spec, status):
         try:
             resp = self._exec(pod, spec, status, self._image_distro.check_rsync())
-            if resp and "runtime exec failed" in resp:
+            if resp and "command not found" in resp:
                 resp = self._exec(pod, spec, status, self._image_distro.install_rsync())
-
-            resp = self._exec(pod, spec, status, self._image_distro.check_rsync())
-            if resp and "runtime exec failed" in resp:
-                return False
+                resp = self._exec(pod, spec, status, self._image_distro.check_rsync())
+                if resp and "command not found" in resp:
+                    return False
 
             return len(resp) > 0
         except:
             return False
 
     def stabilize_deployments(self, image_base):
         # Uncrash crashed deployments
@@ -538,15 +576,15 @@
             if action == "install":
                 self.supervisor_install(pod, spec, status)
             else:
                 self.supervisor_uninstall(pod, spec, status)
             pods[pod.metadata.name] = pod
 
         if not len(pods):
-            print("None of the deployment containers match the given image")
+            print(f"None of the deployment containers match the given image ({image_base})")
             return
 
         please_wait()
         w = watch.Watch()
         cleanup_started = False
         for event in w.stream(self.api.list_pod_for_all_namespaces, timeout_seconds=self.pod_timeout):
             pod = event["object"]
@@ -578,15 +616,35 @@
         if supervisor:
             self.toggle_supervisor(image_base, "install")
         self.status(image_base)
         for p in src_file_paths:
             GIT_FILTER.load_ignored_files(p)
         self.sync(src_file_paths, destination_dir, **kwargs)
 
+    def sync_project(self, src_file_paths, **kwargs):
+        self.sync(src_file_paths, **kwargs)
+
     def on_monitor_exit(self, destination_dir: str = None, supervisor: bool = True, **kwargs):
         image_base, _ = self.split_destination(destination_dir)
         if supervisor:
             self.toggle_supervisor(image_base, "uninstall")
         self.status(image_base)
 
 
+def marshall_dfsync_annotation(container_spec, property_keys):
+    return {k: marshall_spec_property(container_spec, k) for k in property_keys}
+
+
+def marshall_spec_property(container_spec, key):
+    value = getattr(container_spec, key)
+
+    if value is None or isinstance(value, (str, list)):
+        return value
+    elif hasattr(value, "to_dict"):
+        return value.to_dict()
+    elif key == "resources":
+        return {"limits": value.limits, "requests": value.requests}
+    else:
+        return value
+
+
 kube_backend = KubeReDeployer
```

### Comparing `dfsync-0.3.8/dfsync/backends/kube_exec.py` & `dfsync-0.4.0/dfsync/backends/kube_exec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 #!/usr/bin/env python
-import os
-import os.path
-import subprocess
-import sys
+import os, os.path, subprocess, sys, time
 
 from kubernetes import client, config
 
 
 def get_kubectl_exec_command(namespace, pod_name, container_name, kube_config=None, kube_context=None):
     kubeconfig = [f"--kubeconfig={kube_config}"] if kube_config else []
     context = [f"--context={kube_context}"] if kube_context else []
@@ -29,24 +26,34 @@
 
 
 def main():
     pod_name = os.environ.get("KUBEEXEC_POD")
     if not pod_name:
         raise ValueError("Expecting pod name in 'KUBEEXEC_POD' env. variable")
 
+    kube_container = os.environ.get("KUBEEXEC_CONTAINER")
     kubectl_cmd = get_kubectl_exec_command(
         os.environ.get("KUBEEXEC_NAMESPACE"),
         pod_name,
-        os.environ.get("KUBEEXEC_CONTAINER"),
+        kube_container,
         os.environ.get("KUBEEXEC_KUBECONFIG"),
         os.environ.get("KUBEEXEC_CONTEXT"),
     )
 
-    container_cmd = get_container_command()
-    cmd = [*kubectl_cmd, *container_cmd]
-    subprocess.check_call(cmd)
-    # print("MIHAI\n\n", file=sys.stderr)
-    # print(subprocess.check_output(cmd), file=sys.stderr)
+    with open(f"dfsync-{kube_container}.log", "a") as f:
+        container_cmd = get_container_command()
+        cmd = [*kubectl_cmd, *container_cmd]
+        cmd_str = " ".join(cmd)
+        print(f"[{pod_name}] Running: {cmd_str}", file=f, flush=True)
+        try:
+            subprocess.check_call(cmd)
+
+        except Exception as e:
+            err = str(e) or type(e)
+            print(f"[{pod_name}] Error: {err}", file=f, flush=True)
+
+        finally:
+            print(f"[{pod_name}] Exiting", file=f, flush=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dfsync-0.3.8/dfsync/backends/rsync.py` & `dfsync-0.4.0/dfsync/backends/rsync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import logging
-import os.path
-import subprocess
+import logging, os, os.path, subprocess
 
 from dfsync.filters import list_files_to_ignore
 
 EVENT_TYPE_MAP = {
     "created": "Created",
     "deleted": "Deleted",
     "default": "Synced",
     "full-sync": "Full Sync",
 }
 
 
+def echo(msg=""):
+    print(f"{msg}")
+
+
 class FileRsync:
     def __init__(self, **kwargs):
         pass
 
     def sync(self, src_file_path, event=None, watched_dir: str = None, **kwargs):
         rsync_cwd = watched_dir
         event_type = "default"
@@ -34,57 +36,72 @@
         event_type="default",
         rsh=None,
         rsh_env=None,
         blocking_io=False,
         rsync_cwd=None,
         **kwargs,
     ):
+        event_type_str = EVENT_TYPE_MAP.get(event_type) or EVENT_TYPE_MAP.get("default")
+        if event_type == "full-sync":
+            echo(f"{event_type_str} running")
+
         rsh = ["--rsh={}".format(rsh)] if rsh is not None else []
         blocking_io = ["--blocking-io"] if blocking_io else []
 
         src_file_paths = [sanitize_relative_path(src_path) for src_path in src_file_paths]
         destination_dir = destination_dir.rstrip("/")
         destination_dir = "{}/".format(destination_dir)
 
         if event_type == "deleted":
             if len(src_file_paths) > 1:
-                print("multi-source delete is not supported")
+                echo("multi-source delete is not supported")
             rsync_cmd = self._get_rsync_cmd_on_file_delete(src_file_paths[0], destination_dir, blocking_io, rsh)
         elif event_type == "full-sync":
             src_paths = [p or "./" for p in src_file_paths]
             rsync_cmd = self._get_rsync_cmd_on_full_sync(src_paths, destination_dir, blocking_io, rsh)
         else:
             rsync_cmd = [
                 "rsync",
                 "-Rvx",
+                "--temp-dir=/tmp",
+                "--delay-updates",
                 *blocking_io,
                 *rsh,
                 *src_file_paths,
                 destination_dir,
             ]
 
         logging.debug("rsync command: {}".format(" ".join(rsync_cmd)))
 
         popen_args = {}
         if rsync_cwd:
             popen_args.update(dict(cwd=rsync_cwd))
-        subprocess.check_call(
-            rsync_cmd,
-            stdin=subprocess.DEVNULL,
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-            env=rsh_env,
-            **popen_args,
-        )
+        try:
+            subprocess.check_call(
+                rsync_cmd,
+                stdin=subprocess.DEVNULL,
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+                env=rsh_env,
+                **popen_args,
+            )
+        except:
+            echo("Sync failed")
+            env_str = "N/A"
+            if rsh_env:
+                env_str = " ".join(f"{k}={v}" for k, v in rsh_env.items() if k not in os.environ.keys())
+            echo(f"Env Var: {env_str}")
+            cmd_str = " ".join(f"'{arg}'" if " " in arg else arg for arg in rsync_cmd)
+            echo(f"Command: {cmd_str}")
+            raise
 
-        event_type = EVENT_TYPE_MAP.get(event_type) or EVENT_TYPE_MAP.get("default")
         if len(src_file_paths) == 1:
-            print("{} {}".format(event_type, src_file_paths[0]))
+            echo("{} {}".format(event_type_str, src_file_paths[0]))
         else:
-            print("{} {}".format(event_type, src_file_paths))
+            echo("{} {}".format(event_type_str, src_file_paths))
 
     def _get_rsync_cmd_on_file_delete(self, src_file_path, destination_dir: str, blocking_io: list, rsh: list):
         src_dir, file_name = os.path.split(src_file_path)
         intermediate_paths = [file_name]
         while len(src_dir) > 0 and src_dir.strip() != ".":
             if os.path.isdir(src_dir):
                 break
@@ -114,14 +131,16 @@
         return cmd
 
     def _get_rsync_cmd_on_full_sync(self, src_file_paths: list, destination_dir: str, blocking_io: list, rsh: list):
         filters = ["--filter=- {}".format(f) for f in list_files_to_ignore()]
         return [
             "rsync",
             "-rvx",
+            "--temp-dir=/tmp",
+            "--delay-updates",
             "--delete",
             "--filter=- .git/",
             *filters,
             *blocking_io,
             *rsh,
             *[f"{p}/" for p in src_file_paths],
             destination_dir,
```

### Comparing `dfsync-0.3.8/dfsync/exp.py` & `dfsync-0.4.0/dfsync/exp.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.3.8/dfsync/filters.py` & `dfsync-0.4.0/dfsync/filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import fnmatch
+import black, fnmatch
 import os.path
 import git.exc
 import subprocess
 from watchdog.events import FileCreatedEvent, FileModifiedEvent, FileDeletedEvent
 
 
 def exclude_watchdog_directory_events(event=None, **kwargs):
@@ -10,55 +10,101 @@
     for event_class in event_classes:
         if isinstance(event, event_class):
             return True
     return False
 
 
 EMACS_PATTERNS = ["*~", "#*#", ".#*", ".goutputstream-*", "*_flymake.py"]
+PYTHON_PATTERNS = ["*.py"]
+
+
+def echo(msg):
+    print(f"{msg}")
 
 
 class LoggingFilter:
     def __init__(self):
         self.ignored_files = set()
 
     def _ignore(self, src_file_path: str, reason: str = None):
         if src_file_path in self.ignored_files:
             return
         self.ignored_files.add(src_file_path)
 
         reason = reason or ""
         if len(reason):
-            reason = ", {}".format(reason)
+            reason = f", {reason}"
 
-        print("Ignored {}{}".format(src_file_path, reason))
+        echo(f"Ignored {src_file_path}{reason}")
 
     def _unignore(self, src_file_path: str):
         if src_file_path not in self.ignored_files:
             return
         self.ignored_files.remove(src_file_path)
 
     def is_not_filtered(self, *args, **kwargs):
         return self.is_filtered(*args, **kwargs) is False
 
 
-class EmacsBufferFilter(LoggingFilter):
+class UserConfigFilter(LoggingFilter):
+    def __init__(self, ignored_patterns):
+        super().__init__()
+        self._ignored_patterns = ignored_patterns
+        self._ignore_message = "ignoring, matches pattern from ignore_files config"
+        for pattern in ignored_patterns:
+            if "*" not in pattern:
+                self.ignored_files.add(pattern)
+
     def is_filtered(self, src_file_path: str = None, event=None, **kwargs):
         src_file_path = src_file_path or event.src_path
         if src_file_path is None:
             raise ValueError("A file path or watchdog event is required")
 
         parent_path, file_name = os.path.split(os.path.expanduser(src_file_path))
-        for pattern in EMACS_PATTERNS:
+        for pattern in self._ignored_patterns:
             if fnmatch.fnmatch(file_name, pattern):
-                self._ignore(src_file_path, "Emacs buffer backup")
+                self._ignore(src_file_path, self._ignore_message)
                 return True
 
         return False
 
 
+class EmacsBufferFilter(UserConfigFilter):
+    def __init__(self):
+        super().__init__(EMACS_PATTERNS)
+        self._ignore_message = "Emacs buffer backup"
+
+
+class PythonBlackFilter(LoggingFilter):
+    def __init__(self):
+        super().__init__()
+
+    def is_filtered(self, src_file_path: str = None, event=None, **kwargs):
+        src_file_path = src_file_path or event.src_path
+        if src_file_path is None:
+            raise ValueError("A file path or watchdog event is required")
+
+        parent_path, file_name = os.path.split(os.path.expanduser(src_file_path))
+        for pattern in PYTHON_PATTERNS:
+            if fnmatch.fnmatch(file_name, pattern):
+                return self._black_check(src_file_path)
+        return False
+
+    def _black_check(self, src_file_path):
+        try:
+            with open(src_file_path, "r") as f:
+                contents = f.read()
+                black.format_file_contents(contents, fast=False, mode=black.FileMode())
+            return False
+
+        except Exception as e:
+            echo(f"Rejected {src_file_path}, {e}")
+            return True
+
+
 class UntrackedGitFilesFilter(LoggingFilter):
     def __init__(self):
         super().__init__()
         self._repos = {}
         self._is_repo_initialized = {}
         self._untracked_and_ignored_files = {}
 
@@ -89,15 +135,15 @@
             from git import Repo
 
             parent_path = self._get_existing_parent(path)
             if parent_path is not None:
                 repo = Repo(parent_path, search_parent_directories=True)
                 self._repos[repo.working_tree_dir] = repo
                 self._is_repo_initialized[repo.working_tree_dir] = True
-                print("Using git repo: {}".format(repo.working_tree_dir))
+                echo("Using git repo: {}".format(repo.working_tree_dir))
         except git.exc.InvalidGitRepositoryError:
             pass
         except ImportError:
             pass
 
         return repo
 
@@ -129,30 +175,39 @@
             abs_file_path = os.path.join(repo.working_dir, rel_file_path)
             if src_abs_path == abs_file_path:
                 self._ignore(src_file_path, "Untracked GIT file")
                 return True
         return False
 
 
-EDITOR_FILTERS = [EmacsBufferFilter()]
+USER_FILTERS = [EmacsBufferFilter(), PythonBlackFilter()]
 GIT_FILTER = UntrackedGitFilesFilter()
+ALL_FILTERS = [
+    exclude_watchdog_directory_events,
+    *[f.is_not_filtered for f in USER_FILTERS],
+    GIT_FILTER.is_not_filtered,
+]
 
 
 def list_files_to_ignore():
     result = set(GIT_FILTER.get_untracked_and_ignored_files())
-    for editor_filter in EDITOR_FILTERS:
+    for editor_filter in USER_FILTERS:
         result = {*result, *editor_filter.ignored_files}
     return result
 
 
 def path_is_parent(parent_path, child_path):
     parent_path = os.path.abspath(parent_path)
     child_path = os.path.abspath(child_path)
 
     return os.path.commonpath([parent_path]) == os.path.commonpath([parent_path, child_path])
 
 
-ALL_FILTERS = [
-    exclude_watchdog_directory_events,
-    *[f.is_not_filtered for f in EDITOR_FILTERS],
-    GIT_FILTER.is_not_filtered,
-]
+def add_user_filter(f: LoggingFilter):
+    if f is None:
+        raise ValueError("Expecting non-null user filter")
+    USER_FILTERS.append(f)
+    ALL_FILTERS.append(f.is_not_filtered)
+
+
+def add_user_ignored_patterns_filter(patterns: [str]):
+    add_user_filter(UserConfigFilter(patterns))
```

### Comparing `dfsync-0.3.8/dfsync/transactions.py` & `dfsync-0.4.0/dfsync/transactions.py`

 * *Files identical despite different names*

