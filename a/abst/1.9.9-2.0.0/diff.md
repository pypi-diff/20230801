# Comparing `tmp/abst-1.9.9.tar.gz` & `tmp/abst-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.9.tar", last modified: Thu Jul 20 14:46:24 2023, max compression
+gzip compressed data, was "abst-2.0.0.tar", last modified: Tue Aug  1 15:12:37 2023, max compression
```

## Comparing `abst-1.9.9.tar` & `abst-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.194506 abst-1.9.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 14:46:12.000000 abst-1.9.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-20 14:46:24.194506 abst-1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-20 14:46:12.000000 abst-1.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:12.000000 abst-1.9.9/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-20 14:46:12.000000 abst-1.9.9/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:12.000000 abst-1.9.9/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-20 14:46:12.000000 abst-1.9.9/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-20 14:46:12.000000 abst-1.9.9/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-20 14:46:12.000000 abst-1.9.9/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-20 14:46:12.000000 abst-1.9.9/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 14:46:12.000000 abst-1.9.9/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-07-20 14:46:12.000000 abst-1.9.9/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:12.000000 abst-1.9.9/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-20 14:46:12.000000 abst-1.9.9/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 14:46:12.000000 abst-1.9.9/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 14:46:12.000000 abst-1.9.9/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:46:24.194506 abst-1.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 14:46:12.000000 abst-1.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.194506 abst-1.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-20 14:46:12.000000 abst-1.9.9/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:37.856941 abst-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 15:12:25.000000 abst-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-01 15:12:37.856941 abst-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-08-01 15:12:25.000000 abst-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:37.852941 abst-2.0.0/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:25.000000 abst-2.0.0/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-01 15:12:25.000000 abst-2.0.0/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:37.856941 abst-2.0.0/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:25.000000 abst-2.0.0/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-01 15:12:25.000000 abst-2.0.0/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-08-01 15:12:25.000000 abst-2.0.0/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-01 15:12:25.000000 abst-2.0.0/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-01 15:12:25.000000 abst-2.0.0/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 15:12:25.000000 abst-2.0.0/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-08-01 15:12:25.000000 abst-2.0.0/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:37.856941 abst-2.0.0/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:25.000000 abst-2.0.0/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-01 15:12:25.000000 abst-2.0.0/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 15:12:25.000000 abst-2.0.0/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 15:12:25.000000 abst-2.0.0/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:37.856941 abst-2.0.0/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-01 15:12:37.000000 abst-2.0.0/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-01 15:12:37.000000 abst-2.0.0/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:12:37.000000 abst-2.0.0/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 15:12:37.000000 abst-2.0.0/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 15:12:37.000000 abst-2.0.0/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 15:12:37.000000 abst-2.0.0/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:12:37.000000 abst-2.0.0/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:12:37.856941 abst-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-01 15:12:25.000000 abst-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:12:37.856941 abst-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-01 15:12:25.000000 abst-2.0.0/tests/test_sample_dict.py
```

### Comparing `abst-1.9.9/LICENSE.md` & `abst-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/PKG-INFO` & `abst-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.9
+Version: 2.0.0
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.9/README.md` & `abst-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst/bastion_support/bastion_scheduler.py` & `abst-2.0.0/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst/bastion_support/oci_bastion.py` & `abst-2.0.0/abst/bastion_support/oci_bastion.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,20 +119,26 @@
 
         self.current_status = "waiting for session init"
         self.wait_for_prepared()
 
         sleep(1)  # Precaution init delay
 
         self.current_status = "digging tunnel"
-        ssh_tunnel_args = self.run_ssh_tunnel_managed_session(bid, host,
-                                                              creds["private-key-path"],
-                                                              creds[
-                                                                  "resource-os-username"],
-                                                              ip, port,
-                                                              shell)
+        ssh_tunnel_args, exit_code = self.run_ssh_tunnel_managed_session(bid, host,
+                                                                         creds["private-key-path"],
+                                                                         creds[
+                                                                             "resource-os-username"],
+                                                                         ip, port,
+                                                                         shell)
+        logging.info(f"SSH tunnel exited with code {exit_code}")
+        if exit_code == 0:
+            print(f"User requested termination {self.get_print_name()}")
+            self.current_status = "terminated by user"
+            self.kill()
+            return
 
         while status := (sdata := self.get_bastion_state())[
                             "lifecycle_state"] == "ACTIVE":
             deleted = self.connect_till_deleted(sdata, ssh_tunnel_args, status, shell,
                                                 True)
 
             if deleted:
@@ -203,16 +209,16 @@
     def run_ssh_tunnel_managed_session(self, bid, host, private_key_path, username,
                                        ip, port,
                                        shell):
         print(f"Bastion {self.get_print_name()} initialized")
         print(f"Initializing SSH Tunnel for {self.get_print_name()}")
 
         ssh_tunnel_args = f'ssh -i {private_key_path} -o ServerAliveInterval=20 -o ProxyCommand="ssh -i {private_key_path} -W %h:%p -p {port} {bid}@{host} -A" -p {port} {username}@{ip} -A'
-        self.__run_ssh_tunnel_call(ssh_tunnel_args, shell, already_split=True)
-        return ssh_tunnel_args
+        exit_code = self.__run_ssh_tunnel_call(ssh_tunnel_args, shell, already_split=True)
+        return ssh_tunnel_args, exit_code
 
     def run_ssh_tunnel_port_forward(self, bid, host, ip, port, shell, local_port, ssh_pub_key_path):
         print(f"Bastion {self.get_print_name()} initialized")
         print(f"Initializing SSH Tunnel for {self.get_print_name()}")
         ssh_tunnel_arg_str = f"ssh -o ServerAliveInterval=20 -N -L {local_port}:{ip}:{port} -p 22 {bid}@{host} -vvv -i {ssh_pub_key_path.strip('.pub')}"
         self.__run_ssh_tunnel(ssh_tunnel_arg_str, shell)
         return ssh_tunnel_arg_str
@@ -457,15 +463,15 @@
         logging.debug(
             f'({self.get_print_name()}) SSH Tunnel command: '
             f'{" ".join(args_split) if not shell else args_split}')
         return args_split
 
     def __run_ssh_tunnel_call(self, ssh_tunnel_arg_str, shell, already_split=False):
 
-        os.system(ssh_tunnel_arg_str)
+        return os.system(ssh_tunnel_arg_str)
 
     def __run_ssh_tunnel(self, ssh_tunnel_arg_str, shell, already_split=False):
         """
 
         :param ssh_tunnel_arg_str: String for ssh tunnel creation
         :param shell: If you use shell environment (can have different impacts on MAC and
          LINUX)
```

### Comparing `abst-1.9.9/abst/cfg_func.py` & `abst-2.0.0/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst/config.py` & `abst-2.0.0/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst/dialogs.py` & `abst-2.0.0/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst/main.py` & `abst-2.0.0/abst/main.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst/notifier/version_notifier.py` & `abst-2.0.0/abst/notifier/version_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
 
-import eventlet
 import lastversion
 import requests
 import rich
 import semantic_version
 from requests import ConnectTimeout
 
 from abst import __version__
```

### Comparing `abst-1.9.9/abst/tools.py` & `abst-2.0.0/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst/wrappers.py` & `abst-2.0.0/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/abst.egg-info/PKG-INFO` & `abst-2.0.0/abst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.9
+Version: 2.0.0
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.9/abst.egg-info/SOURCES.txt` & `abst-2.0.0/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.9/setup.py` & `abst-2.0.0/setup.py`

 * *Files identical despite different names*

