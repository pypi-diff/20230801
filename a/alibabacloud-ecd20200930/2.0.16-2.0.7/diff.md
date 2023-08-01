# Comparing `tmp/alibabacloud_ecd20200930-2.0.16.tar.gz` & `tmp/alibabacloud_ecd20200930-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ecd20200930-2.0.16.tar", last modified: Tue Aug  1 03:18:32 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ecd20200930-2.0.7.tar", last modified: Tue Jul 12 07:46:30 2022, max compression
```

## Comparing `alibabacloud_ecd20200930-2.0.16.tar` & `alibabacloud_ecd20200930-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/
--rw-r--r--   0 root         (0) root         (0)      574 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2329 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930/
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930/__init__.py
--rw-r--r--   0 root         (0) root         (0)   865355 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930/client.py
--rw-r--r--   0 root         (0) root         (0)  1488917 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2329 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-01 03:18:32.000000 alibabacloud_ecd20200930-2.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2023-08-01 03:18:31.000000 alibabacloud_ecd20200930-2.0.16/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      233 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   526955 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/client.py
+-rw-r--r--   0 root         (0) root         (0)   865360 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/setup.py
```

### Comparing `alibabacloud_ecd20200930-2.0.16/LICENSE` & `alibabacloud_ecd20200930-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930-2.0.16/PKG-INFO` & `alibabacloud_ecd20200930-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ecd20200930
-Version: 2.0.16
+Version: 2.0.7
 Summary: Alibaba Cloud ecd (20200930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20200930-2.0.16/README-CN.md` & `alibabacloud_ecd20200930-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930-2.0.16/README.md` & `alibabacloud_ecd20200930-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930/client.py` & `alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -111,238 +111,14 @@
     async def activate_office_site_async(
         self,
         request: ecd_20200930_models.ActivateOfficeSiteRequest,
     ) -> ecd_20200930_models.ActivateOfficeSiteResponse:
         runtime = util_models.RuntimeOptions()
         return await self.activate_office_site_with_options_async(request, runtime)
 
-    def add_devices_with_options(
-        self,
-        request: ecd_20200930_models.AddDevicesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.AddDevicesResponse:
-        """
-        You can add only one device to a tenant.
-        
-        @param request: AddDevicesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddDevicesResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_ids):
-            query['DeviceIds'] = request.device_ids
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='AddDevices',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.AddDevicesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def add_devices_with_options_async(
-        self,
-        request: ecd_20200930_models.AddDevicesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.AddDevicesResponse:
-        """
-        You can add only one device to a tenant.
-        
-        @param request: AddDevicesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddDevicesResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_ids):
-            query['DeviceIds'] = request.device_ids
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='AddDevices',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.AddDevicesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def add_devices(
-        self,
-        request: ecd_20200930_models.AddDevicesRequest,
-    ) -> ecd_20200930_models.AddDevicesResponse:
-        """
-        You can add only one device to a tenant.
-        
-        @param request: AddDevicesRequest
-        @return: AddDevicesResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.add_devices_with_options(request, runtime)
-
-    async def add_devices_async(
-        self,
-        request: ecd_20200930_models.AddDevicesRequest,
-    ) -> ecd_20200930_models.AddDevicesResponse:
-        """
-        You can add only one device to a tenant.
-        
-        @param request: AddDevicesRequest
-        @return: AddDevicesResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.add_devices_with_options_async(request, runtime)
-
-    def add_file_permission_with_options(
-        self,
-        tmp_req: ecd_20200930_models.AddFilePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.AddFilePermissionResponse:
-        """
-        You can call this operation to share a specific folder with other users. You can also configure the folder permissions.
-        
-        @param tmp_req: AddFilePermissionRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddFilePermissionResponse
-        """
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.AddFilePermissionShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.member_list):
-            request.member_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.member_list, 'MemberList', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.member_list_shrink):
-            query['MemberList'] = request.member_list_shrink
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='AddFilePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.AddFilePermissionResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def add_file_permission_with_options_async(
-        self,
-        tmp_req: ecd_20200930_models.AddFilePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.AddFilePermissionResponse:
-        """
-        You can call this operation to share a specific folder with other users. You can also configure the folder permissions.
-        
-        @param tmp_req: AddFilePermissionRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddFilePermissionResponse
-        """
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.AddFilePermissionShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.member_list):
-            request.member_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.member_list, 'MemberList', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.member_list_shrink):
-            query['MemberList'] = request.member_list_shrink
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='AddFilePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.AddFilePermissionResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def add_file_permission(
-        self,
-        request: ecd_20200930_models.AddFilePermissionRequest,
-    ) -> ecd_20200930_models.AddFilePermissionResponse:
-        """
-        You can call this operation to share a specific folder with other users. You can also configure the folder permissions.
-        
-        @param request: AddFilePermissionRequest
-        @return: AddFilePermissionResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.add_file_permission_with_options(request, runtime)
-
-    async def add_file_permission_async(
-        self,
-        request: ecd_20200930_models.AddFilePermissionRequest,
-    ) -> ecd_20200930_models.AddFilePermissionResponse:
-        """
-        You can call this operation to share a specific folder with other users. You can also configure the folder permissions.
-        
-        @param request: AddFilePermissionRequest
-        @return: AddFilePermissionResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.add_file_permission_with_options_async(request, runtime)
-
     def add_user_to_desktop_group_with_options(
         self,
         request: ecd_20200930_models.AddUserToDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.AddUserToDesktopGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -421,208 +197,14 @@
     async def add_user_to_desktop_group_async(
         self,
         request: ecd_20200930_models.AddUserToDesktopGroupRequest,
     ) -> ecd_20200930_models.AddUserToDesktopGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.add_user_to_desktop_group_with_options_async(request, runtime)
 
-    def apply_auto_snapshot_policy_with_options(
-        self,
-        request: ecd_20200930_models.ApplyAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ApplyAutoSnapshotPolicyResponse:
-        """
-        You can also associate an automatic snapshot policy with a cloud desktop in the Elastic Desktop Service (EDS) console. To do so, perform the following steps: 1. Log on to the EDS console. 2. Choose Desktops and Groups > Desktops in the left-side navigation pane. 3. Find the cloud desktop that you want to manage on the Cloud Desktops page and choose More > Change Automatic Snapshot Policy in the Actions column. 4. Configure a policy for the cloud desktop as prompted in the Change Automatic Snapshot Policy panel.
-        After you associate an automatic snapshot policy with the cloud desktop, the system creates snapshots for the cloud desktop based on the policy.
-        
-        @param request: ApplyAutoSnapshotPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ApplyAutoSnapshotPolicyResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ApplyAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ApplyAutoSnapshotPolicyResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def apply_auto_snapshot_policy_with_options_async(
-        self,
-        request: ecd_20200930_models.ApplyAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ApplyAutoSnapshotPolicyResponse:
-        """
-        You can also associate an automatic snapshot policy with a cloud desktop in the Elastic Desktop Service (EDS) console. To do so, perform the following steps: 1. Log on to the EDS console. 2. Choose Desktops and Groups > Desktops in the left-side navigation pane. 3. Find the cloud desktop that you want to manage on the Cloud Desktops page and choose More > Change Automatic Snapshot Policy in the Actions column. 4. Configure a policy for the cloud desktop as prompted in the Change Automatic Snapshot Policy panel.
-        After you associate an automatic snapshot policy with the cloud desktop, the system creates snapshots for the cloud desktop based on the policy.
-        
-        @param request: ApplyAutoSnapshotPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ApplyAutoSnapshotPolicyResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ApplyAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ApplyAutoSnapshotPolicyResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def apply_auto_snapshot_policy(
-        self,
-        request: ecd_20200930_models.ApplyAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.ApplyAutoSnapshotPolicyResponse:
-        """
-        You can also associate an automatic snapshot policy with a cloud desktop in the Elastic Desktop Service (EDS) console. To do so, perform the following steps: 1. Log on to the EDS console. 2. Choose Desktops and Groups > Desktops in the left-side navigation pane. 3. Find the cloud desktop that you want to manage on the Cloud Desktops page and choose More > Change Automatic Snapshot Policy in the Actions column. 4. Configure a policy for the cloud desktop as prompted in the Change Automatic Snapshot Policy panel.
-        After you associate an automatic snapshot policy with the cloud desktop, the system creates snapshots for the cloud desktop based on the policy.
-        
-        @param request: ApplyAutoSnapshotPolicyRequest
-        @return: ApplyAutoSnapshotPolicyResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.apply_auto_snapshot_policy_with_options(request, runtime)
-
-    async def apply_auto_snapshot_policy_async(
-        self,
-        request: ecd_20200930_models.ApplyAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.ApplyAutoSnapshotPolicyResponse:
-        """
-        You can also associate an automatic snapshot policy with a cloud desktop in the Elastic Desktop Service (EDS) console. To do so, perform the following steps: 1. Log on to the EDS console. 2. Choose Desktops and Groups > Desktops in the left-side navigation pane. 3. Find the cloud desktop that you want to manage on the Cloud Desktops page and choose More > Change Automatic Snapshot Policy in the Actions column. 4. Configure a policy for the cloud desktop as prompted in the Change Automatic Snapshot Policy panel.
-        After you associate an automatic snapshot policy with the cloud desktop, the system creates snapshots for the cloud desktop based on the policy.
-        
-        @param request: ApplyAutoSnapshotPolicyRequest
-        @return: ApplyAutoSnapshotPolicyResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.apply_auto_snapshot_policy_with_options_async(request, runtime)
-
-    def apply_coordinate_privilege_with_options(
-        self,
-        request: ecd_20200930_models.ApplyCoordinatePrivilegeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ApplyCoordinatePrivilegeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.co_id):
-            query['CoId'] = request.co_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        if not UtilClient.is_unset(request.uuid):
-            query['Uuid'] = request.uuid
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ApplyCoordinatePrivilege',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ApplyCoordinatePrivilegeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def apply_coordinate_privilege_with_options_async(
-        self,
-        request: ecd_20200930_models.ApplyCoordinatePrivilegeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ApplyCoordinatePrivilegeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.co_id):
-            query['CoId'] = request.co_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        if not UtilClient.is_unset(request.uuid):
-            query['Uuid'] = request.uuid
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ApplyCoordinatePrivilege',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ApplyCoordinatePrivilegeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def apply_coordinate_privilege(
-        self,
-        request: ecd_20200930_models.ApplyCoordinatePrivilegeRequest,
-    ) -> ecd_20200930_models.ApplyCoordinatePrivilegeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.apply_coordinate_privilege_with_options(request, runtime)
-
-    async def apply_coordinate_privilege_async(
-        self,
-        request: ecd_20200930_models.ApplyCoordinatePrivilegeRequest,
-    ) -> ecd_20200930_models.ApplyCoordinatePrivilegeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.apply_coordinate_privilege_with_options_async(request, runtime)
-
     def apply_coordination_for_monitoring_with_options(
         self,
         request: ecd_20200930_models.ApplyCoordinationForMonitoringRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ApplyCoordinationForMonitoringResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -866,21 +448,14 @@
         return await self.associate_network_package_with_options_async(request, runtime)
 
     def attach_cen_with_options(
         self,
         request: ecd_20200930_models.AttachCenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.AttachCenResponse:
-        """
-        The ID of the CEN instance.
-        
-        @param request: AttachCenRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AttachCenResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cen_id):
             query['CenId'] = request.cen_id
         if not UtilClient.is_unset(request.cen_owner_id):
             query['CenOwnerId'] = request.cen_owner_id
         if not UtilClient.is_unset(request.office_site_id):
@@ -909,21 +484,14 @@
         )
 
     async def attach_cen_with_options_async(
         self,
         request: ecd_20200930_models.AttachCenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.AttachCenResponse:
-        """
-        The ID of the CEN instance.
-        
-        @param request: AttachCenRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AttachCenResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cen_id):
             query['CenId'] = request.cen_id
         if not UtilClient.is_unset(request.cen_owner_id):
             query['CenOwnerId'] = request.cen_owner_id
         if not UtilClient.is_unset(request.office_site_id):
@@ -951,282 +519,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def attach_cen(
         self,
         request: ecd_20200930_models.AttachCenRequest,
     ) -> ecd_20200930_models.AttachCenResponse:
-        """
-        The ID of the CEN instance.
-        
-        @param request: AttachCenRequest
-        @return: AttachCenResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.attach_cen_with_options(request, runtime)
 
     async def attach_cen_async(
         self,
         request: ecd_20200930_models.AttachCenRequest,
     ) -> ecd_20200930_models.AttachCenResponse:
-        """
-        The ID of the CEN instance.
-        
-        @param request: AttachCenRequest
-        @return: AttachCenResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.attach_cen_with_options_async(request, runtime)
 
-    def attach_end_user_with_options(
-        self,
-        request: ecd_20200930_models.AttachEndUserRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.AttachEndUserResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.ad_domain):
-            query['AdDomain'] = request.ad_domain
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_id):
-            query['DeviceId'] = request.device_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='AttachEndUser',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.AttachEndUserResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def attach_end_user_with_options_async(
-        self,
-        request: ecd_20200930_models.AttachEndUserRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.AttachEndUserResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.ad_domain):
-            query['AdDomain'] = request.ad_domain
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_id):
-            query['DeviceId'] = request.device_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='AttachEndUser',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.AttachEndUserResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def attach_end_user(
-        self,
-        request: ecd_20200930_models.AttachEndUserRequest,
-    ) -> ecd_20200930_models.AttachEndUserResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.attach_end_user_with_options(request, runtime)
-
-    async def attach_end_user_async(
-        self,
-        request: ecd_20200930_models.AttachEndUserRequest,
-    ) -> ecd_20200930_models.AttachEndUserResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.attach_end_user_with_options_async(request, runtime)
-
-    def cancel_auto_snapshot_policy_with_options(
-        self,
-        request: ecd_20200930_models.CancelAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CancelAutoSnapshotPolicyResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CancelAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CancelAutoSnapshotPolicyResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def cancel_auto_snapshot_policy_with_options_async(
-        self,
-        request: ecd_20200930_models.CancelAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CancelAutoSnapshotPolicyResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CancelAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CancelAutoSnapshotPolicyResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def cancel_auto_snapshot_policy(
-        self,
-        request: ecd_20200930_models.CancelAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.CancelAutoSnapshotPolicyResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.cancel_auto_snapshot_policy_with_options(request, runtime)
-
-    async def cancel_auto_snapshot_policy_async(
-        self,
-        request: ecd_20200930_models.CancelAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.CancelAutoSnapshotPolicyResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.cancel_auto_snapshot_policy_with_options_async(request, runtime)
-
-    def cancel_cds_file_share_link_with_options(
-        self,
-        request: ecd_20200930_models.CancelCdsFileShareLinkRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CancelCdsFileShareLinkResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.share_id):
-            query['ShareId'] = request.share_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CancelCdsFileShareLink',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CancelCdsFileShareLinkResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def cancel_cds_file_share_link_with_options_async(
-        self,
-        request: ecd_20200930_models.CancelCdsFileShareLinkRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CancelCdsFileShareLinkResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.share_id):
-            query['ShareId'] = request.share_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CancelCdsFileShareLink',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CancelCdsFileShareLinkResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def cancel_cds_file_share_link(
-        self,
-        request: ecd_20200930_models.CancelCdsFileShareLinkRequest,
-    ) -> ecd_20200930_models.CancelCdsFileShareLinkResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.cancel_cds_file_share_link_with_options(request, runtime)
-
-    async def cancel_cds_file_share_link_async(
-        self,
-        request: ecd_20200930_models.CancelCdsFileShareLinkRequest,
-    ) -> ecd_20200930_models.CancelCdsFileShareLinkResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.cancel_cds_file_share_link_with_options_async(request, runtime)
-
     def cancel_coordination_for_monitoring_with_options(
         self,
         request: ecd_20200930_models.CancelCoordinationForMonitoringRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CancelCoordinationForMonitoringResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1453,111 +763,23 @@
     async def clone_policy_group_async(
         self,
         request: ecd_20200930_models.ClonePolicyGroupRequest,
     ) -> ecd_20200930_models.ClonePolicyGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.clone_policy_group_with_options_async(request, runtime)
 
-    def complete_cds_file_with_options(
-        self,
-        request: ecd_20200930_models.CompleteCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CompleteCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.upload_id):
-            query['UploadId'] = request.upload_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CompleteCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CompleteCdsFileResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def complete_cds_file_with_options_async(
-        self,
-        request: ecd_20200930_models.CompleteCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CompleteCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.upload_id):
-            query['UploadId'] = request.upload_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CompleteCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CompleteCdsFileResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def complete_cds_file(
-        self,
-        request: ecd_20200930_models.CompleteCdsFileRequest,
-    ) -> ecd_20200930_models.CompleteCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.complete_cds_file_with_options(request, runtime)
-
-    async def complete_cds_file_async(
-        self,
-        request: ecd_20200930_models.CompleteCdsFileRequest,
-    ) -> ecd_20200930_models.CompleteCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.complete_cds_file_with_options_async(request, runtime)
-
     def config_adconnector_trust_with_options(
         self,
         request: ecd_20200930_models.ConfigADConnectorTrustRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ConfigADConnectorTrustResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.rds_license_domain):
-            query['RdsLicenseDomain'] = request.rds_license_domain
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.trust_key):
             query['TrustKey'] = request.trust_key
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1582,16 +804,14 @@
         request: ecd_20200930_models.ConfigADConnectorTrustRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ConfigADConnectorTrustResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.rds_license_domain):
-            query['RdsLicenseDomain'] = request.rds_license_domain
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.trust_key):
             query['TrustKey'] = request.trust_key
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1707,112 +927,14 @@
     async def config_adconnector_user_async(
         self,
         request: ecd_20200930_models.ConfigADConnectorUserRequest,
     ) -> ecd_20200930_models.ConfigADConnectorUserResponse:
         runtime = util_models.RuntimeOptions()
         return await self.config_adconnector_user_with_options_async(request, runtime)
 
-    def copy_cds_file_with_options(
-        self,
-        request: ecd_20200930_models.CopyCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CopyCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.auto_rename):
-            query['AutoRename'] = request.auto_rename
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.file_receiver_id):
-            query['FileReceiverId'] = request.file_receiver_id
-        if not UtilClient.is_unset(request.file_receiver_type):
-            query['FileReceiverType'] = request.file_receiver_type
-        if not UtilClient.is_unset(request.parent_folder_id):
-            query['ParentFolderId'] = request.parent_folder_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CopyCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CopyCdsFileResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def copy_cds_file_with_options_async(
-        self,
-        request: ecd_20200930_models.CopyCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CopyCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.auto_rename):
-            query['AutoRename'] = request.auto_rename
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.file_receiver_id):
-            query['FileReceiverId'] = request.file_receiver_id
-        if not UtilClient.is_unset(request.file_receiver_type):
-            query['FileReceiverType'] = request.file_receiver_type
-        if not UtilClient.is_unset(request.parent_folder_id):
-            query['ParentFolderId'] = request.parent_folder_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CopyCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CopyCdsFileResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def copy_cds_file(
-        self,
-        request: ecd_20200930_models.CopyCdsFileRequest,
-    ) -> ecd_20200930_models.CopyCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.copy_cds_file_with_options(request, runtime)
-
-    async def copy_cds_file_async(
-        self,
-        request: ecd_20200930_models.CopyCdsFileRequest,
-    ) -> ecd_20200930_models.CopyCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.copy_cds_file_with_options_async(request, runtime)
-
     def copy_image_with_options(
         self,
         request: ecd_20200930_models.CopyImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CopyImageResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1896,21 +1018,14 @@
         return await self.copy_image_with_options_async(request, runtime)
 
     def create_adconnector_directory_with_options(
         self,
         request: ecd_20200930_models.CreateADConnectorDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateADConnectorDirectoryResponse:
-        """
-        The ID of the vSwitch.
-        
-        @param request: CreateADConnectorDirectoryRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateADConnectorDirectoryResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_access_type):
             query['DesktopAccessType'] = request.desktop_access_type
         if not UtilClient.is_unset(request.directory_name):
             query['DirectoryName'] = request.directory_name
         if not UtilClient.is_unset(request.dns_address):
@@ -1955,21 +1070,14 @@
         )
 
     async def create_adconnector_directory_with_options_async(
         self,
         request: ecd_20200930_models.CreateADConnectorDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateADConnectorDirectoryResponse:
-        """
-        The ID of the vSwitch.
-        
-        @param request: CreateADConnectorDirectoryRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateADConnectorDirectoryResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_access_type):
             query['DesktopAccessType'] = request.desktop_access_type
         if not UtilClient.is_unset(request.directory_name):
             query['DirectoryName'] = request.directory_name
         if not UtilClient.is_unset(request.dns_address):
@@ -2013,52 +1121,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_adconnector_directory(
         self,
         request: ecd_20200930_models.CreateADConnectorDirectoryRequest,
     ) -> ecd_20200930_models.CreateADConnectorDirectoryResponse:
-        """
-        The ID of the vSwitch.
-        
-        @param request: CreateADConnectorDirectoryRequest
-        @return: CreateADConnectorDirectoryResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_adconnector_directory_with_options(request, runtime)
 
     async def create_adconnector_directory_async(
         self,
         request: ecd_20200930_models.CreateADConnectorDirectoryRequest,
     ) -> ecd_20200930_models.CreateADConnectorDirectoryResponse:
-        """
-        The ID of the vSwitch.
-        
-        @param request: CreateADConnectorDirectoryRequest
-        @return: CreateADConnectorDirectoryResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_adconnector_directory_with_options_async(request, runtime)
 
     def create_adconnector_office_site_with_options(
         self,
         request: ecd_20200930_models.CreateADConnectorOfficeSiteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateADConnectorOfficeSiteResponse:
-        """
-        When you create a workspace of the enterprise AD account type, AD connectors are automatically created to allow you to connect to enterprise AD systems. You are charged for the AD connectors. For more information, see [Billing overview](~~188395~~).
-        *   After you call this operation to create a workspace of the enterprise AD account type, perform the following steps to configure the AD domain: 1. Configure the conditional forwarder in the Domain Name System (DNS) server. 2. Configure the trust relationship in the AD domain server, and call the [ConfigADConnectorTrust](~~311258~~) operation to configure the trust relationship for the workspace of the enterprise AD account type. 3. Call the [ListUserAdOrganizationUnits](~~311259~~) operation to obtain the organizational unit (OU) details of the AD domain. Then, call the [ConfigADConnectorUser](~~311262~~) operation to specify an OU and an administrator for the workspace of the enterprise AD account type.
-        **\
-        **Note**If you specify DomainUserName and DomainPassword when you create a workspace of the enterprise AD account type, you must configure only the conditional forwarder. If you do not specify DomainUserName or DomainPassword, you must configure the conditional forwarder, trust relationship, and OU.
-        For more information, see [Create a workspace of the enterprise AD account type](~~214469~~).
-        
-        @param request: CreateADConnectorOfficeSiteRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateADConnectorOfficeSiteResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ad_hostname):
             query['AdHostname'] = request.ad_hostname
         if not UtilClient.is_unset(request.bandwidth):
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.cen_id):
@@ -2117,25 +1202,14 @@
         )
 
     async def create_adconnector_office_site_with_options_async(
         self,
         request: ecd_20200930_models.CreateADConnectorOfficeSiteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateADConnectorOfficeSiteResponse:
-        """
-        When you create a workspace of the enterprise AD account type, AD connectors are automatically created to allow you to connect to enterprise AD systems. You are charged for the AD connectors. For more information, see [Billing overview](~~188395~~).
-        *   After you call this operation to create a workspace of the enterprise AD account type, perform the following steps to configure the AD domain: 1. Configure the conditional forwarder in the Domain Name System (DNS) server. 2. Configure the trust relationship in the AD domain server, and call the [ConfigADConnectorTrust](~~311258~~) operation to configure the trust relationship for the workspace of the enterprise AD account type. 3. Call the [ListUserAdOrganizationUnits](~~311259~~) operation to obtain the organizational unit (OU) details of the AD domain. Then, call the [ConfigADConnectorUser](~~311262~~) operation to specify an OU and an administrator for the workspace of the enterprise AD account type.
-        **\
-        **Note**If you specify DomainUserName and DomainPassword when you create a workspace of the enterprise AD account type, you must configure only the conditional forwarder. If you do not specify DomainUserName or DomainPassword, you must configure the conditional forwarder, trust relationship, and OU.
-        For more information, see [Create a workspace of the enterprise AD account type](~~214469~~).
-        
-        @param request: CreateADConnectorOfficeSiteRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateADConnectorOfficeSiteResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ad_hostname):
             query['AdHostname'] = request.ad_hostname
         if not UtilClient.is_unset(request.bandwidth):
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.cen_id):
@@ -2193,267 +1267,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_adconnector_office_site(
         self,
         request: ecd_20200930_models.CreateADConnectorOfficeSiteRequest,
     ) -> ecd_20200930_models.CreateADConnectorOfficeSiteResponse:
-        """
-        When you create a workspace of the enterprise AD account type, AD connectors are automatically created to allow you to connect to enterprise AD systems. You are charged for the AD connectors. For more information, see [Billing overview](~~188395~~).
-        *   After you call this operation to create a workspace of the enterprise AD account type, perform the following steps to configure the AD domain: 1. Configure the conditional forwarder in the Domain Name System (DNS) server. 2. Configure the trust relationship in the AD domain server, and call the [ConfigADConnectorTrust](~~311258~~) operation to configure the trust relationship for the workspace of the enterprise AD account type. 3. Call the [ListUserAdOrganizationUnits](~~311259~~) operation to obtain the organizational unit (OU) details of the AD domain. Then, call the [ConfigADConnectorUser](~~311262~~) operation to specify an OU and an administrator for the workspace of the enterprise AD account type.
-        **\
-        **Note**If you specify DomainUserName and DomainPassword when you create a workspace of the enterprise AD account type, you must configure only the conditional forwarder. If you do not specify DomainUserName or DomainPassword, you must configure the conditional forwarder, trust relationship, and OU.
-        For more information, see [Create a workspace of the enterprise AD account type](~~214469~~).
-        
-        @param request: CreateADConnectorOfficeSiteRequest
-        @return: CreateADConnectorOfficeSiteResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_adconnector_office_site_with_options(request, runtime)
 
     async def create_adconnector_office_site_async(
         self,
         request: ecd_20200930_models.CreateADConnectorOfficeSiteRequest,
     ) -> ecd_20200930_models.CreateADConnectorOfficeSiteResponse:
-        """
-        When you create a workspace of the enterprise AD account type, AD connectors are automatically created to allow you to connect to enterprise AD systems. You are charged for the AD connectors. For more information, see [Billing overview](~~188395~~).
-        *   After you call this operation to create a workspace of the enterprise AD account type, perform the following steps to configure the AD domain: 1. Configure the conditional forwarder in the Domain Name System (DNS) server. 2. Configure the trust relationship in the AD domain server, and call the [ConfigADConnectorTrust](~~311258~~) operation to configure the trust relationship for the workspace of the enterprise AD account type. 3. Call the [ListUserAdOrganizationUnits](~~311259~~) operation to obtain the organizational unit (OU) details of the AD domain. Then, call the [ConfigADConnectorUser](~~311262~~) operation to specify an OU and an administrator for the workspace of the enterprise AD account type.
-        **\
-        **Note**If you specify DomainUserName and DomainPassword when you create a workspace of the enterprise AD account type, you must configure only the conditional forwarder. If you do not specify DomainUserName or DomainPassword, you must configure the conditional forwarder, trust relationship, and OU.
-        For more information, see [Create a workspace of the enterprise AD account type](~~214469~~).
-        
-        @param request: CreateADConnectorOfficeSiteRequest
-        @return: CreateADConnectorOfficeSiteResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_adconnector_office_site_with_options_async(request, runtime)
 
-    def create_and_bind_nas_file_system_with_options(
-        self,
-        request: ecd_20200930_models.CreateAndBindNasFileSystemRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateAndBindNasFileSystemResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.description):
-            query['Description'] = request.description
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.encrypt_type):
-            query['EncryptType'] = request.encrypt_type
-        if not UtilClient.is_unset(request.end_user_ids):
-            query['EndUserIds'] = request.end_user_ids
-        if not UtilClient.is_unset(request.file_system_name):
-            query['FileSystemName'] = request.file_system_name
-        if not UtilClient.is_unset(request.office_site_id):
-            query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.storage_type):
-            query['StorageType'] = request.storage_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateAndBindNasFileSystem',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateAndBindNasFileSystemResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_and_bind_nas_file_system_with_options_async(
-        self,
-        request: ecd_20200930_models.CreateAndBindNasFileSystemRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateAndBindNasFileSystemResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.description):
-            query['Description'] = request.description
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.encrypt_type):
-            query['EncryptType'] = request.encrypt_type
-        if not UtilClient.is_unset(request.end_user_ids):
-            query['EndUserIds'] = request.end_user_ids
-        if not UtilClient.is_unset(request.file_system_name):
-            query['FileSystemName'] = request.file_system_name
-        if not UtilClient.is_unset(request.office_site_id):
-            query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.storage_type):
-            query['StorageType'] = request.storage_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateAndBindNasFileSystem',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateAndBindNasFileSystemResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_and_bind_nas_file_system(
-        self,
-        request: ecd_20200930_models.CreateAndBindNasFileSystemRequest,
-    ) -> ecd_20200930_models.CreateAndBindNasFileSystemResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.create_and_bind_nas_file_system_with_options(request, runtime)
-
-    async def create_and_bind_nas_file_system_async(
-        self,
-        request: ecd_20200930_models.CreateAndBindNasFileSystemRequest,
-    ) -> ecd_20200930_models.CreateAndBindNasFileSystemResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.create_and_bind_nas_file_system_with_options_async(request, runtime)
-
-    def create_auto_snapshot_policy_with_options(
-        self,
-        request: ecd_20200930_models.CreateAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateAutoSnapshotPolicyResponse:
-        """
-        You can call the operation to create an automatic snapshot policy based on a CRON expression. Then, the system automatically creates snapshots of a cloud desktop based on the policy.
-        
-        @param request: CreateAutoSnapshotPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateAutoSnapshotPolicyResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cron_expression):
-            query['CronExpression'] = request.cron_expression
-        if not UtilClient.is_unset(request.policy_name):
-            query['PolicyName'] = request.policy_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.retention_days):
-            query['RetentionDays'] = request.retention_days
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateAutoSnapshotPolicyResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_auto_snapshot_policy_with_options_async(
-        self,
-        request: ecd_20200930_models.CreateAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateAutoSnapshotPolicyResponse:
-        """
-        You can call the operation to create an automatic snapshot policy based on a CRON expression. Then, the system automatically creates snapshots of a cloud desktop based on the policy.
-        
-        @param request: CreateAutoSnapshotPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateAutoSnapshotPolicyResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cron_expression):
-            query['CronExpression'] = request.cron_expression
-        if not UtilClient.is_unset(request.policy_name):
-            query['PolicyName'] = request.policy_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.retention_days):
-            query['RetentionDays'] = request.retention_days
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateAutoSnapshotPolicyResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_auto_snapshot_policy(
-        self,
-        request: ecd_20200930_models.CreateAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.CreateAutoSnapshotPolicyResponse:
-        """
-        You can call the operation to create an automatic snapshot policy based on a CRON expression. Then, the system automatically creates snapshots of a cloud desktop based on the policy.
-        
-        @param request: CreateAutoSnapshotPolicyRequest
-        @return: CreateAutoSnapshotPolicyResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.create_auto_snapshot_policy_with_options(request, runtime)
-
-    async def create_auto_snapshot_policy_async(
-        self,
-        request: ecd_20200930_models.CreateAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.CreateAutoSnapshotPolicyResponse:
-        """
-        You can call the operation to create an automatic snapshot policy based on a CRON expression. Then, the system automatically creates snapshots of a cloud desktop based on the policy.
-        
-        @param request: CreateAutoSnapshotPolicyRequest
-        @return: CreateAutoSnapshotPolicyResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.create_auto_snapshot_policy_with_options_async(request, runtime)
-
     def create_bundle_with_options(
         self,
         request: ecd_20200930_models.CreateBundleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateBundleResponse:
-        """
-        The PL of the data disk. If the cloud desktop type is Graphics or High Frequency, you can set the PL of the data disk. Valid values:
-        *   PL0
-        *   PL1
-        *   PL2
-        *   PL3
-        For more information about the differences between disks at different PLs, see [Enhanced SSDs](~~122389~~).
-        
-        @param request: CreateBundleRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateBundleResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.bundle_name):
             query['BundleName'] = request.bundle_name
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.desktop_type):
@@ -2492,26 +1328,14 @@
         )
 
     async def create_bundle_with_options_async(
         self,
         request: ecd_20200930_models.CreateBundleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateBundleResponse:
-        """
-        The PL of the data disk. If the cloud desktop type is Graphics or High Frequency, you can set the PL of the data disk. Valid values:
-        *   PL0
-        *   PL1
-        *   PL2
-        *   PL3
-        For more information about the differences between disks at different PLs, see [Enhanced SSDs](~~122389~~).
-        
-        @param request: CreateBundleRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateBundleResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.bundle_name):
             query['BundleName'] = request.bundle_name
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.desktop_type):
@@ -2549,431 +1373,59 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_bundle(
         self,
         request: ecd_20200930_models.CreateBundleRequest,
     ) -> ecd_20200930_models.CreateBundleResponse:
-        """
-        The PL of the data disk. If the cloud desktop type is Graphics or High Frequency, you can set the PL of the data disk. Valid values:
-        *   PL0
-        *   PL1
-        *   PL2
-        *   PL3
-        For more information about the differences between disks at different PLs, see [Enhanced SSDs](~~122389~~).
-        
-        @param request: CreateBundleRequest
-        @return: CreateBundleResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_bundle_with_options(request, runtime)
 
     async def create_bundle_async(
         self,
         request: ecd_20200930_models.CreateBundleRequest,
     ) -> ecd_20200930_models.CreateBundleResponse:
-        """
-        The PL of the data disk. If the cloud desktop type is Graphics or High Frequency, you can set the PL of the data disk. Valid values:
-        *   PL0
-        *   PL1
-        *   PL2
-        *   PL3
-        For more information about the differences between disks at different PLs, see [Enhanced SSDs](~~122389~~).
-        
-        @param request: CreateBundleRequest
-        @return: CreateBundleResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_bundle_with_options_async(request, runtime)
 
-    def create_cds_file_with_options(
-        self,
-        request: ecd_20200930_models.CreateCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateCdsFileResponse:
-        """
-        After the RAM permissions are authenticated, you can call the CreateCdsFile operation to obtain the upload URL of a file and upload the file to a cloud disk.
-        
-        @param request: CreateCdsFileRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateCdsFileResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.conflict_policy):
-            query['ConflictPolicy'] = request.conflict_policy
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_hash):
-            query['FileHash'] = request.file_hash
-        if not UtilClient.is_unset(request.file_length):
-            query['FileLength'] = request.file_length
-        if not UtilClient.is_unset(request.file_name):
-            query['FileName'] = request.file_name
-        if not UtilClient.is_unset(request.file_type):
-            query['FileType'] = request.file_type
-        if not UtilClient.is_unset(request.parent_file_id):
-            query['ParentFileId'] = request.parent_file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateCdsFileResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_cds_file_with_options_async(
-        self,
-        request: ecd_20200930_models.CreateCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateCdsFileResponse:
-        """
-        After the RAM permissions are authenticated, you can call the CreateCdsFile operation to obtain the upload URL of a file and upload the file to a cloud disk.
-        
-        @param request: CreateCdsFileRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateCdsFileResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.conflict_policy):
-            query['ConflictPolicy'] = request.conflict_policy
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_hash):
-            query['FileHash'] = request.file_hash
-        if not UtilClient.is_unset(request.file_length):
-            query['FileLength'] = request.file_length
-        if not UtilClient.is_unset(request.file_name):
-            query['FileName'] = request.file_name
-        if not UtilClient.is_unset(request.file_type):
-            query['FileType'] = request.file_type
-        if not UtilClient.is_unset(request.parent_file_id):
-            query['ParentFileId'] = request.parent_file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateCdsFileResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_cds_file(
-        self,
-        request: ecd_20200930_models.CreateCdsFileRequest,
-    ) -> ecd_20200930_models.CreateCdsFileResponse:
-        """
-        After the RAM permissions are authenticated, you can call the CreateCdsFile operation to obtain the upload URL of a file and upload the file to a cloud disk.
-        
-        @param request: CreateCdsFileRequest
-        @return: CreateCdsFileResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.create_cds_file_with_options(request, runtime)
-
-    async def create_cds_file_async(
-        self,
-        request: ecd_20200930_models.CreateCdsFileRequest,
-    ) -> ecd_20200930_models.CreateCdsFileResponse:
-        """
-        After the RAM permissions are authenticated, you can call the CreateCdsFile operation to obtain the upload URL of a file and upload the file to a cloud disk.
-        
-        @param request: CreateCdsFileRequest
-        @return: CreateCdsFileResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.create_cds_file_with_options_async(request, runtime)
-
-    def create_cds_file_share_link_with_options(
-        self,
-        request: ecd_20200930_models.CreateCdsFileShareLinkRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateCdsFileShareLinkResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.description):
-            query['Description'] = request.description
-        if not UtilClient.is_unset(request.disable_download):
-            query['DisableDownload'] = request.disable_download
-        if not UtilClient.is_unset(request.disable_preview):
-            query['DisablePreview'] = request.disable_preview
-        if not UtilClient.is_unset(request.disable_save):
-            query['DisableSave'] = request.disable_save
-        if not UtilClient.is_unset(request.download_limit):
-            query['DownloadLimit'] = request.download_limit
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.expiration):
-            query['Expiration'] = request.expiration
-        if not UtilClient.is_unset(request.file_ids):
-            query['FileIds'] = request.file_ids
-        if not UtilClient.is_unset(request.preview_limit):
-            query['PreviewLimit'] = request.preview_limit
-        if not UtilClient.is_unset(request.save_limit):
-            query['SaveLimit'] = request.save_limit
-        if not UtilClient.is_unset(request.share_name):
-            query['ShareName'] = request.share_name
-        if not UtilClient.is_unset(request.share_pwd):
-            query['SharePwd'] = request.share_pwd
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateCdsFileShareLink',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateCdsFileShareLinkResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_cds_file_share_link_with_options_async(
-        self,
-        request: ecd_20200930_models.CreateCdsFileShareLinkRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateCdsFileShareLinkResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.description):
-            query['Description'] = request.description
-        if not UtilClient.is_unset(request.disable_download):
-            query['DisableDownload'] = request.disable_download
-        if not UtilClient.is_unset(request.disable_preview):
-            query['DisablePreview'] = request.disable_preview
-        if not UtilClient.is_unset(request.disable_save):
-            query['DisableSave'] = request.disable_save
-        if not UtilClient.is_unset(request.download_limit):
-            query['DownloadLimit'] = request.download_limit
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.expiration):
-            query['Expiration'] = request.expiration
-        if not UtilClient.is_unset(request.file_ids):
-            query['FileIds'] = request.file_ids
-        if not UtilClient.is_unset(request.preview_limit):
-            query['PreviewLimit'] = request.preview_limit
-        if not UtilClient.is_unset(request.save_limit):
-            query['SaveLimit'] = request.save_limit
-        if not UtilClient.is_unset(request.share_name):
-            query['ShareName'] = request.share_name
-        if not UtilClient.is_unset(request.share_pwd):
-            query['SharePwd'] = request.share_pwd
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateCdsFileShareLink',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateCdsFileShareLinkResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_cds_file_share_link(
-        self,
-        request: ecd_20200930_models.CreateCdsFileShareLinkRequest,
-    ) -> ecd_20200930_models.CreateCdsFileShareLinkResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.create_cds_file_share_link_with_options(request, runtime)
-
-    async def create_cds_file_share_link_async(
-        self,
-        request: ecd_20200930_models.CreateCdsFileShareLinkRequest,
-    ) -> ecd_20200930_models.CreateCdsFileShareLinkResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.create_cds_file_share_link_with_options_async(request, runtime)
-
-    def create_cloud_drive_users_with_options(
-        self,
-        request: ecd_20200930_models.CreateCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_max_size):
-            query['UserMaxSize'] = request.user_max_size
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateCloudDriveUsersResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_cloud_drive_users_with_options_async(
-        self,
-        request: ecd_20200930_models.CreateCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.CreateCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_max_size):
-            query['UserMaxSize'] = request.user_max_size
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.CreateCloudDriveUsersResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_cloud_drive_users(
-        self,
-        request: ecd_20200930_models.CreateCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.CreateCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.create_cloud_drive_users_with_options(request, runtime)
-
-    async def create_cloud_drive_users_async(
-        self,
-        request: ecd_20200930_models.CreateCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.CreateCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.create_cloud_drive_users_with_options_async(request, runtime)
-
     def create_desktop_group_with_options(
         self,
         request: ecd_20200930_models.CreateDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateDesktopGroupResponse:
-        """
-        # Description
-        Before you call this operation to create a desktop group, make sure that the following operations are complete:
-        *   You are familiar with the features, usage limits, and scaling policies of desktop groups. For more information, see [Overview](~~290959~~) of desktop groups.
-        *   Resources, such as workspaces, users, desktop templates, and policies, are created.
-        
-        @param request: CreateDesktopGroupRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateDesktopGroupResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all_classify_users):
             query['AllClassifyUsers'] = request.all_classify_users
         if not UtilClient.is_unset(request.allow_auto_setup):
             query['AllowAutoSetup'] = request.allow_auto_setup
         if not UtilClient.is_unset(request.allow_buffer_count):
             query['AllowBufferCount'] = request.allow_buffer_count
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
-        if not UtilClient.is_unset(request.auto_renew):
-            query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.bind_amount):
             query['BindAmount'] = request.bind_amount
         if not UtilClient.is_unset(request.bundle_id):
             query['BundleId'] = request.bundle_id
-        if not UtilClient.is_unset(request.buy_desktops_count):
-            query['BuyDesktopsCount'] = request.buy_desktops_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.classify):
             query['Classify'] = request.classify
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.comments):
             query['Comments'] = request.comments
-        if not UtilClient.is_unset(request.connect_duration):
-            query['ConnectDuration'] = request.connect_duration
         if not UtilClient.is_unset(request.default_init_desktop_count):
             query['DefaultInitDesktopCount'] = request.default_init_desktop_count
         if not UtilClient.is_unset(request.desktop_group_name):
             query['DesktopGroupName'] = request.desktop_group_name
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_user_ids):
             query['EndUserIds'] = request.end_user_ids
-        if not UtilClient.is_unset(request.file_system_id):
-            query['FileSystemId'] = request.file_system_id
-        if not UtilClient.is_unset(request.group_version):
-            query['GroupVersion'] = request.group_version
-        if not UtilClient.is_unset(request.idle_disconnect_duration):
-            query['IdleDisconnectDuration'] = request.idle_disconnect_duration
         if not UtilClient.is_unset(request.keep_duration):
             query['KeepDuration'] = request.keep_duration
         if not UtilClient.is_unset(request.load_policy):
             query['LoadPolicy'] = request.load_policy
         if not UtilClient.is_unset(request.max_desktops_count):
             query['MaxDesktopsCount'] = request.max_desktops_count
         if not UtilClient.is_unset(request.min_desktops_count):
@@ -2984,26 +1436,20 @@
             query['OwnType'] = request.own_type
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.profile_follow_switch):
-            query['ProfileFollowSwitch'] = request.profile_follow_switch
-        if not UtilClient.is_unset(request.ratio_threshold):
-            query['RatioThreshold'] = request.ratio_threshold
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.reset_type):
             query['ResetType'] = request.reset_type
         if not UtilClient.is_unset(request.scale_strategy_id):
             query['ScaleStrategyId'] = request.scale_strategy_id
-        if not UtilClient.is_unset(request.stop_duration):
-            query['StopDuration'] = request.stop_duration
         if not UtilClient.is_unset(request.volume_encryption_enabled):
             query['VolumeEncryptionEnabled'] = request.volume_encryption_enabled
         if not UtilClient.is_unset(request.volume_encryption_key):
             query['VolumeEncryptionKey'] = request.volume_encryption_key
         if not UtilClient.is_unset(request.vpc_id):
             query['VpcId'] = request.vpc_id
         req = open_api_models.OpenApiRequest(
@@ -3026,66 +1472,44 @@
         )
 
     async def create_desktop_group_with_options_async(
         self,
         request: ecd_20200930_models.CreateDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateDesktopGroupResponse:
-        """
-        # Description
-        Before you call this operation to create a desktop group, make sure that the following operations are complete:
-        *   You are familiar with the features, usage limits, and scaling policies of desktop groups. For more information, see [Overview](~~290959~~) of desktop groups.
-        *   Resources, such as workspaces, users, desktop templates, and policies, are created.
-        
-        @param request: CreateDesktopGroupRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateDesktopGroupResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all_classify_users):
             query['AllClassifyUsers'] = request.all_classify_users
         if not UtilClient.is_unset(request.allow_auto_setup):
             query['AllowAutoSetup'] = request.allow_auto_setup
         if not UtilClient.is_unset(request.allow_buffer_count):
             query['AllowBufferCount'] = request.allow_buffer_count
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
-        if not UtilClient.is_unset(request.auto_renew):
-            query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.bind_amount):
             query['BindAmount'] = request.bind_amount
         if not UtilClient.is_unset(request.bundle_id):
             query['BundleId'] = request.bundle_id
-        if not UtilClient.is_unset(request.buy_desktops_count):
-            query['BuyDesktopsCount'] = request.buy_desktops_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.classify):
             query['Classify'] = request.classify
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.comments):
             query['Comments'] = request.comments
-        if not UtilClient.is_unset(request.connect_duration):
-            query['ConnectDuration'] = request.connect_duration
         if not UtilClient.is_unset(request.default_init_desktop_count):
             query['DefaultInitDesktopCount'] = request.default_init_desktop_count
         if not UtilClient.is_unset(request.desktop_group_name):
             query['DesktopGroupName'] = request.desktop_group_name
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_user_ids):
             query['EndUserIds'] = request.end_user_ids
-        if not UtilClient.is_unset(request.file_system_id):
-            query['FileSystemId'] = request.file_system_id
-        if not UtilClient.is_unset(request.group_version):
-            query['GroupVersion'] = request.group_version
-        if not UtilClient.is_unset(request.idle_disconnect_duration):
-            query['IdleDisconnectDuration'] = request.idle_disconnect_duration
         if not UtilClient.is_unset(request.keep_duration):
             query['KeepDuration'] = request.keep_duration
         if not UtilClient.is_unset(request.load_policy):
             query['LoadPolicy'] = request.load_policy
         if not UtilClient.is_unset(request.max_desktops_count):
             query['MaxDesktopsCount'] = request.max_desktops_count
         if not UtilClient.is_unset(request.min_desktops_count):
@@ -3096,26 +1520,20 @@
             query['OwnType'] = request.own_type
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.profile_follow_switch):
-            query['ProfileFollowSwitch'] = request.profile_follow_switch
-        if not UtilClient.is_unset(request.ratio_threshold):
-            query['RatioThreshold'] = request.ratio_threshold
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.reset_type):
             query['ResetType'] = request.reset_type
         if not UtilClient.is_unset(request.scale_strategy_id):
             query['ScaleStrategyId'] = request.scale_strategy_id
-        if not UtilClient.is_unset(request.stop_duration):
-            query['StopDuration'] = request.stop_duration
         if not UtilClient.is_unset(request.volume_encryption_enabled):
             query['VolumeEncryptionEnabled'] = request.volume_encryption_enabled
         if not UtilClient.is_unset(request.volume_encryption_key):
             query['VolumeEncryptionKey'] = request.volume_encryption_key
         if not UtilClient.is_unset(request.vpc_id):
             query['VpcId'] = request.vpc_id
         req = open_api_models.OpenApiRequest(
@@ -3137,80 +1555,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_desktop_group(
         self,
         request: ecd_20200930_models.CreateDesktopGroupRequest,
     ) -> ecd_20200930_models.CreateDesktopGroupResponse:
-        """
-        # Description
-        Before you call this operation to create a desktop group, make sure that the following operations are complete:
-        *   You are familiar with the features, usage limits, and scaling policies of desktop groups. For more information, see [Overview](~~290959~~) of desktop groups.
-        *   Resources, such as workspaces, users, desktop templates, and policies, are created.
-        
-        @param request: CreateDesktopGroupRequest
-        @return: CreateDesktopGroupResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_desktop_group_with_options(request, runtime)
 
     async def create_desktop_group_async(
         self,
         request: ecd_20200930_models.CreateDesktopGroupRequest,
     ) -> ecd_20200930_models.CreateDesktopGroupResponse:
-        """
-        # Description
-        Before you call this operation to create a desktop group, make sure that the following operations are complete:
-        *   You are familiar with the features, usage limits, and scaling policies of desktop groups. For more information, see [Overview](~~290959~~) of desktop groups.
-        *   Resources, such as workspaces, users, desktop templates, and policies, are created.
-        
-        @param request: CreateDesktopGroupRequest
-        @return: CreateDesktopGroupResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_desktop_group_with_options_async(request, runtime)
 
     def create_desktops_with_options(
         self,
         request: ecd_20200930_models.CreateDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateDesktopsResponse:
-        """
-        1\\. Before you create a cloud desktop in Elastic Desktop Service (EDS), make sure that the following operations are complete:
-        *   A workspace and a user are created. For more information, see the following topics:
-        *   Create a workspace of the convenience account type and a convenience user: [CreateSimpleOfficeSite](~~215416~~) and [Create a convenience user](~~214472~~)
-        *   Create a workspace of the enterprise Active Directory (AD) account type and an enterprise AD user: [CreateADConnectorOfficeSite](~~215417~~) and [Create an enterprise AD user](~~188619~~)
-        *   A cloud desktop template is created by calling the [CreateBundle](~~188883~~) operation, or an existing cloud desktop template is used.
-        *   A policy is created by calling the [CreatePolicyGroup](~~188889~~) operation, or an existing policy is used.
-        2\\. A custom command script that can be automatically executed after you create the cloud desktop is prepared. You can customize a command script by using the UserCommands parameter.
-        
-        @param request: CreateDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.amount):
             query['Amount'] = request.amount
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.auto_renew):
             query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.bundle_id):
             query['BundleId'] = request.bundle_id
-        if not UtilClient.is_unset(request.bundle_models):
-            query['BundleModels'] = request.bundle_models
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.desktop_name):
             query['DesktopName'] = request.desktop_name
         if not UtilClient.is_unset(request.desktop_name_suffix):
             query['DesktopNameSuffix'] = request.desktop_name_suffix
-        if not UtilClient.is_unset(request.desktop_timers):
-            query['DesktopTimers'] = request.desktop_timers
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.hostname):
@@ -3227,16 +1610,14 @@
             query['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.user_assign_mode):
             query['UserAssignMode'] = request.user_assign_mode
-        if not UtilClient.is_unset(request.user_commands):
-            query['UserCommands'] = request.user_commands
         if not UtilClient.is_unset(request.user_name):
             query['UserName'] = request.user_name
         if not UtilClient.is_unset(request.volume_encryption_enabled):
             query['VolumeEncryptionEnabled'] = request.volume_encryption_enabled
         if not UtilClient.is_unset(request.volume_encryption_key):
             query['VolumeEncryptionKey'] = request.volume_encryption_key
         if not UtilClient.is_unset(request.vpc_id):
@@ -3261,47 +1642,30 @@
         )
 
     async def create_desktops_with_options_async(
         self,
         request: ecd_20200930_models.CreateDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateDesktopsResponse:
-        """
-        1\\. Before you create a cloud desktop in Elastic Desktop Service (EDS), make sure that the following operations are complete:
-        *   A workspace and a user are created. For more information, see the following topics:
-        *   Create a workspace of the convenience account type and a convenience user: [CreateSimpleOfficeSite](~~215416~~) and [Create a convenience user](~~214472~~)
-        *   Create a workspace of the enterprise Active Directory (AD) account type and an enterprise AD user: [CreateADConnectorOfficeSite](~~215417~~) and [Create an enterprise AD user](~~188619~~)
-        *   A cloud desktop template is created by calling the [CreateBundle](~~188883~~) operation, or an existing cloud desktop template is used.
-        *   A policy is created by calling the [CreatePolicyGroup](~~188889~~) operation, or an existing policy is used.
-        2\\. A custom command script that can be automatically executed after you create the cloud desktop is prepared. You can customize a command script by using the UserCommands parameter.
-        
-        @param request: CreateDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.amount):
             query['Amount'] = request.amount
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.auto_renew):
             query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.bundle_id):
             query['BundleId'] = request.bundle_id
-        if not UtilClient.is_unset(request.bundle_models):
-            query['BundleModels'] = request.bundle_models
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.desktop_name):
             query['DesktopName'] = request.desktop_name
         if not UtilClient.is_unset(request.desktop_name_suffix):
             query['DesktopNameSuffix'] = request.desktop_name_suffix
-        if not UtilClient.is_unset(request.desktop_timers):
-            query['DesktopTimers'] = request.desktop_timers
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.hostname):
@@ -3318,16 +1682,14 @@
             query['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.user_assign_mode):
             query['UserAssignMode'] = request.user_assign_mode
-        if not UtilClient.is_unset(request.user_commands):
-            query['UserCommands'] = request.user_commands
         if not UtilClient.is_unset(request.user_name):
             query['UserName'] = request.user_name
         if not UtilClient.is_unset(request.volume_encryption_enabled):
             query['VolumeEncryptionEnabled'] = request.volume_encryption_enabled
         if not UtilClient.is_unset(request.volume_encryption_key):
             query['VolumeEncryptionKey'] = request.volume_encryption_key
         if not UtilClient.is_unset(request.vpc_id):
@@ -3351,45 +1713,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_desktops(
         self,
         request: ecd_20200930_models.CreateDesktopsRequest,
     ) -> ecd_20200930_models.CreateDesktopsResponse:
-        """
-        1\\. Before you create a cloud desktop in Elastic Desktop Service (EDS), make sure that the following operations are complete:
-        *   A workspace and a user are created. For more information, see the following topics:
-        *   Create a workspace of the convenience account type and a convenience user: [CreateSimpleOfficeSite](~~215416~~) and [Create a convenience user](~~214472~~)
-        *   Create a workspace of the enterprise Active Directory (AD) account type and an enterprise AD user: [CreateADConnectorOfficeSite](~~215417~~) and [Create an enterprise AD user](~~188619~~)
-        *   A cloud desktop template is created by calling the [CreateBundle](~~188883~~) operation, or an existing cloud desktop template is used.
-        *   A policy is created by calling the [CreatePolicyGroup](~~188889~~) operation, or an existing policy is used.
-        2\\. A custom command script that can be automatically executed after you create the cloud desktop is prepared. You can customize a command script by using the UserCommands parameter.
-        
-        @param request: CreateDesktopsRequest
-        @return: CreateDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_desktops_with_options(request, runtime)
 
     async def create_desktops_async(
         self,
         request: ecd_20200930_models.CreateDesktopsRequest,
     ) -> ecd_20200930_models.CreateDesktopsResponse:
-        """
-        1\\. Before you create a cloud desktop in Elastic Desktop Service (EDS), make sure that the following operations are complete:
-        *   A workspace and a user are created. For more information, see the following topics:
-        *   Create a workspace of the convenience account type and a convenience user: [CreateSimpleOfficeSite](~~215416~~) and [Create a convenience user](~~214472~~)
-        *   Create a workspace of the enterprise Active Directory (AD) account type and an enterprise AD user: [CreateADConnectorOfficeSite](~~215417~~) and [Create an enterprise AD user](~~188619~~)
-        *   A cloud desktop template is created by calling the [CreateBundle](~~188883~~) operation, or an existing cloud desktop template is used.
-        *   A policy is created by calling the [CreatePolicyGroup](~~188889~~) operation, or an existing policy is used.
-        2\\. A custom command script that can be automatically executed after you create the cloud desktop is prepared. You can customize a command script by using the UserCommands parameter.
-        
-        @param request: CreateDesktopsRequest
-        @return: CreateDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_desktops_with_options_async(request, runtime)
 
     def create_disk_encryption_service_with_options(
         self,
         request: ecd_20200930_models.CreateDiskEncryptionServiceRequest,
         runtime: util_models.RuntimeOptions,
@@ -3664,16 +2002,14 @@
             query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.bandwidth):
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.internet_charge_type):
             query['InternetChargeType'] = request.internet_charge_type
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.pay_type):
-            query['PayType'] = request.pay_type
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.promotion_id):
             query['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.region_id):
@@ -3710,16 +2046,14 @@
             query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.bandwidth):
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.internet_charge_type):
             query['InternetChargeType'] = request.internet_charge_type
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.pay_type):
-            query['PayType'] = request.pay_type
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.promotion_id):
             query['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.region_id):
@@ -3758,115 +2092,66 @@
         return await self.create_network_package_with_options_async(request, runtime)
 
     def create_policy_group_with_options(
         self,
         request: ecd_20200930_models.CreatePolicyGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreatePolicyGroupResponse:
-        """
-        A policy is a set of security rules that are used to control security configurations when end users use cloud desktops. A policy contains basic features, such as USB redirection and watermarking, and other features, such as security group control. For more information, see [Policy overview](~~189345~~).
-        
-        @param request: CreatePolicyGroupRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreatePolicyGroupResponse
-        """
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.app_content_protection):
-            query['AppContentProtection'] = request.app_content_protection
         if not UtilClient.is_unset(request.authorize_access_policy_rule):
             query['AuthorizeAccessPolicyRule'] = request.authorize_access_policy_rule
         if not UtilClient.is_unset(request.authorize_security_policy_rule):
             query['AuthorizeSecurityPolicyRule'] = request.authorize_security_policy_rule
         if not UtilClient.is_unset(request.camera_redirect):
             query['CameraRedirect'] = request.camera_redirect
         if not UtilClient.is_unset(request.client_type):
             query['ClientType'] = request.client_type
         if not UtilClient.is_unset(request.clipboard):
             query['Clipboard'] = request.clipboard
         if not UtilClient.is_unset(request.domain_list):
             query['DomainList'] = request.domain_list
-        if not UtilClient.is_unset(request.domain_resolve_rule):
-            query['DomainResolveRule'] = request.domain_resolve_rule
-        if not UtilClient.is_unset(request.domain_resolve_rule_type):
-            query['DomainResolveRuleType'] = request.domain_resolve_rule_type
-        if not UtilClient.is_unset(request.end_user_apply_admin_coordinate):
-            query['EndUserApplyAdminCoordinate'] = request.end_user_apply_admin_coordinate
-        if not UtilClient.is_unset(request.end_user_group_coordinate):
-            query['EndUserGroupCoordinate'] = request.end_user_group_coordinate
         if not UtilClient.is_unset(request.gpu_acceleration):
             query['GpuAcceleration'] = request.gpu_acceleration
         if not UtilClient.is_unset(request.html_5access):
             query['Html5Access'] = request.html_5access
         if not UtilClient.is_unset(request.html_5file_transfer):
             query['Html5FileTransfer'] = request.html_5file_transfer
-        if not UtilClient.is_unset(request.internet_communication_protocol):
-            query['InternetCommunicationProtocol'] = request.internet_communication_protocol
         if not UtilClient.is_unset(request.local_drive):
             query['LocalDrive'] = request.local_drive
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.net_redirect):
             query['NetRedirect'] = request.net_redirect
         if not UtilClient.is_unset(request.preempt_login):
             query['PreemptLogin'] = request.preempt_login
         if not UtilClient.is_unset(request.preempt_login_user):
             query['PreemptLoginUser'] = request.preempt_login_user
         if not UtilClient.is_unset(request.printer_redirection):
             query['PrinterRedirection'] = request.printer_redirection
-        if not UtilClient.is_unset(request.record_content):
-            query['RecordContent'] = request.record_content
-        if not UtilClient.is_unset(request.record_content_expires):
-            query['RecordContentExpires'] = request.record_content_expires
         if not UtilClient.is_unset(request.recording):
             query['Recording'] = request.recording
-        if not UtilClient.is_unset(request.recording_audio):
-            query['RecordingAudio'] = request.recording_audio
-        if not UtilClient.is_unset(request.recording_duration):
-            query['RecordingDuration'] = request.recording_duration
         if not UtilClient.is_unset(request.recording_end_time):
             query['RecordingEndTime'] = request.recording_end_time
-        if not UtilClient.is_unset(request.recording_expires):
-            query['RecordingExpires'] = request.recording_expires
         if not UtilClient.is_unset(request.recording_fps):
             query['RecordingFps'] = request.recording_fps
         if not UtilClient.is_unset(request.recording_start_time):
             query['RecordingStartTime'] = request.recording_start_time
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.remote_coordinate):
-            query['RemoteCoordinate'] = request.remote_coordinate
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
-        if not UtilClient.is_unset(request.scope_value):
-            query['ScopeValue'] = request.scope_value
         if not UtilClient.is_unset(request.usb_redirect):
             query['UsbRedirect'] = request.usb_redirect
         if not UtilClient.is_unset(request.usb_supply_redirect_rule):
             query['UsbSupplyRedirectRule'] = request.usb_supply_redirect_rule
-        if not UtilClient.is_unset(request.video_redirect):
-            query['VideoRedirect'] = request.video_redirect
         if not UtilClient.is_unset(request.visual_quality):
             query['VisualQuality'] = request.visual_quality
         if not UtilClient.is_unset(request.watermark):
             query['Watermark'] = request.watermark
-        if not UtilClient.is_unset(request.watermark_color):
-            query['WatermarkColor'] = request.watermark_color
-        if not UtilClient.is_unset(request.watermark_degree):
-            query['WatermarkDegree'] = request.watermark_degree
-        if not UtilClient.is_unset(request.watermark_font_size):
-            query['WatermarkFontSize'] = request.watermark_font_size
-        if not UtilClient.is_unset(request.watermark_font_style):
-            query['WatermarkFontStyle'] = request.watermark_font_style
-        if not UtilClient.is_unset(request.watermark_row_amount):
-            query['WatermarkRowAmount'] = request.watermark_row_amount
         if not UtilClient.is_unset(request.watermark_transparency):
             query['WatermarkTransparency'] = request.watermark_transparency
-        if not UtilClient.is_unset(request.watermark_transparency_value):
-            query['WatermarkTransparencyValue'] = request.watermark_transparency_value
         if not UtilClient.is_unset(request.watermark_type):
             query['WatermarkType'] = request.watermark_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePolicyGroup',
@@ -3885,115 +2170,66 @@
         )
 
     async def create_policy_group_with_options_async(
         self,
         request: ecd_20200930_models.CreatePolicyGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreatePolicyGroupResponse:
-        """
-        A policy is a set of security rules that are used to control security configurations when end users use cloud desktops. A policy contains basic features, such as USB redirection and watermarking, and other features, such as security group control. For more information, see [Policy overview](~~189345~~).
-        
-        @param request: CreatePolicyGroupRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreatePolicyGroupResponse
-        """
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.app_content_protection):
-            query['AppContentProtection'] = request.app_content_protection
         if not UtilClient.is_unset(request.authorize_access_policy_rule):
             query['AuthorizeAccessPolicyRule'] = request.authorize_access_policy_rule
         if not UtilClient.is_unset(request.authorize_security_policy_rule):
             query['AuthorizeSecurityPolicyRule'] = request.authorize_security_policy_rule
         if not UtilClient.is_unset(request.camera_redirect):
             query['CameraRedirect'] = request.camera_redirect
         if not UtilClient.is_unset(request.client_type):
             query['ClientType'] = request.client_type
         if not UtilClient.is_unset(request.clipboard):
             query['Clipboard'] = request.clipboard
         if not UtilClient.is_unset(request.domain_list):
             query['DomainList'] = request.domain_list
-        if not UtilClient.is_unset(request.domain_resolve_rule):
-            query['DomainResolveRule'] = request.domain_resolve_rule
-        if not UtilClient.is_unset(request.domain_resolve_rule_type):
-            query['DomainResolveRuleType'] = request.domain_resolve_rule_type
-        if not UtilClient.is_unset(request.end_user_apply_admin_coordinate):
-            query['EndUserApplyAdminCoordinate'] = request.end_user_apply_admin_coordinate
-        if not UtilClient.is_unset(request.end_user_group_coordinate):
-            query['EndUserGroupCoordinate'] = request.end_user_group_coordinate
         if not UtilClient.is_unset(request.gpu_acceleration):
             query['GpuAcceleration'] = request.gpu_acceleration
         if not UtilClient.is_unset(request.html_5access):
             query['Html5Access'] = request.html_5access
         if not UtilClient.is_unset(request.html_5file_transfer):
             query['Html5FileTransfer'] = request.html_5file_transfer
-        if not UtilClient.is_unset(request.internet_communication_protocol):
-            query['InternetCommunicationProtocol'] = request.internet_communication_protocol
         if not UtilClient.is_unset(request.local_drive):
             query['LocalDrive'] = request.local_drive
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.net_redirect):
             query['NetRedirect'] = request.net_redirect
         if not UtilClient.is_unset(request.preempt_login):
             query['PreemptLogin'] = request.preempt_login
         if not UtilClient.is_unset(request.preempt_login_user):
             query['PreemptLoginUser'] = request.preempt_login_user
         if not UtilClient.is_unset(request.printer_redirection):
             query['PrinterRedirection'] = request.printer_redirection
-        if not UtilClient.is_unset(request.record_content):
-            query['RecordContent'] = request.record_content
-        if not UtilClient.is_unset(request.record_content_expires):
-            query['RecordContentExpires'] = request.record_content_expires
         if not UtilClient.is_unset(request.recording):
             query['Recording'] = request.recording
-        if not UtilClient.is_unset(request.recording_audio):
-            query['RecordingAudio'] = request.recording_audio
-        if not UtilClient.is_unset(request.recording_duration):
-            query['RecordingDuration'] = request.recording_duration
         if not UtilClient.is_unset(request.recording_end_time):
             query['RecordingEndTime'] = request.recording_end_time
-        if not UtilClient.is_unset(request.recording_expires):
-            query['RecordingExpires'] = request.recording_expires
         if not UtilClient.is_unset(request.recording_fps):
             query['RecordingFps'] = request.recording_fps
         if not UtilClient.is_unset(request.recording_start_time):
             query['RecordingStartTime'] = request.recording_start_time
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.remote_coordinate):
-            query['RemoteCoordinate'] = request.remote_coordinate
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
-        if not UtilClient.is_unset(request.scope_value):
-            query['ScopeValue'] = request.scope_value
         if not UtilClient.is_unset(request.usb_redirect):
             query['UsbRedirect'] = request.usb_redirect
         if not UtilClient.is_unset(request.usb_supply_redirect_rule):
             query['UsbSupplyRedirectRule'] = request.usb_supply_redirect_rule
-        if not UtilClient.is_unset(request.video_redirect):
-            query['VideoRedirect'] = request.video_redirect
         if not UtilClient.is_unset(request.visual_quality):
             query['VisualQuality'] = request.visual_quality
         if not UtilClient.is_unset(request.watermark):
             query['Watermark'] = request.watermark
-        if not UtilClient.is_unset(request.watermark_color):
-            query['WatermarkColor'] = request.watermark_color
-        if not UtilClient.is_unset(request.watermark_degree):
-            query['WatermarkDegree'] = request.watermark_degree
-        if not UtilClient.is_unset(request.watermark_font_size):
-            query['WatermarkFontSize'] = request.watermark_font_size
-        if not UtilClient.is_unset(request.watermark_font_style):
-            query['WatermarkFontStyle'] = request.watermark_font_style
-        if not UtilClient.is_unset(request.watermark_row_amount):
-            query['WatermarkRowAmount'] = request.watermark_row_amount
         if not UtilClient.is_unset(request.watermark_transparency):
             query['WatermarkTransparency'] = request.watermark_transparency
-        if not UtilClient.is_unset(request.watermark_transparency_value):
-            query['WatermarkTransparencyValue'] = request.watermark_transparency_value
         if not UtilClient.is_unset(request.watermark_type):
             query['WatermarkType'] = request.watermark_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePolicyGroup',
@@ -4011,49 +2247,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_policy_group(
         self,
         request: ecd_20200930_models.CreatePolicyGroupRequest,
     ) -> ecd_20200930_models.CreatePolicyGroupResponse:
-        """
-        A policy is a set of security rules that are used to control security configurations when end users use cloud desktops. A policy contains basic features, such as USB redirection and watermarking, and other features, such as security group control. For more information, see [Policy overview](~~189345~~).
-        
-        @param request: CreatePolicyGroupRequest
-        @return: CreatePolicyGroupResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_policy_group_with_options(request, runtime)
 
     async def create_policy_group_async(
         self,
         request: ecd_20200930_models.CreatePolicyGroupRequest,
     ) -> ecd_20200930_models.CreatePolicyGroupResponse:
-        """
-        A policy is a set of security rules that are used to control security configurations when end users use cloud desktops. A policy contains basic features, such as USB redirection and watermarking, and other features, such as security group control. For more information, see [Policy overview](~~189345~~).
-        
-        @param request: CreatePolicyGroupRequest
-        @return: CreatePolicyGroupResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_policy_group_with_options_async(request, runtime)
 
     def create_ramdirectory_with_options(
         self,
         request: ecd_20200930_models.CreateRAMDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateRAMDirectoryResponse:
-        """
-        The name of the directory. The name must be 2 to 255 characters in length and can contain letters, digits, colons (:), underscores (\\_), and hyphens (-). It must start with a letter and cannot start with `http://` or `https://`.
-        This parameter is empty by default.
-        
-        @param request: CreateRAMDirectoryRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateRAMDirectoryResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_access_type):
             query['DesktopAccessType'] = request.desktop_access_type
         if not UtilClient.is_unset(request.directory_name):
             query['DirectoryName'] = request.directory_name
         if not UtilClient.is_unset(request.enable_admin_access):
@@ -4084,22 +2300,14 @@
         )
 
     async def create_ramdirectory_with_options_async(
         self,
         request: ecd_20200930_models.CreateRAMDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateRAMDirectoryResponse:
-        """
-        The name of the directory. The name must be 2 to 255 characters in length and can contain letters, digits, colons (:), underscores (\\_), and hyphens (-). It must start with a letter and cannot start with `http://` or `https://`.
-        This parameter is empty by default.
-        
-        @param request: CreateRAMDirectoryRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateRAMDirectoryResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_access_type):
             query['DesktopAccessType'] = request.desktop_access_type
         if not UtilClient.is_unset(request.directory_name):
             query['DirectoryName'] = request.directory_name
         if not UtilClient.is_unset(request.enable_admin_access):
@@ -4129,35 +2337,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_ramdirectory(
         self,
         request: ecd_20200930_models.CreateRAMDirectoryRequest,
     ) -> ecd_20200930_models.CreateRAMDirectoryResponse:
-        """
-        The name of the directory. The name must be 2 to 255 characters in length and can contain letters, digits, colons (:), underscores (\\_), and hyphens (-). It must start with a letter and cannot start with `http://` or `https://`.
-        This parameter is empty by default.
-        
-        @param request: CreateRAMDirectoryRequest
-        @return: CreateRAMDirectoryResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_ramdirectory_with_options(request, runtime)
 
     async def create_ramdirectory_async(
         self,
         request: ecd_20200930_models.CreateRAMDirectoryRequest,
     ) -> ecd_20200930_models.CreateRAMDirectoryResponse:
-        """
-        The name of the directory. The name must be 2 to 255 characters in length and can contain letters, digits, colons (:), underscores (\\_), and hyphens (-). It must start with a letter and cannot start with `http://` or `https://`.
-        This parameter is empty by default.
-        
-        @param request: CreateRAMDirectoryRequest
-        @return: CreateRAMDirectoryResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_ramdirectory_with_options_async(request, runtime)
 
     def create_simple_office_site_with_options(
         self,
         request: ecd_20200930_models.CreateSimpleOfficeSiteRequest,
         runtime: util_models.RuntimeOptions,
@@ -4276,21 +2470,14 @@
         return await self.create_simple_office_site_with_options_async(request, runtime)
 
     def create_snapshot_with_options(
         self,
         request: ecd_20200930_models.CreateSnapshotRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateSnapshotResponse:
-        """
-        The cloud desktop for which you want to create a snapshot must be in the *Running** state or **Stopped** state.
-        
-        @param request: CreateSnapshotRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateSnapshotResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
@@ -4319,21 +2506,14 @@
         )
 
     async def create_snapshot_with_options_async(
         self,
         request: ecd_20200930_models.CreateSnapshotRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.CreateSnapshotResponse:
-        """
-        The cloud desktop for which you want to create a snapshot must be in the *Running** state or **Stopped** state.
-        
-        @param request: CreateSnapshotRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateSnapshotResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
@@ -4361,110 +2541,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_snapshot(
         self,
         request: ecd_20200930_models.CreateSnapshotRequest,
     ) -> ecd_20200930_models.CreateSnapshotResponse:
-        """
-        The cloud desktop for which you want to create a snapshot must be in the *Running** state or **Stopped** state.
-        
-        @param request: CreateSnapshotRequest
-        @return: CreateSnapshotResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_snapshot_with_options(request, runtime)
 
     async def create_snapshot_async(
         self,
         request: ecd_20200930_models.CreateSnapshotRequest,
     ) -> ecd_20200930_models.CreateSnapshotResponse:
-        """
-        The cloud desktop for which you want to create a snapshot must be in the *Running** state or **Stopped** state.
-        
-        @param request: CreateSnapshotRequest
-        @return: CreateSnapshotResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_snapshot_with_options_async(request, runtime)
 
-    def delete_auto_snapshot_policy_with_options(
-        self,
-        request: ecd_20200930_models.DeleteAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteAutoSnapshotPolicyResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteAutoSnapshotPolicyResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_auto_snapshot_policy_with_options_async(
-        self,
-        request: ecd_20200930_models.DeleteAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteAutoSnapshotPolicyResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteAutoSnapshotPolicyResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_auto_snapshot_policy(
-        self,
-        request: ecd_20200930_models.DeleteAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.DeleteAutoSnapshotPolicyResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.delete_auto_snapshot_policy_with_options(request, runtime)
-
-    async def delete_auto_snapshot_policy_async(
-        self,
-        request: ecd_20200930_models.DeleteAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.DeleteAutoSnapshotPolicyResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_auto_snapshot_policy_with_options_async(request, runtime)
-
     def delete_bundles_with_options(
         self,
         request: ecd_20200930_models.DeleteBundlesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteBundlesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -4531,252 +2625,14 @@
     async def delete_bundles_async(
         self,
         request: ecd_20200930_models.DeleteBundlesRequest,
     ) -> ecd_20200930_models.DeleteBundlesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_bundles_with_options_async(request, runtime)
 
-    def delete_cds_file_with_options(
-        self,
-        request: ecd_20200930_models.DeleteCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteCdsFileResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_cds_file_with_options_async(
-        self,
-        request: ecd_20200930_models.DeleteCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteCdsFileResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_cds_file(
-        self,
-        request: ecd_20200930_models.DeleteCdsFileRequest,
-    ) -> ecd_20200930_models.DeleteCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.delete_cds_file_with_options(request, runtime)
-
-    async def delete_cds_file_async(
-        self,
-        request: ecd_20200930_models.DeleteCdsFileRequest,
-    ) -> ecd_20200930_models.DeleteCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_cds_file_with_options_async(request, runtime)
-
-    def delete_cloud_drive_groups_with_options(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveGroupsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteCloudDriveGroupsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.group_id):
-            query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteCloudDriveGroups',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteCloudDriveGroupsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_cloud_drive_groups_with_options_async(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveGroupsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteCloudDriveGroupsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.group_id):
-            query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteCloudDriveGroups',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteCloudDriveGroupsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_cloud_drive_groups(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveGroupsRequest,
-    ) -> ecd_20200930_models.DeleteCloudDriveGroupsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.delete_cloud_drive_groups_with_options(request, runtime)
-
-    async def delete_cloud_drive_groups_async(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveGroupsRequest,
-    ) -> ecd_20200930_models.DeleteCloudDriveGroupsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_cloud_drive_groups_with_options_async(request, runtime)
-
-    def delete_cloud_drive_users_with_options(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteCloudDriveUsersResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_cloud_drive_users_with_options_async(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteCloudDriveUsersResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_cloud_drive_users(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.DeleteCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.delete_cloud_drive_users_with_options(request, runtime)
-
-    async def delete_cloud_drive_users_async(
-        self,
-        request: ecd_20200930_models.DeleteCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.DeleteCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_cloud_drive_users_with_options_async(request, runtime)
-
     def delete_desktop_group_with_options(
         self,
         request: ecd_20200930_models.DeleteDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteDesktopGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -4917,134 +2773,19 @@
     async def delete_desktops_async(
         self,
         request: ecd_20200930_models.DeleteDesktopsRequest,
     ) -> ecd_20200930_models.DeleteDesktopsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_desktops_with_options_async(request, runtime)
 
-    def delete_devices_with_options(
-        self,
-        request: ecd_20200930_models.DeleteDevicesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteDevicesResponse:
-        """
-        You can call the operation to manage client devices.
-        
-        @param request: DeleteDevicesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteDevicesResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_ids):
-            query['DeviceIds'] = request.device_ids
-        if not UtilClient.is_unset(request.force):
-            query['Force'] = request.force
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteDevices',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteDevicesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_devices_with_options_async(
-        self,
-        request: ecd_20200930_models.DeleteDevicesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteDevicesResponse:
-        """
-        You can call the operation to manage client devices.
-        
-        @param request: DeleteDevicesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteDevicesResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_ids):
-            query['DeviceIds'] = request.device_ids
-        if not UtilClient.is_unset(request.force):
-            query['Force'] = request.force
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteDevices',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteDevicesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_devices(
-        self,
-        request: ecd_20200930_models.DeleteDevicesRequest,
-    ) -> ecd_20200930_models.DeleteDevicesResponse:
-        """
-        You can call the operation to manage client devices.
-        
-        @param request: DeleteDevicesRequest
-        @return: DeleteDevicesResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.delete_devices_with_options(request, runtime)
-
-    async def delete_devices_async(
-        self,
-        request: ecd_20200930_models.DeleteDevicesRequest,
-    ) -> ecd_20200930_models.DeleteDevicesResponse:
-        """
-        You can call the operation to manage client devices.
-        
-        @param request: DeleteDevicesRequest
-        @return: DeleteDevicesResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_devices_with_options_async(request, runtime)
-
     def delete_directories_with_options(
         self,
         request: ecd_20200930_models.DeleteDirectoriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteDirectoriesResponse:
-        """
-        The ID of directory N. You can specify one or more directory IDs.
-        
-        @param request: DeleteDirectoriesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteDirectoriesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -5067,21 +2808,14 @@
         )
 
     async def delete_directories_with_options_async(
         self,
         request: ecd_20200930_models.DeleteDirectoriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteDirectoriesResponse:
-        """
-        The ID of directory N. You can specify one or more directory IDs.
-        
-        @param request: DeleteDirectoriesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteDirectoriesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -5103,126 +2837,31 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_directories(
         self,
         request: ecd_20200930_models.DeleteDirectoriesRequest,
     ) -> ecd_20200930_models.DeleteDirectoriesResponse:
-        """
-        The ID of directory N. You can specify one or more directory IDs.
-        
-        @param request: DeleteDirectoriesRequest
-        @return: DeleteDirectoriesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_directories_with_options(request, runtime)
 
     async def delete_directories_async(
         self,
         request: ecd_20200930_models.DeleteDirectoriesRequest,
     ) -> ecd_20200930_models.DeleteDirectoriesResponse:
-        """
-        The ID of directory N. You can specify one or more directory IDs.
-        
-        @param request: DeleteDirectoriesRequest
-        @return: DeleteDirectoriesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_directories_with_options_async(request, runtime)
 
-    def delete_edu_room_with_options(
-        self,
-        request: ecd_20200930_models.DeleteEduRoomRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteEduRoomResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.edu_room_id):
-            query['EduRoomId'] = request.edu_room_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteEduRoom',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteEduRoomResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_edu_room_with_options_async(
-        self,
-        request: ecd_20200930_models.DeleteEduRoomRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DeleteEduRoomResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.edu_room_id):
-            query['EduRoomId'] = request.edu_room_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteEduRoom',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DeleteEduRoomResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_edu_room(
-        self,
-        request: ecd_20200930_models.DeleteEduRoomRequest,
-    ) -> ecd_20200930_models.DeleteEduRoomResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.delete_edu_room_with_options(request, runtime)
-
-    async def delete_edu_room_async(
-        self,
-        request: ecd_20200930_models.DeleteEduRoomRequest,
-    ) -> ecd_20200930_models.DeleteEduRoomResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_edu_room_with_options_async(request, runtime)
-
     def delete_images_with_options(
         self,
         request: ecd_20200930_models.DeleteImagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteImagesResponse:
-        """
-        The IDs of the images that you want to delete. You can configure one or more image IDs. Valid values of N: 1 to 100.
-        
-        @param request: DeleteImagesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteImagesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.delete_cascaded_bundle):
-            query['DeleteCascadedBundle'] = request.delete_cascaded_bundle
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5243,25 +2882,16 @@
         )
 
     async def delete_images_with_options_async(
         self,
         request: ecd_20200930_models.DeleteImagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteImagesResponse:
-        """
-        The IDs of the images that you want to delete. You can configure one or more image IDs. Valid values of N: 1 to 100.
-        
-        @param request: DeleteImagesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteImagesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.delete_cascaded_bundle):
-            query['DeleteCascadedBundle'] = request.delete_cascaded_bundle
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5281,50 +2911,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_images(
         self,
         request: ecd_20200930_models.DeleteImagesRequest,
     ) -> ecd_20200930_models.DeleteImagesResponse:
-        """
-        The IDs of the images that you want to delete. You can configure one or more image IDs. Valid values of N: 1 to 100.
-        
-        @param request: DeleteImagesRequest
-        @return: DeleteImagesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_images_with_options(request, runtime)
 
     async def delete_images_async(
         self,
         request: ecd_20200930_models.DeleteImagesRequest,
     ) -> ecd_20200930_models.DeleteImagesResponse:
-        """
-        The IDs of the images that you want to delete. You can configure one or more image IDs. Valid values of N: 1 to 100.
-        
-        @param request: DeleteImagesRequest
-        @return: DeleteImagesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_images_with_options_async(request, runtime)
 
     def delete_nasfile_systems_with_options(
         self,
         request: ecd_20200930_models.DeleteNASFileSystemsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteNASFileSystemsResponse:
-        """
-        Before you delete an Apsara File Storage NAS (NAS) file system, make sure that the data you want to retain is backed up.
-        **\
-        **Warning** If a NAS file system is deleted, data stored in the NAS file system cannot be restored. Proceed with caution when you delete NAS file systems.
-        
-        @param request: DeleteNASFileSystemsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteNASFileSystemsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -5347,23 +2956,14 @@
         )
 
     async def delete_nasfile_systems_with_options_async(
         self,
         request: ecd_20200930_models.DeleteNASFileSystemsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteNASFileSystemsResponse:
-        """
-        Before you delete an Apsara File Storage NAS (NAS) file system, make sure that the data you want to retain is backed up.
-        **\
-        **Warning** If a NAS file system is deleted, data stored in the NAS file system cannot be restored. Proceed with caution when you delete NAS file systems.
-        
-        @param request: DeleteNASFileSystemsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteNASFileSystemsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -5385,37 +2985,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_nasfile_systems(
         self,
         request: ecd_20200930_models.DeleteNASFileSystemsRequest,
     ) -> ecd_20200930_models.DeleteNASFileSystemsResponse:
-        """
-        Before you delete an Apsara File Storage NAS (NAS) file system, make sure that the data you want to retain is backed up.
-        **\
-        **Warning** If a NAS file system is deleted, data stored in the NAS file system cannot be restored. Proceed with caution when you delete NAS file systems.
-        
-        @param request: DeleteNASFileSystemsRequest
-        @return: DeleteNASFileSystemsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_nasfile_systems_with_options(request, runtime)
 
     async def delete_nasfile_systems_async(
         self,
         request: ecd_20200930_models.DeleteNASFileSystemsRequest,
     ) -> ecd_20200930_models.DeleteNASFileSystemsResponse:
-        """
-        Before you delete an Apsara File Storage NAS (NAS) file system, make sure that the data you want to retain is backed up.
-        **\
-        **Warning** If a NAS file system is deleted, data stored in the NAS file system cannot be restored. Proceed with caution when you delete NAS file systems.
-        
-        @param request: DeleteNASFileSystemsRequest
-        @return: DeleteNASFileSystemsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_nasfile_systems_with_options_async(request, runtime)
 
     def delete_network_packages_with_options(
         self,
         request: ecd_20200930_models.DeleteNetworkPackagesRequest,
         runtime: util_models.RuntimeOptions,
@@ -5490,25 +3074,14 @@
         return await self.delete_network_packages_with_options_async(request, runtime)
 
     def delete_office_sites_with_options(
         self,
         request: ecd_20200930_models.DeleteOfficeSitesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteOfficeSitesResponse:
-        """
-        Before you delete a workspace, make sure that the following requirements are met:
-        *   All cloud desktops in the workspace are released.
-        *   The data that you want to retain is backed up.
-        **\
-        **Warning** After you delete a workspace, the resources and data of the workspace cannot be recovered. Exercise with caution.
-        
-        @param request: DeleteOfficeSitesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteOfficeSitesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -5531,25 +3104,14 @@
         )
 
     async def delete_office_sites_with_options_async(
         self,
         request: ecd_20200930_models.DeleteOfficeSitesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteOfficeSitesResponse:
-        """
-        Before you delete a workspace, make sure that the following requirements are met:
-        *   All cloud desktops in the workspace are released.
-        *   The data that you want to retain is backed up.
-        **\
-        **Warning** After you delete a workspace, the resources and data of the workspace cannot be recovered. Exercise with caution.
-        
-        @param request: DeleteOfficeSitesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteOfficeSitesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -5571,41 +3133,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_office_sites(
         self,
         request: ecd_20200930_models.DeleteOfficeSitesRequest,
     ) -> ecd_20200930_models.DeleteOfficeSitesResponse:
-        """
-        Before you delete a workspace, make sure that the following requirements are met:
-        *   All cloud desktops in the workspace are released.
-        *   The data that you want to retain is backed up.
-        **\
-        **Warning** After you delete a workspace, the resources and data of the workspace cannot be recovered. Exercise with caution.
-        
-        @param request: DeleteOfficeSitesRequest
-        @return: DeleteOfficeSitesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_office_sites_with_options(request, runtime)
 
     async def delete_office_sites_async(
         self,
         request: ecd_20200930_models.DeleteOfficeSitesRequest,
     ) -> ecd_20200930_models.DeleteOfficeSitesResponse:
-        """
-        Before you delete a workspace, make sure that the following requirements are met:
-        *   All cloud desktops in the workspace are released.
-        *   The data that you want to retain is backed up.
-        **\
-        **Warning** After you delete a workspace, the resources and data of the workspace cannot be recovered. Exercise with caution.
-        
-        @param request: DeleteOfficeSitesRequest
-        @return: DeleteOfficeSitesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_office_sites_with_options_async(request, runtime)
 
     def delete_policy_groups_with_options(
         self,
         request: ecd_20200930_models.DeletePolicyGroupsRequest,
         runtime: util_models.RuntimeOptions,
@@ -5680,21 +3222,14 @@
         return await self.delete_policy_groups_with_options_async(request, runtime)
 
     def delete_snapshot_with_options(
         self,
         request: ecd_20200930_models.DeleteSnapshotRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteSnapshotResponse:
-        """
-        If the IDs of the snapshots that you specify do not exist, requests are ignored.
-        
-        @param request: DeleteSnapshotRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteSnapshotResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.snapshot_id):
             query['SnapshotId'] = request.snapshot_id
         req = open_api_models.OpenApiRequest(
@@ -5717,21 +3252,14 @@
         )
 
     async def delete_snapshot_with_options_async(
         self,
         request: ecd_20200930_models.DeleteSnapshotRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteSnapshotResponse:
-        """
-        If the IDs of the snapshots that you specify do not exist, requests are ignored.
-        
-        @param request: DeleteSnapshotRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteSnapshotResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.snapshot_id):
             query['SnapshotId'] = request.snapshot_id
         req = open_api_models.OpenApiRequest(
@@ -5753,48 +3281,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_snapshot(
         self,
         request: ecd_20200930_models.DeleteSnapshotRequest,
     ) -> ecd_20200930_models.DeleteSnapshotResponse:
-        """
-        If the IDs of the snapshots that you specify do not exist, requests are ignored.
-        
-        @param request: DeleteSnapshotRequest
-        @return: DeleteSnapshotResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_snapshot_with_options(request, runtime)
 
     async def delete_snapshot_async(
         self,
         request: ecd_20200930_models.DeleteSnapshotRequest,
     ) -> ecd_20200930_models.DeleteSnapshotResponse:
-        """
-        If the IDs of the snapshots that you specify do not exist, requests are ignored.
-        
-        @param request: DeleteSnapshotRequest
-        @return: DeleteSnapshotResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_snapshot_with_options_async(request, runtime)
 
     def delete_virtual_mfadevice_with_options(
         self,
         request: ecd_20200930_models.DeleteVirtualMFADeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: DeleteVirtualMFADeviceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteVirtualMFADeviceResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.serial_number):
             query['SerialNumber'] = request.serial_number
         req = open_api_models.OpenApiRequest(
@@ -5817,21 +3326,14 @@
         )
 
     async def delete_virtual_mfadevice_with_options_async(
         self,
         request: ecd_20200930_models.DeleteVirtualMFADeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DeleteVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: DeleteVirtualMFADeviceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteVirtualMFADeviceResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.serial_number):
             query['SerialNumber'] = request.serial_number
         req = open_api_models.OpenApiRequest(
@@ -5853,122 +3355,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_virtual_mfadevice(
         self,
         request: ecd_20200930_models.DeleteVirtualMFADeviceRequest,
     ) -> ecd_20200930_models.DeleteVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: DeleteVirtualMFADeviceRequest
-        @return: DeleteVirtualMFADeviceResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_virtual_mfadevice_with_options(request, runtime)
 
     async def delete_virtual_mfadevice_async(
         self,
         request: ecd_20200930_models.DeleteVirtualMFADeviceRequest,
     ) -> ecd_20200930_models.DeleteVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: DeleteVirtualMFADeviceRequest
-        @return: DeleteVirtualMFADeviceResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_virtual_mfadevice_with_options_async(request, runtime)
 
-    def describe_acl_entries_with_options(
-        self,
-        request: ecd_20200930_models.DescribeAclEntriesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeAclEntriesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.source_id):
-            query['SourceId'] = request.source_id
-        if not UtilClient.is_unset(request.source_type):
-            query['SourceType'] = request.source_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeAclEntries',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeAclEntriesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_acl_entries_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeAclEntriesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeAclEntriesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.source_id):
-            query['SourceId'] = request.source_id
-        if not UtilClient.is_unset(request.source_type):
-            query['SourceType'] = request.source_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeAclEntries',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeAclEntriesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_acl_entries(
-        self,
-        request: ecd_20200930_models.DescribeAclEntriesRequest,
-    ) -> ecd_20200930_models.DescribeAclEntriesResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_acl_entries_with_options(request, runtime)
-
-    async def describe_acl_entries_async(
-        self,
-        request: ecd_20200930_models.DescribeAclEntriesRequest,
-    ) -> ecd_20200930_models.DescribeAclEntriesResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_acl_entries_with_options_async(request, runtime)
-
     def describe_alarm_event_stack_info_with_options(
         self,
         request: ecd_20200930_models.DescribeAlarmEventStackInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeAlarmEventStackInfoResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6047,126 +3451,14 @@
     async def describe_alarm_event_stack_info_async(
         self,
         request: ecd_20200930_models.DescribeAlarmEventStackInfoRequest,
     ) -> ecd_20200930_models.DescribeAlarmEventStackInfoResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_alarm_event_stack_info_with_options_async(request, runtime)
 
-    def describe_auto_snapshot_policy_with_options(
-        self,
-        request: ecd_20200930_models.DescribeAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeAutoSnapshotPolicyResponse:
-        """
-        You can view an automatic snapshot policy that is associated with a cloud desktop in the Elastic Desktop Service (EDS) console. To view the automatic snapshot policy, you can go to the EDS console, choose Deployment > Snapshots in the left-side navigation pane, and then view an automatic snapshot policy on the Snapshots page.
-        
-        @param request: DescribeAutoSnapshotPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeAutoSnapshotPolicyResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.policy_name):
-            query['PolicyName'] = request.policy_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeAutoSnapshotPolicyResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_auto_snapshot_policy_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeAutoSnapshotPolicyResponse:
-        """
-        You can view an automatic snapshot policy that is associated with a cloud desktop in the Elastic Desktop Service (EDS) console. To view the automatic snapshot policy, you can go to the EDS console, choose Deployment > Snapshots in the left-side navigation pane, and then view an automatic snapshot policy on the Snapshots page.
-        
-        @param request: DescribeAutoSnapshotPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeAutoSnapshotPolicyResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.policy_name):
-            query['PolicyName'] = request.policy_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeAutoSnapshotPolicyResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_auto_snapshot_policy(
-        self,
-        request: ecd_20200930_models.DescribeAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.DescribeAutoSnapshotPolicyResponse:
-        """
-        You can view an automatic snapshot policy that is associated with a cloud desktop in the Elastic Desktop Service (EDS) console. To view the automatic snapshot policy, you can go to the EDS console, choose Deployment > Snapshots in the left-side navigation pane, and then view an automatic snapshot policy on the Snapshots page.
-        
-        @param request: DescribeAutoSnapshotPolicyRequest
-        @return: DescribeAutoSnapshotPolicyResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.describe_auto_snapshot_policy_with_options(request, runtime)
-
-    async def describe_auto_snapshot_policy_async(
-        self,
-        request: ecd_20200930_models.DescribeAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.DescribeAutoSnapshotPolicyResponse:
-        """
-        You can view an automatic snapshot policy that is associated with a cloud desktop in the Elastic Desktop Service (EDS) console. To view the automatic snapshot policy, you can go to the EDS console, choose Deployment > Snapshots in the left-side navigation pane, and then view an automatic snapshot policy on the Snapshots page.
-        
-        @param request: DescribeAutoSnapshotPolicyRequest
-        @return: DescribeAutoSnapshotPolicyResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_auto_snapshot_policy_with_options_async(request, runtime)
-
     def describe_bundles_with_options(
         self,
         request: ecd_20200930_models.DescribeBundlesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeBundlesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6182,34 +3474,24 @@
             query['DesktopTypeFamily'] = request.desktop_type_family
         if not UtilClient.is_unset(request.fota_channel):
             query['FotaChannel'] = request.fota_channel
         if not UtilClient.is_unset(request.from_desktop_group):
             query['FromDesktopGroup'] = request.from_desktop_group
         if not UtilClient.is_unset(request.gpu_count):
             query['GpuCount'] = request.gpu_count
-        if not UtilClient.is_unset(request.image_id):
-            query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.memory_size):
             query['MemorySize'] = request.memory_size
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.os_type):
-            query['OsType'] = request.os_type
         if not UtilClient.is_unset(request.protocol_type):
             query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
-        if not UtilClient.is_unset(request.selected_bundle):
-            query['SelectedBundle'] = request.selected_bundle
-        if not UtilClient.is_unset(request.session_type):
-            query['SessionType'] = request.session_type
         if not UtilClient.is_unset(request.support_multi_session):
             query['SupportMultiSession'] = request.support_multi_session
         if not UtilClient.is_unset(request.volume_encryption_enabled):
             query['VolumeEncryptionEnabled'] = request.volume_encryption_enabled
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -6248,34 +3530,24 @@
             query['DesktopTypeFamily'] = request.desktop_type_family
         if not UtilClient.is_unset(request.fota_channel):
             query['FotaChannel'] = request.fota_channel
         if not UtilClient.is_unset(request.from_desktop_group):
             query['FromDesktopGroup'] = request.from_desktop_group
         if not UtilClient.is_unset(request.gpu_count):
             query['GpuCount'] = request.gpu_count
-        if not UtilClient.is_unset(request.image_id):
-            query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.memory_size):
             query['MemorySize'] = request.memory_size
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.os_type):
-            query['OsType'] = request.os_type
         if not UtilClient.is_unset(request.protocol_type):
             query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
-        if not UtilClient.is_unset(request.selected_bundle):
-            query['SelectedBundle'] = request.selected_bundle
-        if not UtilClient.is_unset(request.session_type):
-            query['SessionType'] = request.session_type
         if not UtilClient.is_unset(request.support_multi_session):
             query['SupportMultiSession'] = request.support_multi_session
         if not UtilClient.is_unset(request.volume_encryption_enabled):
             query['VolumeEncryptionEnabled'] = request.volume_encryption_enabled
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -6305,108 +3577,14 @@
     async def describe_bundles_async(
         self,
         request: ecd_20200930_models.DescribeBundlesRequest,
     ) -> ecd_20200930_models.DescribeBundlesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_bundles_with_options_async(request, runtime)
 
-    def describe_cds_file_share_links_with_options(
-        self,
-        request: ecd_20200930_models.DescribeCdsFileShareLinksRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCdsFileShareLinksResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.creators):
-            query['Creators'] = request.creators
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.share_id):
-            query['ShareId'] = request.share_id
-        if not UtilClient.is_unset(request.share_name):
-            query['ShareName'] = request.share_name
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCdsFileShareLinks',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCdsFileShareLinksResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_cds_file_share_links_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeCdsFileShareLinksRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCdsFileShareLinksResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.creators):
-            query['Creators'] = request.creators
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.share_id):
-            query['ShareId'] = request.share_id
-        if not UtilClient.is_unset(request.share_name):
-            query['ShareName'] = request.share_name
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCdsFileShareLinks',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCdsFileShareLinksResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_cds_file_share_links(
-        self,
-        request: ecd_20200930_models.DescribeCdsFileShareLinksRequest,
-    ) -> ecd_20200930_models.DescribeCdsFileShareLinksResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_cds_file_share_links_with_options(request, runtime)
-
-    async def describe_cds_file_share_links_async(
-        self,
-        request: ecd_20200930_models.DescribeCdsFileShareLinksRequest,
-    ) -> ecd_20200930_models.DescribeCdsFileShareLinksResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_cds_file_share_links_with_options_async(request, runtime)
-
     def describe_cens_with_options(
         self,
         request: ecd_20200930_models.DescribeCensRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeCensResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6482,21 +3660,14 @@
         return await self.describe_cens_with_options_async(request, runtime)
 
     def describe_client_events_with_options(
         self,
         request: ecd_20200930_models.DescribeClientEventsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeClientEventsResponse:
-        """
-        The version of the client.
-        
-        @param request: DescribeClientEventsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeClientEventsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.desktop_ip):
             query['DesktopIp'] = request.desktop_ip
         if not UtilClient.is_unset(request.desktop_name):
@@ -6505,16 +3676,14 @@
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
-        if not UtilClient.is_unset(request.event_types):
-            query['EventTypes'] = request.event_types
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
@@ -6543,21 +3712,14 @@
         )
 
     async def describe_client_events_with_options_async(
         self,
         request: ecd_20200930_models.DescribeClientEventsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeClientEventsResponse:
-        """
-        The version of the client.
-        
-        @param request: DescribeClientEventsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeClientEventsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.desktop_ip):
             query['DesktopIp'] = request.desktop_ip
         if not UtilClient.is_unset(request.desktop_name):
@@ -6566,16 +3728,14 @@
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
-        if not UtilClient.is_unset(request.event_types):
-            query['EventTypes'] = request.event_types
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
@@ -6603,423 +3763,53 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_client_events(
         self,
         request: ecd_20200930_models.DescribeClientEventsRequest,
     ) -> ecd_20200930_models.DescribeClientEventsResponse:
-        """
-        The version of the client.
-        
-        @param request: DescribeClientEventsRequest
-        @return: DescribeClientEventsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_client_events_with_options(request, runtime)
 
     async def describe_client_events_async(
         self,
         request: ecd_20200930_models.DescribeClientEventsRequest,
     ) -> ecd_20200930_models.DescribeClientEventsResponse:
-        """
-        The version of the client.
-        
-        @param request: DescribeClientEventsRequest
-        @return: DescribeClientEventsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_client_events_with_options_async(request, runtime)
 
-    def describe_cloud_drive_groups_with_options(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveGroupsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCloudDriveGroupsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.directory_name):
-            query['DirectoryName'] = request.directory_name
-        if not UtilClient.is_unset(request.drive_status):
-            query['DriveStatus'] = request.drive_status
-        if not UtilClient.is_unset(request.drive_type):
-            query['DriveType'] = request.drive_type
-        if not UtilClient.is_unset(request.group_id):
-            query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.group_name):
-            query['GroupName'] = request.group_name
-        if not UtilClient.is_unset(request.group_type):
-            query['GroupType'] = request.group_type
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.parent_group_id):
-            query['ParentGroupId'] = request.parent_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCloudDriveGroups',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCloudDriveGroupsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_cloud_drive_groups_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveGroupsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCloudDriveGroupsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.directory_name):
-            query['DirectoryName'] = request.directory_name
-        if not UtilClient.is_unset(request.drive_status):
-            query['DriveStatus'] = request.drive_status
-        if not UtilClient.is_unset(request.drive_type):
-            query['DriveType'] = request.drive_type
-        if not UtilClient.is_unset(request.group_id):
-            query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.group_name):
-            query['GroupName'] = request.group_name
-        if not UtilClient.is_unset(request.group_type):
-            query['GroupType'] = request.group_type
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.parent_group_id):
-            query['ParentGroupId'] = request.parent_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCloudDriveGroups',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCloudDriveGroupsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_cloud_drive_groups(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveGroupsRequest,
-    ) -> ecd_20200930_models.DescribeCloudDriveGroupsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_cloud_drive_groups_with_options(request, runtime)
-
-    async def describe_cloud_drive_groups_async(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveGroupsRequest,
-    ) -> ecd_20200930_models.DescribeCloudDriveGroupsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_cloud_drive_groups_with_options_async(request, runtime)
-
-    def describe_cloud_drive_permissions_with_options(
-        self,
-        request: ecd_20200930_models.DescribeCloudDrivePermissionsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCloudDrivePermissionsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCloudDrivePermissions',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCloudDrivePermissionsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_cloud_drive_permissions_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeCloudDrivePermissionsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCloudDrivePermissionsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCloudDrivePermissions',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCloudDrivePermissionsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_cloud_drive_permissions(
-        self,
-        request: ecd_20200930_models.DescribeCloudDrivePermissionsRequest,
-    ) -> ecd_20200930_models.DescribeCloudDrivePermissionsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_cloud_drive_permissions_with_options(request, runtime)
-
-    async def describe_cloud_drive_permissions_async(
-        self,
-        request: ecd_20200930_models.DescribeCloudDrivePermissionsRequest,
-    ) -> ecd_20200930_models.DescribeCloudDrivePermissionsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_cloud_drive_permissions_with_options_async(request, runtime)
-
-    def describe_cloud_drive_users_with_options(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCloudDriveUsersResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_cloud_drive_users_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCloudDriveUsersResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_cloud_drive_users(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.DescribeCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_cloud_drive_users_with_options(request, runtime)
-
-    async def describe_cloud_drive_users_async(
-        self,
-        request: ecd_20200930_models.DescribeCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.DescribeCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_cloud_drive_users_with_options_async(request, runtime)
-
-    def describe_customized_list_headers_with_options(
-        self,
-        request: ecd_20200930_models.DescribeCustomizedListHeadersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCustomizedListHeadersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.lang_type):
-            query['LangType'] = request.lang_type
-        if not UtilClient.is_unset(request.list_type):
-            query['ListType'] = request.list_type
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCustomizedListHeaders',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCustomizedListHeadersResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_customized_list_headers_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeCustomizedListHeadersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeCustomizedListHeadersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.lang_type):
-            query['LangType'] = request.lang_type
-        if not UtilClient.is_unset(request.list_type):
-            query['ListType'] = request.list_type
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeCustomizedListHeaders',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeCustomizedListHeadersResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_customized_list_headers(
-        self,
-        request: ecd_20200930_models.DescribeCustomizedListHeadersRequest,
-    ) -> ecd_20200930_models.DescribeCustomizedListHeadersResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_customized_list_headers_with_options(request, runtime)
-
-    async def describe_customized_list_headers_async(
-        self,
-        request: ecd_20200930_models.DescribeCustomizedListHeadersRequest,
-    ) -> ecd_20200930_models.DescribeCustomizedListHeadersResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_customized_list_headers_with_options_async(request, runtime)
-
     def describe_desktop_groups_with_options(
         self,
         request: ecd_20200930_models.DescribeDesktopGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDesktopGroupsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.bundle_id):
-            query['BundleId'] = request.bundle_id
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_group_name):
             query['DesktopGroupName'] = request.desktop_group_name
         if not UtilClient.is_unset(request.end_user_ids):
             query['EndUserIds'] = request.end_user_ids
         if not UtilClient.is_unset(request.excluded_end_user_ids):
             query['ExcludedEndUserIds'] = request.excluded_end_user_ids
-        if not UtilClient.is_unset(request.image_id):
-            query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.own_type):
             query['OwnType'] = request.own_type
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.protocol_type):
-            query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -7042,42 +3832,36 @@
     async def describe_desktop_groups_with_options_async(
         self,
         request: ecd_20200930_models.DescribeDesktopGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDesktopGroupsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.bundle_id):
-            query['BundleId'] = request.bundle_id
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_group_name):
             query['DesktopGroupName'] = request.desktop_group_name
         if not UtilClient.is_unset(request.end_user_ids):
             query['EndUserIds'] = request.end_user_ids
         if not UtilClient.is_unset(request.excluded_end_user_ids):
             query['ExcludedEndUserIds'] = request.excluded_end_user_ids
-        if not UtilClient.is_unset(request.image_id):
-            query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.own_type):
             query['OwnType'] = request.own_type
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.protocol_type):
-            query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -7193,125 +3977,25 @@
     async def describe_desktop_ids_by_vul_names_async(
         self,
         request: ecd_20200930_models.DescribeDesktopIdsByVulNamesRequest,
     ) -> ecd_20200930_models.DescribeDesktopIdsByVulNamesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_desktop_ids_by_vul_names_with_options_async(request, runtime)
 
-    def describe_desktop_sessions_with_options(
-        self,
-        request: ecd_20200930_models.DescribeDesktopSessionsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeDesktopSessionsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.end_time):
-            query['EndTime'] = request.end_time
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.office_site_id):
-            query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.page_number):
-            query['PageNumber'] = request.page_number
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.session_status):
-            query['SessionStatus'] = request.session_status
-        if not UtilClient.is_unset(request.start_time):
-            query['StartTime'] = request.start_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeDesktopSessions',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeDesktopSessionsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_desktop_sessions_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeDesktopSessionsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeDesktopSessionsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.end_time):
-            query['EndTime'] = request.end_time
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.office_site_id):
-            query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.page_number):
-            query['PageNumber'] = request.page_number
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.session_status):
-            query['SessionStatus'] = request.session_status
-        if not UtilClient.is_unset(request.start_time):
-            query['StartTime'] = request.start_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeDesktopSessions',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeDesktopSessionsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_desktop_sessions(
-        self,
-        request: ecd_20200930_models.DescribeDesktopSessionsRequest,
-    ) -> ecd_20200930_models.DescribeDesktopSessionsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_desktop_sessions_with_options(request, runtime)
-
-    async def describe_desktop_sessions_async(
-        self,
-        request: ecd_20200930_models.DescribeDesktopSessionsRequest,
-    ) -> ecd_20200930_models.DescribeDesktopSessionsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_desktop_sessions_with_options_async(request, runtime)
-
     def describe_desktop_types_with_options(
         self,
         request: ecd_20200930_models.DescribeDesktopTypesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDesktopTypesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.applied_scope):
             query['AppliedScope'] = request.applied_scope
         if not UtilClient.is_unset(request.cpu_count):
             query['CpuCount'] = request.cpu_count
-        if not UtilClient.is_unset(request.desktop_group_id_for_modify):
-            query['DesktopGroupIdForModify'] = request.desktop_group_id_for_modify
         if not UtilClient.is_unset(request.desktop_id_for_modify):
             query['DesktopIdForModify'] = request.desktop_id_for_modify
         if not UtilClient.is_unset(request.desktop_type_id):
             query['DesktopTypeId'] = request.desktop_type_id
         if not UtilClient.is_unset(request.gpu_count):
             query['GpuCount'] = request.gpu_count
         if not UtilClient.is_unset(request.instance_type_family):
@@ -7348,16 +4032,14 @@
     ) -> ecd_20200930_models.DescribeDesktopTypesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.applied_scope):
             query['AppliedScope'] = request.applied_scope
         if not UtilClient.is_unset(request.cpu_count):
             query['CpuCount'] = request.cpu_count
-        if not UtilClient.is_unset(request.desktop_group_id_for_modify):
-            query['DesktopGroupIdForModify'] = request.desktop_group_id_for_modify
         if not UtilClient.is_unset(request.desktop_id_for_modify):
             query['DesktopIdForModify'] = request.desktop_id_for_modify
         if not UtilClient.is_unset(request.desktop_type_id):
             query['DesktopTypeId'] = request.desktop_type_id
         if not UtilClient.is_unset(request.gpu_count):
             query['GpuCount'] = request.gpu_count
         if not UtilClient.is_unset(request.instance_type_family):
@@ -7406,64 +4088,50 @@
         request: ecd_20200930_models.DescribeDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDesktopsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.desktop_name):
             query['DesktopName'] = request.desktop_name
         if not UtilClient.is_unset(request.desktop_status):
             query['DesktopStatus'] = request.desktop_status
-        if not UtilClient.is_unset(request.desktop_status_list):
-            query['DesktopStatusList'] = request.desktop_status_list
-        if not UtilClient.is_unset(request.desktop_type):
-            query['DesktopType'] = request.desktop_type
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.excluded_end_user_id):
             query['ExcludedEndUserId'] = request.excluded_end_user_id
         if not UtilClient.is_unset(request.expired_time):
             query['ExpiredTime'] = request.expired_time
         if not UtilClient.is_unset(request.filter_desktop_group):
             query['FilterDesktopGroup'] = request.filter_desktop_group
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.image_id):
-            query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.management_flag):
             query['ManagementFlag'] = request.management_flag
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
             query['OfficeSiteName'] = request.office_site_name
-        if not UtilClient.is_unset(request.only_desktop_group):
-            query['OnlyDesktopGroup'] = request.only_desktop_group
-        if not UtilClient.is_unset(request.os_types):
-            query['OsTypes'] = request.os_types
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
         if not UtilClient.is_unset(request.protocol_type):
             query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.query_fota_update):
             query['QueryFotaUpdate'] = request.query_fota_update
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.snapshot_policy_id):
-            query['SnapshotPolicyId'] = request.snapshot_policy_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.user_name):
             query['UserName'] = request.user_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -7488,64 +4156,50 @@
         request: ecd_20200930_models.DescribeDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDesktopsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.desktop_name):
             query['DesktopName'] = request.desktop_name
         if not UtilClient.is_unset(request.desktop_status):
             query['DesktopStatus'] = request.desktop_status
-        if not UtilClient.is_unset(request.desktop_status_list):
-            query['DesktopStatusList'] = request.desktop_status_list
-        if not UtilClient.is_unset(request.desktop_type):
-            query['DesktopType'] = request.desktop_type
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.excluded_end_user_id):
             query['ExcludedEndUserId'] = request.excluded_end_user_id
         if not UtilClient.is_unset(request.expired_time):
             query['ExpiredTime'] = request.expired_time
         if not UtilClient.is_unset(request.filter_desktop_group):
             query['FilterDesktopGroup'] = request.filter_desktop_group
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.image_id):
-            query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.management_flag):
             query['ManagementFlag'] = request.management_flag
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
             query['OfficeSiteName'] = request.office_site_name
-        if not UtilClient.is_unset(request.only_desktop_group):
-            query['OnlyDesktopGroup'] = request.only_desktop_group
-        if not UtilClient.is_unset(request.os_types):
-            query['OsTypes'] = request.os_types
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
         if not UtilClient.is_unset(request.protocol_type):
             query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.query_fota_update):
             query['QueryFotaUpdate'] = request.query_fota_update
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.snapshot_policy_id):
-            query['SnapshotPolicyId'] = request.snapshot_policy_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.user_name):
             query['UserName'] = request.user_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -7584,16 +4238,14 @@
         request: ecd_20200930_models.DescribeDesktopsInGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDesktopsInGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.ignore_deleted):
-            query['IgnoreDeleted'] = request.ignore_deleted
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.pay_type):
             query['PayType'] = request.pay_type
         if not UtilClient.is_unset(request.region_id):
@@ -7622,16 +4274,14 @@
         request: ecd_20200930_models.DescribeDesktopsInGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDesktopsInGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.ignore_deleted):
-            query['IgnoreDeleted'] = request.ignore_deleted
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.pay_type):
             query['PayType'] = request.pay_type
         if not UtilClient.is_unset(request.region_id):
@@ -7665,116 +4315,14 @@
     async def describe_desktops_in_group_async(
         self,
         request: ecd_20200930_models.DescribeDesktopsInGroupRequest,
     ) -> ecd_20200930_models.DescribeDesktopsInGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_desktops_in_group_with_options_async(request, runtime)
 
-    def describe_devices_with_options(
-        self,
-        request: ecd_20200930_models.DescribeDevicesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeDevicesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.ad_domain):
-            query['AdDomain'] = request.ad_domain
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_id):
-            query['DeviceId'] = request.device_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.page_number):
-            query['PageNumber'] = request.page_number
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
-        if not UtilClient.is_unset(request.region):
-            query['Region'] = request.region
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeDevices',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeDevicesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_devices_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeDevicesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeDevicesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.ad_domain):
-            query['AdDomain'] = request.ad_domain
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_id):
-            query['DeviceId'] = request.device_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.page_number):
-            query['PageNumber'] = request.page_number
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
-        if not UtilClient.is_unset(request.region):
-            query['Region'] = request.region
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeDevices',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeDevicesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_devices(
-        self,
-        request: ecd_20200930_models.DescribeDevicesRequest,
-    ) -> ecd_20200930_models.DescribeDevicesResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_devices_with_options(request, runtime)
-
-    async def describe_devices_async(
-        self,
-        request: ecd_20200930_models.DescribeDevicesRequest,
-    ) -> ecd_20200930_models.DescribeDevicesResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_devices_with_options_async(request, runtime)
-
     def describe_directories_with_options(
         self,
         request: ecd_20200930_models.DescribeDirectoriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeDirectoriesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7960,21 +4508,14 @@
         return await self.describe_flow_metric_with_options_async(request, runtime)
 
     def describe_flow_statistic_with_options(
         self,
         request: ecd_20200930_models.DescribeFlowStatisticRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeFlowStatisticResponse:
-        """
-        > You can query only the traffic data in the last 90 days.
-        
-        @param request: DescribeFlowStatisticRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeFlowStatisticResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.page_number):
@@ -8005,21 +4546,14 @@
         )
 
     async def describe_flow_statistic_with_options_async(
         self,
         request: ecd_20200930_models.DescribeFlowStatisticRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeFlowStatisticResponse:
-        """
-        > You can query only the traffic data in the last 90 days.
-        
-        @param request: DescribeFlowStatisticRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeFlowStatisticResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.page_number):
@@ -8049,33 +4583,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_flow_statistic(
         self,
         request: ecd_20200930_models.DescribeFlowStatisticRequest,
     ) -> ecd_20200930_models.DescribeFlowStatisticResponse:
-        """
-        > You can query only the traffic data in the last 90 days.
-        
-        @param request: DescribeFlowStatisticRequest
-        @return: DescribeFlowStatisticResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_flow_statistic_with_options(request, runtime)
 
     async def describe_flow_statistic_async(
         self,
         request: ecd_20200930_models.DescribeFlowStatisticRequest,
     ) -> ecd_20200930_models.DescribeFlowStatisticResponse:
-        """
-        > You can query only the traffic data in the last 90 days.
-        
-        @param request: DescribeFlowStatisticRequest
-        @return: DescribeFlowStatisticResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_flow_statistic_with_options_async(request, runtime)
 
     def describe_fota_pending_desktops_with_options(
         self,
         request: ecd_20200930_models.DescribeFotaPendingDesktopsRequest,
         runtime: util_models.RuntimeOptions,
@@ -8314,21 +4836,14 @@
         return await self.describe_front_vul_patch_list_with_options_async(request, runtime)
 
     def describe_grouped_vul_with_options(
         self,
         request: ecd_20200930_models.DescribeGroupedVulRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeGroupedVulResponse:
-        """
-        The number of vulnerabilities processed.
-        
-        @param request: DescribeGroupedVulRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeGroupedVulResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.dealed):
             query['Dealed'] = request.dealed
         if not UtilClient.is_unset(request.lang):
@@ -8363,21 +4878,14 @@
         )
 
     async def describe_grouped_vul_with_options_async(
         self,
         request: ecd_20200930_models.DescribeGroupedVulRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeGroupedVulResponse:
-        """
-        The number of vulnerabilities processed.
-        
-        @param request: DescribeGroupedVulRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeGroupedVulResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.dealed):
             query['Dealed'] = request.dealed
         if not UtilClient.is_unset(request.lang):
@@ -8411,33 +4919,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_grouped_vul(
         self,
         request: ecd_20200930_models.DescribeGroupedVulRequest,
     ) -> ecd_20200930_models.DescribeGroupedVulResponse:
-        """
-        The number of vulnerabilities processed.
-        
-        @param request: DescribeGroupedVulRequest
-        @return: DescribeGroupedVulResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_grouped_vul_with_options(request, runtime)
 
     async def describe_grouped_vul_async(
         self,
         request: ecd_20200930_models.DescribeGroupedVulRequest,
     ) -> ecd_20200930_models.DescribeGroupedVulResponse:
-        """
-        The number of vulnerabilities processed.
-        
-        @param request: DescribeGroupedVulRequest
-        @return: DescribeGroupedVulResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_grouped_vul_with_options_async(request, runtime)
 
     def describe_image_modified_records_with_options(
         self,
         request: ecd_20200930_models.DescribeImageModifiedRecordsRequest,
         runtime: util_models.RuntimeOptions,
@@ -8598,24 +5094,22 @@
         request: ecd_20200930_models.DescribeImagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeImagesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_instance_type):
             query['DesktopInstanceType'] = request.desktop_instance_type
-        if not UtilClient.is_unset(request.fota_version):
-            query['FotaVersion'] = request.fota_version
+        if not UtilClient.is_unset(request.fota_channel):
+            query['FotaChannel'] = request.fota_channel
         if not UtilClient.is_unset(request.gpu_category):
             query['GpuCategory'] = request.gpu_category
         if not UtilClient.is_unset(request.gpu_driver_version):
             query['GpuDriverVersion'] = request.gpu_driver_version
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
-        if not UtilClient.is_unset(request.image_name):
-            query['ImageName'] = request.image_name
         if not UtilClient.is_unset(request.image_status):
             query['ImageStatus'] = request.image_status
         if not UtilClient.is_unset(request.image_type):
             query['ImageType'] = request.image_type
         if not UtilClient.is_unset(request.language_type):
             query['LanguageType'] = request.language_type
         if not UtilClient.is_unset(request.max_results):
@@ -8624,16 +5118,14 @@
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.os_type):
             query['OsType'] = request.os_type
         if not UtilClient.is_unset(request.protocol_type):
             query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.session_type):
-            query['SessionType'] = request.session_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeImages',
             version='2020-09-30',
             protocol='HTTPS',
@@ -8654,24 +5146,22 @@
         request: ecd_20200930_models.DescribeImagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeImagesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_instance_type):
             query['DesktopInstanceType'] = request.desktop_instance_type
-        if not UtilClient.is_unset(request.fota_version):
-            query['FotaVersion'] = request.fota_version
+        if not UtilClient.is_unset(request.fota_channel):
+            query['FotaChannel'] = request.fota_channel
         if not UtilClient.is_unset(request.gpu_category):
             query['GpuCategory'] = request.gpu_category
         if not UtilClient.is_unset(request.gpu_driver_version):
             query['GpuDriverVersion'] = request.gpu_driver_version
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
-        if not UtilClient.is_unset(request.image_name):
-            query['ImageName'] = request.image_name
         if not UtilClient.is_unset(request.image_status):
             query['ImageStatus'] = request.image_status
         if not UtilClient.is_unset(request.image_type):
             query['ImageType'] = request.image_type
         if not UtilClient.is_unset(request.language_type):
             query['LanguageType'] = request.language_type
         if not UtilClient.is_unset(request.max_results):
@@ -8680,16 +5170,14 @@
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.os_type):
             query['OsType'] = request.os_type
         if not UtilClient.is_unset(request.protocol_type):
             query['ProtocolType'] = request.protocol_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.session_type):
-            query['SessionType'] = request.session_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeImages',
             version='2020-09-30',
             protocol='HTTPS',
@@ -8720,47 +5208,22 @@
         return await self.describe_images_with_options_async(request, runtime)
 
     def describe_invocations_with_options(
         self,
         request: ecd_20200930_models.DescribeInvocationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeInvocationsResponse:
-        """
-        The error message that is returned if the command failed to be sent or run.
-        *   If null is returned, the command is run normally.
-        *   If "the specified instance does not exist" is returned, the specified cloud desktop does not exist or is released.
-        *   If "the instance has released when create task" is returned, the specified cloud desktop is released during the command execution.
-        *   If "the instance is not running when create task" is returned, the specified cloud desktop is not in the Running state when the execution is created.
-        *   If "the command is not applicable" is returned, the command cannot be run on the specified cloud desktop.
-        *   If "the aliyun service is not running on the instance" is returned, Cloud Assistant is not running.
-        *   If "the aliyun service in the instance does not response" is returned, Cloud Assistant does not respond to your request.
-        *   If "the aliyun service in the instance is upgrading now" is returned, Cloud Assistant is being upgraded.
-        *   If "the aliyun service in the instance need upgrade" is returned, you must upgrade Cloud Assistant.
-        *   If "the command delivery has been timeout" is returned, the operation to send the command times out.
-        *   If "the command execution has been timeout" is returned, the command execution times out.
-        *   If "the command execution got an exception" is returned, an exception occurs during the command execution.
-        *   If "the command execution has been interrupted" is returned, the command execution is interrupted.
-        *   If "the command execution exit code is not zero" is returned, the command execution is complete, but the exit code is not 0.
-        
-        @param request: DescribeInvocationsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeInvocationsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.command_type):
             query['CommandType'] = request.command_type
         if not UtilClient.is_unset(request.content_encoding):
             query['ContentEncoding'] = request.content_encoding
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.desktop_ids):
-            query['DesktopIds'] = request.desktop_ids
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.include_output):
             query['IncludeOutput'] = request.include_output
         if not UtilClient.is_unset(request.invoke_id):
             query['InvokeId'] = request.invoke_id
         if not UtilClient.is_unset(request.invoke_status):
             query['InvokeStatus'] = request.invoke_status
         if not UtilClient.is_unset(request.max_results):
@@ -8789,47 +5252,22 @@
         )
 
     async def describe_invocations_with_options_async(
         self,
         request: ecd_20200930_models.DescribeInvocationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeInvocationsResponse:
-        """
-        The error message that is returned if the command failed to be sent or run.
-        *   If null is returned, the command is run normally.
-        *   If "the specified instance does not exist" is returned, the specified cloud desktop does not exist or is released.
-        *   If "the instance has released when create task" is returned, the specified cloud desktop is released during the command execution.
-        *   If "the instance is not running when create task" is returned, the specified cloud desktop is not in the Running state when the execution is created.
-        *   If "the command is not applicable" is returned, the command cannot be run on the specified cloud desktop.
-        *   If "the aliyun service is not running on the instance" is returned, Cloud Assistant is not running.
-        *   If "the aliyun service in the instance does not response" is returned, Cloud Assistant does not respond to your request.
-        *   If "the aliyun service in the instance is upgrading now" is returned, Cloud Assistant is being upgraded.
-        *   If "the aliyun service in the instance need upgrade" is returned, you must upgrade Cloud Assistant.
-        *   If "the command delivery has been timeout" is returned, the operation to send the command times out.
-        *   If "the command execution has been timeout" is returned, the command execution times out.
-        *   If "the command execution got an exception" is returned, an exception occurs during the command execution.
-        *   If "the command execution has been interrupted" is returned, the command execution is interrupted.
-        *   If "the command execution exit code is not zero" is returned, the command execution is complete, but the exit code is not 0.
-        
-        @param request: DescribeInvocationsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeInvocationsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.command_type):
             query['CommandType'] = request.command_type
         if not UtilClient.is_unset(request.content_encoding):
             query['ContentEncoding'] = request.content_encoding
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.desktop_ids):
-            query['DesktopIds'] = request.desktop_ids
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.include_output):
             query['IncludeOutput'] = request.include_output
         if not UtilClient.is_unset(request.invoke_id):
             query['InvokeId'] = request.invoke_id
         if not UtilClient.is_unset(request.invoke_status):
             query['InvokeStatus'] = request.invoke_status
         if not UtilClient.is_unset(request.max_results):
@@ -8857,61 +5295,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_invocations(
         self,
         request: ecd_20200930_models.DescribeInvocationsRequest,
     ) -> ecd_20200930_models.DescribeInvocationsResponse:
-        """
-        The error message that is returned if the command failed to be sent or run.
-        *   If null is returned, the command is run normally.
-        *   If "the specified instance does not exist" is returned, the specified cloud desktop does not exist or is released.
-        *   If "the instance has released when create task" is returned, the specified cloud desktop is released during the command execution.
-        *   If "the instance is not running when create task" is returned, the specified cloud desktop is not in the Running state when the execution is created.
-        *   If "the command is not applicable" is returned, the command cannot be run on the specified cloud desktop.
-        *   If "the aliyun service is not running on the instance" is returned, Cloud Assistant is not running.
-        *   If "the aliyun service in the instance does not response" is returned, Cloud Assistant does not respond to your request.
-        *   If "the aliyun service in the instance is upgrading now" is returned, Cloud Assistant is being upgraded.
-        *   If "the aliyun service in the instance need upgrade" is returned, you must upgrade Cloud Assistant.
-        *   If "the command delivery has been timeout" is returned, the operation to send the command times out.
-        *   If "the command execution has been timeout" is returned, the command execution times out.
-        *   If "the command execution got an exception" is returned, an exception occurs during the command execution.
-        *   If "the command execution has been interrupted" is returned, the command execution is interrupted.
-        *   If "the command execution exit code is not zero" is returned, the command execution is complete, but the exit code is not 0.
-        
-        @param request: DescribeInvocationsRequest
-        @return: DescribeInvocationsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_invocations_with_options(request, runtime)
 
     async def describe_invocations_async(
         self,
         request: ecd_20200930_models.DescribeInvocationsRequest,
     ) -> ecd_20200930_models.DescribeInvocationsResponse:
-        """
-        The error message that is returned if the command failed to be sent or run.
-        *   If null is returned, the command is run normally.
-        *   If "the specified instance does not exist" is returned, the specified cloud desktop does not exist or is released.
-        *   If "the instance has released when create task" is returned, the specified cloud desktop is released during the command execution.
-        *   If "the instance is not running when create task" is returned, the specified cloud desktop is not in the Running state when the execution is created.
-        *   If "the command is not applicable" is returned, the command cannot be run on the specified cloud desktop.
-        *   If "the aliyun service is not running on the instance" is returned, Cloud Assistant is not running.
-        *   If "the aliyun service in the instance does not response" is returned, Cloud Assistant does not respond to your request.
-        *   If "the aliyun service in the instance is upgrading now" is returned, Cloud Assistant is being upgraded.
-        *   If "the aliyun service in the instance need upgrade" is returned, you must upgrade Cloud Assistant.
-        *   If "the command delivery has been timeout" is returned, the operation to send the command times out.
-        *   If "the command execution has been timeout" is returned, the command execution times out.
-        *   If "the command execution got an exception" is returned, an exception occurs during the command execution.
-        *   If "the command execution has been interrupted" is returned, the command execution is interrupted.
-        *   If "the command execution exit code is not zero" is returned, the command execution is complete, but the exit code is not 0.
-        
-        @param request: DescribeInvocationsRequest
-        @return: DescribeInvocationsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_invocations_with_options_async(request, runtime)
 
     def describe_kms_keys_with_options(
         self,
         request: ecd_20200930_models.DescribeKmsKeysRequest,
         runtime: util_models.RuntimeOptions,
@@ -8986,16 +5384,14 @@
         request: ecd_20200930_models.DescribeNASFileSystemsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeNASFileSystemsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
-        if not UtilClient.is_unset(request.match_compatible_profile):
-            query['MatchCompatibleProfile'] = request.match_compatible_profile
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
@@ -9024,16 +5420,14 @@
         request: ecd_20200930_models.DescribeNASFileSystemsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeNASFileSystemsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
-        if not UtilClient.is_unset(request.match_compatible_profile):
-            query['MatchCompatibleProfile'] = request.match_compatible_profile
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
@@ -9258,16 +5652,14 @@
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePolicyGroups',
             version='2020-09-30',
             protocol='HTTPS',
@@ -9294,16 +5686,14 @@
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePolicyGroups',
             version='2020-09-30',
             protocol='HTTPS',
@@ -9329,255 +5719,99 @@
     async def describe_policy_groups_async(
         self,
         request: ecd_20200930_models.DescribePolicyGroupsRequest,
     ) -> ecd_20200930_models.DescribePolicyGroupsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_policy_groups_with_options_async(request, runtime)
 
-    def describe_price_with_options(
+    def describe_recordings_with_options(
         self,
-        request: ecd_20200930_models.DescribePriceRequest,
+        request: ecd_20200930_models.DescribeRecordingsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribePriceResponse:
-        """
-        ## Usage notes
-        The request parameters vary based on the type of desktop resources whose price you want to query. Take note of the following items:
-        *   If you set ResourceType to OfficeSite, you must specify InstanceType.
-        *   If you set ResourceType to Bandwidth, the pay-by-data-transfer metering method is used for network billing.
-        *   If you set ResourceType to Desktop, you must specify InstanceType, RootDiskSizeGib, and UserDiskSizeGib. You can specify OsType, PeriodUnit, Period, and Amount based on your business requirements.
-        > Before you call this operation to query the prices of cloud desktops by setting ResourceType to Desktop, you must know the desktop types and disk sizes that EDS provides. The disk sizes vary based on the desktop types. For more information, see [Cloud desktop types](~~188609~~).
-        
-        @param request: DescribePriceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribePriceResponse
-        """
+    ) -> ecd_20200930_models.DescribeRecordingsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.amount):
-            query['Amount'] = request.amount
-        if not UtilClient.is_unset(request.bandwidth):
-            query['Bandwidth'] = request.bandwidth
-        if not UtilClient.is_unset(request.bundle_models):
-            query['BundleModels'] = request.bundle_models
-        if not UtilClient.is_unset(request.edu_cds_size):
-            query['EduCdsSize'] = request.edu_cds_size
-        if not UtilClient.is_unset(request.edu_committed_time):
-            query['EduCommittedTime'] = request.edu_committed_time
-        if not UtilClient.is_unset(request.edu_desktop_bundle_id):
-            query['EduDesktopBundleId'] = request.edu_desktop_bundle_id
-        if not UtilClient.is_unset(request.edu_desktop_num):
-            query['EduDesktopNum'] = request.edu_desktop_num
-        if not UtilClient.is_unset(request.edu_room_classify):
-            query['EduRoomClassify'] = request.edu_room_classify
-        if not UtilClient.is_unset(request.edu_student_bundle_id):
-            query['EduStudentBundleId'] = request.edu_student_bundle_id
-        if not UtilClient.is_unset(request.edu_student_num):
-            query['EduStudentNum'] = request.edu_student_num
-        if not UtilClient.is_unset(request.edu_teacher_bundle_id):
-            query['EduTeacherBundleId'] = request.edu_teacher_bundle_id
-        if not UtilClient.is_unset(request.edu_teacher_num):
-            query['EduTeacherNum'] = request.edu_teacher_num
-        if not UtilClient.is_unset(request.group_desktop_count):
-            query['GroupDesktopCount'] = request.group_desktop_count
-        if not UtilClient.is_unset(request.hardware_version):
-            query['HardwareVersion'] = request.hardware_version
-        if not UtilClient.is_unset(request.instance_type):
-            query['InstanceType'] = request.instance_type
-        if not UtilClient.is_unset(request.internet_charge_type):
-            query['InternetChargeType'] = request.internet_charge_type
-        if not UtilClient.is_unset(request.os_type):
-            query['OsType'] = request.os_type
-        if not UtilClient.is_unset(request.package_size):
-            query['PackageSize'] = request.package_size
-        if not UtilClient.is_unset(request.period):
-            query['Period'] = request.period
-        if not UtilClient.is_unset(request.period_unit):
-            query['PeriodUnit'] = request.period_unit
-        if not UtilClient.is_unset(request.promotion_id):
-            query['PromotionId'] = request.promotion_id
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_type):
-            query['ResourceType'] = request.resource_type
-        if not UtilClient.is_unset(request.root_disk_performance_level):
-            query['RootDiskPerformanceLevel'] = request.root_disk_performance_level
-        if not UtilClient.is_unset(request.root_disk_size_gib):
-            query['RootDiskSizeGib'] = request.root_disk_size_gib
-        if not UtilClient.is_unset(request.sp_period_info):
-            query['SpPeriodInfo'] = request.sp_period_info
-        if not UtilClient.is_unset(request.sp_price):
-            query['SpPrice'] = request.sp_price
-        if not UtilClient.is_unset(request.sp_type):
-            query['SpType'] = request.sp_type
-        if not UtilClient.is_unset(request.user_disk_performance_level):
-            query['UserDiskPerformanceLevel'] = request.user_disk_performance_level
-        if not UtilClient.is_unset(request.user_disk_size_gib):
-            query['UserDiskSizeGib'] = request.user_disk_size_gib
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='DescribePrice',
+            action='DescribeRecordings',
             version='2020-09-30',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            ecd_20200930_models.DescribePriceResponse(),
+            ecd_20200930_models.DescribeRecordingsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def describe_price_with_options_async(
+    async def describe_recordings_with_options_async(
         self,
-        request: ecd_20200930_models.DescribePriceRequest,
+        request: ecd_20200930_models.DescribeRecordingsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribePriceResponse:
-        """
-        ## Usage notes
-        The request parameters vary based on the type of desktop resources whose price you want to query. Take note of the following items:
-        *   If you set ResourceType to OfficeSite, you must specify InstanceType.
-        *   If you set ResourceType to Bandwidth, the pay-by-data-transfer metering method is used for network billing.
-        *   If you set ResourceType to Desktop, you must specify InstanceType, RootDiskSizeGib, and UserDiskSizeGib. You can specify OsType, PeriodUnit, Period, and Amount based on your business requirements.
-        > Before you call this operation to query the prices of cloud desktops by setting ResourceType to Desktop, you must know the desktop types and disk sizes that EDS provides. The disk sizes vary based on the desktop types. For more information, see [Cloud desktop types](~~188609~~).
-        
-        @param request: DescribePriceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribePriceResponse
-        """
+    ) -> ecd_20200930_models.DescribeRecordingsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.amount):
-            query['Amount'] = request.amount
-        if not UtilClient.is_unset(request.bandwidth):
-            query['Bandwidth'] = request.bandwidth
-        if not UtilClient.is_unset(request.bundle_models):
-            query['BundleModels'] = request.bundle_models
-        if not UtilClient.is_unset(request.edu_cds_size):
-            query['EduCdsSize'] = request.edu_cds_size
-        if not UtilClient.is_unset(request.edu_committed_time):
-            query['EduCommittedTime'] = request.edu_committed_time
-        if not UtilClient.is_unset(request.edu_desktop_bundle_id):
-            query['EduDesktopBundleId'] = request.edu_desktop_bundle_id
-        if not UtilClient.is_unset(request.edu_desktop_num):
-            query['EduDesktopNum'] = request.edu_desktop_num
-        if not UtilClient.is_unset(request.edu_room_classify):
-            query['EduRoomClassify'] = request.edu_room_classify
-        if not UtilClient.is_unset(request.edu_student_bundle_id):
-            query['EduStudentBundleId'] = request.edu_student_bundle_id
-        if not UtilClient.is_unset(request.edu_student_num):
-            query['EduStudentNum'] = request.edu_student_num
-        if not UtilClient.is_unset(request.edu_teacher_bundle_id):
-            query['EduTeacherBundleId'] = request.edu_teacher_bundle_id
-        if not UtilClient.is_unset(request.edu_teacher_num):
-            query['EduTeacherNum'] = request.edu_teacher_num
-        if not UtilClient.is_unset(request.group_desktop_count):
-            query['GroupDesktopCount'] = request.group_desktop_count
-        if not UtilClient.is_unset(request.hardware_version):
-            query['HardwareVersion'] = request.hardware_version
-        if not UtilClient.is_unset(request.instance_type):
-            query['InstanceType'] = request.instance_type
-        if not UtilClient.is_unset(request.internet_charge_type):
-            query['InternetChargeType'] = request.internet_charge_type
-        if not UtilClient.is_unset(request.os_type):
-            query['OsType'] = request.os_type
-        if not UtilClient.is_unset(request.package_size):
-            query['PackageSize'] = request.package_size
-        if not UtilClient.is_unset(request.period):
-            query['Period'] = request.period
-        if not UtilClient.is_unset(request.period_unit):
-            query['PeriodUnit'] = request.period_unit
-        if not UtilClient.is_unset(request.promotion_id):
-            query['PromotionId'] = request.promotion_id
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_type):
-            query['ResourceType'] = request.resource_type
-        if not UtilClient.is_unset(request.root_disk_performance_level):
-            query['RootDiskPerformanceLevel'] = request.root_disk_performance_level
-        if not UtilClient.is_unset(request.root_disk_size_gib):
-            query['RootDiskSizeGib'] = request.root_disk_size_gib
-        if not UtilClient.is_unset(request.sp_period_info):
-            query['SpPeriodInfo'] = request.sp_period_info
-        if not UtilClient.is_unset(request.sp_price):
-            query['SpPrice'] = request.sp_price
-        if not UtilClient.is_unset(request.sp_type):
-            query['SpType'] = request.sp_type
-        if not UtilClient.is_unset(request.user_disk_performance_level):
-            query['UserDiskPerformanceLevel'] = request.user_disk_performance_level
-        if not UtilClient.is_unset(request.user_disk_size_gib):
-            query['UserDiskSizeGib'] = request.user_disk_size_gib
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='DescribePrice',
+            action='DescribeRecordings',
             version='2020-09-30',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            ecd_20200930_models.DescribePriceResponse(),
+            ecd_20200930_models.DescribeRecordingsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def describe_price(
+    def describe_recordings(
         self,
-        request: ecd_20200930_models.DescribePriceRequest,
-    ) -> ecd_20200930_models.DescribePriceResponse:
-        """
-        ## Usage notes
-        The request parameters vary based on the type of desktop resources whose price you want to query. Take note of the following items:
-        *   If you set ResourceType to OfficeSite, you must specify InstanceType.
-        *   If you set ResourceType to Bandwidth, the pay-by-data-transfer metering method is used for network billing.
-        *   If you set ResourceType to Desktop, you must specify InstanceType, RootDiskSizeGib, and UserDiskSizeGib. You can specify OsType, PeriodUnit, Period, and Amount based on your business requirements.
-        > Before you call this operation to query the prices of cloud desktops by setting ResourceType to Desktop, you must know the desktop types and disk sizes that EDS provides. The disk sizes vary based on the desktop types. For more information, see [Cloud desktop types](~~188609~~).
-        
-        @param request: DescribePriceRequest
-        @return: DescribePriceResponse
-        """
+        request: ecd_20200930_models.DescribeRecordingsRequest,
+    ) -> ecd_20200930_models.DescribeRecordingsResponse:
         runtime = util_models.RuntimeOptions()
-        return self.describe_price_with_options(request, runtime)
+        return self.describe_recordings_with_options(request, runtime)
 
-    async def describe_price_async(
+    async def describe_recordings_async(
         self,
-        request: ecd_20200930_models.DescribePriceRequest,
-    ) -> ecd_20200930_models.DescribePriceResponse:
-        """
-        ## Usage notes
-        The request parameters vary based on the type of desktop resources whose price you want to query. Take note of the following items:
-        *   If you set ResourceType to OfficeSite, you must specify InstanceType.
-        *   If you set ResourceType to Bandwidth, the pay-by-data-transfer metering method is used for network billing.
-        *   If you set ResourceType to Desktop, you must specify InstanceType, RootDiskSizeGib, and UserDiskSizeGib. You can specify OsType, PeriodUnit, Period, and Amount based on your business requirements.
-        > Before you call this operation to query the prices of cloud desktops by setting ResourceType to Desktop, you must know the desktop types and disk sizes that EDS provides. The disk sizes vary based on the desktop types. For more information, see [Cloud desktop types](~~188609~~).
-        
-        @param request: DescribePriceRequest
-        @return: DescribePriceResponse
-        """
+        request: ecd_20200930_models.DescribeRecordingsRequest,
+    ) -> ecd_20200930_models.DescribeRecordingsResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.describe_price_with_options_async(request, runtime)
+        return await self.describe_recordings_with_options_async(request, runtime)
 
     def describe_regions_with_options(
         self,
         request: ecd_20200930_models.DescribeRegionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeRegionsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.accept_language):
-            query['AcceptLanguage'] = request.accept_language
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRegions',
@@ -9598,16 +5832,14 @@
     async def describe_regions_with_options_async(
         self,
         request: ecd_20200930_models.DescribeRegionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeRegionsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.accept_language):
-            query['AcceptLanguage'] = request.accept_language
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRegions',
@@ -9861,135 +6093,31 @@
     async def describe_security_event_operations_async(
         self,
         request: ecd_20200930_models.DescribeSecurityEventOperationsRequest,
     ) -> ecd_20200930_models.DescribeSecurityEventOperationsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_security_event_operations_with_options_async(request, runtime)
 
-    def describe_session_statistic_with_options(
-        self,
-        request: ecd_20200930_models.DescribeSessionStatisticRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeSessionStatisticResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.end_time):
-            query['EndTime'] = request.end_time
-        if not UtilClient.is_unset(request.office_site_id):
-            query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.period):
-            query['Period'] = request.period
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.search_region_id):
-            query['SearchRegionId'] = request.search_region_id
-        if not UtilClient.is_unset(request.start_time):
-            query['StartTime'] = request.start_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeSessionStatistic',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeSessionStatisticResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_session_statistic_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeSessionStatisticRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeSessionStatisticResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.end_time):
-            query['EndTime'] = request.end_time
-        if not UtilClient.is_unset(request.office_site_id):
-            query['OfficeSiteId'] = request.office_site_id
-        if not UtilClient.is_unset(request.period):
-            query['Period'] = request.period
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.search_region_id):
-            query['SearchRegionId'] = request.search_region_id
-        if not UtilClient.is_unset(request.start_time):
-            query['StartTime'] = request.start_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeSessionStatistic',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeSessionStatisticResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_session_statistic(
-        self,
-        request: ecd_20200930_models.DescribeSessionStatisticRequest,
-    ) -> ecd_20200930_models.DescribeSessionStatisticResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_session_statistic_with_options(request, runtime)
-
-    async def describe_session_statistic_async(
-        self,
-        request: ecd_20200930_models.DescribeSessionStatisticRequest,
-    ) -> ecd_20200930_models.DescribeSessionStatisticResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_session_statistic_with_options_async(request, runtime)
-
     def describe_snapshots_with_options(
         self,
         request: ecd_20200930_models.DescribeSnapshotsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeSnapshotsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.creator):
-            query['Creator'] = request.creator
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.desktop_name):
-            query['DesktopName'] = request.desktop_name
-        if not UtilClient.is_unset(request.end_time):
-            query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.snapshot_id):
             query['SnapshotId'] = request.snapshot_id
-        if not UtilClient.is_unset(request.snapshot_name):
-            query['SnapshotName'] = request.snapshot_name
-        if not UtilClient.is_unset(request.snapshot_type):
-            query['SnapshotType'] = request.snapshot_type
-        if not UtilClient.is_unset(request.source_disk_type):
-            query['SourceDiskType'] = request.source_disk_type
-        if not UtilClient.is_unset(request.start_time):
-            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeSnapshots',
             version='2020-09-30',
             protocol='HTTPS',
@@ -10008,38 +6136,24 @@
     async def describe_snapshots_with_options_async(
         self,
         request: ecd_20200930_models.DescribeSnapshotsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeSnapshotsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.creator):
-            query['Creator'] = request.creator
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.desktop_name):
-            query['DesktopName'] = request.desktop_name
-        if not UtilClient.is_unset(request.end_time):
-            query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.snapshot_id):
             query['SnapshotId'] = request.snapshot_id
-        if not UtilClient.is_unset(request.snapshot_name):
-            query['SnapshotName'] = request.snapshot_name
-        if not UtilClient.is_unset(request.snapshot_type):
-            query['SnapshotType'] = request.snapshot_type
-        if not UtilClient.is_unset(request.source_disk_type):
-            query['SourceDiskType'] = request.source_disk_type
-        if not UtilClient.is_unset(request.start_time):
-            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeSnapshots',
             version='2020-09-30',
             protocol='HTTPS',
@@ -10140,21 +6254,14 @@
         return await self.describe_susp_event_overview_with_options_async(request, runtime)
 
     def describe_susp_event_quara_files_with_options(
         self,
         request: ecd_20200930_models.DescribeSuspEventQuaraFilesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeSuspEventQuaraFilesResponse:
-        """
-        The path where the quarantined file is stored on the cloud desktop.
-        
-        @param request: DescribeSuspEventQuaraFilesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeSuspEventQuaraFilesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.page_size):
@@ -10183,21 +6290,14 @@
         )
 
     async def describe_susp_event_quara_files_with_options_async(
         self,
         request: ecd_20200930_models.DescribeSuspEventQuaraFilesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeSuspEventQuaraFilesResponse:
-        """
-        The path where the quarantined file is stored on the cloud desktop.
-        
-        @param request: DescribeSuspEventQuaraFilesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeSuspEventQuaraFilesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.page_size):
@@ -10225,33 +6325,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_susp_event_quara_files(
         self,
         request: ecd_20200930_models.DescribeSuspEventQuaraFilesRequest,
     ) -> ecd_20200930_models.DescribeSuspEventQuaraFilesResponse:
-        """
-        The path where the quarantined file is stored on the cloud desktop.
-        
-        @param request: DescribeSuspEventQuaraFilesRequest
-        @return: DescribeSuspEventQuaraFilesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_susp_event_quara_files_with_options(request, runtime)
 
     async def describe_susp_event_quara_files_async(
         self,
         request: ecd_20200930_models.DescribeSuspEventQuaraFilesRequest,
     ) -> ecd_20200930_models.DescribeSuspEventQuaraFilesResponse:
-        """
-        The path where the quarantined file is stored on the cloud desktop.
-        
-        @param request: DescribeSuspEventQuaraFilesRequest
-        @return: DescribeSuspEventQuaraFilesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_susp_event_quara_files_with_options_async(request, runtime)
 
     def describe_susp_events_with_options(
         self,
         request: ecd_20200930_models.DescribeSuspEventsRequest,
         runtime: util_models.RuntimeOptions,
@@ -10467,115 +6555,33 @@
     async def describe_user_connection_records_async(
         self,
         request: ecd_20200930_models.DescribeUserConnectionRecordsRequest,
     ) -> ecd_20200930_models.DescribeUserConnectionRecordsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_connection_records_with_options_async(request, runtime)
 
-    def describe_user_profile_path_rules_with_options(
-        self,
-        request: ecd_20200930_models.DescribeUserProfilePathRulesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeUserProfilePathRulesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.rule_type):
-            query['RuleType'] = request.rule_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeUserProfilePathRules',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeUserProfilePathRulesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_user_profile_path_rules_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeUserProfilePathRulesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeUserProfilePathRulesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.rule_type):
-            query['RuleType'] = request.rule_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeUserProfilePathRules',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeUserProfilePathRulesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_user_profile_path_rules(
-        self,
-        request: ecd_20200930_models.DescribeUserProfilePathRulesRequest,
-    ) -> ecd_20200930_models.DescribeUserProfilePathRulesResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_user_profile_path_rules_with_options(request, runtime)
-
-    async def describe_user_profile_path_rules_async(
-        self,
-        request: ecd_20200930_models.DescribeUserProfilePathRulesRequest,
-    ) -> ecd_20200930_models.DescribeUserProfilePathRulesResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_user_profile_path_rules_with_options_async(request, runtime)
-
     def describe_users_in_group_with_options(
         self,
         request: ecd_20200930_models.DescribeUsersInGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeUsersInGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.connect_state):
             query['ConnectState'] = request.connect_state
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.end_user_ids):
-            query['EndUserIds'] = request.end_user_ids
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.org_id):
-            query['OrgId'] = request.org_id
         if not UtilClient.is_unset(request.query_user_detail):
             query['QueryUserDetail'] = request.query_user_detail
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -10604,24 +6610,20 @@
         query = {}
         if not UtilClient.is_unset(request.connect_state):
             query['ConnectState'] = request.connect_state
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.end_user_ids):
-            query['EndUserIds'] = request.end_user_ids
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.org_id):
-            query['OrgId'] = request.org_id
         if not UtilClient.is_unset(request.query_user_detail):
             query['QueryUserDetail'] = request.query_user_detail
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -10651,88 +6653,14 @@
     async def describe_users_in_group_async(
         self,
         request: ecd_20200930_models.DescribeUsersInGroupRequest,
     ) -> ecd_20200930_models.DescribeUsersInGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_users_in_group_with_options_async(request, runtime)
 
-    def describe_users_password_with_options(
-        self,
-        request: ecd_20200930_models.DescribeUsersPasswordRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeUsersPasswordResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeUsersPassword',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeUsersPasswordResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_users_password_with_options_async(
-        self,
-        request: ecd_20200930_models.DescribeUsersPasswordRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DescribeUsersPasswordResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeUsersPassword',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DescribeUsersPasswordResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_users_password(
-        self,
-        request: ecd_20200930_models.DescribeUsersPasswordRequest,
-    ) -> ecd_20200930_models.DescribeUsersPasswordResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_users_password_with_options(request, runtime)
-
-    async def describe_users_password_async(
-        self,
-        request: ecd_20200930_models.DescribeUsersPasswordRequest,
-    ) -> ecd_20200930_models.DescribeUsersPasswordResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_users_password_with_options_async(request, runtime)
-
     def describe_virtual_mfadevices_with_options(
         self,
         request: ecd_20200930_models.DescribeVirtualMFADevicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DescribeVirtualMFADevicesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -10912,16 +6840,14 @@
             query['AliasName'] = request.alias_name
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.dealed):
             query['Dealed'] = request.dealed
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
-        if not UtilClient.is_unset(request.name):
-            query['Name'] = request.name
         if not UtilClient.is_unset(request.necessity):
             query['Necessity'] = request.necessity
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
@@ -10958,16 +6884,14 @@
             query['AliasName'] = request.alias_name
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.dealed):
             query['Dealed'] = request.dealed
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
-        if not UtilClient.is_unset(request.name):
-            query['Name'] = request.name
         if not UtilClient.is_unset(request.necessity):
             query['Necessity'] = request.necessity
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
@@ -11221,104 +7145,14 @@
     async def detach_cen_async(
         self,
         request: ecd_20200930_models.DetachCenRequest,
     ) -> ecd_20200930_models.DetachCenResponse:
         runtime = util_models.RuntimeOptions()
         return await self.detach_cen_with_options_async(request, runtime)
 
-    def detach_end_user_with_options(
-        self,
-        request: ecd_20200930_models.DetachEndUserRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DetachEndUserResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.ad_domain):
-            query['AdDomain'] = request.ad_domain
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_id):
-            query['DeviceId'] = request.device_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region):
-            query['Region'] = request.region
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DetachEndUser',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DetachEndUserResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def detach_end_user_with_options_async(
-        self,
-        request: ecd_20200930_models.DetachEndUserRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.DetachEndUserResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.ad_domain):
-            query['AdDomain'] = request.ad_domain
-        if not UtilClient.is_unset(request.client_type):
-            query['ClientType'] = request.client_type
-        if not UtilClient.is_unset(request.device_id):
-            query['DeviceId'] = request.device_id
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region):
-            query['Region'] = request.region
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DetachEndUser',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.DetachEndUserResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def detach_end_user(
-        self,
-        request: ecd_20200930_models.DetachEndUserRequest,
-    ) -> ecd_20200930_models.DetachEndUserResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.detach_end_user_with_options(request, runtime)
-
-    async def detach_end_user_async(
-        self,
-        request: ecd_20200930_models.DetachEndUserRequest,
-    ) -> ecd_20200930_models.DetachEndUserResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.detach_end_user_with_options_async(request, runtime)
-
     def disable_desktops_in_group_with_options(
         self,
         request: ecd_20200930_models.DisableDesktopsInGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.DisableDesktopsInGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -11480,18 +7314,14 @@
             query['DesktopName'] = request.desktop_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
-        if not UtilClient.is_unset(request.event_types):
-            query['EventTypes'] = request.event_types
-        if not UtilClient.is_unset(request.lang_type):
-            query['LangType'] = request.lang_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
             query['OfficeSiteName'] = request.office_site_name
         if not UtilClient.is_unset(request.region_id):
@@ -11530,18 +7360,14 @@
             query['DesktopName'] = request.desktop_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
-        if not UtilClient.is_unset(request.event_types):
-            query['EventTypes'] = request.event_types
-        if not UtilClient.is_unset(request.lang_type):
-            query['LangType'] = request.lang_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
             query['OfficeSiteName'] = request.office_site_name
         if not UtilClient.is_unset(request.region_id):
@@ -11813,97 +7639,21 @@
     async def export_desktop_list_info_async(
         self,
         request: ecd_20200930_models.ExportDesktopListInfoRequest,
     ) -> ecd_20200930_models.ExportDesktopListInfoResponse:
         runtime = util_models.RuntimeOptions()
         return await self.export_desktop_list_info_with_options_async(request, runtime)
 
-    def get_async_task_with_options(
-        self,
-        request: ecd_20200930_models.GetAsyncTaskRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.GetAsyncTaskResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.async_task_id):
-            query['AsyncTaskId'] = request.async_task_id
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='GetAsyncTask',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.GetAsyncTaskResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def get_async_task_with_options_async(
-        self,
-        request: ecd_20200930_models.GetAsyncTaskRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.GetAsyncTaskResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.async_task_id):
-            query['AsyncTaskId'] = request.async_task_id
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='GetAsyncTask',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.GetAsyncTaskResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def get_async_task(
-        self,
-        request: ecd_20200930_models.GetAsyncTaskRequest,
-    ) -> ecd_20200930_models.GetAsyncTaskResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.get_async_task_with_options(request, runtime)
-
-    async def get_async_task_async(
-        self,
-        request: ecd_20200930_models.GetAsyncTaskRequest,
-    ) -> ecd_20200930_models.GetAsyncTaskResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.get_async_task_with_options_async(request, runtime)
-
     def get_connection_ticket_with_options(
         self,
         request: ecd_20200930_models.GetConnectionTicketRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.GetConnectionTicketResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.command_content):
-            query['CommandContent'] = request.command_content
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
@@ -11940,16 +7690,14 @@
     async def get_connection_ticket_with_options_async(
         self,
         request: ecd_20200930_models.GetConnectionTicketRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.GetConnectionTicketResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.command_content):
-            query['CommandContent'] = request.command_content
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
@@ -12146,21 +7894,14 @@
         return await self.get_office_site_sso_status_with_options_async(request, runtime)
 
     def get_sp_metadata_with_options(
         self,
         request: ecd_20200930_models.GetSpMetadataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.GetSpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: GetSpMetadataRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: GetSpMetadataResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
@@ -12185,21 +7926,14 @@
         )
 
     async def get_sp_metadata_with_options_async(
         self,
         request: ecd_20200930_models.GetSpMetadataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.GetSpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: GetSpMetadataRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: GetSpMetadataResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
@@ -12223,33 +7957,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_sp_metadata(
         self,
         request: ecd_20200930_models.GetSpMetadataRequest,
     ) -> ecd_20200930_models.GetSpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: GetSpMetadataRequest
-        @return: GetSpMetadataResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.get_sp_metadata_with_options(request, runtime)
 
     async def get_sp_metadata_async(
         self,
         request: ecd_20200930_models.GetSpMetadataRequest,
     ) -> ecd_20200930_models.GetSpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: GetSpMetadataRequest
-        @return: GetSpMetadataResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.get_sp_metadata_with_options_async(request, runtime)
 
     def handle_security_events_with_options(
         self,
         request: ecd_20200930_models.HandleSecurityEventsRequest,
         runtime: util_models.RuntimeOptions,
@@ -12327,198 +8049,14 @@
     async def handle_security_events_async(
         self,
         request: ecd_20200930_models.HandleSecurityEventsRequest,
     ) -> ecd_20200930_models.HandleSecurityEventsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.handle_security_events_with_options_async(request, runtime)
 
-    def hibernate_desktops_with_options(
-        self,
-        request: ecd_20200930_models.HibernateDesktopsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.HibernateDesktopsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='HibernateDesktops',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.HibernateDesktopsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def hibernate_desktops_with_options_async(
-        self,
-        request: ecd_20200930_models.HibernateDesktopsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.HibernateDesktopsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='HibernateDesktops',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.HibernateDesktopsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def hibernate_desktops(
-        self,
-        request: ecd_20200930_models.HibernateDesktopsRequest,
-    ) -> ecd_20200930_models.HibernateDesktopsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.hibernate_desktops_with_options(request, runtime)
-
-    async def hibernate_desktops_async(
-        self,
-        request: ecd_20200930_models.HibernateDesktopsRequest,
-    ) -> ecd_20200930_models.HibernateDesktopsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.hibernate_desktops_with_options_async(request, runtime)
-
-    def list_cds_files_with_options(
-        self,
-        tmp_req: ecd_20200930_models.ListCdsFilesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ListCdsFilesResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.ListCdsFilesShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.file_ids):
-            request.file_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.file_ids, 'FileIds', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_ids_shrink):
-            query['FileIds'] = request.file_ids_shrink
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.order_type):
-            query['OrderType'] = request.order_type
-        if not UtilClient.is_unset(request.parent_file_id):
-            query['ParentFileId'] = request.parent_file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ListCdsFiles',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ListCdsFilesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def list_cds_files_with_options_async(
-        self,
-        tmp_req: ecd_20200930_models.ListCdsFilesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ListCdsFilesResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.ListCdsFilesShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.file_ids):
-            request.file_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.file_ids, 'FileIds', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_ids_shrink):
-            query['FileIds'] = request.file_ids_shrink
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.order_type):
-            query['OrderType'] = request.order_type
-        if not UtilClient.is_unset(request.parent_file_id):
-            query['ParentFileId'] = request.parent_file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ListCdsFiles',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ListCdsFilesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def list_cds_files(
-        self,
-        request: ecd_20200930_models.ListCdsFilesRequest,
-    ) -> ecd_20200930_models.ListCdsFilesResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.list_cds_files_with_options(request, runtime)
-
-    async def list_cds_files_async(
-        self,
-        request: ecd_20200930_models.ListCdsFilesRequest,
-    ) -> ecd_20200930_models.ListCdsFilesResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.list_cds_files_with_options_async(request, runtime)
-
     def list_directory_users_with_options(
         self,
         request: ecd_20200930_models.ListDirectoryUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ListDirectoryUsersResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -12601,96 +8139,14 @@
     async def list_directory_users_async(
         self,
         request: ecd_20200930_models.ListDirectoryUsersRequest,
     ) -> ecd_20200930_models.ListDirectoryUsersResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_directory_users_with_options_async(request, runtime)
 
-    def list_file_permission_with_options(
-        self,
-        request: ecd_20200930_models.ListFilePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ListFilePermissionResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ListFilePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ListFilePermissionResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def list_file_permission_with_options_async(
-        self,
-        request: ecd_20200930_models.ListFilePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ListFilePermissionResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ListFilePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ListFilePermissionResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def list_file_permission(
-        self,
-        request: ecd_20200930_models.ListFilePermissionRequest,
-    ) -> ecd_20200930_models.ListFilePermissionResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.list_file_permission_with_options(request, runtime)
-
-    async def list_file_permission_async(
-        self,
-        request: ecd_20200930_models.ListFilePermissionRequest,
-    ) -> ecd_20200930_models.ListFilePermissionResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.list_file_permission_with_options_async(request, runtime)
-
     def list_office_site_overview_with_options(
         self,
         request: ecd_20200930_models.ListOfficeSiteOverviewRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ListOfficeSiteOverviewResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -12868,21 +8324,14 @@
         return await self.list_office_site_users_with_options_async(request, runtime)
 
     def list_tag_resources_with_options(
         self,
         request: ecd_20200930_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ListTagResourcesResponse:
-        """
-        The tag key of the resource.
-        
-        @param request: ListTagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ListTagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
@@ -12913,21 +8362,14 @@
         )
 
     async def list_tag_resources_with_options_async(
         self,
         request: ecd_20200930_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ListTagResourcesResponse:
-        """
-        The tag key of the resource.
-        
-        @param request: ListTagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ListTagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
@@ -12957,49 +8399,31 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tag_resources(
         self,
         request: ecd_20200930_models.ListTagResourcesRequest,
     ) -> ecd_20200930_models.ListTagResourcesResponse:
-        """
-        The tag key of the resource.
-        
-        @param request: ListTagResourcesRequest
-        @return: ListTagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.list_tag_resources_with_options(request, runtime)
 
     async def list_tag_resources_async(
         self,
         request: ecd_20200930_models.ListTagResourcesRequest,
     ) -> ecd_20200930_models.ListTagResourcesResponse:
-        """
-        The tag key of the resource.
-        
-        @param request: ListTagResourcesRequest
-        @return: ListTagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.list_tag_resources_with_options_async(request, runtime)
 
     def list_user_ad_organization_units_with_options(
         self,
         request: ecd_20200930_models.ListUserAdOrganizationUnitsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ListUserAdOrganizationUnitsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.filter):
-            query['Filter'] = request.filter
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -13022,20 +8446,14 @@
     async def list_user_ad_organization_units_with_options_async(
         self,
         request: ecd_20200930_models.ListUserAdOrganizationUnitsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ListUserAdOrganizationUnitsResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.filter):
-            query['Filter'] = request.filter
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -13070,21 +8488,14 @@
         return await self.list_user_ad_organization_units_with_options_async(request, runtime)
 
     def lock_virtual_mfadevice_with_options(
         self,
         request: ecd_20200930_models.LockVirtualMFADeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.LockVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: LockVirtualMFADeviceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: LockVirtualMFADeviceResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.serial_number):
             query['SerialNumber'] = request.serial_number
         req = open_api_models.OpenApiRequest(
@@ -13107,21 +8518,14 @@
         )
 
     async def lock_virtual_mfadevice_with_options_async(
         self,
         request: ecd_20200930_models.LockVirtualMFADeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.LockVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: LockVirtualMFADeviceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: LockVirtualMFADeviceResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.serial_number):
             query['SerialNumber'] = request.serial_number
         req = open_api_models.OpenApiRequest(
@@ -13143,114 +8547,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def lock_virtual_mfadevice(
         self,
         request: ecd_20200930_models.LockVirtualMFADeviceRequest,
     ) -> ecd_20200930_models.LockVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: LockVirtualMFADeviceRequest
-        @return: LockVirtualMFADeviceResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.lock_virtual_mfadevice_with_options(request, runtime)
 
     async def lock_virtual_mfadevice_async(
         self,
         request: ecd_20200930_models.LockVirtualMFADeviceRequest,
     ) -> ecd_20200930_models.LockVirtualMFADeviceResponse:
-        """
-        The ID of the request.
-        
-        @param request: LockVirtualMFADeviceRequest
-        @return: LockVirtualMFADeviceResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.lock_virtual_mfadevice_with_options_async(request, runtime)
 
-    def migrate_desktops_with_options(
-        self,
-        request: ecd_20200930_models.MigrateDesktopsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.MigrateDesktopsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.target_office_site_id):
-            query['TargetOfficeSiteId'] = request.target_office_site_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='MigrateDesktops',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.MigrateDesktopsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def migrate_desktops_with_options_async(
-        self,
-        request: ecd_20200930_models.MigrateDesktopsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.MigrateDesktopsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.target_office_site_id):
-            query['TargetOfficeSiteId'] = request.target_office_site_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='MigrateDesktops',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.MigrateDesktopsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def migrate_desktops(
-        self,
-        request: ecd_20200930_models.MigrateDesktopsRequest,
-    ) -> ecd_20200930_models.MigrateDesktopsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.migrate_desktops_with_options(request, runtime)
-
-    async def migrate_desktops_async(
-        self,
-        request: ecd_20200930_models.MigrateDesktopsRequest,
-    ) -> ecd_20200930_models.MigrateDesktopsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.migrate_desktops_with_options_async(request, runtime)
-
     def modify_adconnector_directory_with_options(
         self,
         request: ecd_20200930_models.ModifyADConnectorDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyADConnectorDirectoryResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -13471,194 +8785,19 @@
     async def modify_adconnector_office_site_async(
         self,
         request: ecd_20200930_models.ModifyADConnectorOfficeSiteRequest,
     ) -> ecd_20200930_models.ModifyADConnectorOfficeSiteResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_adconnector_office_site_with_options_async(request, runtime)
 
-    def modify_acl_entries_with_options(
-        self,
-        request: ecd_20200930_models.ModifyAclEntriesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyAclEntriesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.policy):
-            query['Policy'] = request.policy
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.source_id):
-            query['SourceId'] = request.source_id
-        if not UtilClient.is_unset(request.source_type):
-            query['SourceType'] = request.source_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyAclEntries',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyAclEntriesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_acl_entries_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyAclEntriesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyAclEntriesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.policy):
-            query['Policy'] = request.policy
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.source_id):
-            query['SourceId'] = request.source_id
-        if not UtilClient.is_unset(request.source_type):
-            query['SourceType'] = request.source_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyAclEntries',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyAclEntriesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_acl_entries(
-        self,
-        request: ecd_20200930_models.ModifyAclEntriesRequest,
-    ) -> ecd_20200930_models.ModifyAclEntriesResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_acl_entries_with_options(request, runtime)
-
-    async def modify_acl_entries_async(
-        self,
-        request: ecd_20200930_models.ModifyAclEntriesRequest,
-    ) -> ecd_20200930_models.ModifyAclEntriesResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_acl_entries_with_options_async(request, runtime)
-
-    def modify_auto_snapshot_policy_with_options(
-        self,
-        request: ecd_20200930_models.ModifyAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyAutoSnapshotPolicyResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cron_expression):
-            query['CronExpression'] = request.cron_expression
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.policy_name):
-            query['PolicyName'] = request.policy_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.retention_days):
-            query['RetentionDays'] = request.retention_days
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyAutoSnapshotPolicyResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_auto_snapshot_policy_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyAutoSnapshotPolicyRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyAutoSnapshotPolicyResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cron_expression):
-            query['CronExpression'] = request.cron_expression
-        if not UtilClient.is_unset(request.policy_id):
-            query['PolicyId'] = request.policy_id
-        if not UtilClient.is_unset(request.policy_name):
-            query['PolicyName'] = request.policy_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.retention_days):
-            query['RetentionDays'] = request.retention_days
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyAutoSnapshotPolicy',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyAutoSnapshotPolicyResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_auto_snapshot_policy(
-        self,
-        request: ecd_20200930_models.ModifyAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.ModifyAutoSnapshotPolicyResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_auto_snapshot_policy_with_options(request, runtime)
-
-    async def modify_auto_snapshot_policy_async(
-        self,
-        request: ecd_20200930_models.ModifyAutoSnapshotPolicyRequest,
-    ) -> ecd_20200930_models.ModifyAutoSnapshotPolicyResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_auto_snapshot_policy_with_options_async(request, runtime)
-
     def modify_bundle_with_options(
         self,
         request: ecd_20200930_models.ModifyBundleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyBundleResponse:
-        """
-        The ID of the desktop template.
-        
-        @param request: ModifyBundleRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyBundleResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.bundle_id):
             query['BundleId'] = request.bundle_id
         if not UtilClient.is_unset(request.bundle_name):
             query['BundleName'] = request.bundle_name
         if not UtilClient.is_unset(request.description):
@@ -13689,21 +8828,14 @@
         )
 
     async def modify_bundle_with_options_async(
         self,
         request: ecd_20200930_models.ModifyBundleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyBundleResponse:
-        """
-        The ID of the desktop template.
-        
-        @param request: ModifyBundleRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyBundleResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.bundle_id):
             query['BundleId'] = request.bundle_id
         if not UtilClient.is_unset(request.bundle_name):
             query['BundleName'] = request.bundle_name
         if not UtilClient.is_unset(request.description):
@@ -13733,608 +8865,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_bundle(
         self,
         request: ecd_20200930_models.ModifyBundleRequest,
     ) -> ecd_20200930_models.ModifyBundleResponse:
-        """
-        The ID of the desktop template.
-        
-        @param request: ModifyBundleRequest
-        @return: ModifyBundleResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_bundle_with_options(request, runtime)
 
     async def modify_bundle_async(
         self,
         request: ecd_20200930_models.ModifyBundleRequest,
     ) -> ecd_20200930_models.ModifyBundleResponse:
-        """
-        The ID of the desktop template.
-        
-        @param request: ModifyBundleRequest
-        @return: ModifyBundleResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_bundle_with_options_async(request, runtime)
 
-    def modify_cds_file_with_options(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.conflict_policy):
-            query['ConflictPolicy'] = request.conflict_policy
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.file_name):
-            query['FileName'] = request.file_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCdsFileResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_cds_file_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.conflict_policy):
-            query['ConflictPolicy'] = request.conflict_policy
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.file_name):
-            query['FileName'] = request.file_name
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCdsFileResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_cds_file(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileRequest,
-    ) -> ecd_20200930_models.ModifyCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_cds_file_with_options(request, runtime)
-
-    async def modify_cds_file_async(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileRequest,
-    ) -> ecd_20200930_models.ModifyCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_cds_file_with_options_async(request, runtime)
-
-    def modify_cds_file_share_link_with_options(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileShareLinkRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCdsFileShareLinkResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.description):
-            query['Description'] = request.description
-        if not UtilClient.is_unset(request.disable_download):
-            query['DisableDownload'] = request.disable_download
-        if not UtilClient.is_unset(request.disable_preview):
-            query['DisablePreview'] = request.disable_preview
-        if not UtilClient.is_unset(request.disable_save):
-            query['DisableSave'] = request.disable_save
-        if not UtilClient.is_unset(request.download_count):
-            query['DownloadCount'] = request.download_count
-        if not UtilClient.is_unset(request.download_limit):
-            query['DownloadLimit'] = request.download_limit
-        if not UtilClient.is_unset(request.expiration):
-            query['Expiration'] = request.expiration
-        if not UtilClient.is_unset(request.preview_count):
-            query['PreviewCount'] = request.preview_count
-        if not UtilClient.is_unset(request.preview_limit):
-            query['PreviewLimit'] = request.preview_limit
-        if not UtilClient.is_unset(request.report_count):
-            query['ReportCount'] = request.report_count
-        if not UtilClient.is_unset(request.save_count):
-            query['SaveCount'] = request.save_count
-        if not UtilClient.is_unset(request.save_limit):
-            query['SaveLimit'] = request.save_limit
-        if not UtilClient.is_unset(request.share_id):
-            query['ShareId'] = request.share_id
-        if not UtilClient.is_unset(request.share_name):
-            query['ShareName'] = request.share_name
-        if not UtilClient.is_unset(request.share_pwd):
-            query['SharePwd'] = request.share_pwd
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.video_preview_count):
-            query['VideoPreviewCount'] = request.video_preview_count
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCdsFileShareLink',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCdsFileShareLinkResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_cds_file_share_link_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileShareLinkRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCdsFileShareLinkResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.description):
-            query['Description'] = request.description
-        if not UtilClient.is_unset(request.disable_download):
-            query['DisableDownload'] = request.disable_download
-        if not UtilClient.is_unset(request.disable_preview):
-            query['DisablePreview'] = request.disable_preview
-        if not UtilClient.is_unset(request.disable_save):
-            query['DisableSave'] = request.disable_save
-        if not UtilClient.is_unset(request.download_count):
-            query['DownloadCount'] = request.download_count
-        if not UtilClient.is_unset(request.download_limit):
-            query['DownloadLimit'] = request.download_limit
-        if not UtilClient.is_unset(request.expiration):
-            query['Expiration'] = request.expiration
-        if not UtilClient.is_unset(request.preview_count):
-            query['PreviewCount'] = request.preview_count
-        if not UtilClient.is_unset(request.preview_limit):
-            query['PreviewLimit'] = request.preview_limit
-        if not UtilClient.is_unset(request.report_count):
-            query['ReportCount'] = request.report_count
-        if not UtilClient.is_unset(request.save_count):
-            query['SaveCount'] = request.save_count
-        if not UtilClient.is_unset(request.save_limit):
-            query['SaveLimit'] = request.save_limit
-        if not UtilClient.is_unset(request.share_id):
-            query['ShareId'] = request.share_id
-        if not UtilClient.is_unset(request.share_name):
-            query['ShareName'] = request.share_name
-        if not UtilClient.is_unset(request.share_pwd):
-            query['SharePwd'] = request.share_pwd
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.video_preview_count):
-            query['VideoPreviewCount'] = request.video_preview_count
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCdsFileShareLink',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCdsFileShareLinkResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_cds_file_share_link(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileShareLinkRequest,
-    ) -> ecd_20200930_models.ModifyCdsFileShareLinkResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_cds_file_share_link_with_options(request, runtime)
-
-    async def modify_cds_file_share_link_async(
-        self,
-        request: ecd_20200930_models.ModifyCdsFileShareLinkRequest,
-    ) -> ecd_20200930_models.ModifyCdsFileShareLinkResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_cds_file_share_link_with_options_async(request, runtime)
-
-    def modify_cloud_drive_groups_with_options(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveGroupsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCloudDriveGroupsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.group_id):
-            query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.total_size):
-            query['TotalSize'] = request.total_size
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCloudDriveGroups',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCloudDriveGroupsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_cloud_drive_groups_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveGroupsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCloudDriveGroupsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.group_id):
-            query['GroupId'] = request.group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.total_size):
-            query['TotalSize'] = request.total_size
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCloudDriveGroups',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCloudDriveGroupsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_cloud_drive_groups(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveGroupsRequest,
-    ) -> ecd_20200930_models.ModifyCloudDriveGroupsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_cloud_drive_groups_with_options(request, runtime)
-
-    async def modify_cloud_drive_groups_async(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveGroupsRequest,
-    ) -> ecd_20200930_models.ModifyCloudDriveGroupsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_cloud_drive_groups_with_options_async(request, runtime)
-
-    def modify_cloud_drive_permission_with_options(
-        self,
-        request: ecd_20200930_models.ModifyCloudDrivePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCloudDrivePermissionResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.download_end_user_ids):
-            query['DownloadEndUserIds'] = request.download_end_user_ids
-        if not UtilClient.is_unset(request.download_upload_end_user_ids):
-            query['DownloadUploadEndUserIds'] = request.download_upload_end_user_ids
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCloudDrivePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCloudDrivePermissionResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_cloud_drive_permission_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyCloudDrivePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCloudDrivePermissionResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.download_end_user_ids):
-            query['DownloadEndUserIds'] = request.download_end_user_ids
-        if not UtilClient.is_unset(request.download_upload_end_user_ids):
-            query['DownloadUploadEndUserIds'] = request.download_upload_end_user_ids
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCloudDrivePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCloudDrivePermissionResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_cloud_drive_permission(
-        self,
-        request: ecd_20200930_models.ModifyCloudDrivePermissionRequest,
-    ) -> ecd_20200930_models.ModifyCloudDrivePermissionResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_cloud_drive_permission_with_options(request, runtime)
-
-    async def modify_cloud_drive_permission_async(
-        self,
-        request: ecd_20200930_models.ModifyCloudDrivePermissionRequest,
-    ) -> ecd_20200930_models.ModifyCloudDrivePermissionResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_cloud_drive_permission_with_options_async(request, runtime)
-
-    def modify_cloud_drive_users_with_options(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.user_max_size):
-            query['UserMaxSize'] = request.user_max_size
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCloudDriveUsersResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_cloud_drive_users_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveUsersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCloudDriveUsersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.user_max_size):
-            query['UserMaxSize'] = request.user_max_size
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCloudDriveUsers',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCloudDriveUsersResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_cloud_drive_users(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.ModifyCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_cloud_drive_users_with_options(request, runtime)
-
-    async def modify_cloud_drive_users_async(
-        self,
-        request: ecd_20200930_models.ModifyCloudDriveUsersRequest,
-    ) -> ecd_20200930_models.ModifyCloudDriveUsersResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_cloud_drive_users_with_options_async(request, runtime)
-
-    def modify_customized_list_headers_with_options(
-        self,
-        request: ecd_20200930_models.ModifyCustomizedListHeadersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCustomizedListHeadersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.headers):
-            query['Headers'] = request.headers
-        if not UtilClient.is_unset(request.list_type):
-            query['ListType'] = request.list_type
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCustomizedListHeaders',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCustomizedListHeadersResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_customized_list_headers_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyCustomizedListHeadersRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyCustomizedListHeadersResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.headers):
-            query['Headers'] = request.headers
-        if not UtilClient.is_unset(request.list_type):
-            query['ListType'] = request.list_type
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyCustomizedListHeaders',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyCustomizedListHeadersResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_customized_list_headers(
-        self,
-        request: ecd_20200930_models.ModifyCustomizedListHeadersRequest,
-    ) -> ecd_20200930_models.ModifyCustomizedListHeadersResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_customized_list_headers_with_options(request, runtime)
-
-    async def modify_customized_list_headers_async(
-        self,
-        request: ecd_20200930_models.ModifyCustomizedListHeadersRequest,
-    ) -> ecd_20200930_models.ModifyCustomizedListHeadersResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_customized_list_headers_with_options_async(request, runtime)
-
     def modify_desktop_charge_type_with_options(
         self,
         request: ecd_20200930_models.ModifyDesktopChargeTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopChargeTypeResponse:
-        """
-        The new billing method that you want to use for the desktop group.
-        
-        @param request: ModifyDesktopChargeTypeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopChargeTypeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.desktop_id):
@@ -14343,16 +8896,14 @@
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.promotion_id):
             query['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.use_duration):
-            query['UseDuration'] = request.use_duration
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDesktopChargeType',
             version='2020-09-30',
             protocol='HTTPS',
@@ -14369,21 +8920,14 @@
         )
 
     async def modify_desktop_charge_type_with_options_async(
         self,
         request: ecd_20200930_models.ModifyDesktopChargeTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopChargeTypeResponse:
-        """
-        The new billing method that you want to use for the desktop group.
-        
-        @param request: ModifyDesktopChargeTypeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopChargeTypeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.desktop_id):
@@ -14392,16 +8936,14 @@
             query['Period'] = request.period
         if not UtilClient.is_unset(request.period_unit):
             query['PeriodUnit'] = request.period_unit
         if not UtilClient.is_unset(request.promotion_id):
             query['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.use_duration):
-            query['UseDuration'] = request.use_duration
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDesktopChargeType',
             version='2020-09-30',
             protocol='HTTPS',
@@ -14417,106 +8959,65 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_desktop_charge_type(
         self,
         request: ecd_20200930_models.ModifyDesktopChargeTypeRequest,
     ) -> ecd_20200930_models.ModifyDesktopChargeTypeResponse:
-        """
-        The new billing method that you want to use for the desktop group.
-        
-        @param request: ModifyDesktopChargeTypeRequest
-        @return: ModifyDesktopChargeTypeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_desktop_charge_type_with_options(request, runtime)
 
     async def modify_desktop_charge_type_async(
         self,
         request: ecd_20200930_models.ModifyDesktopChargeTypeRequest,
     ) -> ecd_20200930_models.ModifyDesktopChargeTypeResponse:
-        """
-        The new billing method that you want to use for the desktop group.
-        
-        @param request: ModifyDesktopChargeTypeRequest
-        @return: ModifyDesktopChargeTypeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_desktop_charge_type_with_options_async(request, runtime)
 
     def modify_desktop_group_with_options(
         self,
         request: ecd_20200930_models.ModifyDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopGroupResponse:
-        """
-        After you create a desktop group, the system creates a specific number of cloud desktops based on the scaling policy that you configure for the desktop group and the number of end users who request to connect to the cloud desktops. Cloud desktops in a desktop group are created by using the same desktop template and security policy. You can modify the configurations of the desktop group in different scenarios to manage cloud desktops in a centralized manner.
-        *   By default, a desktop group has the same name as all cloud desktops in the group. You can modify the desktop group name, which is specified by the DesktopGroupName parameter, to distinguish the desktop group from the cloud desktops.
-        *   If the number of vCPUs and memory size of the cloud desktop cannot meet your business requirements in high performance scenarios, you can change the desktop template that is used to create the cloud desktop to a desktop template (OwnBundleId) that has higher specifications.
-        *   If a security policy that is associated with the desktop group cannot meet your requirements on security, you can change the policy to another policy (PolicyGroupId) that provides higher security.
-        *   If the number of cloud desktops in the desktop group is insufficient to meet the business requirements of end users, you can modify the parameter settings in the scaling policy. The parameters include MinDesktopsCount, MaxDesktopsCount, and AllowBufferCount.
-        
-        @param request: ModifyDesktopGroupRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopGroupResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_auto_setup):
             query['AllowAutoSetup'] = request.allow_auto_setup
         if not UtilClient.is_unset(request.allow_buffer_count):
             query['AllowBufferCount'] = request.allow_buffer_count
         if not UtilClient.is_unset(request.bind_amount):
             query['BindAmount'] = request.bind_amount
-        if not UtilClient.is_unset(request.buy_desktops_count):
-            query['BuyDesktopsCount'] = request.buy_desktops_count
         if not UtilClient.is_unset(request.classify):
             query['Classify'] = request.classify
         if not UtilClient.is_unset(request.comments):
             query['Comments'] = request.comments
-        if not UtilClient.is_unset(request.connect_duration):
-            query['ConnectDuration'] = request.connect_duration
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_group_name):
             query['DesktopGroupName'] = request.desktop_group_name
-        if not UtilClient.is_unset(request.disable_session_config):
-            query['DisableSessionConfig'] = request.disable_session_config
-        if not UtilClient.is_unset(request.file_system_id):
-            query['FileSystemId'] = request.file_system_id
-        if not UtilClient.is_unset(request.idle_disconnect_duration):
-            query['IdleDisconnectDuration'] = request.idle_disconnect_duration
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.keep_duration):
             query['KeepDuration'] = request.keep_duration
         if not UtilClient.is_unset(request.load_policy):
             query['LoadPolicy'] = request.load_policy
         if not UtilClient.is_unset(request.max_desktops_count):
             query['MaxDesktopsCount'] = request.max_desktops_count
         if not UtilClient.is_unset(request.min_desktops_count):
             query['MinDesktopsCount'] = request.min_desktops_count
         if not UtilClient.is_unset(request.own_bundle_id):
             query['OwnBundleId'] = request.own_bundle_id
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.policy_group_ids):
-            query['PolicyGroupIds'] = request.policy_group_ids
-        if not UtilClient.is_unset(request.profile_follow_switch):
-            query['ProfileFollowSwitch'] = request.profile_follow_switch
-        if not UtilClient.is_unset(request.ratio_threshold):
-            query['RatioThreshold'] = request.ratio_threshold
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.reset_type):
             query['ResetType'] = request.reset_type
         if not UtilClient.is_unset(request.scale_strategy_id):
             query['ScaleStrategyId'] = request.scale_strategy_id
-        if not UtilClient.is_unset(request.stop_duration):
-            query['StopDuration'] = request.stop_duration
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDesktopGroup',
             version='2020-09-30',
             protocol='HTTPS',
@@ -14533,79 +9034,50 @@
         )
 
     async def modify_desktop_group_with_options_async(
         self,
         request: ecd_20200930_models.ModifyDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopGroupResponse:
-        """
-        After you create a desktop group, the system creates a specific number of cloud desktops based on the scaling policy that you configure for the desktop group and the number of end users who request to connect to the cloud desktops. Cloud desktops in a desktop group are created by using the same desktop template and security policy. You can modify the configurations of the desktop group in different scenarios to manage cloud desktops in a centralized manner.
-        *   By default, a desktop group has the same name as all cloud desktops in the group. You can modify the desktop group name, which is specified by the DesktopGroupName parameter, to distinguish the desktop group from the cloud desktops.
-        *   If the number of vCPUs and memory size of the cloud desktop cannot meet your business requirements in high performance scenarios, you can change the desktop template that is used to create the cloud desktop to a desktop template (OwnBundleId) that has higher specifications.
-        *   If a security policy that is associated with the desktop group cannot meet your requirements on security, you can change the policy to another policy (PolicyGroupId) that provides higher security.
-        *   If the number of cloud desktops in the desktop group is insufficient to meet the business requirements of end users, you can modify the parameter settings in the scaling policy. The parameters include MinDesktopsCount, MaxDesktopsCount, and AllowBufferCount.
-        
-        @param request: ModifyDesktopGroupRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopGroupResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_auto_setup):
             query['AllowAutoSetup'] = request.allow_auto_setup
         if not UtilClient.is_unset(request.allow_buffer_count):
             query['AllowBufferCount'] = request.allow_buffer_count
         if not UtilClient.is_unset(request.bind_amount):
             query['BindAmount'] = request.bind_amount
-        if not UtilClient.is_unset(request.buy_desktops_count):
-            query['BuyDesktopsCount'] = request.buy_desktops_count
         if not UtilClient.is_unset(request.classify):
             query['Classify'] = request.classify
         if not UtilClient.is_unset(request.comments):
             query['Comments'] = request.comments
-        if not UtilClient.is_unset(request.connect_duration):
-            query['ConnectDuration'] = request.connect_duration
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_group_name):
             query['DesktopGroupName'] = request.desktop_group_name
-        if not UtilClient.is_unset(request.disable_session_config):
-            query['DisableSessionConfig'] = request.disable_session_config
-        if not UtilClient.is_unset(request.file_system_id):
-            query['FileSystemId'] = request.file_system_id
-        if not UtilClient.is_unset(request.idle_disconnect_duration):
-            query['IdleDisconnectDuration'] = request.idle_disconnect_duration
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.keep_duration):
             query['KeepDuration'] = request.keep_duration
         if not UtilClient.is_unset(request.load_policy):
             query['LoadPolicy'] = request.load_policy
         if not UtilClient.is_unset(request.max_desktops_count):
             query['MaxDesktopsCount'] = request.max_desktops_count
         if not UtilClient.is_unset(request.min_desktops_count):
             query['MinDesktopsCount'] = request.min_desktops_count
         if not UtilClient.is_unset(request.own_bundle_id):
             query['OwnBundleId'] = request.own_bundle_id
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.policy_group_ids):
-            query['PolicyGroupIds'] = request.policy_group_ids
-        if not UtilClient.is_unset(request.profile_follow_switch):
-            query['ProfileFollowSwitch'] = request.profile_follow_switch
-        if not UtilClient.is_unset(request.ratio_threshold):
-            query['RatioThreshold'] = request.ratio_threshold
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.reset_type):
             query['ResetType'] = request.reset_type
         if not UtilClient.is_unset(request.scale_strategy_id):
             query['ScaleStrategyId'] = request.scale_strategy_id
-        if not UtilClient.is_unset(request.stop_duration):
-            query['StopDuration'] = request.stop_duration
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDesktopGroup',
             version='2020-09-30',
             protocol='HTTPS',
@@ -14621,56 +9093,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_desktop_group(
         self,
         request: ecd_20200930_models.ModifyDesktopGroupRequest,
     ) -> ecd_20200930_models.ModifyDesktopGroupResponse:
-        """
-        After you create a desktop group, the system creates a specific number of cloud desktops based on the scaling policy that you configure for the desktop group and the number of end users who request to connect to the cloud desktops. Cloud desktops in a desktop group are created by using the same desktop template and security policy. You can modify the configurations of the desktop group in different scenarios to manage cloud desktops in a centralized manner.
-        *   By default, a desktop group has the same name as all cloud desktops in the group. You can modify the desktop group name, which is specified by the DesktopGroupName parameter, to distinguish the desktop group from the cloud desktops.
-        *   If the number of vCPUs and memory size of the cloud desktop cannot meet your business requirements in high performance scenarios, you can change the desktop template that is used to create the cloud desktop to a desktop template (OwnBundleId) that has higher specifications.
-        *   If a security policy that is associated with the desktop group cannot meet your requirements on security, you can change the policy to another policy (PolicyGroupId) that provides higher security.
-        *   If the number of cloud desktops in the desktop group is insufficient to meet the business requirements of end users, you can modify the parameter settings in the scaling policy. The parameters include MinDesktopsCount, MaxDesktopsCount, and AllowBufferCount.
-        
-        @param request: ModifyDesktopGroupRequest
-        @return: ModifyDesktopGroupResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_desktop_group_with_options(request, runtime)
 
     async def modify_desktop_group_async(
         self,
         request: ecd_20200930_models.ModifyDesktopGroupRequest,
     ) -> ecd_20200930_models.ModifyDesktopGroupResponse:
-        """
-        After you create a desktop group, the system creates a specific number of cloud desktops based on the scaling policy that you configure for the desktop group and the number of end users who request to connect to the cloud desktops. Cloud desktops in a desktop group are created by using the same desktop template and security policy. You can modify the configurations of the desktop group in different scenarios to manage cloud desktops in a centralized manner.
-        *   By default, a desktop group has the same name as all cloud desktops in the group. You can modify the desktop group name, which is specified by the DesktopGroupName parameter, to distinguish the desktop group from the cloud desktops.
-        *   If the number of vCPUs and memory size of the cloud desktop cannot meet your business requirements in high performance scenarios, you can change the desktop template that is used to create the cloud desktop to a desktop template (OwnBundleId) that has higher specifications.
-        *   If a security policy that is associated with the desktop group cannot meet your requirements on security, you can change the policy to another policy (PolicyGroupId) that provides higher security.
-        *   If the number of cloud desktops in the desktop group is insufficient to meet the business requirements of end users, you can modify the parameter settings in the scaling policy. The parameters include MinDesktopsCount, MaxDesktopsCount, and AllowBufferCount.
-        
-        @param request: ModifyDesktopGroupRequest
-        @return: ModifyDesktopGroupResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_desktop_group_with_options_async(request, runtime)
 
     def modify_desktop_host_name_with_options(
         self,
         request: ecd_20200930_models.ModifyDesktopHostNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopHostNameResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyDesktopHostNameRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopHostNameResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.new_host_name):
             query['NewHostName'] = request.new_host_name
         if not UtilClient.is_unset(request.region_id):
@@ -14695,21 +9140,14 @@
         )
 
     async def modify_desktop_host_name_with_options_async(
         self,
         request: ecd_20200930_models.ModifyDesktopHostNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopHostNameResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyDesktopHostNameRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopHostNameResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.new_host_name):
             query['NewHostName'] = request.new_host_name
         if not UtilClient.is_unset(request.region_id):
@@ -14733,33 +9171,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_desktop_host_name(
         self,
         request: ecd_20200930_models.ModifyDesktopHostNameRequest,
     ) -> ecd_20200930_models.ModifyDesktopHostNameResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyDesktopHostNameRequest
-        @return: ModifyDesktopHostNameResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_desktop_host_name_with_options(request, runtime)
 
     async def modify_desktop_host_name_async(
         self,
         request: ecd_20200930_models.ModifyDesktopHostNameRequest,
     ) -> ecd_20200930_models.ModifyDesktopHostNameResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyDesktopHostNameRequest
-        @return: ModifyDesktopHostNameResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_desktop_host_name_with_options_async(request, runtime)
 
     def modify_desktop_name_with_options(
         self,
         request: ecd_20200930_models.ModifyDesktopNameRequest,
         runtime: util_models.RuntimeOptions,
@@ -14838,30 +9264,14 @@
         return await self.modify_desktop_name_with_options_async(request, runtime)
 
     def modify_desktop_spec_with_options(
         self,
         request: ecd_20200930_models.ModifyDesktopSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, take note of the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides. For more information, see [Cloud desktop types](~~188609~~).
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. You must take note of the following items:
-        *   Each desktop type contains different desktop specifications, such as vCPUs, memory, and GPUs. When you change the desktop configurations, you can only change the desktop type from one to another. However, you cannot change only one of the specifications, such as vCPUs, memory, and GPUs.
-        *   You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        *   You can only increase the sizes of system and data disks.
-        *   If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or pay for the price difference.
-        *   If you want to change the configurations of your cloud desktop for multiple times, we recommend that you wait at least 5 minutes the next time you change the configurations of the same cloud desktop.
-        *   The cloud desktop for which you want to change configurations must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDesktopSpecRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopSpecResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.desktop_type):
@@ -14896,30 +9306,14 @@
         )
 
     async def modify_desktop_spec_with_options_async(
         self,
         request: ecd_20200930_models.ModifyDesktopSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, take note of the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides. For more information, see [Cloud desktop types](~~188609~~).
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. You must take note of the following items:
-        *   Each desktop type contains different desktop specifications, such as vCPUs, memory, and GPUs. When you change the desktop configurations, you can only change the desktop type from one to another. However, you cannot change only one of the specifications, such as vCPUs, memory, and GPUs.
-        *   You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        *   You can only increase the sizes of system and data disks.
-        *   If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or pay for the price difference.
-        *   If you want to change the configurations of your cloud desktop for multiple times, we recommend that you wait at least 5 minutes the next time you change the configurations of the same cloud desktop.
-        *   The cloud desktop for which you want to change configurations must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDesktopSpecRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDesktopSpecResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.desktop_type):
@@ -14953,149 +9347,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_desktop_spec(
         self,
         request: ecd_20200930_models.ModifyDesktopSpecRequest,
     ) -> ecd_20200930_models.ModifyDesktopSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, take note of the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides. For more information, see [Cloud desktop types](~~188609~~).
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. You must take note of the following items:
-        *   Each desktop type contains different desktop specifications, such as vCPUs, memory, and GPUs. When you change the desktop configurations, you can only change the desktop type from one to another. However, you cannot change only one of the specifications, such as vCPUs, memory, and GPUs.
-        *   You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        *   You can only increase the sizes of system and data disks.
-        *   If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or pay for the price difference.
-        *   If you want to change the configurations of your cloud desktop for multiple times, we recommend that you wait at least 5 minutes the next time you change the configurations of the same cloud desktop.
-        *   The cloud desktop for which you want to change configurations must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDesktopSpecRequest
-        @return: ModifyDesktopSpecResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_desktop_spec_with_options(request, runtime)
 
     async def modify_desktop_spec_async(
         self,
         request: ecd_20200930_models.ModifyDesktopSpecRequest,
     ) -> ecd_20200930_models.ModifyDesktopSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, take note of the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides. For more information, see [Cloud desktop types](~~188609~~).
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. You must take note of the following items:
-        *   Each desktop type contains different desktop specifications, such as vCPUs, memory, and GPUs. When you change the desktop configurations, you can only change the desktop type from one to another. However, you cannot change only one of the specifications, such as vCPUs, memory, and GPUs.
-        *   You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        *   You can only increase the sizes of system and data disks.
-        *   If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or pay for the price difference.
-        *   If you want to change the configurations of your cloud desktop for multiple times, we recommend that you wait at least 5 minutes the next time you change the configurations of the same cloud desktop.
-        *   The cloud desktop for which you want to change configurations must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDesktopSpecRequest
-        @return: ModifyDesktopSpecResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_desktop_spec_with_options_async(request, runtime)
 
-    def modify_desktop_timer_with_options(
-        self,
-        request: ecd_20200930_models.ModifyDesktopTimerRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyDesktopTimerResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.desktop_timers):
-            query['DesktopTimers'] = request.desktop_timers
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.use_desktop_timers):
-            query['UseDesktopTimers'] = request.use_desktop_timers
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyDesktopTimer',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyDesktopTimerResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_desktop_timer_with_options_async(
-        self,
-        request: ecd_20200930_models.ModifyDesktopTimerRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.ModifyDesktopTimerResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.desktop_timers):
-            query['DesktopTimers'] = request.desktop_timers
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.use_desktop_timers):
-            query['UseDesktopTimers'] = request.use_desktop_timers
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyDesktopTimer',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.ModifyDesktopTimerResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_desktop_timer(
-        self,
-        request: ecd_20200930_models.ModifyDesktopTimerRequest,
-    ) -> ecd_20200930_models.ModifyDesktopTimerResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_desktop_timer_with_options(request, runtime)
-
-    async def modify_desktop_timer_async(
-        self,
-        request: ecd_20200930_models.ModifyDesktopTimerRequest,
-    ) -> ecd_20200930_models.ModifyDesktopTimerResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_desktop_timer_with_options_async(request, runtime)
-
     def modify_desktops_policy_group_with_options(
         self,
         request: ecd_20200930_models.ModifyDesktopsPolicyGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDesktopsPolicyGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.policy_group_ids):
-            query['PolicyGroupIds'] = request.policy_group_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDesktopsPolicyGroup',
@@ -15120,16 +9400,14 @@
     ) -> ecd_20200930_models.ModifyDesktopsPolicyGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
-        if not UtilClient.is_unset(request.policy_group_ids):
-            query['PolicyGroupIds'] = request.policy_group_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDesktopsPolicyGroup',
@@ -15162,30 +9440,14 @@
         return await self.modify_desktops_policy_group_with_options_async(request, runtime)
 
     def modify_disk_spec_with_options(
         self,
         request: ecd_20200930_models.ModifyDiskSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDiskSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, you must know the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides.
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. Take note of the following items:
-        1\\. Desktop types include the specifications of vCPUs, memory, and GPUs. You can change only the desktop type, instead of one of the specifications.
-        2\\. You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        3\\. You can only increase the sizes of system and data disks. You cannot decrease the sizes of system and data disks.
-        4\\. If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or must pay for the price difference.
-        5\\. If you need to change the configurations of a cloud desktop multiple times, we recommend that you wait at least 5 minutes between consecutive operations on the cloud desktop.
-        6\\. The cloud desktop for which you want to change the desktop type must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDiskSpecRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDiskSpecResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.promotion_id):
@@ -15216,30 +9478,14 @@
         )
 
     async def modify_disk_spec_with_options_async(
         self,
         request: ecd_20200930_models.ModifyDiskSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyDiskSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, you must know the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides.
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. Take note of the following items:
-        1\\. Desktop types include the specifications of vCPUs, memory, and GPUs. You can change only the desktop type, instead of one of the specifications.
-        2\\. You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        3\\. You can only increase the sizes of system and data disks. You cannot decrease the sizes of system and data disks.
-        4\\. If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or must pay for the price difference.
-        5\\. If you need to change the configurations of a cloud desktop multiple times, we recommend that you wait at least 5 minutes between consecutive operations on the cloud desktop.
-        6\\. The cloud desktop for which you want to change the desktop type must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDiskSpecRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDiskSpecResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.promotion_id):
@@ -15269,66 +9515,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_disk_spec(
         self,
         request: ecd_20200930_models.ModifyDiskSpecRequest,
     ) -> ecd_20200930_models.ModifyDiskSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, you must know the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides.
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. Take note of the following items:
-        1\\. Desktop types include the specifications of vCPUs, memory, and GPUs. You can change only the desktop type, instead of one of the specifications.
-        2\\. You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        3\\. You can only increase the sizes of system and data disks. You cannot decrease the sizes of system and data disks.
-        4\\. If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or must pay for the price difference.
-        5\\. If you need to change the configurations of a cloud desktop multiple times, we recommend that you wait at least 5 minutes between consecutive operations on the cloud desktop.
-        6\\. The cloud desktop for which you want to change the desktop type must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDiskSpecRequest
-        @return: ModifyDiskSpecResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_disk_spec_with_options(request, runtime)
 
     async def modify_disk_spec_async(
         self,
         request: ecd_20200930_models.ModifyDiskSpecRequest,
     ) -> ecd_20200930_models.ModifyDiskSpecResponse:
-        """
-        You can call this operation to change the configurations, such as the desktop type and disk size, of a cloud desktop.
-        *   Before you call this operation, you must know the cloud desktop types and the disk sizes for each type of cloud desktop that Elastic Desktop Service (EDS) provides.
-        *   When you change the configurations of a cloud desktop, you must change the desktop type or the size of the system disk or data disk. You must configure at least one of the following parameters: DesktopType, RootDiskSizeGib, and UserDiskSizeGib. Take note of the following items:
-        1\\. Desktop types include the specifications of vCPUs, memory, and GPUs. You can change only the desktop type, instead of one of the specifications.
-        2\\. You cannot change a cloud desktop from the General Office type to a non-General Office type, or from a non-General Office type to the General Office type. You cannot change a cloud desktop from the Graphics type to a non-Graphics type, or from a non-Graphics type to the Graphics type.
-        3\\. You can only increase the sizes of system and data disks. You cannot decrease the sizes of system and data disks.
-        4\\. If your cloud desktop uses the subscription billing method, the price difference is calculated based on the price before and after configuration changes. You may receive a refund, or must pay for the price difference.
-        5\\. If you need to change the configurations of a cloud desktop multiple times, we recommend that you wait at least 5 minutes between consecutive operations on the cloud desktop.
-        6\\. The cloud desktop for which you want to change the desktop type must be in the Stopped state.
-        *   The changes do not affect your personal data on the cloud desktop.
-        
-        @param request: ModifyDiskSpecRequest
-        @return: ModifyDiskSpecResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_disk_spec_with_options_async(request, runtime)
 
     def modify_entitlement_with_options(
         self,
         request: ecd_20200930_models.ModifyEntitlementRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyEntitlementResponse:
-        """
-        The cloud desktop must be in the Running state.
-        
-        @param request: ModifyEntitlementRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyEntitlementResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.region_id):
@@ -15353,21 +9562,14 @@
         )
 
     async def modify_entitlement_with_options_async(
         self,
         request: ecd_20200930_models.ModifyEntitlementRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyEntitlementResponse:
-        """
-        The cloud desktop must be in the Running state.
-        
-        @param request: ModifyEntitlementRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyEntitlementResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.region_id):
@@ -15391,48 +9593,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_entitlement(
         self,
         request: ecd_20200930_models.ModifyEntitlementRequest,
     ) -> ecd_20200930_models.ModifyEntitlementResponse:
-        """
-        The cloud desktop must be in the Running state.
-        
-        @param request: ModifyEntitlementRequest
-        @return: ModifyEntitlementResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_entitlement_with_options(request, runtime)
 
     async def modify_entitlement_async(
         self,
         request: ecd_20200930_models.ModifyEntitlementRequest,
     ) -> ecd_20200930_models.ModifyEntitlementResponse:
-        """
-        The cloud desktop must be in the Running state.
-        
-        @param request: ModifyEntitlementRequest
-        @return: ModifyEntitlementResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_entitlement_with_options_async(request, runtime)
 
     def modify_image_attribute_with_options(
         self,
         request: ecd_20200930_models.ModifyImageAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyImageAttributeResponse:
-        """
-        The ID of the image.
-        
-        @param request: ModifyImageAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyImageAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.name):
@@ -15459,21 +9642,14 @@
         )
 
     async def modify_image_attribute_with_options_async(
         self,
         request: ecd_20200930_models.ModifyImageAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyImageAttributeResponse:
-        """
-        The ID of the image.
-        
-        @param request: ModifyImageAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyImageAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.name):
@@ -15499,33 +9675,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_image_attribute(
         self,
         request: ecd_20200930_models.ModifyImageAttributeRequest,
     ) -> ecd_20200930_models.ModifyImageAttributeResponse:
-        """
-        The ID of the image.
-        
-        @param request: ModifyImageAttributeRequest
-        @return: ModifyImageAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_image_attribute_with_options(request, runtime)
 
     async def modify_image_attribute_async(
         self,
         request: ecd_20200930_models.ModifyImageAttributeRequest,
     ) -> ecd_20200930_models.ModifyImageAttributeResponse:
-        """
-        The ID of the image.
-        
-        @param request: ModifyImageAttributeRequest
-        @return: ModifyImageAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_image_attribute_with_options_async(request, runtime)
 
     def modify_image_permission_with_options(
         self,
         request: ecd_20200930_models.ModifyImagePermissionRequest,
         runtime: util_models.RuntimeOptions,
@@ -15608,21 +9772,14 @@
         return await self.modify_image_permission_with_options_async(request, runtime)
 
     def modify_nasdefault_mount_target_with_options(
         self,
         request: ecd_20200930_models.ModifyNASDefaultMountTargetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyNASDefaultMountTargetResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNASDefaultMountTargetRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyNASDefaultMountTargetResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
         if not UtilClient.is_unset(request.mount_target_domain):
             query['MountTargetDomain'] = request.mount_target_domain
         if not UtilClient.is_unset(request.region_id):
@@ -15647,21 +9804,14 @@
         )
 
     async def modify_nasdefault_mount_target_with_options_async(
         self,
         request: ecd_20200930_models.ModifyNASDefaultMountTargetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyNASDefaultMountTargetResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNASDefaultMountTargetRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyNASDefaultMountTargetResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
         if not UtilClient.is_unset(request.mount_target_domain):
             query['MountTargetDomain'] = request.mount_target_domain
         if not UtilClient.is_unset(request.region_id):
@@ -15685,33 +9835,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_nasdefault_mount_target(
         self,
         request: ecd_20200930_models.ModifyNASDefaultMountTargetRequest,
     ) -> ecd_20200930_models.ModifyNASDefaultMountTargetResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNASDefaultMountTargetRequest
-        @return: ModifyNASDefaultMountTargetResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_nasdefault_mount_target_with_options(request, runtime)
 
     async def modify_nasdefault_mount_target_async(
         self,
         request: ecd_20200930_models.ModifyNASDefaultMountTargetRequest,
     ) -> ecd_20200930_models.ModifyNASDefaultMountTargetResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNASDefaultMountTargetRequest
-        @return: ModifyNASDefaultMountTargetResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_nasdefault_mount_target_with_options_async(request, runtime)
 
     def modify_network_package_bandwidth_with_options(
         self,
         request: ecd_20200930_models.ModifyNetworkPackageBandwidthRequest,
         runtime: util_models.RuntimeOptions,
@@ -15798,21 +9936,14 @@
         return await self.modify_network_package_bandwidth_with_options_async(request, runtime)
 
     def modify_network_package_enabled_with_options(
         self,
         request: ecd_20200930_models.ModifyNetworkPackageEnabledRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyNetworkPackageEnabledResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNetworkPackageEnabledRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyNetworkPackageEnabledResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.enabled):
             query['Enabled'] = request.enabled
         if not UtilClient.is_unset(request.network_package_id):
             query['NetworkPackageId'] = request.network_package_id
         if not UtilClient.is_unset(request.region_id):
@@ -15837,21 +9968,14 @@
         )
 
     async def modify_network_package_enabled_with_options_async(
         self,
         request: ecd_20200930_models.ModifyNetworkPackageEnabledRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyNetworkPackageEnabledResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNetworkPackageEnabledRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyNetworkPackageEnabledResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.enabled):
             query['Enabled'] = request.enabled
         if not UtilClient.is_unset(request.network_package_id):
             query['NetworkPackageId'] = request.network_package_id
         if not UtilClient.is_unset(request.region_id):
@@ -15875,47 +9999,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_network_package_enabled(
         self,
         request: ecd_20200930_models.ModifyNetworkPackageEnabledRequest,
     ) -> ecd_20200930_models.ModifyNetworkPackageEnabledResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNetworkPackageEnabledRequest
-        @return: ModifyNetworkPackageEnabledResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_network_package_enabled_with_options(request, runtime)
 
     async def modify_network_package_enabled_async(
         self,
         request: ecd_20200930_models.ModifyNetworkPackageEnabledRequest,
     ) -> ecd_20200930_models.ModifyNetworkPackageEnabledResponse:
-        """
-        The ID of the region.
-        
-        @param request: ModifyNetworkPackageEnabledRequest
-        @return: ModifyNetworkPackageEnabledResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_network_package_enabled_with_options_async(request, runtime)
 
     def modify_office_site_attribute_with_options(
         self,
         request: ecd_20200930_models.ModifyOfficeSiteAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyOfficeSiteAttributeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_access_type):
             query['DesktopAccessType'] = request.desktop_access_type
-        if not UtilClient.is_unset(request.enable_admin_access):
-            query['EnableAdminAccess'] = request.enable_admin_access
         if not UtilClient.is_unset(request.need_verify_login_risk):
             query['NeedVerifyLoginRisk'] = request.need_verify_login_risk
         if not UtilClient.is_unset(request.need_verify_zero_device):
             query['NeedVerifyZeroDevice'] = request.need_verify_zero_device
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
@@ -15946,16 +10056,14 @@
         request: ecd_20200930_models.ModifyOfficeSiteAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyOfficeSiteAttributeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_access_type):
             query['DesktopAccessType'] = request.desktop_access_type
-        if not UtilClient.is_unset(request.enable_admin_access):
-            query['EnableAdminAccess'] = request.enable_admin_access
         if not UtilClient.is_unset(request.need_verify_login_risk):
             query['NeedVerifyLoginRisk'] = request.need_verify_login_risk
         if not UtilClient.is_unset(request.need_verify_zero_device):
             query['NeedVerifyZeroDevice'] = request.need_verify_zero_device
         if not UtilClient.is_unset(request.office_site_id):
             query['OfficeSiteId'] = request.office_site_id
         if not UtilClient.is_unset(request.office_site_name):
@@ -16240,112 +10348,70 @@
     def modify_policy_group_with_options(
         self,
         request: ecd_20200930_models.ModifyPolicyGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyPolicyGroupResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.app_content_protection):
-            query['AppContentProtection'] = request.app_content_protection
         if not UtilClient.is_unset(request.authorize_access_policy_rule):
             query['AuthorizeAccessPolicyRule'] = request.authorize_access_policy_rule
         if not UtilClient.is_unset(request.authorize_security_policy_rule):
             query['AuthorizeSecurityPolicyRule'] = request.authorize_security_policy_rule
         if not UtilClient.is_unset(request.camera_redirect):
             query['CameraRedirect'] = request.camera_redirect
         if not UtilClient.is_unset(request.client_type):
             query['ClientType'] = request.client_type
         if not UtilClient.is_unset(request.clipboard):
             query['Clipboard'] = request.clipboard
         if not UtilClient.is_unset(request.domain_list):
             query['DomainList'] = request.domain_list
-        if not UtilClient.is_unset(request.domain_resolve_rule):
-            query['DomainResolveRule'] = request.domain_resolve_rule
-        if not UtilClient.is_unset(request.domain_resolve_rule_type):
-            query['DomainResolveRuleType'] = request.domain_resolve_rule_type
-        if not UtilClient.is_unset(request.end_user_apply_admin_coordinate):
-            query['EndUserApplyAdminCoordinate'] = request.end_user_apply_admin_coordinate
-        if not UtilClient.is_unset(request.end_user_group_coordinate):
-            query['EndUserGroupCoordinate'] = request.end_user_group_coordinate
         if not UtilClient.is_unset(request.gpu_acceleration):
             query['GpuAcceleration'] = request.gpu_acceleration
         if not UtilClient.is_unset(request.html_5access):
             query['Html5Access'] = request.html_5access
         if not UtilClient.is_unset(request.html_5file_transfer):
             query['Html5FileTransfer'] = request.html_5file_transfer
-        if not UtilClient.is_unset(request.internet_communication_protocol):
-            query['InternetCommunicationProtocol'] = request.internet_communication_protocol
         if not UtilClient.is_unset(request.local_drive):
             query['LocalDrive'] = request.local_drive
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.net_redirect):
             query['NetRedirect'] = request.net_redirect
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
         if not UtilClient.is_unset(request.preempt_login):
             query['PreemptLogin'] = request.preempt_login
         if not UtilClient.is_unset(request.preempt_login_user):
             query['PreemptLoginUser'] = request.preempt_login_user
         if not UtilClient.is_unset(request.printer_redirection):
             query['PrinterRedirection'] = request.printer_redirection
-        if not UtilClient.is_unset(request.record_content):
-            query['RecordContent'] = request.record_content
-        if not UtilClient.is_unset(request.record_content_expires):
-            query['RecordContentExpires'] = request.record_content_expires
         if not UtilClient.is_unset(request.recording):
             query['Recording'] = request.recording
-        if not UtilClient.is_unset(request.recording_audio):
-            query['RecordingAudio'] = request.recording_audio
-        if not UtilClient.is_unset(request.recording_duration):
-            query['RecordingDuration'] = request.recording_duration
         if not UtilClient.is_unset(request.recording_end_time):
             query['RecordingEndTime'] = request.recording_end_time
-        if not UtilClient.is_unset(request.recording_expires):
-            query['RecordingExpires'] = request.recording_expires
         if not UtilClient.is_unset(request.recording_fps):
             query['RecordingFps'] = request.recording_fps
         if not UtilClient.is_unset(request.recording_start_time):
             query['RecordingStartTime'] = request.recording_start_time
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.remote_coordinate):
-            query['RemoteCoordinate'] = request.remote_coordinate
         if not UtilClient.is_unset(request.revoke_access_policy_rule):
             query['RevokeAccessPolicyRule'] = request.revoke_access_policy_rule
         if not UtilClient.is_unset(request.revoke_security_policy_rule):
             query['RevokeSecurityPolicyRule'] = request.revoke_security_policy_rule
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
-        if not UtilClient.is_unset(request.scope_value):
-            query['ScopeValue'] = request.scope_value
         if not UtilClient.is_unset(request.usb_redirect):
             query['UsbRedirect'] = request.usb_redirect
         if not UtilClient.is_unset(request.usb_supply_redirect_rule):
             query['UsbSupplyRedirectRule'] = request.usb_supply_redirect_rule
-        if not UtilClient.is_unset(request.video_redirect):
-            query['VideoRedirect'] = request.video_redirect
         if not UtilClient.is_unset(request.visual_quality):
             query['VisualQuality'] = request.visual_quality
         if not UtilClient.is_unset(request.watermark):
             query['Watermark'] = request.watermark
-        if not UtilClient.is_unset(request.watermark_color):
-            query['WatermarkColor'] = request.watermark_color
-        if not UtilClient.is_unset(request.watermark_degree):
-            query['WatermarkDegree'] = request.watermark_degree
-        if not UtilClient.is_unset(request.watermark_font_size):
-            query['WatermarkFontSize'] = request.watermark_font_size
-        if not UtilClient.is_unset(request.watermark_font_style):
-            query['WatermarkFontStyle'] = request.watermark_font_style
-        if not UtilClient.is_unset(request.watermark_row_amount):
-            query['WatermarkRowAmount'] = request.watermark_row_amount
         if not UtilClient.is_unset(request.watermark_transparency):
             query['WatermarkTransparency'] = request.watermark_transparency
-        if not UtilClient.is_unset(request.watermark_transparency_value):
-            query['WatermarkTransparencyValue'] = request.watermark_transparency_value
         if not UtilClient.is_unset(request.watermark_type):
             query['WatermarkType'] = request.watermark_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyPolicyGroup',
@@ -16366,112 +10432,70 @@
     async def modify_policy_group_with_options_async(
         self,
         request: ecd_20200930_models.ModifyPolicyGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyPolicyGroupResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.app_content_protection):
-            query['AppContentProtection'] = request.app_content_protection
         if not UtilClient.is_unset(request.authorize_access_policy_rule):
             query['AuthorizeAccessPolicyRule'] = request.authorize_access_policy_rule
         if not UtilClient.is_unset(request.authorize_security_policy_rule):
             query['AuthorizeSecurityPolicyRule'] = request.authorize_security_policy_rule
         if not UtilClient.is_unset(request.camera_redirect):
             query['CameraRedirect'] = request.camera_redirect
         if not UtilClient.is_unset(request.client_type):
             query['ClientType'] = request.client_type
         if not UtilClient.is_unset(request.clipboard):
             query['Clipboard'] = request.clipboard
         if not UtilClient.is_unset(request.domain_list):
             query['DomainList'] = request.domain_list
-        if not UtilClient.is_unset(request.domain_resolve_rule):
-            query['DomainResolveRule'] = request.domain_resolve_rule
-        if not UtilClient.is_unset(request.domain_resolve_rule_type):
-            query['DomainResolveRuleType'] = request.domain_resolve_rule_type
-        if not UtilClient.is_unset(request.end_user_apply_admin_coordinate):
-            query['EndUserApplyAdminCoordinate'] = request.end_user_apply_admin_coordinate
-        if not UtilClient.is_unset(request.end_user_group_coordinate):
-            query['EndUserGroupCoordinate'] = request.end_user_group_coordinate
         if not UtilClient.is_unset(request.gpu_acceleration):
             query['GpuAcceleration'] = request.gpu_acceleration
         if not UtilClient.is_unset(request.html_5access):
             query['Html5Access'] = request.html_5access
         if not UtilClient.is_unset(request.html_5file_transfer):
             query['Html5FileTransfer'] = request.html_5file_transfer
-        if not UtilClient.is_unset(request.internet_communication_protocol):
-            query['InternetCommunicationProtocol'] = request.internet_communication_protocol
         if not UtilClient.is_unset(request.local_drive):
             query['LocalDrive'] = request.local_drive
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.net_redirect):
             query['NetRedirect'] = request.net_redirect
         if not UtilClient.is_unset(request.policy_group_id):
             query['PolicyGroupId'] = request.policy_group_id
         if not UtilClient.is_unset(request.preempt_login):
             query['PreemptLogin'] = request.preempt_login
         if not UtilClient.is_unset(request.preempt_login_user):
             query['PreemptLoginUser'] = request.preempt_login_user
         if not UtilClient.is_unset(request.printer_redirection):
             query['PrinterRedirection'] = request.printer_redirection
-        if not UtilClient.is_unset(request.record_content):
-            query['RecordContent'] = request.record_content
-        if not UtilClient.is_unset(request.record_content_expires):
-            query['RecordContentExpires'] = request.record_content_expires
         if not UtilClient.is_unset(request.recording):
             query['Recording'] = request.recording
-        if not UtilClient.is_unset(request.recording_audio):
-            query['RecordingAudio'] = request.recording_audio
-        if not UtilClient.is_unset(request.recording_duration):
-            query['RecordingDuration'] = request.recording_duration
         if not UtilClient.is_unset(request.recording_end_time):
             query['RecordingEndTime'] = request.recording_end_time
-        if not UtilClient.is_unset(request.recording_expires):
-            query['RecordingExpires'] = request.recording_expires
         if not UtilClient.is_unset(request.recording_fps):
             query['RecordingFps'] = request.recording_fps
         if not UtilClient.is_unset(request.recording_start_time):
             query['RecordingStartTime'] = request.recording_start_time
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.remote_coordinate):
-            query['RemoteCoordinate'] = request.remote_coordinate
         if not UtilClient.is_unset(request.revoke_access_policy_rule):
             query['RevokeAccessPolicyRule'] = request.revoke_access_policy_rule
         if not UtilClient.is_unset(request.revoke_security_policy_rule):
             query['RevokeSecurityPolicyRule'] = request.revoke_security_policy_rule
-        if not UtilClient.is_unset(request.scope):
-            query['Scope'] = request.scope
-        if not UtilClient.is_unset(request.scope_value):
-            query['ScopeValue'] = request.scope_value
         if not UtilClient.is_unset(request.usb_redirect):
             query['UsbRedirect'] = request.usb_redirect
         if not UtilClient.is_unset(request.usb_supply_redirect_rule):
             query['UsbSupplyRedirectRule'] = request.usb_supply_redirect_rule
-        if not UtilClient.is_unset(request.video_redirect):
-            query['VideoRedirect'] = request.video_redirect
         if not UtilClient.is_unset(request.visual_quality):
             query['VisualQuality'] = request.visual_quality
         if not UtilClient.is_unset(request.watermark):
             query['Watermark'] = request.watermark
-        if not UtilClient.is_unset(request.watermark_color):
-            query['WatermarkColor'] = request.watermark_color
-        if not UtilClient.is_unset(request.watermark_degree):
-            query['WatermarkDegree'] = request.watermark_degree
-        if not UtilClient.is_unset(request.watermark_font_size):
-            query['WatermarkFontSize'] = request.watermark_font_size
-        if not UtilClient.is_unset(request.watermark_font_style):
-            query['WatermarkFontStyle'] = request.watermark_font_style
-        if not UtilClient.is_unset(request.watermark_row_amount):
-            query['WatermarkRowAmount'] = request.watermark_row_amount
         if not UtilClient.is_unset(request.watermark_transparency):
             query['WatermarkTransparency'] = request.watermark_transparency
-        if not UtilClient.is_unset(request.watermark_transparency_value):
-            query['WatermarkTransparencyValue'] = request.watermark_transparency_value
         if not UtilClient.is_unset(request.watermark_type):
             query['WatermarkType'] = request.watermark_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyPolicyGroup',
@@ -16504,21 +10528,14 @@
         return await self.modify_policy_group_with_options_async(request, runtime)
 
     def modify_user_entitlement_with_options(
         self,
         request: ecd_20200930_models.ModifyUserEntitlementRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyUserEntitlementResponse:
-        """
-        The IDs of regular users.
-        
-        @param request: ModifyUserEntitlementRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyUserEntitlementResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.authorize_desktop_id):
             query['AuthorizeDesktopId'] = request.authorize_desktop_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.region_id):
@@ -16545,21 +10562,14 @@
         )
 
     async def modify_user_entitlement_with_options_async(
         self,
         request: ecd_20200930_models.ModifyUserEntitlementRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ModifyUserEntitlementResponse:
-        """
-        The IDs of regular users.
-        
-        @param request: ModifyUserEntitlementRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyUserEntitlementResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.authorize_desktop_id):
             query['AuthorizeDesktopId'] = request.authorize_desktop_id
         if not UtilClient.is_unset(request.end_user_id):
             query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.region_id):
@@ -16585,33 +10595,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_user_entitlement(
         self,
         request: ecd_20200930_models.ModifyUserEntitlementRequest,
     ) -> ecd_20200930_models.ModifyUserEntitlementResponse:
-        """
-        The IDs of regular users.
-        
-        @param request: ModifyUserEntitlementRequest
-        @return: ModifyUserEntitlementResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_user_entitlement_with_options(request, runtime)
 
     async def modify_user_entitlement_async(
         self,
         request: ecd_20200930_models.ModifyUserEntitlementRequest,
     ) -> ecd_20200930_models.ModifyUserEntitlementResponse:
-        """
-        The IDs of regular users.
-        
-        @param request: ModifyUserEntitlementRequest
-        @return: ModifyUserEntitlementResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_user_entitlement_with_options_async(request, runtime)
 
     def modify_user_to_desktop_group_with_options(
         self,
         request: ecd_20200930_models.ModifyUserToDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
@@ -16689,104 +10687,14 @@
     async def modify_user_to_desktop_group_async(
         self,
         request: ecd_20200930_models.ModifyUserToDesktopGroupRequest,
     ) -> ecd_20200930_models.ModifyUserToDesktopGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_user_to_desktop_group_with_options_async(request, runtime)
 
-    def move_cds_file_with_options(
-        self,
-        request: ecd_20200930_models.MoveCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.MoveCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.conflict_policy):
-            query['ConflictPolicy'] = request.conflict_policy
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.parent_folder_id):
-            query['ParentFolderId'] = request.parent_folder_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='MoveCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.MoveCdsFileResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def move_cds_file_with_options_async(
-        self,
-        request: ecd_20200930_models.MoveCdsFileRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.MoveCdsFileResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.conflict_policy):
-            query['ConflictPolicy'] = request.conflict_policy
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.parent_folder_id):
-            query['ParentFolderId'] = request.parent_folder_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='MoveCdsFile',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.MoveCdsFileResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def move_cds_file(
-        self,
-        request: ecd_20200930_models.MoveCdsFileRequest,
-    ) -> ecd_20200930_models.MoveCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.move_cds_file_with_options(request, runtime)
-
-    async def move_cds_file_async(
-        self,
-        request: ecd_20200930_models.MoveCdsFileRequest,
-    ) -> ecd_20200930_models.MoveCdsFileResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.move_cds_file_with_options_async(request, runtime)
-
     def operate_vuls_with_options(
         self,
         request: ecd_20200930_models.OperateVulsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.OperateVulsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -16878,21 +10786,14 @@
         return await self.operate_vuls_with_options_async(request, runtime)
 
     def reboot_desktops_with_options(
         self,
         request: ecd_20200930_models.RebootDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.RebootDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: RebootDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RebootDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -16915,21 +10816,14 @@
         )
 
     async def reboot_desktops_with_options_async(
         self,
         request: ecd_20200930_models.RebootDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.RebootDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: RebootDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RebootDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -16951,56 +10845,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reboot_desktops(
         self,
         request: ecd_20200930_models.RebootDesktopsRequest,
     ) -> ecd_20200930_models.RebootDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: RebootDesktopsRequest
-        @return: RebootDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.reboot_desktops_with_options(request, runtime)
 
     async def reboot_desktops_async(
         self,
         request: ecd_20200930_models.RebootDesktopsRequest,
     ) -> ecd_20200930_models.RebootDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: RebootDesktopsRequest
-        @return: RebootDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.reboot_desktops_with_options_async(request, runtime)
 
     def rebuild_desktops_with_options(
         self,
         request: ecd_20200930_models.RebuildDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.RebuildDesktopsResponse:
-        """
-        The error message. This parameter is not returned if the value of Code is success.
-        
-        @param request: RebuildDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RebuildDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
-        if not UtilClient.is_unset(request.operate_type):
-            query['OperateType'] = request.operate_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RebuildDesktops',
@@ -17019,29 +10892,20 @@
         )
 
     async def rebuild_desktops_with_options_async(
         self,
         request: ecd_20200930_models.RebuildDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.RebuildDesktopsResponse:
-        """
-        The error message. This parameter is not returned if the value of Code is success.
-        
-        @param request: RebuildDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RebuildDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
-        if not UtilClient.is_unset(request.operate_type):
-            query['OperateType'] = request.operate_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RebuildDesktops',
@@ -17059,130 +10923,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def rebuild_desktops(
         self,
         request: ecd_20200930_models.RebuildDesktopsRequest,
     ) -> ecd_20200930_models.RebuildDesktopsResponse:
-        """
-        The error message. This parameter is not returned if the value of Code is success.
-        
-        @param request: RebuildDesktopsRequest
-        @return: RebuildDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.rebuild_desktops_with_options(request, runtime)
 
     async def rebuild_desktops_async(
         self,
         request: ecd_20200930_models.RebuildDesktopsRequest,
     ) -> ecd_20200930_models.RebuildDesktopsResponse:
-        """
-        The error message. This parameter is not returned if the value of Code is success.
-        
-        @param request: RebuildDesktopsRequest
-        @return: RebuildDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.rebuild_desktops_with_options_async(request, runtime)
 
-    def remove_file_permission_with_options(
-        self,
-        tmp_req: ecd_20200930_models.RemoveFilePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.RemoveFilePermissionResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.RemoveFilePermissionShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.member_list):
-            request.member_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.member_list, 'MemberList', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.member_list_shrink):
-            query['MemberList'] = request.member_list_shrink
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='RemoveFilePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.RemoveFilePermissionResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def remove_file_permission_with_options_async(
-        self,
-        tmp_req: ecd_20200930_models.RemoveFilePermissionRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.RemoveFilePermissionResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.RemoveFilePermissionShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.member_list):
-            request.member_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.member_list, 'MemberList', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.cds_id):
-            query['CdsId'] = request.cds_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.file_id):
-            query['FileId'] = request.file_id
-        if not UtilClient.is_unset(request.member_list_shrink):
-            query['MemberList'] = request.member_list_shrink
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='RemoveFilePermission',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.RemoveFilePermissionResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def remove_file_permission(
-        self,
-        request: ecd_20200930_models.RemoveFilePermissionRequest,
-    ) -> ecd_20200930_models.RemoveFilePermissionResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.remove_file_permission_with_options(request, runtime)
-
-    async def remove_file_permission_async(
-        self,
-        request: ecd_20200930_models.RemoveFilePermissionRequest,
-    ) -> ecd_20200930_models.RemoveFilePermissionResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.remove_file_permission_with_options_async(request, runtime)
-
     def remove_user_from_desktop_group_with_options(
         self,
         request: ecd_20200930_models.RemoveUserFromDesktopGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.RemoveUserFromDesktopGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -17442,21 +11200,14 @@
         return await self.renew_network_packages_with_options_async(request, runtime)
 
     def reset_desktops_with_options(
         self,
         request: ecd_20200930_models.ResetDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ResetDesktopsResponse:
-        """
-        > You can call this operation to reset only cloud desktops that are managed by a cloud desktop group. You cannot reset an independent cloud desktop.
-        
-        @param request: ResetDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ResetDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.image_id):
@@ -17487,21 +11238,14 @@
         )
 
     async def reset_desktops_with_options_async(
         self,
         request: ecd_20200930_models.ResetDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ResetDesktopsResponse:
-        """
-        > You can call this operation to reset only cloud desktops that are managed by a cloud desktop group. You cannot reset an independent cloud desktop.
-        
-        @param request: ResetDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ResetDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_group_id):
             query['DesktopGroupId'] = request.desktop_group_id
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.image_id):
@@ -17531,48 +11275,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reset_desktops(
         self,
         request: ecd_20200930_models.ResetDesktopsRequest,
     ) -> ecd_20200930_models.ResetDesktopsResponse:
-        """
-        > You can call this operation to reset only cloud desktops that are managed by a cloud desktop group. You cannot reset an independent cloud desktop.
-        
-        @param request: ResetDesktopsRequest
-        @return: ResetDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.reset_desktops_with_options(request, runtime)
 
     async def reset_desktops_async(
         self,
         request: ecd_20200930_models.ResetDesktopsRequest,
     ) -> ecd_20200930_models.ResetDesktopsResponse:
-        """
-        > You can call this operation to reset only cloud desktops that are managed by a cloud desktop group. You cannot reset an independent cloud desktop.
-        
-        @param request: ResetDesktopsRequest
-        @return: ResetDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.reset_desktops_with_options_async(request, runtime)
 
     def reset_nasdefault_mount_target_with_options(
         self,
         request: ecd_20200930_models.ResetNASDefaultMountTargetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ResetNASDefaultMountTargetResponse:
-        """
-        The ID of the request.
-        
-        @param request: ResetNASDefaultMountTargetRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ResetNASDefaultMountTargetResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -17595,21 +11320,14 @@
         )
 
     async def reset_nasdefault_mount_target_with_options_async(
         self,
         request: ecd_20200930_models.ResetNASDefaultMountTargetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ResetNASDefaultMountTargetResponse:
-        """
-        The ID of the request.
-        
-        @param request: ResetNASDefaultMountTargetRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ResetNASDefaultMountTargetResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_system_id):
             query['FileSystemId'] = request.file_system_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -17631,52 +11349,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reset_nasdefault_mount_target(
         self,
         request: ecd_20200930_models.ResetNASDefaultMountTargetRequest,
     ) -> ecd_20200930_models.ResetNASDefaultMountTargetResponse:
-        """
-        The ID of the request.
-        
-        @param request: ResetNASDefaultMountTargetRequest
-        @return: ResetNASDefaultMountTargetResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.reset_nasdefault_mount_target_with_options(request, runtime)
 
     async def reset_nasdefault_mount_target_async(
         self,
         request: ecd_20200930_models.ResetNASDefaultMountTargetRequest,
     ) -> ecd_20200930_models.ResetNASDefaultMountTargetResponse:
-        """
-        The ID of the request.
-        
-        @param request: ResetNASDefaultMountTargetRequest
-        @return: ResetNASDefaultMountTargetResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.reset_nasdefault_mount_target_with_options_async(request, runtime)
 
     def reset_snapshot_with_options(
         self,
         request: ecd_20200930_models.ResetSnapshotRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ResetSnapshotResponse:
-        """
-        Before you call this operation, make sure that the following operations are performed:
-        *   The data that you want to retain in the disk is backed up.
-        **\
-        **Note**The disk restoration operation is irreversible. After you restore data on a disk, the disk is restored to the status at the point in time when the snapshot was created. Data that is generated between the snapshot creation time and the current time is lost. Before you restore a disk from a snapshot, make sure that you back up important data.
-        *   The cloud desktop whose disk you want to restore is stopped.
-        
-        @param request: ResetSnapshotRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ResetSnapshotResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.snapshot_id):
             query['SnapshotId'] = request.snapshot_id
         req = open_api_models.OpenApiRequest(
@@ -17699,25 +11394,14 @@
         )
 
     async def reset_snapshot_with_options_async(
         self,
         request: ecd_20200930_models.ResetSnapshotRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.ResetSnapshotResponse:
-        """
-        Before you call this operation, make sure that the following operations are performed:
-        *   The data that you want to retain in the disk is backed up.
-        **\
-        **Note**The disk restoration operation is irreversible. After you restore data on a disk, the disk is restored to the status at the point in time when the snapshot was created. Data that is generated between the snapshot creation time and the current time is lost. Before you restore a disk from a snapshot, make sure that you back up important data.
-        *   The cloud desktop whose disk you want to restore is stopped.
-        
-        @param request: ResetSnapshotRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ResetSnapshotResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.snapshot_id):
             query['SnapshotId'] = request.snapshot_id
         req = open_api_models.OpenApiRequest(
@@ -17739,142 +11423,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reset_snapshot(
         self,
         request: ecd_20200930_models.ResetSnapshotRequest,
     ) -> ecd_20200930_models.ResetSnapshotResponse:
-        """
-        Before you call this operation, make sure that the following operations are performed:
-        *   The data that you want to retain in the disk is backed up.
-        **\
-        **Note**The disk restoration operation is irreversible. After you restore data on a disk, the disk is restored to the status at the point in time when the snapshot was created. Data that is generated between the snapshot creation time and the current time is lost. Before you restore a disk from a snapshot, make sure that you back up important data.
-        *   The cloud desktop whose disk you want to restore is stopped.
-        
-        @param request: ResetSnapshotRequest
-        @return: ResetSnapshotResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.reset_snapshot_with_options(request, runtime)
 
     async def reset_snapshot_async(
         self,
         request: ecd_20200930_models.ResetSnapshotRequest,
     ) -> ecd_20200930_models.ResetSnapshotResponse:
-        """
-        Before you call this operation, make sure that the following operations are performed:
-        *   The data that you want to retain in the disk is backed up.
-        **\
-        **Note**The disk restoration operation is irreversible. After you restore data on a disk, the disk is restored to the status at the point in time when the snapshot was created. Data that is generated between the snapshot creation time and the current time is lost. Before you restore a disk from a snapshot, make sure that you back up important data.
-        *   The cloud desktop whose disk you want to restore is stopped.
-        
-        @param request: ResetSnapshotRequest
-        @return: ResetSnapshotResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.reset_snapshot_with_options_async(request, runtime)
 
-    def revoke_coordinate_privilege_with_options(
-        self,
-        request: ecd_20200930_models.RevokeCoordinatePrivilegeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.RevokeCoordinatePrivilegeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.co_id):
-            query['CoId'] = request.co_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        if not UtilClient.is_unset(request.uuid):
-            query['Uuid'] = request.uuid
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='RevokeCoordinatePrivilege',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.RevokeCoordinatePrivilegeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def revoke_coordinate_privilege_with_options_async(
-        self,
-        request: ecd_20200930_models.RevokeCoordinatePrivilegeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.RevokeCoordinatePrivilegeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.co_id):
-            query['CoId'] = request.co_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_type):
-            query['UserType'] = request.user_type
-        if not UtilClient.is_unset(request.uuid):
-            query['Uuid'] = request.uuid
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='RevokeCoordinatePrivilege',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.RevokeCoordinatePrivilegeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def revoke_coordinate_privilege(
-        self,
-        request: ecd_20200930_models.RevokeCoordinatePrivilegeRequest,
-    ) -> ecd_20200930_models.RevokeCoordinatePrivilegeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.revoke_coordinate_privilege_with_options(request, runtime)
-
-    async def revoke_coordinate_privilege_async(
-        self,
-        request: ecd_20200930_models.RevokeCoordinatePrivilegeRequest,
-    ) -> ecd_20200930_models.RevokeCoordinatePrivilegeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.revoke_coordinate_privilege_with_options_async(request, runtime)
-
     def rollback_susp_event_quara_file_with_options(
         self,
         request: ecd_20200930_models.RollbackSuspEventQuaraFileRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.RollbackSuspEventQuaraFileResponse:
-        """
-        The ID of the region.
-        
-        @param request: RollbackSuspEventQuaraFileRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RollbackSuspEventQuaraFileResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.quara_field_id):
             query['QuaraFieldId'] = request.quara_field_id
         if not UtilClient.is_unset(request.region_id):
@@ -17899,21 +11470,14 @@
         )
 
     async def rollback_susp_event_quara_file_with_options_async(
         self,
         request: ecd_20200930_models.RollbackSuspEventQuaraFileRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.RollbackSuspEventQuaraFileResponse:
-        """
-        The ID of the region.
-        
-        @param request: RollbackSuspEventQuaraFileRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RollbackSuspEventQuaraFileResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.quara_field_id):
             query['QuaraFieldId'] = request.quara_field_id
         if not UtilClient.is_unset(request.region_id):
@@ -17937,33 +11501,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def rollback_susp_event_quara_file(
         self,
         request: ecd_20200930_models.RollbackSuspEventQuaraFileRequest,
     ) -> ecd_20200930_models.RollbackSuspEventQuaraFileResponse:
-        """
-        The ID of the region.
-        
-        @param request: RollbackSuspEventQuaraFileRequest
-        @return: RollbackSuspEventQuaraFileResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.rollback_susp_event_quara_file_with_options(request, runtime)
 
     async def rollback_susp_event_quara_file_async(
         self,
         request: ecd_20200930_models.RollbackSuspEventQuaraFileRequest,
     ) -> ecd_20200930_models.RollbackSuspEventQuaraFileResponse:
-        """
-        The ID of the region.
-        
-        @param request: RollbackSuspEventQuaraFileRequest
-        @return: RollbackSuspEventQuaraFileResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.rollback_susp_event_quara_file_with_options_async(request, runtime)
 
     def run_command_with_options(
         self,
         request: ecd_20200930_models.RunCommandRequest,
         runtime: util_models.RuntimeOptions,
@@ -17972,16 +11524,14 @@
         query = {}
         if not UtilClient.is_unset(request.command_content):
             query['CommandContent'] = request.command_content
         if not UtilClient.is_unset(request.content_encoding):
             query['ContentEncoding'] = request.content_encoding
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.timeout):
             query['Timeout'] = request.timeout
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
@@ -18012,16 +11562,14 @@
         query = {}
         if not UtilClient.is_unset(request.command_content):
             query['CommandContent'] = request.command_content
         if not UtilClient.is_unset(request.content_encoding):
             query['ContentEncoding'] = request.content_encoding
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.end_user_id):
-            query['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.timeout):
             query['Timeout'] = request.timeout
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
@@ -18058,22 +11606,14 @@
         return await self.run_command_with_options_async(request, runtime)
 
     def send_verify_code_with_options(
         self,
         request: ecd_20200930_models.SendVerifyCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.SendVerifyCodeResponse:
-        """
-        ## Description
-        When you attach your workspace network to a Cloud Enterprise Network (CEN) instance in another Alibaba Cloud account, you need to call this operation to obtain a verification code. After the call is successful, the system sends a verification code to the email address associated with the Alibaba Cloud account.
-        
-        @param request: SendVerifyCodeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SendVerifyCodeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.extra_info):
             query['ExtraInfo'] = request.extra_info
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.verify_code_action):
@@ -18098,22 +11638,14 @@
         )
 
     async def send_verify_code_with_options_async(
         self,
         request: ecd_20200930_models.SendVerifyCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.SendVerifyCodeResponse:
-        """
-        ## Description
-        When you attach your workspace network to a Cloud Enterprise Network (CEN) instance in another Alibaba Cloud account, you need to call this operation to obtain a verification code. After the call is successful, the system sends a verification code to the email address associated with the Alibaba Cloud account.
-        
-        @param request: SendVerifyCodeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SendVerifyCodeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.extra_info):
             query['ExtraInfo'] = request.extra_info
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.verify_code_action):
@@ -18137,404 +11669,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def send_verify_code(
         self,
         request: ecd_20200930_models.SendVerifyCodeRequest,
     ) -> ecd_20200930_models.SendVerifyCodeResponse:
-        """
-        ## Description
-        When you attach your workspace network to a Cloud Enterprise Network (CEN) instance in another Alibaba Cloud account, you need to call this operation to obtain a verification code. After the call is successful, the system sends a verification code to the email address associated with the Alibaba Cloud account.
-        
-        @param request: SendVerifyCodeRequest
-        @return: SendVerifyCodeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.send_verify_code_with_options(request, runtime)
 
     async def send_verify_code_async(
         self,
         request: ecd_20200930_models.SendVerifyCodeRequest,
     ) -> ecd_20200930_models.SendVerifyCodeResponse:
-        """
-        ## Description
-        When you attach your workspace network to a Cloud Enterprise Network (CEN) instance in another Alibaba Cloud account, you need to call this operation to obtain a verification code. After the call is successful, the system sends a verification code to the email address associated with the Alibaba Cloud account.
-        
-        @param request: SendVerifyCodeRequest
-        @return: SendVerifyCodeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.send_verify_code_with_options_async(request, runtime)
 
-    def set_desktop_group_scale_timer_with_options(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupScaleTimerRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDesktopGroupScaleTimerResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.scale_timer_infos):
-            query['ScaleTimerInfos'] = request.scale_timer_infos
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDesktopGroupScaleTimer',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDesktopGroupScaleTimerResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def set_desktop_group_scale_timer_with_options_async(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupScaleTimerRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDesktopGroupScaleTimerResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.scale_timer_infos):
-            query['ScaleTimerInfos'] = request.scale_timer_infos
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDesktopGroupScaleTimer',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDesktopGroupScaleTimerResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def set_desktop_group_scale_timer(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupScaleTimerRequest,
-    ) -> ecd_20200930_models.SetDesktopGroupScaleTimerResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.set_desktop_group_scale_timer_with_options(request, runtime)
-
-    async def set_desktop_group_scale_timer_async(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupScaleTimerRequest,
-    ) -> ecd_20200930_models.SetDesktopGroupScaleTimerResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.set_desktop_group_scale_timer_with_options_async(request, runtime)
-
-    def set_desktop_group_timer_with_options(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cron_expression):
-            query['CronExpression'] = request.cron_expression
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.force):
-            query['Force'] = request.force
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.reset_type):
-            query['ResetType'] = request.reset_type
-        if not UtilClient.is_unset(request.timer_type):
-            query['TimerType'] = request.timer_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDesktopGroupTimer',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDesktopGroupTimerResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def set_desktop_group_timer_with_options_async(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.cron_expression):
-            query['CronExpression'] = request.cron_expression
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.force):
-            query['Force'] = request.force
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.reset_type):
-            query['ResetType'] = request.reset_type
-        if not UtilClient.is_unset(request.timer_type):
-            query['TimerType'] = request.timer_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDesktopGroupTimer',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDesktopGroupTimerResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def set_desktop_group_timer(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerRequest,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.set_desktop_group_timer_with_options(request, runtime)
-
-    async def set_desktop_group_timer_async(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerRequest,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.set_desktop_group_timer_with_options_async(request, runtime)
-
-    def set_desktop_group_timer_status_with_options(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerStatusRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerStatusResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.timer_type):
-            query['TimerType'] = request.timer_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDesktopGroupTimerStatus',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDesktopGroupTimerStatusResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def set_desktop_group_timer_status_with_options_async(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerStatusRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerStatusResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.status):
-            query['Status'] = request.status
-        if not UtilClient.is_unset(request.timer_type):
-            query['TimerType'] = request.timer_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDesktopGroupTimerStatus',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDesktopGroupTimerStatusResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def set_desktop_group_timer_status(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerStatusRequest,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerStatusResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.set_desktop_group_timer_status_with_options(request, runtime)
-
-    async def set_desktop_group_timer_status_async(
-        self,
-        request: ecd_20200930_models.SetDesktopGroupTimerStatusRequest,
-    ) -> ecd_20200930_models.SetDesktopGroupTimerStatusResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.set_desktop_group_timer_status_with_options_async(request, runtime)
-
-    def set_directory_sso_status_with_options(
-        self,
-        request: ecd_20200930_models.SetDirectorySsoStatusRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDirectorySsoStatusResponse:
-        """
-        This operation is supported only for AD directories, not for RAM directories.
-        
-        @param request: SetDirectorySsoStatusRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetDirectorySsoStatusResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.enable_sso):
-            query['EnableSso'] = request.enable_sso
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDirectorySsoStatus',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDirectorySsoStatusResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def set_directory_sso_status_with_options_async(
-        self,
-        request: ecd_20200930_models.SetDirectorySsoStatusRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetDirectorySsoStatusResponse:
-        """
-        This operation is supported only for AD directories, not for RAM directories.
-        
-        @param request: SetDirectorySsoStatusRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetDirectorySsoStatusResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.directory_id):
-            query['DirectoryId'] = request.directory_id
-        if not UtilClient.is_unset(request.enable_sso):
-            query['EnableSso'] = request.enable_sso
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetDirectorySsoStatus',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetDirectorySsoStatusResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def set_directory_sso_status(
-        self,
-        request: ecd_20200930_models.SetDirectorySsoStatusRequest,
-    ) -> ecd_20200930_models.SetDirectorySsoStatusResponse:
-        """
-        This operation is supported only for AD directories, not for RAM directories.
-        
-        @param request: SetDirectorySsoStatusRequest
-        @return: SetDirectorySsoStatusResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.set_directory_sso_status_with_options(request, runtime)
-
-    async def set_directory_sso_status_async(
-        self,
-        request: ecd_20200930_models.SetDirectorySsoStatusRequest,
-    ) -> ecd_20200930_models.SetDirectorySsoStatusResponse:
-        """
-        This operation is supported only for AD directories, not for RAM directories.
-        
-        @param request: SetDirectorySsoStatusRequest
-        @return: SetDirectorySsoStatusResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.set_directory_sso_status_with_options_async(request, runtime)
-
     def set_idp_metadata_with_options(
         self,
         request: ecd_20200930_models.SetIdpMetadataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.SetIdpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: SetIdpMetadataRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetIdpMetadataResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.idp_metadata):
             query['IdpMetadata'] = request.idp_metadata
         if not UtilClient.is_unset(request.office_site_id):
@@ -18561,21 +11718,14 @@
         )
 
     async def set_idp_metadata_with_options_async(
         self,
         request: ecd_20200930_models.SetIdpMetadataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.SetIdpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: SetIdpMetadataRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetIdpMetadataResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.idp_metadata):
             query['IdpMetadata'] = request.idp_metadata
         if not UtilClient.is_unset(request.office_site_id):
@@ -18601,33 +11751,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_idp_metadata(
         self,
         request: ecd_20200930_models.SetIdpMetadataRequest,
     ) -> ecd_20200930_models.SetIdpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: SetIdpMetadataRequest
-        @return: SetIdpMetadataResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.set_idp_metadata_with_options(request, runtime)
 
     async def set_idp_metadata_async(
         self,
         request: ecd_20200930_models.SetIdpMetadataRequest,
     ) -> ecd_20200930_models.SetIdpMetadataResponse:
-        """
-        You can call this operation only for workspaces of the Active Directory (AD) and convenience account types.
-        
-        @param request: SetIdpMetadataRequest
-        @return: SetIdpMetadataResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.set_idp_metadata_with_options_async(request, runtime)
 
     def set_office_site_sso_status_with_options(
         self,
         request: ecd_20200930_models.SetOfficeSiteSsoStatusRequest,
         runtime: util_models.RuntimeOptions,
@@ -18701,116 +11839,19 @@
     async def set_office_site_sso_status_async(
         self,
         request: ecd_20200930_models.SetOfficeSiteSsoStatusRequest,
     ) -> ecd_20200930_models.SetOfficeSiteSsoStatusResponse:
         runtime = util_models.RuntimeOptions()
         return await self.set_office_site_sso_status_with_options_async(request, runtime)
 
-    def set_user_profile_path_rules_with_options(
-        self,
-        tmp_req: ecd_20200930_models.SetUserProfilePathRulesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetUserProfilePathRulesResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.SetUserProfilePathRulesShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_profile_path_rule):
-            request.user_profile_path_rule_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_profile_path_rule, 'UserProfilePathRule', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_profile_path_rule_shrink):
-            query['UserProfilePathRule'] = request.user_profile_path_rule_shrink
-        if not UtilClient.is_unset(request.user_profile_rule_type):
-            query['UserProfileRuleType'] = request.user_profile_rule_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetUserProfilePathRules',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetUserProfilePathRulesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def set_user_profile_path_rules_with_options_async(
-        self,
-        tmp_req: ecd_20200930_models.SetUserProfilePathRulesRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.SetUserProfilePathRulesResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ecd_20200930_models.SetUserProfilePathRulesShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_profile_path_rule):
-            request.user_profile_path_rule_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_profile_path_rule, 'UserProfilePathRule', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.desktop_group_id):
-            query['DesktopGroupId'] = request.desktop_group_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.user_profile_path_rule_shrink):
-            query['UserProfilePathRule'] = request.user_profile_path_rule_shrink
-        if not UtilClient.is_unset(request.user_profile_rule_type):
-            query['UserProfileRuleType'] = request.user_profile_rule_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetUserProfilePathRules',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.SetUserProfilePathRulesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def set_user_profile_path_rules(
-        self,
-        request: ecd_20200930_models.SetUserProfilePathRulesRequest,
-    ) -> ecd_20200930_models.SetUserProfilePathRulesResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.set_user_profile_path_rules_with_options(request, runtime)
-
-    async def set_user_profile_path_rules_async(
-        self,
-        request: ecd_20200930_models.SetUserProfilePathRulesRequest,
-    ) -> ecd_20200930_models.SetUserProfilePathRulesResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.set_user_profile_path_rules_with_options_async(request, runtime)
-
     def start_desktops_with_options(
         self,
         request: ecd_20200930_models.StartDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.StartDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: StartDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StartDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -18833,21 +11874,14 @@
         )
 
     async def start_desktops_with_options_async(
         self,
         request: ecd_20200930_models.StartDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.StartDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: StartDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StartDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -18869,33 +11903,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_desktops(
         self,
         request: ecd_20200930_models.StartDesktopsRequest,
     ) -> ecd_20200930_models.StartDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: StartDesktopsRequest
-        @return: StartDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.start_desktops_with_options(request, runtime)
 
     async def start_desktops_async(
         self,
         request: ecd_20200930_models.StartDesktopsRequest,
     ) -> ecd_20200930_models.StartDesktopsResponse:
-        """
-        The ID of the request.
-        
-        @param request: StartDesktopsRequest
-        @return: StartDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.start_desktops_with_options_async(request, runtime)
 
     def start_virus_scan_task_with_options(
         self,
         request: ecd_20200930_models.StartVirusScanTaskRequest,
         runtime: util_models.RuntimeOptions,
@@ -18974,24 +11996,14 @@
         return await self.start_virus_scan_task_with_options_async(request, runtime)
 
     def stop_desktops_with_options(
         self,
         request: ecd_20200930_models.StopDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.StopDesktopsResponse:
-        """
-        The billing mode after you stop the cloud desktop.
-        *   StopCharging: Computing resources are not billed after you stop the cloud desktop. After the cloud desktop is stopped, the system automatically reclaims computing resources. From this point on, you are no longer charged for computing resources. However, you are still charged for storage resources.
-        *   KeepCharging: The billing continues after you stop the cloud desktop. After the cloud desktop is stopped, the system does not reclaim resources to avoid startup failures due to insufficient resources. You are still charged for the resources.
-        Default value: StopCharging
-        
-        @param request: StopDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StopDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.stopped_mode):
@@ -19016,24 +12028,14 @@
         )
 
     async def stop_desktops_with_options_async(
         self,
         request: ecd_20200930_models.StopDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.StopDesktopsResponse:
-        """
-        The billing mode after you stop the cloud desktop.
-        *   StopCharging: Computing resources are not billed after you stop the cloud desktop. After the cloud desktop is stopped, the system automatically reclaims computing resources. From this point on, you are no longer charged for computing resources. However, you are still charged for storage resources.
-        *   KeepCharging: The billing continues after you stop the cloud desktop. After the cloud desktop is stopped, the system does not reclaim resources to avoid startup failures due to insufficient resources. You are still charged for the resources.
-        Default value: StopCharging
-        
-        @param request: StopDesktopsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StopDesktopsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.stopped_mode):
@@ -19057,54 +12059,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_desktops(
         self,
         request: ecd_20200930_models.StopDesktopsRequest,
     ) -> ecd_20200930_models.StopDesktopsResponse:
-        """
-        The billing mode after you stop the cloud desktop.
-        *   StopCharging: Computing resources are not billed after you stop the cloud desktop. After the cloud desktop is stopped, the system automatically reclaims computing resources. From this point on, you are no longer charged for computing resources. However, you are still charged for storage resources.
-        *   KeepCharging: The billing continues after you stop the cloud desktop. After the cloud desktop is stopped, the system does not reclaim resources to avoid startup failures due to insufficient resources. You are still charged for the resources.
-        Default value: StopCharging
-        
-        @param request: StopDesktopsRequest
-        @return: StopDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.stop_desktops_with_options(request, runtime)
 
     async def stop_desktops_async(
         self,
         request: ecd_20200930_models.StopDesktopsRequest,
     ) -> ecd_20200930_models.StopDesktopsResponse:
-        """
-        The billing mode after you stop the cloud desktop.
-        *   StopCharging: Computing resources are not billed after you stop the cloud desktop. After the cloud desktop is stopped, the system automatically reclaims computing resources. From this point on, you are no longer charged for computing resources. However, you are still charged for storage resources.
-        *   KeepCharging: The billing continues after you stop the cloud desktop. After the cloud desktop is stopped, the system does not reclaim resources to avoid startup failures due to insufficient resources. You are still charged for the resources.
-        Default value: StopCharging
-        
-        @param request: StopDesktopsRequest
-        @return: StopDesktopsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_desktops_with_options_async(request, runtime)
 
     def stop_invocation_with_options(
         self,
         request: ecd_20200930_models.StopInvocationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.StopInvocationResponse:
-        """
-        The ID of the execution.
-        
-        @param request: StopInvocationRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StopInvocationResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.invoke_id):
             query['InvokeId'] = request.invoke_id
         if not UtilClient.is_unset(request.region_id):
@@ -19129,21 +12106,14 @@
         )
 
     async def stop_invocation_with_options_async(
         self,
         request: ecd_20200930_models.StopInvocationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.StopInvocationResponse:
-        """
-        The ID of the execution.
-        
-        @param request: StopInvocationRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StopInvocationResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desktop_id):
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.invoke_id):
             query['InvokeId'] = request.invoke_id
         if not UtilClient.is_unset(request.region_id):
@@ -19167,48 +12137,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_invocation(
         self,
         request: ecd_20200930_models.StopInvocationRequest,
     ) -> ecd_20200930_models.StopInvocationResponse:
-        """
-        The ID of the execution.
-        
-        @param request: StopInvocationRequest
-        @return: StopInvocationResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.stop_invocation_with_options(request, runtime)
 
     async def stop_invocation_async(
         self,
         request: ecd_20200930_models.StopInvocationRequest,
     ) -> ecd_20200930_models.StopInvocationResponse:
-        """
-        The ID of the execution.
-        
-        @param request: StopInvocationRequest
-        @return: StopInvocationResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_invocation_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: ecd_20200930_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.TagResourcesResponse:
-        """
-        If TagKey is specified, the new TagValue value overrides the original TagValue value.
-        
-        @param request: TagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: TagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
@@ -19235,21 +12186,14 @@
         )
 
     async def tag_resources_with_options_async(
         self,
         request: ecd_20200930_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20200930_models.TagResourcesResponse:
-        """
-        If TagKey is specified, the new TagValue value overrides the original TagValue value.
-        
-        @param request: TagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: TagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
@@ -19275,33 +12219,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def tag_resources(
         self,
         request: ecd_20200930_models.TagResourcesRequest,
     ) -> ecd_20200930_models.TagResourcesResponse:
-        """
-        If TagKey is specified, the new TagValue value overrides the original TagValue value.
-        
-        @param request: TagResourcesRequest
-        @return: TagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     async def tag_resources_async(
         self,
         request: ecd_20200930_models.TagResourcesRequest,
     ) -> ecd_20200930_models.TagResourcesResponse:
-        """
-        If TagKey is specified, the new TagValue value overrides the original TagValue value.
-        
-        @param request: TagResourcesRequest
-        @return: TagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.tag_resources_with_options_async(request, runtime)
 
     def unlock_virtual_mfadevice_with_options(
         self,
         request: ecd_20200930_models.UnlockVirtualMFADeviceRequest,
         runtime: util_models.RuntimeOptions,
@@ -19730,81 +12662,7 @@
 
     async def verify_cen_async(
         self,
         request: ecd_20200930_models.VerifyCenRequest,
     ) -> ecd_20200930_models.VerifyCenResponse:
         runtime = util_models.RuntimeOptions()
         return await self.verify_cen_with_options_async(request, runtime)
-
-    def wakeup_desktops_with_options(
-        self,
-        request: ecd_20200930_models.WakeupDesktopsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.WakeupDesktopsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='WakeupDesktops',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.WakeupDesktopsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def wakeup_desktops_with_options_async(
-        self,
-        request: ecd_20200930_models.WakeupDesktopsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ecd_20200930_models.WakeupDesktopsResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.desktop_id):
-            query['DesktopId'] = request.desktop_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='WakeupDesktops',
-            version='2020-09-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ecd_20200930_models.WakeupDesktopsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def wakeup_desktops(
-        self,
-        request: ecd_20200930_models.WakeupDesktopsRequest,
-    ) -> ecd_20200930_models.WakeupDesktopsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.wakeup_desktops_with_options(request, runtime)
-
-    async def wakeup_desktops_async(
-        self,
-        request: ecd_20200930_models.WakeupDesktopsRequest,
-    ) -> ecd_20200930_models.WakeupDesktopsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.wakeup_desktops_with_options_async(request, runtime)
```

### Comparing `alibabacloud_ecd20200930-2.0.16/alibabacloud_ecd20200930.egg-info/PKG-INFO` & `alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ecd20200930
-Version: 2.0.16
+Version: 2.0.7
 Summary: Alibaba Cloud ecd (20200930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20200930-2.0.16/setup.py` & `alibabacloud_ecd20200930-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ecd20200930.
 
-Created on 01/08/2023
+Created on 12/07/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ecd20200930"
 NAME = "alibabacloud_ecd20200930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ecd (20200930) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

