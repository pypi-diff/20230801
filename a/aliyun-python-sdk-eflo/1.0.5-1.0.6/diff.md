# Comparing `tmp/aliyun-python-sdk-eflo-1.0.5.tar.gz` & `tmp/aliyun-python-sdk-eflo-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eflo-1.0.5.tar", last modified: Wed Apr 26 09:32:50 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eflo-1.0.6.tar", last modified: Tue Aug  1 06:29:22 2023, max compression
```

## Comparing `aliyun-python-sdk-eflo-1.0.5.tar` & `aliyun-python-sdk-eflo-1.0.6.tar`

### file list

```diff
@@ -1,72 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3420 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/
--rw-r--r--   0 root         (0) root         (0)     2042 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateErRequest.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2887 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteErRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErRequest.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1224 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     3200 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3556 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVccsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateErRequest.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-04-26 09:32:50.000000 aliyun-python-sdk-eflo-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:29:22.000000 aliyun-python-sdk-eflo-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-08-01 06:29:22.000000 aliyun-python-sdk-eflo-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:29:22.000000 aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:29:22.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:29:22.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:29:22.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/AssociateVpdCidrBlockRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetFabricTopologyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListInstancesByNcdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVccsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/QueryInstanceNcdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UnAssociateVpdCidrBlockRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-01 06:29:22.000000 aliyun-python-sdk-eflo-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-08-01 06:29:21.000000 aliyun-python-sdk-eflo-1.0.6/setup.py
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/LICENSE` & `aliyun-python-sdk-eflo-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/PKG-INFO` & `aliyun-python-sdk-eflo-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eflo
-Version: 1.0.5
+Version: 1.0.6
 Summary: The eflo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eflo
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/README.rst` & `aliyun-python-sdk-eflo-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/PKG-INFO` & `aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eflo
-Version: 1.0.5
+Version: 1.0.6
 Summary: The eflo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eflo
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyun_python_sdk_eflo.egg-info/SOURCES.txt` & `aliyun-python-sdk-eflo-1.0.6/aliyun_python_sdk_eflo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 aliyun_python_sdk_eflo.egg-info/SOURCES.txt
 aliyun_python_sdk_eflo.egg-info/dependency_links.txt
 aliyun_python_sdk_eflo.egg-info/requires.txt
 aliyun_python_sdk_eflo.egg-info/top_level.txt
 aliyunsdkeflo/__init__.py
 aliyunsdkeflo/request/__init__.py
 aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
+aliyunsdkeflo/request/v20220530/AssociateVpdCidrBlockRequest.py
 aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py
 aliyunsdkeflo/request/v20220530/CreateErRequest.py
 aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py
 aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
 aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/CreateVccRequest.py
 aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py
@@ -29,38 +30,42 @@
 aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
 aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
 aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
 aliyunsdkeflo/request/v20220530/GetErRequest.py
 aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
+aliyunsdkeflo/request/v20220530/GetFabricTopologyRequest.py
 aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
 aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
 aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
 aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/GetVccRequest.py
 aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/GetVpdRequest.py
 aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
 aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
 aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
 aliyunsdkeflo/request/v20220530/ListErsRequest.py
+aliyunsdkeflo/request/v20220530/ListInstancesByNcdRequest.py
 aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
 aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
 aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
 aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
 aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListVccsRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
+aliyunsdkeflo/request/v20220530/QueryInstanceNcdRequest.py
 aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
+aliyunsdkeflo/request/v20220530/UnAssociateVpdCidrBlockRequest.py
 aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py
 aliyunsdkeflo/request/v20220530/UpdateErRequest.py
 aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py
 aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
 aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
 aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
 aliyunsdkeflo/request/v20220530/__init__.py
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,29 +21,34 @@
 
 class AssignPrivateIpAddressRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'AssignPrivateIpAddress','eflo')
 		self.set_method('POST')
 
+	def get_Description(self): # String
+		return self.get_body_params().get('Description')
+
+	def set_Description(self, Description):  # String
+		self.add_body_params('Description', Description)
+	def get_AssignMac(self): # Boolean
+		return self.get_body_params().get('AssignMac')
+
+	def set_AssignMac(self, AssignMac):  # Boolean
+		self.add_body_params('AssignMac', AssignMac)
 	def get_SubnetId(self): # String
 		return self.get_body_params().get('SubnetId')
 
 	def set_SubnetId(self, SubnetId):  # String
 		self.add_body_params('SubnetId', SubnetId)
 	def get_SkipConfig(self): # Boolean
 		return self.get_body_params().get('SkipConfig')
 
 	def set_SkipConfig(self, SkipConfig):  # Boolean
 		self.add_body_params('SkipConfig', SkipConfig)
-	def get_AssignMac(self): # Boolean
-		return self.get_body_params().get('AssignMac')
-
-	def set_AssignMac(self, AssignMac):  # Boolean
-		self.add_body_params('AssignMac', AssignMac)
 	def get_PrivateIpAddress(self): # String
 		return self.get_body_params().get('PrivateIpAddress')
 
 	def set_PrivateIpAddress(self, PrivateIpAddress):  # String
 		self.add_body_params('PrivateIpAddress', PrivateIpAddress)
 	def get_NetworkInterfaceId(self): # String
 		return self.get_body_params().get('NetworkInterfaceId')
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateErRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVccRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVccRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 	def set_CenId(self, CenId):  # String
 		self.add_body_params('CenId', CenId)
 	def get_Description(self): # String
 		return self.get_body_params().get('Description')
 
 	def set_Description(self, Description):  # String
 		self.add_body_params('Description', Description)
+	def get_CenOwnerId(self): # String
+		return self.get_body_params().get('CenOwnerId')
+
+	def set_CenOwnerId(self, CenOwnerId):  # String
+		self.add_body_params('CenOwnerId', CenOwnerId)
 	def get_AccessCouldService(self): # Boolean
 		return self.get_body_params().get('AccessCouldService')
 
 	def set_AccessCouldService(self, AccessCouldService):  # Boolean
 		self.add_body_params('AccessCouldService', AccessCouldService)
 	def get_ResourceGroupId(self): # String
 		return self.get_body_params().get('ResourceGroupId')
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteErRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVccRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,63 +15,72 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ListErRouteEntriesRequest(RpcRequest):
+class ListSubnetsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListErRouteEntries','eflo')
+		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListSubnets','eflo')
 		self.set_method('POST')
 
+	def get_Type(self): # String
+		return self.get_body_params().get('Type')
+
+	def set_Type(self, Type):  # String
+		self.add_body_params('Type', Type)
 	def get_PageNumber(self): # Integer
 		return self.get_body_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_body_params('PageNumber', PageNumber)
-	def get_RouteType(self): # String
-		return self.get_body_params().get('RouteType')
+	def get_ResourceGroupId(self): # String
+		return self.get_body_params().get('ResourceGroupId')
 
-	def set_RouteType(self, RouteType):  # String
-		self.add_body_params('RouteType', RouteType)
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_body_params('ResourceGroupId', ResourceGroupId)
 	def get_PageSize(self): # Integer
 		return self.get_body_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_body_params('PageSize', PageSize)
-	def get_NextHopId(self): # String
-		return self.get_body_params().get('NextHopId')
+	def get_Tags(self): # RepeatList
+		return self.get_body_params().get('Tag')
 
-	def set_NextHopId(self, NextHopId):  # String
-		self.add_body_params('NextHopId', NextHopId)
-	def get_NextHopType(self): # String
-		return self.get_body_params().get('NextHopType')
-
-	def set_NextHopType(self, NextHopType):  # String
-		self.add_body_params('NextHopType', NextHopType)
-	def get_DestinationCidrBlock(self): # String
-		return self.get_body_params().get('DestinationCidrBlock')
-
-	def set_DestinationCidrBlock(self, DestinationCidrBlock):  # String
-		self.add_body_params('DestinationCidrBlock', DestinationCidrBlock)
-	def get_ErId(self): # String
-		return self.get_body_params().get('ErId')
-
-	def set_ErId(self, ErId):  # String
-		self.add_body_params('ErId', ErId)
-	def get_InstanceId(self): # String
-		return self.get_body_params().get('InstanceId')
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Value') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+			if Tag[depth1].get('Key') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+	def get_SubnetId(self): # String
+		return self.get_body_params().get('SubnetId')
+
+	def set_SubnetId(self, SubnetId):  # String
+		self.add_body_params('SubnetId', SubnetId)
+	def get_VpdId(self): # String
+		return self.get_body_params().get('VpdId')
 
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_body_params('InstanceId', InstanceId)
+	def set_VpdId(self, VpdId):  # String
+		self.add_body_params('VpdId', VpdId)
 	def get_EnablePage(self): # Boolean
 		return self.get_body_params().get('EnablePage')
 
 	def set_EnablePage(self, EnablePage):  # Boolean
 		self.add_body_params('EnablePage', EnablePage)
+	def get_ZoneId(self): # String
+		return self.get_body_params().get('ZoneId')
+
+	def set_ZoneId(self, ZoneId):  # String
+		self.add_body_params('ZoneId', ZoneId)
+	def get_SubnetName(self): # String
+		return self.get_body_params().get('SubnetName')
+
+	def set_SubnetName(self, SubnetName):  # String
+		self.add_body_params('SubnetName', SubnetName)
 	def get_Status(self): # String
 		return self.get_body_params().get('Status')
 
 	def set_Status(self, Status):  # String
 		self.add_body_params('Status', Status)
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListErsRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 
 class ListLniPrivateIpAddressRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListLniPrivateIpAddress','eflo')
 		self.set_method('POST')
 
+	def get_Description(self): # String
+		return self.get_body_params().get('Description')
+
+	def set_Description(self, Description):  # String
+		self.add_body_params('Description', Description)
 	def get_PageNumber(self): # Integer
 		return self.get_body_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_body_params('PageNumber', PageNumber)
 	def get_PageSize(self): # Integer
 		return self.get_body_params().get('PageSize')
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,72 +15,77 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ListSubnetsRequest(RpcRequest):
+class ListVpdsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListSubnets','eflo')
+		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListVpds','eflo')
 		self.set_method('POST')
 
-	def get_Type(self): # String
-		return self.get_body_params().get('Type')
+	def get_VpdName(self): # String
+		return self.get_body_params().get('VpdName')
 
-	def set_Type(self, Type):  # String
-		self.add_body_params('Type', Type)
+	def set_VpdName(self, VpdName):  # String
+		self.add_body_params('VpdName', VpdName)
 	def get_PageNumber(self): # Integer
 		return self.get_body_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_body_params('PageNumber', PageNumber)
+	def get_WithDependence(self): # Boolean
+		return self.get_body_params().get('WithDependence')
+
+	def set_WithDependence(self, WithDependence):  # Boolean
+		self.add_body_params('WithDependence', WithDependence)
 	def get_ResourceGroupId(self): # String
 		return self.get_body_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_body_params('ResourceGroupId', ResourceGroupId)
+	def get_WithoutVcc(self): # Boolean
+		return self.get_body_params().get('WithoutVcc')
+
+	def set_WithoutVcc(self, WithoutVcc):  # Boolean
+		self.add_body_params('WithoutVcc', WithoutVcc)
 	def get_PageSize(self): # Integer
 		return self.get_body_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_body_params('PageSize', PageSize)
 	def get_Tags(self): # RepeatList
 		return self.get_body_params().get('Tag')
 
 	def set_Tags(self, Tag):  # RepeatList
 		for depth1 in range(len(Tag)):
 			if Tag[depth1].get('Value') is not None:
 				self.add_body_params('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 			if Tag[depth1].get('Key') is not None:
 				self.add_body_params('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
-	def get_SubnetId(self): # String
-		return self.get_body_params().get('SubnetId')
+	def get_ForSelect(self): # Boolean
+		return self.get_body_params().get('ForSelect')
+
+	def set_ForSelect(self, ForSelect):  # Boolean
+		self.add_body_params('ForSelect', ForSelect)
+	def get_FilterErId(self): # String
+		return self.get_body_params().get('FilterErId')
 
-	def set_SubnetId(self, SubnetId):  # String
-		self.add_body_params('SubnetId', SubnetId)
+	def set_FilterErId(self, FilterErId):  # String
+		self.add_body_params('FilterErId', FilterErId)
 	def get_VpdId(self): # String
 		return self.get_body_params().get('VpdId')
 
 	def set_VpdId(self, VpdId):  # String
 		self.add_body_params('VpdId', VpdId)
 	def get_EnablePage(self): # Boolean
 		return self.get_body_params().get('EnablePage')
 
 	def set_EnablePage(self, EnablePage):  # Boolean
 		self.add_body_params('EnablePage', EnablePage)
-	def get_ZoneId(self): # String
-		return self.get_body_params().get('ZoneId')
-
-	def set_ZoneId(self, ZoneId):  # String
-		self.add_body_params('ZoneId', ZoneId)
-	def get_SubnetName(self): # String
-		return self.get_body_params().get('SubnetName')
-
-	def set_SubnetName(self, SubnetName):  # String
-		self.add_body_params('SubnetName', SubnetName)
 	def get_Status(self): # String
 		return self.get_body_params().get('Status')
 
 	def set_Status(self, Status):  # String
 		self.add_body_params('Status', Status)
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 
 class ListVccRouteEntriesRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListVccRouteEntries','eflo')
 		self.set_method('POST')
 
+	def get_IgnoreDetailedRouteEntry(self): # Boolean
+		return self.get_body_params().get('IgnoreDetailedRouteEntry')
+
+	def set_IgnoreDetailedRouteEntry(self, IgnoreDetailedRouteEntry):  # Boolean
+		self.add_body_params('IgnoreDetailedRouteEntry', IgnoreDetailedRouteEntry)
 	def get_PageNumber(self): # Integer
 		return self.get_body_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_body_params('PageNumber', PageNumber)
 	def get_RouteType(self): # String
 		return self.get_body_params().get('RouteType')
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVccsRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVccsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 
 class ListVpdRouteEntriesRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListVpdRouteEntries','eflo')
 		self.set_method('POST')
 
+	def get_IgnoreDetailedRouteEntry(self): # Boolean
+		return self.get_body_params().get('IgnoreDetailedRouteEntry')
+
+	def set_IgnoreDetailedRouteEntry(self, IgnoreDetailedRouteEntry):  # Boolean
+		self.add_body_params('IgnoreDetailedRouteEntry', IgnoreDetailedRouteEntry)
 	def get_PageNumber(self): # Integer
 		return self.get_body_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_body_params('PageNumber', PageNumber)
 	def get_RouteType(self): # String
 		return self.get_body_params().get('RouteType')
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,74 +15,65 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ListVpdsRequest(RpcRequest):
+class ListErRouteEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListVpds','eflo')
+		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListErRouteEntries','eflo')
 		self.set_method('POST')
 
-	def get_VpdName(self): # String
-		return self.get_body_params().get('VpdName')
+	def get_IgnoreDetailedRouteEntry(self): # Boolean
+		return self.get_body_params().get('IgnoreDetailedRouteEntry')
 
-	def set_VpdName(self, VpdName):  # String
-		self.add_body_params('VpdName', VpdName)
+	def set_IgnoreDetailedRouteEntry(self, IgnoreDetailedRouteEntry):  # Boolean
+		self.add_body_params('IgnoreDetailedRouteEntry', IgnoreDetailedRouteEntry)
 	def get_PageNumber(self): # Integer
 		return self.get_body_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_body_params('PageNumber', PageNumber)
-	def get_WithDependence(self): # Boolean
-		return self.get_body_params().get('WithDependence')
+	def get_RouteType(self): # String
+		return self.get_body_params().get('RouteType')
 
-	def set_WithDependence(self, WithDependence):  # Boolean
-		self.add_body_params('WithDependence', WithDependence)
-	def get_ResourceGroupId(self): # String
-		return self.get_body_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_body_params('ResourceGroupId', ResourceGroupId)
-	def get_WithoutVcc(self): # Boolean
-		return self.get_body_params().get('WithoutVcc')
-
-	def set_WithoutVcc(self, WithoutVcc):  # Boolean
-		self.add_body_params('WithoutVcc', WithoutVcc)
+	def set_RouteType(self, RouteType):  # String
+		self.add_body_params('RouteType', RouteType)
 	def get_PageSize(self): # Integer
 		return self.get_body_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_body_params('PageSize', PageSize)
-	def get_Tags(self): # RepeatList
-		return self.get_body_params().get('Tag')
+	def get_NextHopId(self): # String
+		return self.get_body_params().get('NextHopId')
 
-	def set_Tags(self, Tag):  # RepeatList
-		for depth1 in range(len(Tag)):
-			if Tag[depth1].get('Value') is not None:
-				self.add_body_params('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
-			if Tag[depth1].get('Key') is not None:
-				self.add_body_params('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
-	def get_ForSelect(self): # Boolean
-		return self.get_body_params().get('ForSelect')
-
-	def set_ForSelect(self, ForSelect):  # Boolean
-		self.add_body_params('ForSelect', ForSelect)
-	def get_FilterErId(self): # String
-		return self.get_body_params().get('FilterErId')
-
-	def set_FilterErId(self, FilterErId):  # String
-		self.add_body_params('FilterErId', FilterErId)
-	def get_VpdId(self): # String
-		return self.get_body_params().get('VpdId')
+	def set_NextHopId(self, NextHopId):  # String
+		self.add_body_params('NextHopId', NextHopId)
+	def get_NextHopType(self): # String
+		return self.get_body_params().get('NextHopType')
+
+	def set_NextHopType(self, NextHopType):  # String
+		self.add_body_params('NextHopType', NextHopType)
+	def get_DestinationCidrBlock(self): # String
+		return self.get_body_params().get('DestinationCidrBlock')
+
+	def set_DestinationCidrBlock(self, DestinationCidrBlock):  # String
+		self.add_body_params('DestinationCidrBlock', DestinationCidrBlock)
+	def get_ErId(self): # String
+		return self.get_body_params().get('ErId')
+
+	def set_ErId(self, ErId):  # String
+		self.add_body_params('ErId', ErId)
+	def get_InstanceId(self): # String
+		return self.get_body_params().get('InstanceId')
 
-	def set_VpdId(self, VpdId):  # String
-		self.add_body_params('VpdId', VpdId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_body_params('InstanceId', InstanceId)
 	def get_EnablePage(self): # Boolean
 		return self.get_body_params().get('EnablePage')
 
 	def set_EnablePage(self, EnablePage):  # Boolean
 		self.add_body_params('EnablePage', EnablePage)
 	def get_Status(self): # String
 		return self.get_body_params().get('Status')
```

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateErRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateErRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.6/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.5/setup.py` & `aliyun-python-sdk-eflo-1.0.6/setup.py`

 * *Files identical despite different names*

