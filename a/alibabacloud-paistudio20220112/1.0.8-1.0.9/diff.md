# Comparing `tmp/alibabacloud_paistudio20220112-1.0.8.tar.gz` & `tmp/alibabacloud_paistudio20220112-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_paistudio20220112-1.0.8.tar", last modified: Mon Sep 26 11:58:59 2022, max compression
+gzip compressed data, was "dist/alibabacloud_paistudio20220112-1.0.9.tar", last modified: Mon Nov 14 07:26:38 2022, max compression
```

## Comparing `alibabacloud_paistudio20220112-1.0.8.tar` & `alibabacloud_paistudio20220112-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      346 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112/__init__.py
--rw-r--r--   0 root         (0) root         (0)   101874 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112/client.py
--rw-r--r--   0 root         (0) root         (0)   197989 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2022-09-26 11:58:59.000000 alibabacloud_paistudio20220112-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      405 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101810 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112/client.py
+-rw-r--r--   0 root         (0) root         (0)   208132 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2022-11-14 07:26:38.000000 alibabacloud_paistudio20220112-1.0.9/setup.py
```

### Comparing `alibabacloud_paistudio20220112-1.0.8/LICENSE` & `alibabacloud_paistudio20220112-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_paistudio20220112-1.0.8/PKG-INFO` & `alibabacloud_paistudio20220112-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_paistudio20220112
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud PaiStudio (20220112) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paistudio20220112-1.0.8/README-CN.md` & `alibabacloud_paistudio20220112-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paistudio20220112-1.0.8/README.md` & `alibabacloud_paistudio20220112-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112/client.py` & `alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20220112_models.CreateAlgorithmVersionResponse:
         UtilClient.validate_model(tmp_req)
         request = pai_studio_20220112_models.CreateAlgorithmVersionShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.algorithm_spec):
-            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.algorithm_spec), 'AlgorithmSpec', 'json')
+            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.algorithm_spec, 'AlgorithmSpec', 'json')
         body = {}
         if not UtilClient.is_unset(request.algorithm_spec_shrink):
             body['AlgorithmSpec'] = request.algorithm_spec_shrink
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -207,15 +207,15 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20220112_models.CreateAlgorithmVersionResponse:
         UtilClient.validate_model(tmp_req)
         request = pai_studio_20220112_models.CreateAlgorithmVersionShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.algorithm_spec):
-            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.algorithm_spec), 'AlgorithmSpec', 'json')
+            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.algorithm_spec, 'AlgorithmSpec', 'json')
         body = {}
         if not UtilClient.is_unset(request.algorithm_spec_shrink):
             body['AlgorithmSpec'] = request.algorithm_spec_shrink
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -2275,15 +2275,15 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20220112_models.UpdateAlgorithmVersionResponse:
         UtilClient.validate_model(tmp_req)
         request = pai_studio_20220112_models.UpdateAlgorithmVersionShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.algorithm_spec):
-            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.algorithm_spec), 'AlgorithmSpec', 'json')
+            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.algorithm_spec, 'AlgorithmSpec', 'json')
         body = {}
         if not UtilClient.is_unset(request.algorithm_spec_shrink):
             body['AlgorithmSpec'] = request.algorithm_spec_shrink
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -2311,15 +2311,15 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20220112_models.UpdateAlgorithmVersionResponse:
         UtilClient.validate_model(tmp_req)
         request = pai_studio_20220112_models.UpdateAlgorithmVersionShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.algorithm_spec):
-            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.algorithm_spec), 'AlgorithmSpec', 'json')
+            request.algorithm_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.algorithm_spec, 'AlgorithmSpec', 'json')
         body = {}
         if not UtilClient.is_unset(request.algorithm_spec_shrink):
             body['AlgorithmSpec'] = request.algorithm_spec_shrink
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
```

### Comparing `alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112/models.py` & `alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,14 +396,143 @@
         if m.get('count') is not None:
             self.count = m.get('count')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class JobViewMetric(TeaModel):
+    def __init__(
+        self,
+        cpuusage_rate: str = None,
+        disk_read_rate: str = None,
+        disk_write_rate: str = None,
+        gpuusage_rate: str = None,
+        job_id: str = None,
+        job_type: str = None,
+        memory_usage_rate: str = None,
+        network_input_rate: str = None,
+        network_output_rate: str = None,
+        node_names: List[str] = None,
+        request_cpu: int = None,
+        request_gpu: int = None,
+        request_memory: int = None,
+        resource_group_id: str = None,
+        total_cpu: int = None,
+        total_gpu: int = None,
+        total_memory: int = None,
+        user_id: str = None,
+    ):
+        self.cpuusage_rate = cpuusage_rate
+        self.disk_read_rate = disk_read_rate
+        self.disk_write_rate = disk_write_rate
+        self.gpuusage_rate = gpuusage_rate
+        self.job_id = job_id
+        self.job_type = job_type
+        self.memory_usage_rate = memory_usage_rate
+        self.network_input_rate = network_input_rate
+        self.network_output_rate = network_output_rate
+        self.node_names = node_names
+        self.request_cpu = request_cpu
+        self.request_gpu = request_gpu
+        self.request_memory = request_memory
+        self.resource_group_id = resource_group_id
+        self.total_cpu = total_cpu
+        self.total_gpu = total_gpu
+        self.total_memory = total_memory
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cpuusage_rate is not None:
+            result['CPUUsageRate'] = self.cpuusage_rate
+        if self.disk_read_rate is not None:
+            result['DiskReadRate'] = self.disk_read_rate
+        if self.disk_write_rate is not None:
+            result['DiskWriteRate'] = self.disk_write_rate
+        if self.gpuusage_rate is not None:
+            result['GPUUsageRate'] = self.gpuusage_rate
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.job_type is not None:
+            result['JobType'] = self.job_type
+        if self.memory_usage_rate is not None:
+            result['MemoryUsageRate'] = self.memory_usage_rate
+        if self.network_input_rate is not None:
+            result['NetworkInputRate'] = self.network_input_rate
+        if self.network_output_rate is not None:
+            result['NetworkOutputRate'] = self.network_output_rate
+        if self.node_names is not None:
+            result['NodeNames'] = self.node_names
+        if self.request_cpu is not None:
+            result['RequestCPU'] = self.request_cpu
+        if self.request_gpu is not None:
+            result['RequestGPU'] = self.request_gpu
+        if self.request_memory is not None:
+            result['RequestMemory'] = self.request_memory
+        if self.resource_group_id is not None:
+            result['ResourceGroupID'] = self.resource_group_id
+        if self.total_cpu is not None:
+            result['TotalCPU'] = self.total_cpu
+        if self.total_gpu is not None:
+            result['TotalGPU'] = self.total_gpu
+        if self.total_memory is not None:
+            result['TotalMemory'] = self.total_memory
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CPUUsageRate') is not None:
+            self.cpuusage_rate = m.get('CPUUsageRate')
+        if m.get('DiskReadRate') is not None:
+            self.disk_read_rate = m.get('DiskReadRate')
+        if m.get('DiskWriteRate') is not None:
+            self.disk_write_rate = m.get('DiskWriteRate')
+        if m.get('GPUUsageRate') is not None:
+            self.gpuusage_rate = m.get('GPUUsageRate')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('JobType') is not None:
+            self.job_type = m.get('JobType')
+        if m.get('MemoryUsageRate') is not None:
+            self.memory_usage_rate = m.get('MemoryUsageRate')
+        if m.get('NetworkInputRate') is not None:
+            self.network_input_rate = m.get('NetworkInputRate')
+        if m.get('NetworkOutputRate') is not None:
+            self.network_output_rate = m.get('NetworkOutputRate')
+        if m.get('NodeNames') is not None:
+            self.node_names = m.get('NodeNames')
+        if m.get('RequestCPU') is not None:
+            self.request_cpu = m.get('RequestCPU')
+        if m.get('RequestGPU') is not None:
+            self.request_gpu = m.get('RequestGPU')
+        if m.get('RequestMemory') is not None:
+            self.request_memory = m.get('RequestMemory')
+        if m.get('ResourceGroupID') is not None:
+            self.resource_group_id = m.get('ResourceGroupID')
+        if m.get('TotalCPU') is not None:
+            self.total_cpu = m.get('TotalCPU')
+        if m.get('TotalGPU') is not None:
+            self.total_gpu = m.get('TotalGPU')
+        if m.get('TotalMemory') is not None:
+            self.total_memory = m.get('TotalMemory')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
 class MachineGroup(TeaModel):
     def __init__(
         self,
         creator_id: str = None,
         ecs_count: int = None,
         ecs_spec: str = None,
         gmt_created_time: str = None,
@@ -587,14 +716,137 @@
                 temp_model = Metric()
                 self.metrics.append(temp_model.from_map(k))
         if m.get('NodeID') is not None:
             self.node_id = m.get('NodeID')
         return self
 
 
+class NodeViewMetric(TeaModel):
+    def __init__(
+        self,
+        created_time: str = None,
+        disk_read_rate: str = None,
+        disk_write_rate: str = None,
+        gputype: str = None,
+        machine_group_id: str = None,
+        network_input_rate: str = None,
+        network_output_rate: str = None,
+        node_id: str = None,
+        node_type: str = None,
+        request_cpu: int = None,
+        request_gpu: int = None,
+        request_memory: int = None,
+        total_cpu: int = None,
+        total_gpu: int = None,
+        total_memory: int = None,
+        user_ids: List[str] = None,
+        user_number: str = None,
+    ):
+        self.created_time = created_time
+        self.disk_read_rate = disk_read_rate
+        self.disk_write_rate = disk_write_rate
+        self.gputype = gputype
+        self.machine_group_id = machine_group_id
+        self.network_input_rate = network_input_rate
+        self.network_output_rate = network_output_rate
+        self.node_id = node_id
+        self.node_type = node_type
+        self.request_cpu = request_cpu
+        self.request_gpu = request_gpu
+        self.request_memory = request_memory
+        self.total_cpu = total_cpu
+        self.total_gpu = total_gpu
+        self.total_memory = total_memory
+        self.user_ids = user_ids
+        self.user_number = user_number
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.created_time is not None:
+            result['CreatedTime'] = self.created_time
+        if self.disk_read_rate is not None:
+            result['DiskReadRate'] = self.disk_read_rate
+        if self.disk_write_rate is not None:
+            result['DiskWriteRate'] = self.disk_write_rate
+        if self.gputype is not None:
+            result['GPUType'] = self.gputype
+        if self.machine_group_id is not None:
+            result['MachineGroupID'] = self.machine_group_id
+        if self.network_input_rate is not None:
+            result['NetworkInputRate'] = self.network_input_rate
+        if self.network_output_rate is not None:
+            result['NetworkOutputRate'] = self.network_output_rate
+        if self.node_id is not None:
+            result['NodeID'] = self.node_id
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        if self.request_cpu is not None:
+            result['RequestCPU'] = self.request_cpu
+        if self.request_gpu is not None:
+            result['RequestGPU'] = self.request_gpu
+        if self.request_memory is not None:
+            result['RequestMemory'] = self.request_memory
+        if self.total_cpu is not None:
+            result['TotalCPU'] = self.total_cpu
+        if self.total_gpu is not None:
+            result['TotalGPU'] = self.total_gpu
+        if self.total_memory is not None:
+            result['TotalMemory'] = self.total_memory
+        if self.user_ids is not None:
+            result['UserIDs'] = self.user_ids
+        if self.user_number is not None:
+            result['UserNumber'] = self.user_number
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreatedTime') is not None:
+            self.created_time = m.get('CreatedTime')
+        if m.get('DiskReadRate') is not None:
+            self.disk_read_rate = m.get('DiskReadRate')
+        if m.get('DiskWriteRate') is not None:
+            self.disk_write_rate = m.get('DiskWriteRate')
+        if m.get('GPUType') is not None:
+            self.gputype = m.get('GPUType')
+        if m.get('MachineGroupID') is not None:
+            self.machine_group_id = m.get('MachineGroupID')
+        if m.get('NetworkInputRate') is not None:
+            self.network_input_rate = m.get('NetworkInputRate')
+        if m.get('NetworkOutputRate') is not None:
+            self.network_output_rate = m.get('NetworkOutputRate')
+        if m.get('NodeID') is not None:
+            self.node_id = m.get('NodeID')
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('RequestCPU') is not None:
+            self.request_cpu = m.get('RequestCPU')
+        if m.get('RequestGPU') is not None:
+            self.request_gpu = m.get('RequestGPU')
+        if m.get('RequestMemory') is not None:
+            self.request_memory = m.get('RequestMemory')
+        if m.get('TotalCPU') is not None:
+            self.total_cpu = m.get('TotalCPU')
+        if m.get('TotalGPU') is not None:
+            self.total_gpu = m.get('TotalGPU')
+        if m.get('TotalMemory') is not None:
+            self.total_memory = m.get('TotalMemory')
+        if m.get('UserIDs') is not None:
+            self.user_ids = m.get('UserIDs')
+        if m.get('UserNumber') is not None:
+            self.user_number = m.get('UserNumber')
+        return self
+
+
 class UserVpc(TeaModel):
     def __init__(
         self,
         extended_cidrs: List[str] = None,
         role_arn: str = None,
         security_group_id: str = None,
         switch_id: str = None,
```

### Comparing `alibabacloud_paistudio20220112-1.0.8/alibabacloud_paistudio20220112.egg-info/PKG-INFO` & `alibabacloud_paistudio20220112-1.0.9/alibabacloud_paistudio20220112.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-paistudio20220112
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud PaiStudio (20220112) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paistudio20220112-1.0.8/setup.py` & `alibabacloud_paistudio20220112-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_paistudio20220112.
 
-Created on 26/09/2022
+Created on 14/11/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_paistudio20220112"
 NAME = "alibabacloud_paistudio20220112" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PaiStudio (20220112) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.5, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

