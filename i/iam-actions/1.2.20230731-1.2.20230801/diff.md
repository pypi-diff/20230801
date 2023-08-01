# Comparing `tmp/iam_actions-1.2.20230731.tar.gz` & `tmp/iam_actions-1.2.20230801.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230731.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230801.tar", max compression
```

## Comparing `iam_actions-1.2.20230731.tar` & `iam_actions-1.2.20230801.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/README.md
--rw-r--r--   0        0        0      228 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/__init__.py
--rw-r--r--   0        0        0  4382239 2023-07-31 02:28:06.302043 iam_actions-1.2.20230731/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-31 02:26:08.910301 iam_actions-1.2.20230731/iam_actions/generate/services.py
--rw-r--r--   0        0        0   565259 2023-07-31 02:28:06.302043 iam_actions-1.2.20230731/iam_actions/policies.json
--rw-r--r--   0        0        0   196251 2023-07-31 02:28:06.302043 iam_actions-1.2.20230731/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   548317 2023-07-31 02:28:06.302043 iam_actions-1.2.20230731/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-31 02:28:07.050044 iam_actions-1.2.20230731/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230731/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230731/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/LICENSE
+-rw-r--r--   0        0        0     2302 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/README.md
+-rw-r--r--   0        0        0      228 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4384975 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   565668 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/policies.json
+-rw-r--r--   0        0        0   196374 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   548714 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-08-01 02:34:01.697726 iam_actions-1.2.20230801/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230801/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230801/PKG-INFO
```

### Comparing `iam_actions-1.2.20230731/LICENSE` & `iam_actions-1.2.20230801/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/README.md` & `iam_actions-1.2.20230801/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/iam_actions/actions.json` & `iam_actions-1.2.20230801/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996521608591887%*

 * *Differences: {"'cleanrooms'": "{'BatchGetCollaborationAnalysisTemplate': OrderedDict([('access_level', "*

 * *                 "'Undocumented'), ('action', 'BatchGetCollaborationAnalysisTemplate'), "*

 * *                 "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *                 "False), ('resources', [])]), 'UpdateAnalysisTemplate': "*

 * *                 "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                 "'UpdateAnalysisTemplate'), ('condition_keys', []), ('descripti […]*

```diff
@@ -17773,22 +17773,38 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
+        "BatchGetCollaborationAnalysisTemplate": {
+            "access_level": "Undocumented",
+            "action": "BatchGetCollaborationAnalysisTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchGetSchema": {
             "access_level": "Undocumented",
             "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "CreateAnalysisTemplate": {
+            "access_level": "Undocumented",
+            "action": "CreateAnalysisTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateCollaboration": {
             "access_level": "Undocumented",
             "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -17821,14 +17837,22 @@
             "access_level": "Undocumented",
             "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "DeleteAnalysisTemplate": {
+            "access_level": "Undocumented",
+            "action": "DeleteAnalysisTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteCollaboration": {
             "access_level": "Undocumented",
             "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -17869,22 +17893,38 @@
             "access_level": "Undocumented",
             "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetAnalysisTemplate": {
+            "access_level": "Undocumented",
+            "action": "GetAnalysisTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetCollaboration": {
             "access_level": "Undocumented",
             "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetCollaborationAnalysisTemplate": {
+            "access_level": "Undocumented",
+            "action": "GetCollaborationAnalysisTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetConfiguredTable": {
             "access_level": "Undocumented",
             "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -17933,14 +17973,30 @@
             "access_level": "Undocumented",
             "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListAnalysisTemplates": {
+            "access_level": "Undocumented",
+            "action": "ListAnalysisTemplates",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListCollaborationAnalysisTemplates": {
+            "access_level": "Undocumented",
+            "action": "ListCollaborationAnalysisTemplates",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListCollaborations": {
             "access_level": "Undocumented",
             "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -18021,14 +18077,22 @@
             "access_level": "Undocumented",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "UpdateAnalysisTemplate": {
+            "access_level": "Undocumented",
+            "action": "UpdateAnalysisTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateCollaboration": {
             "access_level": "Undocumented",
             "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -29644,17 +29708,15 @@
         },
         "DescribeComplianceByConfigRule": {
             "access_level": "Read",
             "action": "DescribeComplianceByConfigRule",
             "condition_keys": [],
             "description": "Grants permission to indicate whether the specified AWS Config rules are compliant",
             "orphan": false,
-            "resources": [
-                "ConfigRule"
-            ]
+            "resources": []
         },
         "DescribeComplianceByResource": {
             "access_level": "Read",
             "action": "DescribeComplianceByResource",
             "condition_keys": [],
             "description": "Grants permission to indicate whether the specified AWS resources are compliant",
             "orphan": false,
@@ -29662,27 +29724,23 @@
         },
         "DescribeConfigRuleEvaluationStatus": {
             "access_level": "Read",
             "action": "DescribeConfigRuleEvaluationStatus",
             "condition_keys": [],
             "description": "Grants permission to return status information for each of your AWS managed Config rules",
             "orphan": false,
-            "resources": [
-                "ConfigRule"
-            ]
+            "resources": []
         },
         "DescribeConfigRules": {
             "access_level": "List",
             "action": "DescribeConfigRules",
             "condition_keys": [],
             "description": "Grants permission to return details about your AWS Config rules",
             "orphan": false,
-            "resources": [
-                "ConfigRule"
-            ]
+            "resources": []
         },
         "DescribeConfigurationAggregatorSourcesStatus": {
             "access_level": "Read",
             "action": "DescribeConfigurationAggregatorSourcesStatus",
             "condition_keys": [],
             "description": "Grants permission to return status information for sources within an aggregator",
             "orphan": false,
@@ -29726,27 +29784,23 @@
         },
         "DescribeConformancePackStatus": {
             "access_level": "Read",
             "action": "DescribeConformancePackStatus",
             "condition_keys": [],
             "description": "Grants permission to provide one or more conformance packs deployment status",
             "orphan": false,
-            "resources": [
-                "ConformancePack"
-            ]
+            "resources": []
         },
         "DescribeConformancePacks": {
             "access_level": "List",
             "action": "DescribeConformancePacks",
             "condition_keys": [],
             "description": "Grants permission to return a list of one or more conformance packs",
             "orphan": false,
-            "resources": [
-                "ConformancePack"
-            ]
+            "resources": []
         },
         "DescribeDeliveryChannelStatus": {
             "access_level": "Read",
             "action": "DescribeDeliveryChannelStatus",
             "condition_keys": [],
             "description": "Grants permission to return the current status of the specified delivery channel",
             "orphan": false,
@@ -29762,47 +29816,39 @@
         },
         "DescribeOrganizationConfigRuleStatuses": {
             "access_level": "Read",
             "action": "DescribeOrganizationConfigRuleStatuses",
             "condition_keys": [],
             "description": "Grants permission to provide organization config rule deployment status for an organization",
             "orphan": false,
-            "resources": [
-                "OrganizationConfigRule"
-            ]
+            "resources": []
         },
         "DescribeOrganizationConfigRules": {
             "access_level": "List",
             "action": "DescribeOrganizationConfigRules",
             "condition_keys": [],
             "description": "Grants permission to return a list of organization config rules",
             "orphan": false,
-            "resources": [
-                "OrganizationConfigRule"
-            ]
+            "resources": []
         },
         "DescribeOrganizationConformancePackStatuses": {
             "access_level": "Read",
             "action": "DescribeOrganizationConformancePackStatuses",
             "condition_keys": [],
             "description": "Grants permission to provide organization conformance pack deployment status for an organization",
             "orphan": false,
-            "resources": [
-                "OrganizationConformancePack"
-            ]
+            "resources": []
         },
         "DescribeOrganizationConformancePacks": {
             "access_level": "List",
             "action": "DescribeOrganizationConformancePacks",
             "condition_keys": [],
             "description": "Grants permission to return a list of organization conformance packs",
             "orphan": false,
-            "resources": [
-                "OrganizationConformancePack"
-            ]
+            "resources": []
         },
         "DescribePendingAggregationRequests": {
             "access_level": "List",
             "action": "DescribePendingAggregationRequests",
             "condition_keys": [],
             "description": "Grants permission to return a list of all pending aggregation requests",
             "orphan": false,
@@ -84207,18 +84253,18 @@
             "action": "DescribeClusterOperation",
             "condition_keys": [],
             "description": "Grants permission to describe the cluster operation that is specified by the given ARN",
             "orphan": false,
             "resources": []
         },
         "DescribeClusterOperationV2": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeClusterOperationV2",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe the cluster operation that is specified by the given ARN",
             "orphan": false,
             "resources": []
         },
         "DescribeClusterV2": {
             "access_level": "Read",
             "action": "DescribeClusterV2",
             "condition_keys": [],
@@ -84301,20 +84347,22 @@
             "description": "Grants permission to return a list of all the operations that have been performed on the specified MSK cluster",
             "orphan": false,
             "resources": [
                 "cluster"
             ]
         },
         "ListClusterOperationsV2": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListClusterOperationsV2",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return a list of all the operations that have been performed on the specified MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "ListClusters": {
             "access_level": "List",
             "action": "ListClusters",
             "condition_keys": [],
             "description": "Grants permission to list all MSK clusters in this account",
             "orphan": false,
@@ -96668,14 +96716,22 @@
                 "channel",
                 "input",
                 "input-security-group",
                 "multiplex",
                 "reservation"
             ]
         },
+        "DescribeAccountConfiguration": {
+            "access_level": "Undocumented",
+            "action": "DescribeAccountConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeChannel": {
             "access_level": "Read",
             "action": "DescribeChannel",
             "condition_keys": [],
             "description": "Grants permission to get details about a channel",
             "orphan": false,
             "resources": [
@@ -96768,14 +96824,22 @@
             "condition_keys": [],
             "description": "Grants permission to view a list of actions scheduled on a channel",
             "orphan": false,
             "resources": [
                 "channel"
             ]
         },
+        "DescribeThumbnails": {
+            "access_level": "Undocumented",
+            "action": "DescribeThumbnails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListChannels": {
             "access_level": "List",
             "action": "ListChannels",
             "condition_keys": [],
             "description": "Grants permission to list channels",
             "orphan": false,
             "resources": []
@@ -96948,14 +97012,22 @@
             "condition_keys": [],
             "description": "Grants permission to transfer an input device",
             "orphan": false,
             "resources": [
                 "input-device"
             ]
         },
+        "UpdateAccountConfiguration": {
+            "access_level": "Undocumented",
+            "action": "UpdateAccountConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateChannel": {
             "access_level": "Write",
             "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Grants permission to update a channel",
             "orphan": false,
             "resources": [
@@ -110503,20 +110575,22 @@
             "description": "Grants permission to delete component",
             "orphan": false,
             "resources": [
                 "component"
             ]
         },
         "DeleteDeployment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteDeployment",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a deployment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "deployment"
+            ]
         },
         "DeleteEnvironment": {
             "access_level": "Write",
             "action": "DeleteEnvironment",
             "condition_keys": [
                 "proton:EnvironmentTemplate"
             ],
@@ -110677,20 +110751,22 @@
             "description": "Grants permission to describe a component",
             "orphan": false,
             "resources": [
                 "component"
             ]
         },
         "GetDeployment": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetDeployment",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a deployment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "deployment"
+            ]
         },
         "GetEnvironment": {
             "access_level": "Read",
             "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Grants permission to describe an environment",
             "orphan": false,
@@ -110885,15 +110961,16 @@
         "ListComponentOutputs": {
             "access_level": "List",
             "action": "ListComponentOutputs",
             "condition_keys": [],
             "description": "Grants permission to list component outputs",
             "orphan": false,
             "resources": [
-                "component"
+                "component",
+                "deployment"
             ]
         },
         "ListComponentProvisionedResources": {
             "access_level": "List",
             "action": "ListComponentProvisionedResources",
             "condition_keys": [],
             "description": "Grants permission to list component provisioned resources",
@@ -110911,18 +110988,18 @@
             "resources": [
                 "environment",
                 "service",
                 "service-instance"
             ]
         },
         "ListDeployments": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListDeployments",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list deployments",
             "orphan": false,
             "resources": []
         },
         "ListEnvironmentAccountConnections": {
             "access_level": "List",
             "action": "ListEnvironmentAccountConnections",
             "condition_keys": [],
@@ -110933,14 +111010,15 @@
         "ListEnvironmentOutputs": {
             "access_level": "List",
             "action": "ListEnvironmentOutputs",
             "condition_keys": [],
             "description": "Grants permission to list environment outputs",
             "orphan": false,
             "resources": [
+                "deployment",
                 "environment"
             ]
         },
         "ListEnvironmentProvisionedResources": {
             "access_level": "List",
             "action": "ListEnvironmentProvisionedResources",
             "condition_keys": [],
@@ -111015,14 +111093,15 @@
         "ListServiceInstanceOutputs": {
             "access_level": "List",
             "action": "ListServiceInstanceOutputs",
             "condition_keys": [],
             "description": "Grants permission to list service instance outputs",
             "orphan": false,
             "resources": [
+                "deployment",
                 "service",
                 "service-instance"
             ]
         },
         "ListServiceInstanceProvisionedResources": {
             "access_level": "List",
             "action": "ListServiceInstanceProvisionedResources",
@@ -111045,14 +111124,15 @@
         "ListServicePipelineOutputs": {
             "access_level": "List",
             "action": "ListServicePipelineOutputs",
             "condition_keys": [],
             "description": "Grants permission to list service pipeline outputs",
             "orphan": false,
             "resources": [
+                "deployment",
                 "service"
             ]
         },
         "ListServicePipelineProvisionedResources": {
             "access_level": "List",
             "action": "ListServicePipelineProvisionedResources",
             "condition_keys": [],
@@ -153893,14 +153973,22 @@
         "UpdateUser": {
             "access_level": "Write",
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Grants permission to update the specified attributes of the specified user, and grants or revokes administrative privileges to the Amazon WorkDocs site",
             "orphan": false,
             "resources": []
+        },
+        "UpdateUserAdministrativeSettings": {
+            "access_level": "Undocumented",
+            "action": "UpdateUserAdministrativeSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "worklink": {
         "AssociateDomain": {
             "access_level": "Write",
             "action": "AssociateDomain",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230731/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230801/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230801/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/iam_actions/generate/generate.py` & `iam_actions-1.2.20230801/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230801/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230801/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/iam_actions/generate/services.py` & `iam_actions-1.2.20230801/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230731/iam_actions/policies.json` & `iam_actions-1.2.20230801/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999971781339015%*

 * *Differences: {"'serviceMap'": "{'AWS Clean Rooms': {'Actions': {insert: [(0, "*

 * *                 "'BatchGetCollaborationAnalysisTemplate'), (2, 'CreateAnalysisTemplate'), (8, "*

 * *                 "'DeleteAnalysisTemplate'), (15, 'GetAnalysisTemplate'), (17, "*

 * *                 "'GetCollaborationAnalysisTemplate'), (25, 'ListAnalysisTemplates'), (26, "*

 * *                 "'ListCollaborationAnalysisTemplates'), (38, 'UpdateAnalysisTemplate')]}}, "*

 * *                 "'Amazon WorkDocs': {'Actions': {insert: [(58, "*

 * *                […]*

```diff
@@ -1346,45 +1346,53 @@
             "HasResource": true,
             "StringPrefix": "chatbot"
         },
         "AWS Clean Rooms": {
             "ARNFormat": "arn:aws:cleanrooms:${Region}:${Account}:${ResourceType}/${PathToResource}",
             "ARNRegex": "^arn:aws:cleanrooms:.+",
             "Actions": [
+                "BatchGetCollaborationAnalysisTemplate",
                 "BatchGetSchema",
+                "CreateAnalysisTemplate",
                 "CreateCollaboration",
                 "CreateConfiguredTable",
                 "CreateConfiguredTableAnalysisRule",
                 "CreateConfiguredTableAssociation",
                 "CreateMembership",
+                "DeleteAnalysisTemplate",
                 "DeleteCollaboration",
                 "DeleteConfiguredTable",
                 "DeleteConfiguredTableAnalysisRule",
                 "DeleteConfiguredTableAssociation",
                 "DeleteMember",
                 "DeleteMembership",
+                "GetAnalysisTemplate",
                 "GetCollaboration",
+                "GetCollaborationAnalysisTemplate",
                 "GetConfiguredTable",
                 "GetConfiguredTableAnalysisRule",
                 "GetConfiguredTableAssociation",
                 "GetMembership",
                 "GetProtectedQuery",
                 "GetSchema",
                 "GetSchemaAnalysisRule",
+                "ListAnalysisTemplates",
+                "ListCollaborationAnalysisTemplates",
                 "ListCollaborations",
                 "ListConfiguredTableAssociations",
                 "ListConfiguredTables",
                 "ListMembers",
                 "ListMemberships",
                 "ListProtectedQueries",
                 "ListSchemas",
                 "ListTagsForResource",
                 "StartProtectedQuery",
                 "TagResource",
                 "UntagResource",
+                "UpdateAnalysisTemplate",
                 "UpdateCollaboration",
                 "UpdateConfiguredTable",
                 "UpdateConfiguredTableAnalysisRule",
                 "UpdateConfiguredTableAssociation",
                 "UpdateMembership",
                 "UpdateProtectedQuery"
             ],
@@ -3665,24 +3673,26 @@
                 "DeleteInput",
                 "DeleteInputSecurityGroup",
                 "DeleteMultiplex",
                 "DeleteMultiplexProgram",
                 "DeleteReservation",
                 "DeleteSchedule",
                 "DeleteTags",
+                "DescribeAccountConfiguration",
                 "DescribeChannel",
                 "DescribeInput",
                 "DescribeInputDevice",
                 "DescribeInputDeviceThumbnail",
                 "DescribeInputSecurityGroup",
                 "DescribeMultiplex",
                 "DescribeMultiplexProgram",
                 "DescribeOffering",
                 "DescribeReservation",
                 "DescribeSchedule",
+                "DescribeThumbnails",
                 "ListChannels",
                 "ListInputDeviceTransfers",
                 "ListInputDevices",
                 "ListInputSecurityGroups",
                 "ListInputs",
                 "ListMultiplexPrograms",
                 "ListMultiplexes",
@@ -3694,14 +3704,15 @@
                 "RejectInputDeviceTransfer",
                 "StartChannel",
                 "StartInputDeviceMaintenanceWindow",
                 "StartMultiplex",
                 "StopChannel",
                 "StopMultiplex",
                 "TransferInputDevice",
+                "UpdateAccountConfiguration",
                 "UpdateChannel",
                 "UpdateChannelClass",
                 "UpdateInput",
                 "UpdateInputDevice",
                 "UpdateInputSecurityGroup",
                 "UpdateMultiplex",
                 "UpdateMultiplexProgram",
@@ -19828,15 +19839,16 @@
                 "RemoveResourcePermission",
                 "RestoreDocumentVersions",
                 "SearchResources",
                 "UpdateDocument",
                 "UpdateDocumentVersion",
                 "UpdateFolder",
                 "UpdateInstanceAlias",
-                "UpdateUser"
+                "UpdateUser",
+                "UpdateUserAdministrativeSettings"
             ],
             "HasResource": false,
             "StringPrefix": "workdocs"
         },
         "Amazon WorkLink": {
             "ARNFormat": "arn:aws:worklink::${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:worklink:.+",
```

### Comparing `iam_actions-1.2.20230731/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230801/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999091734786557%*

 * *Differences: {"'proton'": "{'deployment': OrderedDict([('arn_pattern', 'arn:*:proton:*:*:deployment/*'), "*

 * *             "('condition_keys', 'aws:ResourceTag/${TagKey}')])}"}*

```diff
@@ -4800,14 +4800,18 @@
         }
     },
     "proton": {
         "component": {
             "arn_pattern": "arn:*:proton:*:*:component/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "deployment": {
+            "arn_pattern": "arn:*:proton:*:*:deployment/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "environment": {
             "arn_pattern": "arn:*:proton:*:*:environment/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "environment-account-connection": {
             "arn_pattern": "arn:*:proton:*:*:environment-account-connection/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230731/iam_actions/services.json` & `iam_actions-1.2.20230801/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999723984982862%*

 * *Differences: {"'cleanrooms'": "{'Actions': {insert: [(0, 'BatchGetCollaborationAnalysisTemplate'), (2, "*

 * *                 "'CreateAnalysisTemplate'), (8, 'DeleteAnalysisTemplate'), (15, "*

 * *                 "'GetAnalysisTemplate'), (17, 'GetCollaborationAnalysisTemplate'), (25, "*

 * *                 "'ListAnalysisTemplates'), (26, 'ListCollaborationAnalysisTemplates'), (38, "*

 * *                 "'UpdateAnalysisTemplate')]}}",*

 * * "'medialive'": "{'Actions': {insert: [(22, 'DescribeAccountConfiguration'), (33, "*

 * *                "' […]*

```diff
@@ -2755,45 +2755,53 @@
         "ARNFormats": [
             "arn:aws:cleanrooms:${Region}:${Account}:${ResourceType}/${PathToResource}"
         ],
         "ARNRegexes": [
             "^arn:aws:cleanrooms:.+"
         ],
         "Actions": [
+            "BatchGetCollaborationAnalysisTemplate",
             "BatchGetSchema",
+            "CreateAnalysisTemplate",
             "CreateCollaboration",
             "CreateConfiguredTable",
             "CreateConfiguredTableAnalysisRule",
             "CreateConfiguredTableAssociation",
             "CreateMembership",
+            "DeleteAnalysisTemplate",
             "DeleteCollaboration",
             "DeleteConfiguredTable",
             "DeleteConfiguredTableAnalysisRule",
             "DeleteConfiguredTableAssociation",
             "DeleteMember",
             "DeleteMembership",
+            "GetAnalysisTemplate",
             "GetCollaboration",
+            "GetCollaborationAnalysisTemplate",
             "GetConfiguredTable",
             "GetConfiguredTableAnalysisRule",
             "GetConfiguredTableAssociation",
             "GetMembership",
             "GetProtectedQuery",
             "GetSchema",
             "GetSchemaAnalysisRule",
+            "ListAnalysisTemplates",
+            "ListCollaborationAnalysisTemplates",
             "ListCollaborations",
             "ListConfiguredTableAssociations",
             "ListConfiguredTables",
             "ListMembers",
             "ListMemberships",
             "ListProtectedQueries",
             "ListSchemas",
             "ListTagsForResource",
             "StartProtectedQuery",
             "TagResource",
             "UntagResource",
+            "UpdateAnalysisTemplate",
             "UpdateCollaboration",
             "UpdateConfiguredTable",
             "UpdateConfiguredTableAnalysisRule",
             "UpdateConfiguredTableAssociation",
             "UpdateMembership",
             "UpdateProtectedQuery"
         ],
@@ -13511,24 +13519,26 @@
             "DeleteInput",
             "DeleteInputSecurityGroup",
             "DeleteMultiplex",
             "DeleteMultiplexProgram",
             "DeleteReservation",
             "DeleteSchedule",
             "DeleteTags",
+            "DescribeAccountConfiguration",
             "DescribeChannel",
             "DescribeInput",
             "DescribeInputDevice",
             "DescribeInputDeviceThumbnail",
             "DescribeInputSecurityGroup",
             "DescribeMultiplex",
             "DescribeMultiplexProgram",
             "DescribeOffering",
             "DescribeReservation",
             "DescribeSchedule",
+            "DescribeThumbnails",
             "ListChannels",
             "ListInputDeviceTransfers",
             "ListInputDevices",
             "ListInputSecurityGroups",
             "ListInputs",
             "ListMultiplexPrograms",
             "ListMultiplexes",
@@ -13540,14 +13550,15 @@
             "RejectInputDeviceTransfer",
             "StartChannel",
             "StartInputDeviceMaintenanceWindow",
             "StartMultiplex",
             "StopChannel",
             "StopMultiplex",
             "TransferInputDevice",
+            "UpdateAccountConfiguration",
             "UpdateChannel",
             "UpdateChannelClass",
             "UpdateInput",
             "UpdateInputDevice",
             "UpdateInputSecurityGroup",
             "UpdateMultiplex",
             "UpdateMultiplexProgram",
@@ -21684,15 +21695,16 @@
             "RemoveResourcePermission",
             "RestoreDocumentVersions",
             "SearchResources",
             "UpdateDocument",
             "UpdateDocumentVersion",
             "UpdateFolder",
             "UpdateInstanceAlias",
-            "UpdateUser"
+            "UpdateUser",
+            "UpdateUserAdministrativeSettings"
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
             "Amazon WorkDocs"
         ]
     },
```

### Comparing `iam_actions-1.2.20230731/pyproject.toml` & `iam_actions-1.2.20230801/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230731"
+version = "1.2.20230801"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230731/setup.py` & `iam_actions-1.2.20230801/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230731',
+    'version': '1.2.20230801',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230731/PKG-INFO` & `iam_actions-1.2.20230801/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230731
+Version: 1.2.20230801
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

