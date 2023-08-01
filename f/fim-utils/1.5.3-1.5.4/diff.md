# Comparing `tmp/fim_utils-1.5.3.tar.gz` & `tmp/fim_utils-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim_utils-1.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fim_utils-1.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fim_utils-1.5.3.tar` & `fim_utils-1.5.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1955 2023-06-14 13:08:12.061187 fim_utils-1.5.3/.gitignore
--rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.3/LICENSE
--rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.3/MANIFEST.in
--rw-r--r--   0        0        0     7348 2023-06-14 13:08:12.061836 fim_utils-1.5.3/README.md
--rw-r--r--   0        0        0      156 2023-06-30 20:01:29.261689 fim_utils-1.5.3/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.3/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.3/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.3/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.3/fimutil/al2s/oess.py
--rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.3/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    19815 2023-06-14 13:08:12.063296 fim_utils-1.5.3/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.3/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.3/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.3/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3456 2023-06-14 20:11:33.885819 fim_utils-1.5.3/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.3/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2023-06-14 13:08:12.064708 fim_utils-1.5.3/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    21991 2023-06-14 13:08:12.065444 fim_utils-1.5.3/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2574 2023-06-14 20:11:33.888572 fim_utils-1.5.3/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     1304 2023-06-14 20:11:33.889490 fim_utils-1.5.3/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.3/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1666 2023-06-14 13:08:12.067133 fim_utils-1.5.3/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.3/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     6407 2023-06-30 19:52:17.512322 fim_utils-1.5.3/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.3/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    10922 2023-06-14 20:11:33.890225 fim_utils-1.5.3/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2023-06-14 13:08:12.067791 fim_utils-1.5.3/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6183 2023-06-14 13:08:12.068611 fim_utils-1.5.3/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1717 2023-06-14 13:08:12.069196 fim_utils-1.5.3/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     1351 2023-06-14 13:08:12.069677 fim_utils-1.5.3/fimutil/utilities/scan_oess.py
--rw-r--r--   0        0        0     5594 2023-06-14 20:11:33.890832 fim_utils-1.5.3/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2121 2023-06-14 20:11:33.891406 fim_utils-1.5.3/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0     1008 2023-06-14 13:08:12.071273 fim_utils-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.3/setup.py
--rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.3/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.3/test/netam_test.py
--rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.3/test/ralph_test.py
--rw-r--r--   0        0        0     8070 1970-01-01 00:00:00.000000 fim_utils-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1955 2023-06-14 13:08:12.061187 fim_utils-1.5.4/.gitignore
+-rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.4/LICENSE
+-rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.4/MANIFEST.in
+-rw-r--r--   0        0        0     7602 2023-08-01 20:56:35.356420 fim_utils-1.5.4/README.md
+-rw-r--r--   0        0        0      156 2023-08-01 21:50:24.054188 fim_utils-1.5.4/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.4/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.4/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.4/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.4/fimutil/al2s/oess.py
+-rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.4/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    19815 2023-06-14 13:08:12.063296 fim_utils-1.5.4/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.4/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.4/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.4/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3456 2023-06-14 20:11:33.885819 fim_utils-1.5.4/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.4/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2023-06-14 13:08:12.064708 fim_utils-1.5.4/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    21991 2023-06-14 13:08:12.065444 fim_utils-1.5.4/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2574 2023-06-14 20:11:33.888572 fim_utils-1.5.4/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     1304 2023-06-14 20:11:33.889490 fim_utils-1.5.4/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.4/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1666 2023-06-14 13:08:12.067133 fim_utils-1.5.4/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.4/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     6752 2023-08-01 21:44:39.997310 fim_utils-1.5.4/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.4/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    10922 2023-06-14 20:11:33.890225 fim_utils-1.5.4/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:08:12.067791 fim_utils-1.5.4/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6183 2023-06-14 13:08:12.068611 fim_utils-1.5.4/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1717 2023-06-14 13:08:12.069196 fim_utils-1.5.4/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     1351 2023-06-14 13:08:12.069677 fim_utils-1.5.4/fimutil/utilities/scan_oess.py
+-rw-r--r--   0        0        0     5625 2023-08-01 20:57:56.479340 fim_utils-1.5.4/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2121 2023-06-14 20:11:33.891406 fim_utils-1.5.4/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1008 2023-06-14 13:08:12.071273 fim_utils-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.4/setup.py
+-rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.4/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.4/test/netam_test.py
+-rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.4/test/ralph_test.py
+-rw-r--r--   0        0        0     8324 1970-01-01 00:00:00.000000 fim_utils-1.5.4/PKG-INFO
```

### Comparing `fim_utils-1.5.3/.gitignore` & `fim_utils-1.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/LICENSE` & `fim_utils-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/README.md` & `fim_utils-1.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,32 +94,37 @@
 ```
 {
   "SITE1": {
     "dpswitch": {
       "URL": <URL of SITE2's dp switch in Ralph>,
       "Site": "SITE2"
     },
+    "ptp": true,
     "storage": {
       "Disk": "500TB"
     },
     "workers": {
       <worker FQDN>: {
         "Disk": "100TB",
         "Core": "15",
         "RAM": "2TB",
         "CPU": "4"
       }
     },
     "mac_offset": "f2:ab"
+    "connected_ports": [ "HundredGigE0/0/0/15" ]
   }
 }
 ```
 `mac_offset` intended to be used with OpenStack sites to aid unique MAC generation for vNICs. Note
 that the first octet of mac_offset must be [even](https://github.com/openstack/neutron-lib/blob/cf494c8be10b36daf238fa12cf7c615656e6640d/neutron_lib/api/validators/__init__.py#L40).
 
+`connected_ports` are only effective for generating JSON files (do not affect ARMs) which are then used to put other ports
+(not include uplinks and facility ports) into admin DOWN state.
+
 ### scan_net.py
 
 Similar to above, interrogates NSO, PCE (future work) to create a model of the inter-site network.
 
 Invocation:
 ```
 $ scan_net.py -c config_file -m <model name>.graphml --isis-link-validation
```

### Comparing `fim_utils-1.5.3/fimutil/al2s/arm.py` & `fim_utils-1.5.4/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/al2s/cloud_cfg.py` & `fim_utils-1.5.4/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/al2s/oess.py` & `fim_utils-1.5.4/fimutil/al2s/oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/netam/arm.py` & `fim_utils-1.5.4/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/netam/nso.py` & `fim_utils-1.5.4/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/netam/sr_pce.py` & `fim_utils-1.5.4/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/asset.py` & `fim_utils-1.5.4/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/dp_switch.py` & `fim_utils-1.5.4/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/ethernetport.py` & `fim_utils-1.5.4/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/fim_helper.py` & `fim_utils-1.5.4/fimutil/ralph/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/fpga.py` & `fim_utils-1.5.4/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/gpu.py` & `fim_utils-1.5.4/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/model.py` & `fim_utils-1.5.4/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/nvme.py` & `fim_utils-1.5.4/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/ralph_uri.py` & `fim_utils-1.5.4/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/site.py` & `fim_utils-1.5.4/fimutil/ralph/site.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,13 +133,19 @@
             ret["Storage"] = self.storage.fields.copy()
         if self.dp_switch:
             ret["DataPlane"] = self.dp_switch.fields.copy()
         # collect port information from all workers
         dp_ports = list()
         for w in self.workers:
             dp_ports.extend(w.get_dp_ports())
+        # see if any extra ports are mentioned in the config file
+        if self.config and self.config.get(self.name) and self.config.get(self.name).get('connected_ports'):
+            dp_ports.extend(self.config.get(self.name).get('connected_ports'))
+        # uniquify and sort
+        dp_ports = list(set(dp_ports))
+        dp_ports.sort()
         ret["DataPlane"]["Connected_ports"] = dp_ports
         n = list()
         for w in self.workers:
             n.append(w.to_json())
         ret["Nodes"] = n
         return ret
```

### Comparing `fim_utils-1.5.3/fimutil/ralph/storage.py` & `fim_utils-1.5.4/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/ralph/worker_node.py` & `fim_utils-1.5.4/fimutil/ralph/worker_node.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/utilities/generate_instance_flavors.py` & `fim_utils-1.5.4/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/utilities/scan_net.py` & `fim_utils-1.5.4/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/utilities/scan_oess.py` & `fim_utils-1.5.4/fimutil/utilities/scan_oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/fimutil/utilities/scan_site.py` & `fim_utils-1.5.4/fimutil/utilities/scan_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                         help="Print only a brief description of assets")
     parser.add_argument("-j", "--json", action="store",
                         help="Produce simplified output in JSON format and save to specified file")
     parser.add_argument("-l", "--lightweight", action="store_true",
                         help="This is a lightweight site supporting only OpenStack virtual NICs")
     parser.add_argument("-c", "--config", action="store", default=".scan-config.json",
                         help="JSON-formatted additional configuration file, "
-                             "including e.g. odd site-dataplane switch mapping")
+                             "including e.g. odd site-dataplane switch mapping. Defaults to .scan-config.json")
 
     args = parser.parse_args()
 
     if args.debug is None:
         logging.basicConfig(level=logging.INFO)
     elif args.debug >= 1:
         logging.basicConfig(level=logging.DEBUG)
```

### Comparing `fim_utils-1.5.3/fimutil/utilities/scan_worker.py` & `fim_utils-1.5.4/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/pyproject.toml` & `fim_utils-1.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/setup.py` & `fim_utils-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/test/netam_test.py` & `fim_utils-1.5.4/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.3/PKG-INFO` & `fim_utils-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.5.3
+Version: 1.5.4
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>, Hussamuddin Nasir <nasir@netlab.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -112,32 +112,37 @@
 ```
 {
   "SITE1": {
     "dpswitch": {
       "URL": <URL of SITE2's dp switch in Ralph>,
       "Site": "SITE2"
     },
+    "ptp": true,
     "storage": {
       "Disk": "500TB"
     },
     "workers": {
       <worker FQDN>: {
         "Disk": "100TB",
         "Core": "15",
         "RAM": "2TB",
         "CPU": "4"
       }
     },
     "mac_offset": "f2:ab"
+    "connected_ports": [ "HundredGigE0/0/0/15" ]
   }
 }
 ```
 `mac_offset` intended to be used with OpenStack sites to aid unique MAC generation for vNICs. Note
 that the first octet of mac_offset must be [even](https://github.com/openstack/neutron-lib/blob/cf494c8be10b36daf238fa12cf7c615656e6640d/neutron_lib/api/validators/__init__.py#L40).
 
+`connected_ports` are only effective for generating JSON files (do not affect ARMs) which are then used to put other ports
+(not include uplinks and facility ports) into admin DOWN state.
+
 ### scan_net.py
 
 Similar to above, interrogates NSO, PCE (future work) to create a model of the inter-site network.
 
 Invocation:
 ```
 $ scan_net.py -c config_file -m <model name>.graphml --isis-link-validation
```

