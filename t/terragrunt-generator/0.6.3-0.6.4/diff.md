# Comparing `tmp/terragrunt-generator-0.6.3.tar.gz` & `tmp/terragrunt-generator-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragrunt-generator-0.6.3.tar", last modified: Tue Aug  1 17:39:53 2023, max compression
+gzip compressed data, was "terragrunt-generator-0.6.4.tar", last modified: Tue Aug  1 20:11:26 2023, max compression
```

## Comparing `terragrunt-generator-0.6.3.tar` & `terragrunt-generator-0.6.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 17:39:42.000000 terragrunt-generator-0.6.3/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 17:39:42.000000 terragrunt-generator-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 17:39:53.000000 terragrunt-generator-0.6.3/terragrunt_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:53.686094 terragrunt-generator-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 17:39:31.000000 terragrunt-generator-0.6.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 20:11:16.000000 terragrunt-generator-0.6.4/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 20:11:16.000000 terragrunt-generator-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_utils.py
```

### Comparing `terragrunt-generator-0.6.3/COPYING` & `terragrunt-generator-0.6.4/COPYING`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.3/PKG-INFO` & `terragrunt-generator-0.6.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: terragrunt-generator
-Version: 0.6.3
-Summary: generate terragrunt manifest from terraform module.
-Author: Chris
-Author-email: goabonga@pm.me
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: COPYING
-
 # terragrunt-generator
 
 **terragrunt-generator** provide a way to generate a ```terragrunt.hcl``` file with documented inputs who's coming from variables exposed by terraform module.
 
 The result is easily configurable with a **yaml** file.
 ## Requirements
 
@@ -24,266 +14,291 @@
 ```
 
 ## Usages
 
 ### Exec
 
 ```sh
-$ terragrunt-generator -u https://github.com/terraform-google-modules/terraform-google-project-factory.git -v v14.2.1 -l 'project' | wl-copy
+$ terragrunt-generator --help
+usage: terragrunt-gernerator [-h] [-V] -u URL [-v VERSION] [-p PATH] [--include | --no-include] [-l LOOKUP]
+
+generate terragrunt.hcl confirugation from terraform module
+
+options:
+  -h, --help            show this help message and exit
+  -V                    show program's version number and exit
+  -u URL, --url URL     the module repository url
+  -v VERSION, --version VERSION
+                        the module version to use
+  -p PATH, --path PATH  define the module path if needed
+  --include, --no-include
+                        do no rendering the include block
+  -l LOOKUP, --lookup LOOKUP
+                        define the lookup path
+```
+
+#### Example
+
+```sh
+$ terragrunt-generator \
+-u https://github.com/terraform-google-modules/terraform-google-project-factory.git \
+-v v14.2.1 \
+-l 'project'
 ```
 
 ### Results
 
 ```hcl
 # terraform-google-project-factory v14.2.1
 # https://github.com/terraform-google-modules/terraform-google-project-factory/tree/v14.2.1/
 #
 # yaml config
 # ```
 # project:
 #   enabled: true
 #   # org_id - The organization ID.
-#   org_id: 
+#   org_id:
 #   # name - The name for the project
-#   name: 
+#   name:
 #   # billing_account - The ID of the billing account to associate this project with
-#   billing_account: 
+#   billing_account:
 #   # random_project_id - Adds a suffix of 4 random characters to the `project_id`.
-#   random_project_id: 
+#   random_project_id:
 #   # domain - The domain name (optional).
-#   domain: 
+#   domain:
 #   # project_id - The ID to give the project. If not provided, the `name` will be used.
-#   project_id: 
+#   project_id:
 #   # svpc_host_project_id - The ID of the host project which hosts the shared VPC
-#   svpc_host_project_id: 
+#   svpc_host_project_id:
 #   # enable_shared_vpc_host_project - If this project is a shared VPC host project. If true, you must *not* set svpc_host_project_id variable. Default is false.
-#   enable_shared_vpc_host_project: 
+#   enable_shared_vpc_host_project:
 #   # folder_id - The ID of a folder to host this project
-#   folder_id: 
+#   folder_id:
 #   # group_name - A group to control the project by being assigned group_role (defaults to project editor)
-#   group_name: 
+#   group_name:
 #   # group_role - The role to give the controlling group (group_name) over the project (defaults to project editor)
 #   group_role: "roles/editor"
 #   # create_project_sa - Whether the default service account for the project shall be created
 #   create_project_sa: true
 #   # project_sa_name - Default service account name for the project.
 #   project_sa_name: "project-service-account"
 #   # sa_role - A role to give the default Service Account for the project (defaults to none)
-#   sa_role: 
+#   sa_role:
 #   # activate_apis - The list of apis to activate within the project
 #   activate_apis: ["compute.googleapis.com"]
 #   # activate_api_identities - The list of service identities (Google Managed service account for the API) to force-create for the project (e.g. in order to grant additional roles).
 #   #    APIs in this list will automatically be appended to `activate_apis`.
 #   #    Not including the API in this list will follow the default behaviour for identity creation (which is usually when the first resource using the API is created).
 #   #    Any roles (e.g. service agent role) must be explicitly listed. See https://cloud.google.com/iam/docs/understanding-roles#service-agent-roles-roles for a list of related roles.
-#   activate_api_identities: 
+#   activate_api_identities:
 #   # usage_bucket_name - Name of a GCS bucket to store GCE usage reports in (optional)
-#   usage_bucket_name: 
+#   usage_bucket_name:
 #   # usage_bucket_prefix - Prefix in the GCS bucket to store GCE usage reports in (optional)
-#   usage_bucket_prefix: 
+#   usage_bucket_prefix:
 #   # shared_vpc_subnets - List of subnets fully qualified subnet IDs (ie. projects/$project_id/regions/$region/subnetworks/$subnet_id)
-#   shared_vpc_subnets: 
+#   shared_vpc_subnets:
 #   # labels - Map of labels for project
-#   labels: 
+#   labels:
 #   # bucket_project - A project to create a GCS bucket (bucket_name) in, useful for Terraform state (optional)
-#   bucket_project: 
+#   bucket_project:
 #   # bucket_name - A name for a GCS bucket to create (in the bucket_project project), useful for Terraform state (optional)
-#   bucket_name: 
+#   bucket_name:
 #   # bucket_location - The location for a GCS bucket to create (optional)
 #   bucket_location: "US"
 #   # bucket_versioning - Enable versioning for a GCS bucket to create (optional)
-#   bucket_versioning: 
+#   bucket_versioning:
 #   # bucket_labels -  A map of key/value label pairs to assign to the bucket (optional)
-#   bucket_labels: 
+#   bucket_labels:
 #   # bucket_force_destroy - Force the deletion of all objects within the GCS bucket when deleting the bucket (optional)
-#   bucket_force_destroy: 
+#   bucket_force_destroy:
 #   # bucket_ula - Enable Uniform Bucket Level Access
 #   bucket_ula: true
 #   # bucket_pap - Enable Public Access Prevention. Possible values are "enforced" or "inherited".
 #   bucket_pap: "inherited"
 #   # auto_create_network - Create the default network
-#   auto_create_network: 
+#   auto_create_network:
 #   # lien - Add a lien on the project to prevent accidental deletion
-#   lien: 
+#   lien:
 #   # disable_services_on_destroy - Whether project services will be disabled when the resources are destroyed
 #   disable_services_on_destroy: true
 #   # default_service_account - Project default service account setting: can be one of `delete`, `deprivilege`, `disable`, or `keep`.
 #   default_service_account: "disable"
 #   # disable_dependent_services - Whether services that are enabled and which depend on this service should also be disabled when this service is destroyed.
 #   disable_dependent_services: true
 #   # budget_monitoring_notification_channels - A list of monitoring notification channels in the form `[projects/{project_id}/notificationChannels/{channel_id}]`. A maximum of 5 channels are allowed.
-#   budget_monitoring_notification_channels: 
+#   budget_monitoring_notification_channels:
 #   # budget_alert_spent_percents - A list of percentages of the budget to alert on when threshold is exceeded
 #   budget_alert_spent_percents: [0.5, 0.7, 1.0]
 #   # budget_alert_spend_basis - The type of basis used to determine if spend has passed the threshold
 #   budget_alert_spend_basis: "CURRENT_SPEND"
 #   # budget_labels - A single label and value pair specifying that usage from only this set of labeled resources should be included in the budget.
-#   budget_labels: 
+#   budget_labels:
 #   # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
-#   vpc_service_control_attach_enabled: 
+#   vpc_service_control_attach_enabled:
 #   # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
 #   vpc_service_control_sleep_duration: "5s"
 #   # grant_services_security_admin_role - Whether or not to grant Kubernetes Engine Service Agent the Security Admin role on the host project so it can manage firewall rules
-#   grant_services_security_admin_role: 
+#   grant_services_security_admin_role:
 #   # grant_network_role - Whether or not to grant networkUser role on the host project/subnets
 #   grant_network_role: true
 #   # consumer_quotas - The quotas configuration you want to override for the project.
-#   consumer_quotas: 
+#   consumer_quotas:
 #   # default_network_tier - Default Network Service Tier for resources created in this project. If unset, the value will not be modified. See https://cloud.google.com/network-tiers/docs/using-network-service-tiers and https://cloud.google.com/network-tiers.
-#   default_network_tier: 
+#   default_network_tier:
 #   # essential_contacts - A mapping of users or groups to be assigned as Essential Contacts to the project, specifying a notification category
-#   essential_contacts: 
+#   essential_contacts:
 #   # language_tag - Language code to be used for essential contacts notifications
 #   language_tag: "en-US"
 #   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
-#   # random_project_id_length: 
+#   # random_project_id_length:
 #   # budget_amount - The amount to use for a budget alert
-#   # budget_amount: 
-#   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>` 
-#   # budget_display_name: 
+#   # budget_amount:
+#   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
+#   # budget_display_name:
 #   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
-#   # budget_alert_pubsub_topic: 
+#   # budget_alert_pubsub_topic:
 #   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
-#   # budget_calendar_period: 
+#   # budget_calendar_period:
 #   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
-#   # budget_custom_period_start_date: 
+#   # budget_custom_period_start_date:
 #   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
-#   # budget_custom_period_end_date: 
+#   # budget_custom_period_end_date:
 #   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
-#   # vpc_service_control_perimeter_name: 
+#   # vpc_service_control_perimeter_name:
 # ```
 #
 
 include {
     path = find_in_parent_folders()
 }
 
 locals {
     module = {
         repository = "github.com/terraform-google-modules/terraform-google-project-factory.git"
         path = null
         version = "v14.2.1"
         source =  "${local.module.repository}${local.module.path != null ? local.module.path : ''}?ref=${local.module.version}"
     }
-    environment = get_env("ENV", "development")
+    environment = get_env("CONFIG", "test")
     all = merge(
         yamldecode(file(find_in_parent_folders(format("config.%s.yaml", local.environment)))),
     )
 }
 
 terraform {
-    source = lookup(project, "enabled", true) == true ? local.module.source : null
+    source = lookup(local.all.project, "enabled", true) == true ? local.module.source : null
 }
 
 inputs = merge({
     # billing_account - The ID of the billing account to associate this project with - required
-    billing_account = lookup(project, "billing_account", "")
+    billing_account = lookup(local.all.project, "billing_account", "")
     # name - The name for the project - required
-    name = lookup(project, "name", "")
+    name = lookup(local.all.project, "name", "")
     # org_id - The organization ID. - required
-    org_id = lookup(project, "org_id", "")
+    org_id = lookup(local.all.project, "org_id", "")
     # activate_api_identities - The list of service identities (Google Managed service account for the API) to force-create for the project (e.g. in order to grant additional roles).
     # APIs in this list will automatically be appended to `activate_apis`.
     # Not including the API in this list will follow the default behaviour for identity creation (which is usually when the first resource using the API is created).
     # Any roles (e.g. service agent role) must be explicitly listed. See https://cloud.google.com/iam/docs/understanding-roles#service-agent-roles-roles for a list of related roles.
-    activate_api_identities = lookup(project, "activate_api_identities", [])
+    activate_api_identities = lookup(local.all.project, "activate_api_identities", [])
     # activate_apis - The list of apis to activate within the project
-    activate_apis = lookup(project, "activate_apis", ["compute.googleapis.com"])
+    activate_apis = lookup(local.all.project, "activate_apis", ["compute.googleapis.com"])
     # auto_create_network - Create the default network
-    auto_create_network = lookup(project, "auto_create_network", false)
+    auto_create_network = lookup(local.all.project, "auto_create_network", false)
     # bucket_force_destroy - Force the deletion of all objects within the GCS bucket when deleting the bucket (optional)
-    bucket_force_destroy = lookup(project, "bucket_force_destroy", false)
+    bucket_force_destroy = lookup(local.all.project, "bucket_force_destroy", false)
     # bucket_labels -  A map of key/value label pairs to assign to the bucket (optional)
-    bucket_labels = lookup(project, "bucket_labels", {})
+    bucket_labels = lookup(local.all.project, "bucket_labels", {})
     # bucket_location - The location for a GCS bucket to create (optional)
-    bucket_location = lookup(project, "bucket_location", "US")
+    bucket_location = lookup(local.all.project, "bucket_location", "US")
     # bucket_name - A name for a GCS bucket to create (in the bucket_project project), useful for Terraform state (optional)
-    bucket_name = lookup(project, "bucket_name", "")
+    bucket_name = lookup(local.all.project, "bucket_name", "")
     # bucket_pap - Enable Public Access Prevention. Possible values are "enforced" or "inherited".
-    bucket_pap = lookup(project, "bucket_pap", "inherited")
+    bucket_pap = lookup(local.all.project, "bucket_pap", "inherited")
     # bucket_project - A project to create a GCS bucket (bucket_name) in, useful for Terraform state (optional)
-    bucket_project = lookup(project, "bucket_project", "")
+    bucket_project = lookup(local.all.project, "bucket_project", "")
     # bucket_ula - Enable Uniform Bucket Level Access
-    bucket_ula = lookup(project, "bucket_ula", true)
+    bucket_ula = lookup(local.all.project, "bucket_ula", true)
     # bucket_versioning - Enable versioning for a GCS bucket to create (optional)
-    bucket_versioning = lookup(project, "bucket_versioning", false)
+    bucket_versioning = lookup(local.all.project, "bucket_versioning", false)
     # budget_alert_spend_basis - The type of basis used to determine if spend has passed the threshold
-    budget_alert_spend_basis = lookup(project, "budget_alert_spend_basis", "CURRENT_SPEND")
+    budget_alert_spend_basis = lookup(local.all.project, "budget_alert_spend_basis", "CURRENT_SPEND")
     # budget_alert_spent_percents - A list of percentages of the budget to alert on when threshold is exceeded
-    budget_alert_spent_percents = lookup(project, "budget_alert_spent_percents", [0.5, 0.7, 1.0])
+    budget_alert_spent_percents = lookup(local.all.project, "budget_alert_spent_percents", [0.5, 0.7, 1.0])
     # budget_labels - A single label and value pair specifying that usage from only this set of labeled resources should be included in the budget.
-    budget_labels = lookup(project, "budget_labels", {})
+    budget_labels = lookup(local.all.project, "budget_labels", {})
     # budget_monitoring_notification_channels - A list of monitoring notification channels in the form `[projects/{project_id}/notificationChannels/{channel_id}]`. A maximum of 5 channels are allowed.
-    budget_monitoring_notification_channels = lookup(project, "budget_monitoring_notification_channels", [])
+    budget_monitoring_notification_channels = lookup(local.all.project, "budget_monitoring_notification_channels", [])
     # consumer_quotas - The quotas configuration you want to override for the project.
-    consumer_quotas = lookup(project, "consumer_quotas", [])
+    consumer_quotas = lookup(local.all.project, "consumer_quotas", [])
     # create_project_sa - Whether the default service account for the project shall be created
-    create_project_sa = lookup(project, "create_project_sa", true)
+    create_project_sa = lookup(local.all.project, "create_project_sa", true)
     # default_network_tier - Default Network Service Tier for resources created in this project. If unset, the value will not be modified. See https://cloud.google.com/network-tiers/docs/using-network-service-tiers and https://cloud.google.com/network-tiers.
-    default_network_tier = lookup(project, "default_network_tier", "")
+    default_network_tier = lookup(local.all.project, "default_network_tier", "")
     # default_service_account - Project default service account setting: can be one of `delete`, `deprivilege`, `disable`, or `keep`.
-    default_service_account = lookup(project, "default_service_account", "disable")
+    default_service_account = lookup(local.all.project, "default_service_account", "disable")
     # disable_dependent_services - Whether services that are enabled and which depend on this service should also be disabled when this service is destroyed.
-    disable_dependent_services = lookup(project, "disable_dependent_services", true)
+    disable_dependent_services = lookup(local.all.project, "disable_dependent_services", true)
     # disable_services_on_destroy - Whether project services will be disabled when the resources are destroyed
-    disable_services_on_destroy = lookup(project, "disable_services_on_destroy", true)
+    disable_services_on_destroy = lookup(local.all.project, "disable_services_on_destroy", true)
     # domain - The domain name (optional).
-    domain = lookup(project, "domain", "")
+    domain = lookup(local.all.project, "domain", "")
     # enable_shared_vpc_host_project - If this project is a shared VPC host project. If true, you must *not* set svpc_host_project_id variable. Default is false.
-    enable_shared_vpc_host_project = lookup(project, "enable_shared_vpc_host_project", false)
+    enable_shared_vpc_host_project = lookup(local.all.project, "enable_shared_vpc_host_project", false)
     # essential_contacts - A mapping of users or groups to be assigned as Essential Contacts to the project, specifying a notification category
-    essential_contacts = lookup(project, "essential_contacts", {})
+    essential_contacts = lookup(local.all.project, "essential_contacts", {})
     # folder_id - The ID of a folder to host this project
-    folder_id = lookup(project, "folder_id", "")
+    folder_id = lookup(local.all.project, "folder_id", "")
     # grant_network_role - Whether or not to grant networkUser role on the host project/subnets
-    grant_network_role = lookup(project, "grant_network_role", true)
+    grant_network_role = lookup(local.all.project, "grant_network_role", true)
     # grant_services_security_admin_role - Whether or not to grant Kubernetes Engine Service Agent the Security Admin role on the host project so it can manage firewall rules
-    grant_services_security_admin_role = lookup(project, "grant_services_security_admin_role", false)
+    grant_services_security_admin_role = lookup(local.all.project, "grant_services_security_admin_role", false)
     # group_name - A group to control the project by being assigned group_role (defaults to project editor)
-    group_name = lookup(project, "group_name", "")
+    group_name = lookup(local.all.project, "group_name", "")
     # group_role - The role to give the controlling group (group_name) over the project (defaults to project editor)
-    group_role = lookup(project, "group_role", "roles/editor")
+    group_role = lookup(local.all.project, "group_role", "roles/editor")
     # labels - Map of labels for project
-    labels = lookup(project, "labels", {})
+    labels = lookup(local.all.project, "labels", {})
     # language_tag - Language code to be used for essential contacts notifications
-    language_tag = lookup(project, "language_tag", "en-US")
+    language_tag = lookup(local.all.project, "language_tag", "en-US")
     # lien - Add a lien on the project to prevent accidental deletion
-    lien = lookup(project, "lien", false)
+    lien = lookup(local.all.project, "lien", false)
     # project_id - The ID to give the project. If not provided, the `name` will be used.
-    project_id = lookup(project, "project_id", "")
+    project_id = lookup(local.all.project, "project_id", "")
     # project_sa_name - Default service account name for the project.
-    project_sa_name = lookup(project, "project_sa_name", "project-service-account")
+    project_sa_name = lookup(local.all.project, "project_sa_name", "project-service-account")
     # random_project_id - Adds a suffix of 4 random characters to the `project_id`.
-    random_project_id = lookup(project, "random_project_id", false)
+    random_project_id = lookup(local.all.project, "random_project_id", false)
     # sa_role - A role to give the default Service Account for the project (defaults to none)
-    sa_role = lookup(project, "sa_role", "")
+    sa_role = lookup(local.all.project, "sa_role", "")
     # shared_vpc_subnets - List of subnets fully qualified subnet IDs (ie. projects/$project_id/regions/$region/subnetworks/$subnet_id)
-    shared_vpc_subnets = lookup(project, "shared_vpc_subnets", [])
+    shared_vpc_subnets = lookup(local.all.project, "shared_vpc_subnets", [])
     # svpc_host_project_id - The ID of the host project which hosts the shared VPC
-    svpc_host_project_id = lookup(project, "svpc_host_project_id", "")
+    svpc_host_project_id = lookup(local.all.project, "svpc_host_project_id", "")
     # usage_bucket_name - Name of a GCS bucket to store GCE usage reports in (optional)
-    usage_bucket_name = lookup(project, "usage_bucket_name", "")
+    usage_bucket_name = lookup(local.all.project, "usage_bucket_name", "")
     # usage_bucket_prefix - Prefix in the GCS bucket to store GCE usage reports in (optional)
-    usage_bucket_prefix = lookup(project, "usage_bucket_prefix", "")
+    usage_bucket_prefix = lookup(local.all.project, "usage_bucket_prefix", "")
     # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
-    vpc_service_control_attach_enabled = lookup(project, "vpc_service_control_attach_enabled", false)
+    vpc_service_control_attach_enabled = lookup(local.all.project, "vpc_service_control_attach_enabled", false)
     # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
-    vpc_service_control_sleep_duration = lookup(project, "vpc_service_control_sleep_duration", "5s")
+    vpc_service_control_sleep_duration = lookup(local.all.project, "vpc_service_control_sleep_duration", "5s")
 },
   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
   (lookup(project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(project, "budget_alert_pubsub_topic") }),
   # budget_amount - The amount to use for a budget alert
   (lookup(project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(project, "budget_amount") }),
   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
   (lookup(project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(project, "budget_calendar_period") }),
   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
   (lookup(project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(project, "budget_custom_period_end_date") }),
   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
   (lookup(project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(project, "budget_custom_period_start_date") }),
-  # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>` 
+  # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
   (lookup(project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(project, "budget_display_name") }),
   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
   (lookup(project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(project, "random_project_id_length") }),
   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
   (lookup(project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(project, "vpc_service_control_perimeter_name") })
 )
+
 ```
```

### Comparing `terragrunt-generator-0.6.3/README.md` & `terragrunt-generator-0.6.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: terragrunt-generator
+Version: 0.6.4
+Summary: generate terragrunt manifest from terraform module.
+Author: Chris
+Author-email: goabonga@pm.me
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: COPYING
+
 # terragrunt-generator
 
 **terragrunt-generator** provide a way to generate a ```terragrunt.hcl``` file with documented inputs who's coming from variables exposed by terraform module.
 
 The result is easily configurable with a **yaml** file.
 ## Requirements
 
@@ -14,266 +24,291 @@
 ```
 
 ## Usages
 
 ### Exec
 
 ```sh
-$ terragrunt-generator -u https://github.com/terraform-google-modules/terraform-google-project-factory.git -v v14.2.1 -l 'project' | wl-copy
+$ terragrunt-generator --help
+usage: terragrunt-gernerator [-h] [-V] -u URL [-v VERSION] [-p PATH] [--include | --no-include] [-l LOOKUP]
+
+generate terragrunt.hcl confirugation from terraform module
+
+options:
+  -h, --help            show this help message and exit
+  -V                    show program's version number and exit
+  -u URL, --url URL     the module repository url
+  -v VERSION, --version VERSION
+                        the module version to use
+  -p PATH, --path PATH  define the module path if needed
+  --include, --no-include
+                        do no rendering the include block
+  -l LOOKUP, --lookup LOOKUP
+                        define the lookup path
+```
+
+#### Example
+
+```sh
+$ terragrunt-generator \
+-u https://github.com/terraform-google-modules/terraform-google-project-factory.git \
+-v v14.2.1 \
+-l 'project'
 ```
 
 ### Results
 
 ```hcl
 # terraform-google-project-factory v14.2.1
 # https://github.com/terraform-google-modules/terraform-google-project-factory/tree/v14.2.1/
 #
 # yaml config
 # ```
 # project:
 #   enabled: true
 #   # org_id - The organization ID.
-#   org_id: 
+#   org_id:
 #   # name - The name for the project
-#   name: 
+#   name:
 #   # billing_account - The ID of the billing account to associate this project with
-#   billing_account: 
+#   billing_account:
 #   # random_project_id - Adds a suffix of 4 random characters to the `project_id`.
-#   random_project_id: 
+#   random_project_id:
 #   # domain - The domain name (optional).
-#   domain: 
+#   domain:
 #   # project_id - The ID to give the project. If not provided, the `name` will be used.
-#   project_id: 
+#   project_id:
 #   # svpc_host_project_id - The ID of the host project which hosts the shared VPC
-#   svpc_host_project_id: 
+#   svpc_host_project_id:
 #   # enable_shared_vpc_host_project - If this project is a shared VPC host project. If true, you must *not* set svpc_host_project_id variable. Default is false.
-#   enable_shared_vpc_host_project: 
+#   enable_shared_vpc_host_project:
 #   # folder_id - The ID of a folder to host this project
-#   folder_id: 
+#   folder_id:
 #   # group_name - A group to control the project by being assigned group_role (defaults to project editor)
-#   group_name: 
+#   group_name:
 #   # group_role - The role to give the controlling group (group_name) over the project (defaults to project editor)
 #   group_role: "roles/editor"
 #   # create_project_sa - Whether the default service account for the project shall be created
 #   create_project_sa: true
 #   # project_sa_name - Default service account name for the project.
 #   project_sa_name: "project-service-account"
 #   # sa_role - A role to give the default Service Account for the project (defaults to none)
-#   sa_role: 
+#   sa_role:
 #   # activate_apis - The list of apis to activate within the project
 #   activate_apis: ["compute.googleapis.com"]
 #   # activate_api_identities - The list of service identities (Google Managed service account for the API) to force-create for the project (e.g. in order to grant additional roles).
 #   #    APIs in this list will automatically be appended to `activate_apis`.
 #   #    Not including the API in this list will follow the default behaviour for identity creation (which is usually when the first resource using the API is created).
 #   #    Any roles (e.g. service agent role) must be explicitly listed. See https://cloud.google.com/iam/docs/understanding-roles#service-agent-roles-roles for a list of related roles.
-#   activate_api_identities: 
+#   activate_api_identities:
 #   # usage_bucket_name - Name of a GCS bucket to store GCE usage reports in (optional)
-#   usage_bucket_name: 
+#   usage_bucket_name:
 #   # usage_bucket_prefix - Prefix in the GCS bucket to store GCE usage reports in (optional)
-#   usage_bucket_prefix: 
+#   usage_bucket_prefix:
 #   # shared_vpc_subnets - List of subnets fully qualified subnet IDs (ie. projects/$project_id/regions/$region/subnetworks/$subnet_id)
-#   shared_vpc_subnets: 
+#   shared_vpc_subnets:
 #   # labels - Map of labels for project
-#   labels: 
+#   labels:
 #   # bucket_project - A project to create a GCS bucket (bucket_name) in, useful for Terraform state (optional)
-#   bucket_project: 
+#   bucket_project:
 #   # bucket_name - A name for a GCS bucket to create (in the bucket_project project), useful for Terraform state (optional)
-#   bucket_name: 
+#   bucket_name:
 #   # bucket_location - The location for a GCS bucket to create (optional)
 #   bucket_location: "US"
 #   # bucket_versioning - Enable versioning for a GCS bucket to create (optional)
-#   bucket_versioning: 
+#   bucket_versioning:
 #   # bucket_labels -  A map of key/value label pairs to assign to the bucket (optional)
-#   bucket_labels: 
+#   bucket_labels:
 #   # bucket_force_destroy - Force the deletion of all objects within the GCS bucket when deleting the bucket (optional)
-#   bucket_force_destroy: 
+#   bucket_force_destroy:
 #   # bucket_ula - Enable Uniform Bucket Level Access
 #   bucket_ula: true
 #   # bucket_pap - Enable Public Access Prevention. Possible values are "enforced" or "inherited".
 #   bucket_pap: "inherited"
 #   # auto_create_network - Create the default network
-#   auto_create_network: 
+#   auto_create_network:
 #   # lien - Add a lien on the project to prevent accidental deletion
-#   lien: 
+#   lien:
 #   # disable_services_on_destroy - Whether project services will be disabled when the resources are destroyed
 #   disable_services_on_destroy: true
 #   # default_service_account - Project default service account setting: can be one of `delete`, `deprivilege`, `disable`, or `keep`.
 #   default_service_account: "disable"
 #   # disable_dependent_services - Whether services that are enabled and which depend on this service should also be disabled when this service is destroyed.
 #   disable_dependent_services: true
 #   # budget_monitoring_notification_channels - A list of monitoring notification channels in the form `[projects/{project_id}/notificationChannels/{channel_id}]`. A maximum of 5 channels are allowed.
-#   budget_monitoring_notification_channels: 
+#   budget_monitoring_notification_channels:
 #   # budget_alert_spent_percents - A list of percentages of the budget to alert on when threshold is exceeded
 #   budget_alert_spent_percents: [0.5, 0.7, 1.0]
 #   # budget_alert_spend_basis - The type of basis used to determine if spend has passed the threshold
 #   budget_alert_spend_basis: "CURRENT_SPEND"
 #   # budget_labels - A single label and value pair specifying that usage from only this set of labeled resources should be included in the budget.
-#   budget_labels: 
+#   budget_labels:
 #   # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
-#   vpc_service_control_attach_enabled: 
+#   vpc_service_control_attach_enabled:
 #   # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
 #   vpc_service_control_sleep_duration: "5s"
 #   # grant_services_security_admin_role - Whether or not to grant Kubernetes Engine Service Agent the Security Admin role on the host project so it can manage firewall rules
-#   grant_services_security_admin_role: 
+#   grant_services_security_admin_role:
 #   # grant_network_role - Whether or not to grant networkUser role on the host project/subnets
 #   grant_network_role: true
 #   # consumer_quotas - The quotas configuration you want to override for the project.
-#   consumer_quotas: 
+#   consumer_quotas:
 #   # default_network_tier - Default Network Service Tier for resources created in this project. If unset, the value will not be modified. See https://cloud.google.com/network-tiers/docs/using-network-service-tiers and https://cloud.google.com/network-tiers.
-#   default_network_tier: 
+#   default_network_tier:
 #   # essential_contacts - A mapping of users or groups to be assigned as Essential Contacts to the project, specifying a notification category
-#   essential_contacts: 
+#   essential_contacts:
 #   # language_tag - Language code to be used for essential contacts notifications
 #   language_tag: "en-US"
 #   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
-#   # random_project_id_length: 
+#   # random_project_id_length:
 #   # budget_amount - The amount to use for a budget alert
-#   # budget_amount: 
-#   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>` 
-#   # budget_display_name: 
+#   # budget_amount:
+#   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
+#   # budget_display_name:
 #   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
-#   # budget_alert_pubsub_topic: 
+#   # budget_alert_pubsub_topic:
 #   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
-#   # budget_calendar_period: 
+#   # budget_calendar_period:
 #   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
-#   # budget_custom_period_start_date: 
+#   # budget_custom_period_start_date:
 #   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
-#   # budget_custom_period_end_date: 
+#   # budget_custom_period_end_date:
 #   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
-#   # vpc_service_control_perimeter_name: 
+#   # vpc_service_control_perimeter_name:
 # ```
 #
 
 include {
     path = find_in_parent_folders()
 }
 
 locals {
     module = {
         repository = "github.com/terraform-google-modules/terraform-google-project-factory.git"
         path = null
         version = "v14.2.1"
         source =  "${local.module.repository}${local.module.path != null ? local.module.path : ''}?ref=${local.module.version}"
     }
-    environment = get_env("ENV", "development")
+    environment = get_env("CONFIG", "test")
     all = merge(
         yamldecode(file(find_in_parent_folders(format("config.%s.yaml", local.environment)))),
     )
 }
 
 terraform {
-    source = lookup(project, "enabled", true) == true ? local.module.source : null
+    source = lookup(local.all.project, "enabled", true) == true ? local.module.source : null
 }
 
 inputs = merge({
     # billing_account - The ID of the billing account to associate this project with - required
-    billing_account = lookup(project, "billing_account", "")
+    billing_account = lookup(local.all.project, "billing_account", "")
     # name - The name for the project - required
-    name = lookup(project, "name", "")
+    name = lookup(local.all.project, "name", "")
     # org_id - The organization ID. - required
-    org_id = lookup(project, "org_id", "")
+    org_id = lookup(local.all.project, "org_id", "")
     # activate_api_identities - The list of service identities (Google Managed service account for the API) to force-create for the project (e.g. in order to grant additional roles).
     # APIs in this list will automatically be appended to `activate_apis`.
     # Not including the API in this list will follow the default behaviour for identity creation (which is usually when the first resource using the API is created).
     # Any roles (e.g. service agent role) must be explicitly listed. See https://cloud.google.com/iam/docs/understanding-roles#service-agent-roles-roles for a list of related roles.
-    activate_api_identities = lookup(project, "activate_api_identities", [])
+    activate_api_identities = lookup(local.all.project, "activate_api_identities", [])
     # activate_apis - The list of apis to activate within the project
-    activate_apis = lookup(project, "activate_apis", ["compute.googleapis.com"])
+    activate_apis = lookup(local.all.project, "activate_apis", ["compute.googleapis.com"])
     # auto_create_network - Create the default network
-    auto_create_network = lookup(project, "auto_create_network", false)
+    auto_create_network = lookup(local.all.project, "auto_create_network", false)
     # bucket_force_destroy - Force the deletion of all objects within the GCS bucket when deleting the bucket (optional)
-    bucket_force_destroy = lookup(project, "bucket_force_destroy", false)
+    bucket_force_destroy = lookup(local.all.project, "bucket_force_destroy", false)
     # bucket_labels -  A map of key/value label pairs to assign to the bucket (optional)
-    bucket_labels = lookup(project, "bucket_labels", {})
+    bucket_labels = lookup(local.all.project, "bucket_labels", {})
     # bucket_location - The location for a GCS bucket to create (optional)
-    bucket_location = lookup(project, "bucket_location", "US")
+    bucket_location = lookup(local.all.project, "bucket_location", "US")
     # bucket_name - A name for a GCS bucket to create (in the bucket_project project), useful for Terraform state (optional)
-    bucket_name = lookup(project, "bucket_name", "")
+    bucket_name = lookup(local.all.project, "bucket_name", "")
     # bucket_pap - Enable Public Access Prevention. Possible values are "enforced" or "inherited".
-    bucket_pap = lookup(project, "bucket_pap", "inherited")
+    bucket_pap = lookup(local.all.project, "bucket_pap", "inherited")
     # bucket_project - A project to create a GCS bucket (bucket_name) in, useful for Terraform state (optional)
-    bucket_project = lookup(project, "bucket_project", "")
+    bucket_project = lookup(local.all.project, "bucket_project", "")
     # bucket_ula - Enable Uniform Bucket Level Access
-    bucket_ula = lookup(project, "bucket_ula", true)
+    bucket_ula = lookup(local.all.project, "bucket_ula", true)
     # bucket_versioning - Enable versioning for a GCS bucket to create (optional)
-    bucket_versioning = lookup(project, "bucket_versioning", false)
+    bucket_versioning = lookup(local.all.project, "bucket_versioning", false)
     # budget_alert_spend_basis - The type of basis used to determine if spend has passed the threshold
-    budget_alert_spend_basis = lookup(project, "budget_alert_spend_basis", "CURRENT_SPEND")
+    budget_alert_spend_basis = lookup(local.all.project, "budget_alert_spend_basis", "CURRENT_SPEND")
     # budget_alert_spent_percents - A list of percentages of the budget to alert on when threshold is exceeded
-    budget_alert_spent_percents = lookup(project, "budget_alert_spent_percents", [0.5, 0.7, 1.0])
+    budget_alert_spent_percents = lookup(local.all.project, "budget_alert_spent_percents", [0.5, 0.7, 1.0])
     # budget_labels - A single label and value pair specifying that usage from only this set of labeled resources should be included in the budget.
-    budget_labels = lookup(project, "budget_labels", {})
+    budget_labels = lookup(local.all.project, "budget_labels", {})
     # budget_monitoring_notification_channels - A list of monitoring notification channels in the form `[projects/{project_id}/notificationChannels/{channel_id}]`. A maximum of 5 channels are allowed.
-    budget_monitoring_notification_channels = lookup(project, "budget_monitoring_notification_channels", [])
+    budget_monitoring_notification_channels = lookup(local.all.project, "budget_monitoring_notification_channels", [])
     # consumer_quotas - The quotas configuration you want to override for the project.
-    consumer_quotas = lookup(project, "consumer_quotas", [])
+    consumer_quotas = lookup(local.all.project, "consumer_quotas", [])
     # create_project_sa - Whether the default service account for the project shall be created
-    create_project_sa = lookup(project, "create_project_sa", true)
+    create_project_sa = lookup(local.all.project, "create_project_sa", true)
     # default_network_tier - Default Network Service Tier for resources created in this project. If unset, the value will not be modified. See https://cloud.google.com/network-tiers/docs/using-network-service-tiers and https://cloud.google.com/network-tiers.
-    default_network_tier = lookup(project, "default_network_tier", "")
+    default_network_tier = lookup(local.all.project, "default_network_tier", "")
     # default_service_account - Project default service account setting: can be one of `delete`, `deprivilege`, `disable`, or `keep`.
-    default_service_account = lookup(project, "default_service_account", "disable")
+    default_service_account = lookup(local.all.project, "default_service_account", "disable")
     # disable_dependent_services - Whether services that are enabled and which depend on this service should also be disabled when this service is destroyed.
-    disable_dependent_services = lookup(project, "disable_dependent_services", true)
+    disable_dependent_services = lookup(local.all.project, "disable_dependent_services", true)
     # disable_services_on_destroy - Whether project services will be disabled when the resources are destroyed
-    disable_services_on_destroy = lookup(project, "disable_services_on_destroy", true)
+    disable_services_on_destroy = lookup(local.all.project, "disable_services_on_destroy", true)
     # domain - The domain name (optional).
-    domain = lookup(project, "domain", "")
+    domain = lookup(local.all.project, "domain", "")
     # enable_shared_vpc_host_project - If this project is a shared VPC host project. If true, you must *not* set svpc_host_project_id variable. Default is false.
-    enable_shared_vpc_host_project = lookup(project, "enable_shared_vpc_host_project", false)
+    enable_shared_vpc_host_project = lookup(local.all.project, "enable_shared_vpc_host_project", false)
     # essential_contacts - A mapping of users or groups to be assigned as Essential Contacts to the project, specifying a notification category
-    essential_contacts = lookup(project, "essential_contacts", {})
+    essential_contacts = lookup(local.all.project, "essential_contacts", {})
     # folder_id - The ID of a folder to host this project
-    folder_id = lookup(project, "folder_id", "")
+    folder_id = lookup(local.all.project, "folder_id", "")
     # grant_network_role - Whether or not to grant networkUser role on the host project/subnets
-    grant_network_role = lookup(project, "grant_network_role", true)
+    grant_network_role = lookup(local.all.project, "grant_network_role", true)
     # grant_services_security_admin_role - Whether or not to grant Kubernetes Engine Service Agent the Security Admin role on the host project so it can manage firewall rules
-    grant_services_security_admin_role = lookup(project, "grant_services_security_admin_role", false)
+    grant_services_security_admin_role = lookup(local.all.project, "grant_services_security_admin_role", false)
     # group_name - A group to control the project by being assigned group_role (defaults to project editor)
-    group_name = lookup(project, "group_name", "")
+    group_name = lookup(local.all.project, "group_name", "")
     # group_role - The role to give the controlling group (group_name) over the project (defaults to project editor)
-    group_role = lookup(project, "group_role", "roles/editor")
+    group_role = lookup(local.all.project, "group_role", "roles/editor")
     # labels - Map of labels for project
-    labels = lookup(project, "labels", {})
+    labels = lookup(local.all.project, "labels", {})
     # language_tag - Language code to be used for essential contacts notifications
-    language_tag = lookup(project, "language_tag", "en-US")
+    language_tag = lookup(local.all.project, "language_tag", "en-US")
     # lien - Add a lien on the project to prevent accidental deletion
-    lien = lookup(project, "lien", false)
+    lien = lookup(local.all.project, "lien", false)
     # project_id - The ID to give the project. If not provided, the `name` will be used.
-    project_id = lookup(project, "project_id", "")
+    project_id = lookup(local.all.project, "project_id", "")
     # project_sa_name - Default service account name for the project.
-    project_sa_name = lookup(project, "project_sa_name", "project-service-account")
+    project_sa_name = lookup(local.all.project, "project_sa_name", "project-service-account")
     # random_project_id - Adds a suffix of 4 random characters to the `project_id`.
-    random_project_id = lookup(project, "random_project_id", false)
+    random_project_id = lookup(local.all.project, "random_project_id", false)
     # sa_role - A role to give the default Service Account for the project (defaults to none)
-    sa_role = lookup(project, "sa_role", "")
+    sa_role = lookup(local.all.project, "sa_role", "")
     # shared_vpc_subnets - List of subnets fully qualified subnet IDs (ie. projects/$project_id/regions/$region/subnetworks/$subnet_id)
-    shared_vpc_subnets = lookup(project, "shared_vpc_subnets", [])
+    shared_vpc_subnets = lookup(local.all.project, "shared_vpc_subnets", [])
     # svpc_host_project_id - The ID of the host project which hosts the shared VPC
-    svpc_host_project_id = lookup(project, "svpc_host_project_id", "")
+    svpc_host_project_id = lookup(local.all.project, "svpc_host_project_id", "")
     # usage_bucket_name - Name of a GCS bucket to store GCE usage reports in (optional)
-    usage_bucket_name = lookup(project, "usage_bucket_name", "")
+    usage_bucket_name = lookup(local.all.project, "usage_bucket_name", "")
     # usage_bucket_prefix - Prefix in the GCS bucket to store GCE usage reports in (optional)
-    usage_bucket_prefix = lookup(project, "usage_bucket_prefix", "")
+    usage_bucket_prefix = lookup(local.all.project, "usage_bucket_prefix", "")
     # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
-    vpc_service_control_attach_enabled = lookup(project, "vpc_service_control_attach_enabled", false)
+    vpc_service_control_attach_enabled = lookup(local.all.project, "vpc_service_control_attach_enabled", false)
     # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
-    vpc_service_control_sleep_duration = lookup(project, "vpc_service_control_sleep_duration", "5s")
+    vpc_service_control_sleep_duration = lookup(local.all.project, "vpc_service_control_sleep_duration", "5s")
 },
   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
   (lookup(project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(project, "budget_alert_pubsub_topic") }),
   # budget_amount - The amount to use for a budget alert
   (lookup(project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(project, "budget_amount") }),
   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
   (lookup(project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(project, "budget_calendar_period") }),
   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
   (lookup(project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(project, "budget_custom_period_end_date") }),
   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
   (lookup(project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(project, "budget_custom_period_start_date") }),
-  # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>` 
+  # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
   (lookup(project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(project, "budget_display_name") }),
   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
   (lookup(project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(project, "random_project_id_length") }),
   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
   (lookup(project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(project, "vpc_service_control_perimeter_name") })
 )
+
 ```
```

### Comparing `terragrunt-generator-0.6.3/generator/generate.py` & `terragrunt-generator-0.6.4/generator/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,31 @@
     url: str,
     path: str,
     version: str,
     lookup: str,
     variables: list = [],
 ) -> str:
     text = ''
+
     for var_type in ('mandatories', 'optionals', 'nullables'):
         for variable in variables.get(var_type, []):
             default = variable.get('default')
-            description = variable.get('description', '').replace('    ', '', 1).replace('\n', '\n#   #').replace('\\"', '"')
-
+            description = (
+                variable.get('description', '')
+                .replace('    ', '', 1)
+                .replace('\n', '\n#   #')
+                .replace('\\"', '"')
+            )
+            text += f"#   # {variable['name']} - {description}\n"
             if var_type == 'nullables':
-                text += f"#   # {variable['name']} - {description}\n"
                 text += f"#   # {variable['name']}: {json.JSONEncoder().encode(default) if default else ''}\n"
-            elif var_type == 'optionals':
-                text += f"#   # {variable['name']} - {description}\n"
-                text += f"#   {variable['name']}: {json.JSONEncoder().encode(default) if default else ''}\n"
             else:
-                text += f"#   # {variable['name']} - {description}\n"
                 text += f"#   {variable['name']}: {json.JSONEncoder().encode(default) if default else ''}\n"
 
     lookup = lookup.replace('local.all', '')
-    
     path = path or ''
     url = f"{url.replace('.git', '')}/tree/{version}/{path}"
 
     return f"""# {name} {version}
 # {url}
 #
 # yaml config
@@ -47,88 +47,76 @@
     if enable is True:
         content = '    path = find_in_parent_folders()'
         return f"""
 include {{
 {content}
 }}
 """
-    return ""
+    return ''
 
 
 def generate_locals(
-    filename: str = 'config.yaml',
     url: str = None,
     path: str = None,
     version: str = None,
 ) -> str:
-    filename = (
-        f"{filename.removeprefix('#')}"
-        if filename.startswith('#') is True
-        else f'{filename}'
-    )
-
     return f"""
 locals {{
     module = {{
         repository = "{url.replace("https://", "").replace("http://", "")}"
         path = {f'"//{path}"' if path != None else "null"}
         version = "{version}"
         source =  "${{local.module.repository}}${{local.module.path != null ? local.module.path : \'\'}}?ref=${{local.module.version}}"
     }}
-    environment = get_env("ENV", "development")
+    environment = get_env("CONFIG", "test")
     all = merge(
         yamldecode(file(find_in_parent_folders(format("config.%s.yaml", local.environment)))),
     )
 }}
 """
 
 
 def generate_terraform(url: str, path: str, version: str, lookup: str) -> str:
     path = f'//{path}' if path is not None else ''
     url = f'{url.replace("https://", "").replace("http://", "")}{path}?ref={version}'
 
-    if lookup.startswith('['):
-        lookup = lookup.strip('[]').strip('"')
-
-    source = f'lookup({lookup}, "enabled", true) == true ? local.module.source : null'
+    source = f'lookup(local.all.{lookup}, "enabled", true) == true ? local.module.source : null'
 
     return f"""
 terraform {{
     source = {source}
 }}
 """
 
 
 def generate_inputs(variables: list = [], lookup: str = 'local.all') -> str:
     content_fisrt: str = ''
     content_next: str = ''
     content_nullable: str = ''
     variables = sorted(variables, key=lambda d: d['name'], reverse=False)
-        
-    for variable in variables:
 
+    for variable in variables:
         description = (
             variable.get('description', '')
             .replace('    ', '')
             .replace('\n', '\n    # ')
             .replace('\\"', '"')
         )
 
-
         if variable.get('nullable', False) is False:
             _content: str = ''
 
             line_doc = f"{variable.get('name')} - {description}"
             mandatory = variable.get('mandatory', False)
             line_doc += ' - required' if mandatory is True else ''
 
             line_content = f"{variable.get('name')} = "
             name = variable.get('name')
 
-            line_content += f'lookup({lookup}, "{name}"'
+            line_content += f'lookup(local.all.{lookup}, "{name}"'
 
             value = ''
             if variable.get('type', None) == 'string':
                 value = f', "{variable.get("default", "")}"'
             else:
                 value = f', {json.dumps(variable.get("default"))}'
             line_content += value
@@ -203,33 +191,32 @@
     }
 
 
 def generate(
     url: str,
     path: str,
     version: str,
+    lookup: str,
     hcl_files: list,
     include: bool = True,
-    config: str = 'config.yaml',
-    lookup: str = '["{name}"]',
     name: str = None,
 ) -> str:
     variables, variables_object = parse_variables(hcl_files['variable'])
 
     name = (
         (
             path.split('/')[-1:][0]
             if path is not None
             else url.split('/')[-1:][0].replace('.git', '')
         )
         if name is None
         else name
     )
 
-    #lookup = f'local.all{lookup.format(name=name,)}'
+    # lookup = f'local.all{lookup.format(name=name,)}'
     results: str
     results = generate_header(name, url, path, version, lookup, variables_object)
     results += generate_include(include)
-    results += generate_locals(config, url, path, version)
+    results += generate_locals(url, path, version)
     results += generate_terraform(url, path, version, lookup)
     results += generate_inputs(variables, lookup)
     return results
```

### Comparing `terragrunt-generator-0.6.3/generator/main.py` & `terragrunt-generator-0.6.4/generator/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,22 +34,18 @@
         '--include',
         help='do no rendering the include block',
         action=argparse.BooleanOptionalAction,
         default=True,
     )
 
     parser.add_argument(
-        '-c',
-        '--config',
-        help='define the yaml config path',
-        default='find_in_parent_folders("config.yaml")',
-    )
-
-    parser.add_argument(
-        '-l', '--lookup', help='define the lookup path', default='["{name}"]'
+        '-l',
+        '--lookup',
+        help='define the lookup path'
+        # , default='["{name}"]'
     )
 
     args = parser.parse_args()
 
     tempdir = f'{gettempdir()}/{uuid4()}'
 
     if is_local(args.url):
@@ -61,14 +57,13 @@
         f"{tempdir}/{'' if args.path is None else args.path}"
     )
 
     output: str = generate(
         args.url,
         None if args.path is None else args.path,
         args.version,
+        args.lookup,
         hcl_files,
         args.include,
-        args.config,
-        args.lookup,
     )
 
     print(output)
```

### Comparing `terragrunt-generator-0.6.3/pyproject.toml` & `terragrunt-generator-0.6.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,13 +19,13 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.3"
+version = "0.6.4"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "generator/__init__.py",
 ]
```

### Comparing `terragrunt-generator-0.6.3/setup.py` & `terragrunt-generator-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.3/terragrunt_generator.egg-info/PKG-INFO` & `terragrunt-generator-0.6.4/terragrunt_generator.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.6.3
+Version: 0.6.4
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
 
@@ -24,266 +24,291 @@
 ```
 
 ## Usages
 
 ### Exec
 
 ```sh
-$ terragrunt-generator -u https://github.com/terraform-google-modules/terraform-google-project-factory.git -v v14.2.1 -l 'project' | wl-copy
+$ terragrunt-generator --help
+usage: terragrunt-gernerator [-h] [-V] -u URL [-v VERSION] [-p PATH] [--include | --no-include] [-l LOOKUP]
+
+generate terragrunt.hcl confirugation from terraform module
+
+options:
+  -h, --help            show this help message and exit
+  -V                    show program's version number and exit
+  -u URL, --url URL     the module repository url
+  -v VERSION, --version VERSION
+                        the module version to use
+  -p PATH, --path PATH  define the module path if needed
+  --include, --no-include
+                        do no rendering the include block
+  -l LOOKUP, --lookup LOOKUP
+                        define the lookup path
+```
+
+#### Example
+
+```sh
+$ terragrunt-generator \
+-u https://github.com/terraform-google-modules/terraform-google-project-factory.git \
+-v v14.2.1 \
+-l 'project'
 ```
 
 ### Results
 
 ```hcl
 # terraform-google-project-factory v14.2.1
 # https://github.com/terraform-google-modules/terraform-google-project-factory/tree/v14.2.1/
 #
 # yaml config
 # ```
 # project:
 #   enabled: true
 #   # org_id - The organization ID.
-#   org_id: 
+#   org_id:
 #   # name - The name for the project
-#   name: 
+#   name:
 #   # billing_account - The ID of the billing account to associate this project with
-#   billing_account: 
+#   billing_account:
 #   # random_project_id - Adds a suffix of 4 random characters to the `project_id`.
-#   random_project_id: 
+#   random_project_id:
 #   # domain - The domain name (optional).
-#   domain: 
+#   domain:
 #   # project_id - The ID to give the project. If not provided, the `name` will be used.
-#   project_id: 
+#   project_id:
 #   # svpc_host_project_id - The ID of the host project which hosts the shared VPC
-#   svpc_host_project_id: 
+#   svpc_host_project_id:
 #   # enable_shared_vpc_host_project - If this project is a shared VPC host project. If true, you must *not* set svpc_host_project_id variable. Default is false.
-#   enable_shared_vpc_host_project: 
+#   enable_shared_vpc_host_project:
 #   # folder_id - The ID of a folder to host this project
-#   folder_id: 
+#   folder_id:
 #   # group_name - A group to control the project by being assigned group_role (defaults to project editor)
-#   group_name: 
+#   group_name:
 #   # group_role - The role to give the controlling group (group_name) over the project (defaults to project editor)
 #   group_role: "roles/editor"
 #   # create_project_sa - Whether the default service account for the project shall be created
 #   create_project_sa: true
 #   # project_sa_name - Default service account name for the project.
 #   project_sa_name: "project-service-account"
 #   # sa_role - A role to give the default Service Account for the project (defaults to none)
-#   sa_role: 
+#   sa_role:
 #   # activate_apis - The list of apis to activate within the project
 #   activate_apis: ["compute.googleapis.com"]
 #   # activate_api_identities - The list of service identities (Google Managed service account for the API) to force-create for the project (e.g. in order to grant additional roles).
 #   #    APIs in this list will automatically be appended to `activate_apis`.
 #   #    Not including the API in this list will follow the default behaviour for identity creation (which is usually when the first resource using the API is created).
 #   #    Any roles (e.g. service agent role) must be explicitly listed. See https://cloud.google.com/iam/docs/understanding-roles#service-agent-roles-roles for a list of related roles.
-#   activate_api_identities: 
+#   activate_api_identities:
 #   # usage_bucket_name - Name of a GCS bucket to store GCE usage reports in (optional)
-#   usage_bucket_name: 
+#   usage_bucket_name:
 #   # usage_bucket_prefix - Prefix in the GCS bucket to store GCE usage reports in (optional)
-#   usage_bucket_prefix: 
+#   usage_bucket_prefix:
 #   # shared_vpc_subnets - List of subnets fully qualified subnet IDs (ie. projects/$project_id/regions/$region/subnetworks/$subnet_id)
-#   shared_vpc_subnets: 
+#   shared_vpc_subnets:
 #   # labels - Map of labels for project
-#   labels: 
+#   labels:
 #   # bucket_project - A project to create a GCS bucket (bucket_name) in, useful for Terraform state (optional)
-#   bucket_project: 
+#   bucket_project:
 #   # bucket_name - A name for a GCS bucket to create (in the bucket_project project), useful for Terraform state (optional)
-#   bucket_name: 
+#   bucket_name:
 #   # bucket_location - The location for a GCS bucket to create (optional)
 #   bucket_location: "US"
 #   # bucket_versioning - Enable versioning for a GCS bucket to create (optional)
-#   bucket_versioning: 
+#   bucket_versioning:
 #   # bucket_labels -  A map of key/value label pairs to assign to the bucket (optional)
-#   bucket_labels: 
+#   bucket_labels:
 #   # bucket_force_destroy - Force the deletion of all objects within the GCS bucket when deleting the bucket (optional)
-#   bucket_force_destroy: 
+#   bucket_force_destroy:
 #   # bucket_ula - Enable Uniform Bucket Level Access
 #   bucket_ula: true
 #   # bucket_pap - Enable Public Access Prevention. Possible values are "enforced" or "inherited".
 #   bucket_pap: "inherited"
 #   # auto_create_network - Create the default network
-#   auto_create_network: 
+#   auto_create_network:
 #   # lien - Add a lien on the project to prevent accidental deletion
-#   lien: 
+#   lien:
 #   # disable_services_on_destroy - Whether project services will be disabled when the resources are destroyed
 #   disable_services_on_destroy: true
 #   # default_service_account - Project default service account setting: can be one of `delete`, `deprivilege`, `disable`, or `keep`.
 #   default_service_account: "disable"
 #   # disable_dependent_services - Whether services that are enabled and which depend on this service should also be disabled when this service is destroyed.
 #   disable_dependent_services: true
 #   # budget_monitoring_notification_channels - A list of monitoring notification channels in the form `[projects/{project_id}/notificationChannels/{channel_id}]`. A maximum of 5 channels are allowed.
-#   budget_monitoring_notification_channels: 
+#   budget_monitoring_notification_channels:
 #   # budget_alert_spent_percents - A list of percentages of the budget to alert on when threshold is exceeded
 #   budget_alert_spent_percents: [0.5, 0.7, 1.0]
 #   # budget_alert_spend_basis - The type of basis used to determine if spend has passed the threshold
 #   budget_alert_spend_basis: "CURRENT_SPEND"
 #   # budget_labels - A single label and value pair specifying that usage from only this set of labeled resources should be included in the budget.
-#   budget_labels: 
+#   budget_labels:
 #   # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
-#   vpc_service_control_attach_enabled: 
+#   vpc_service_control_attach_enabled:
 #   # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
 #   vpc_service_control_sleep_duration: "5s"
 #   # grant_services_security_admin_role - Whether or not to grant Kubernetes Engine Service Agent the Security Admin role on the host project so it can manage firewall rules
-#   grant_services_security_admin_role: 
+#   grant_services_security_admin_role:
 #   # grant_network_role - Whether or not to grant networkUser role on the host project/subnets
 #   grant_network_role: true
 #   # consumer_quotas - The quotas configuration you want to override for the project.
-#   consumer_quotas: 
+#   consumer_quotas:
 #   # default_network_tier - Default Network Service Tier for resources created in this project. If unset, the value will not be modified. See https://cloud.google.com/network-tiers/docs/using-network-service-tiers and https://cloud.google.com/network-tiers.
-#   default_network_tier: 
+#   default_network_tier:
 #   # essential_contacts - A mapping of users or groups to be assigned as Essential Contacts to the project, specifying a notification category
-#   essential_contacts: 
+#   essential_contacts:
 #   # language_tag - Language code to be used for essential contacts notifications
 #   language_tag: "en-US"
 #   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
-#   # random_project_id_length: 
+#   # random_project_id_length:
 #   # budget_amount - The amount to use for a budget alert
-#   # budget_amount: 
-#   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>` 
-#   # budget_display_name: 
+#   # budget_amount:
+#   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
+#   # budget_display_name:
 #   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
-#   # budget_alert_pubsub_topic: 
+#   # budget_alert_pubsub_topic:
 #   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
-#   # budget_calendar_period: 
+#   # budget_calendar_period:
 #   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
-#   # budget_custom_period_start_date: 
+#   # budget_custom_period_start_date:
 #   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
-#   # budget_custom_period_end_date: 
+#   # budget_custom_period_end_date:
 #   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
-#   # vpc_service_control_perimeter_name: 
+#   # vpc_service_control_perimeter_name:
 # ```
 #
 
 include {
     path = find_in_parent_folders()
 }
 
 locals {
     module = {
         repository = "github.com/terraform-google-modules/terraform-google-project-factory.git"
         path = null
         version = "v14.2.1"
         source =  "${local.module.repository}${local.module.path != null ? local.module.path : ''}?ref=${local.module.version}"
     }
-    environment = get_env("ENV", "development")
+    environment = get_env("CONFIG", "test")
     all = merge(
         yamldecode(file(find_in_parent_folders(format("config.%s.yaml", local.environment)))),
     )
 }
 
 terraform {
-    source = lookup(project, "enabled", true) == true ? local.module.source : null
+    source = lookup(local.all.project, "enabled", true) == true ? local.module.source : null
 }
 
 inputs = merge({
     # billing_account - The ID of the billing account to associate this project with - required
-    billing_account = lookup(project, "billing_account", "")
+    billing_account = lookup(local.all.project, "billing_account", "")
     # name - The name for the project - required
-    name = lookup(project, "name", "")
+    name = lookup(local.all.project, "name", "")
     # org_id - The organization ID. - required
-    org_id = lookup(project, "org_id", "")
+    org_id = lookup(local.all.project, "org_id", "")
     # activate_api_identities - The list of service identities (Google Managed service account for the API) to force-create for the project (e.g. in order to grant additional roles).
     # APIs in this list will automatically be appended to `activate_apis`.
     # Not including the API in this list will follow the default behaviour for identity creation (which is usually when the first resource using the API is created).
     # Any roles (e.g. service agent role) must be explicitly listed. See https://cloud.google.com/iam/docs/understanding-roles#service-agent-roles-roles for a list of related roles.
-    activate_api_identities = lookup(project, "activate_api_identities", [])
+    activate_api_identities = lookup(local.all.project, "activate_api_identities", [])
     # activate_apis - The list of apis to activate within the project
-    activate_apis = lookup(project, "activate_apis", ["compute.googleapis.com"])
+    activate_apis = lookup(local.all.project, "activate_apis", ["compute.googleapis.com"])
     # auto_create_network - Create the default network
-    auto_create_network = lookup(project, "auto_create_network", false)
+    auto_create_network = lookup(local.all.project, "auto_create_network", false)
     # bucket_force_destroy - Force the deletion of all objects within the GCS bucket when deleting the bucket (optional)
-    bucket_force_destroy = lookup(project, "bucket_force_destroy", false)
+    bucket_force_destroy = lookup(local.all.project, "bucket_force_destroy", false)
     # bucket_labels -  A map of key/value label pairs to assign to the bucket (optional)
-    bucket_labels = lookup(project, "bucket_labels", {})
+    bucket_labels = lookup(local.all.project, "bucket_labels", {})
     # bucket_location - The location for a GCS bucket to create (optional)
-    bucket_location = lookup(project, "bucket_location", "US")
+    bucket_location = lookup(local.all.project, "bucket_location", "US")
     # bucket_name - A name for a GCS bucket to create (in the bucket_project project), useful for Terraform state (optional)
-    bucket_name = lookup(project, "bucket_name", "")
+    bucket_name = lookup(local.all.project, "bucket_name", "")
     # bucket_pap - Enable Public Access Prevention. Possible values are "enforced" or "inherited".
-    bucket_pap = lookup(project, "bucket_pap", "inherited")
+    bucket_pap = lookup(local.all.project, "bucket_pap", "inherited")
     # bucket_project - A project to create a GCS bucket (bucket_name) in, useful for Terraform state (optional)
-    bucket_project = lookup(project, "bucket_project", "")
+    bucket_project = lookup(local.all.project, "bucket_project", "")
     # bucket_ula - Enable Uniform Bucket Level Access
-    bucket_ula = lookup(project, "bucket_ula", true)
+    bucket_ula = lookup(local.all.project, "bucket_ula", true)
     # bucket_versioning - Enable versioning for a GCS bucket to create (optional)
-    bucket_versioning = lookup(project, "bucket_versioning", false)
+    bucket_versioning = lookup(local.all.project, "bucket_versioning", false)
     # budget_alert_spend_basis - The type of basis used to determine if spend has passed the threshold
-    budget_alert_spend_basis = lookup(project, "budget_alert_spend_basis", "CURRENT_SPEND")
+    budget_alert_spend_basis = lookup(local.all.project, "budget_alert_spend_basis", "CURRENT_SPEND")
     # budget_alert_spent_percents - A list of percentages of the budget to alert on when threshold is exceeded
-    budget_alert_spent_percents = lookup(project, "budget_alert_spent_percents", [0.5, 0.7, 1.0])
+    budget_alert_spent_percents = lookup(local.all.project, "budget_alert_spent_percents", [0.5, 0.7, 1.0])
     # budget_labels - A single label and value pair specifying that usage from only this set of labeled resources should be included in the budget.
-    budget_labels = lookup(project, "budget_labels", {})
+    budget_labels = lookup(local.all.project, "budget_labels", {})
     # budget_monitoring_notification_channels - A list of monitoring notification channels in the form `[projects/{project_id}/notificationChannels/{channel_id}]`. A maximum of 5 channels are allowed.
-    budget_monitoring_notification_channels = lookup(project, "budget_monitoring_notification_channels", [])
+    budget_monitoring_notification_channels = lookup(local.all.project, "budget_monitoring_notification_channels", [])
     # consumer_quotas - The quotas configuration you want to override for the project.
-    consumer_quotas = lookup(project, "consumer_quotas", [])
+    consumer_quotas = lookup(local.all.project, "consumer_quotas", [])
     # create_project_sa - Whether the default service account for the project shall be created
-    create_project_sa = lookup(project, "create_project_sa", true)
+    create_project_sa = lookup(local.all.project, "create_project_sa", true)
     # default_network_tier - Default Network Service Tier for resources created in this project. If unset, the value will not be modified. See https://cloud.google.com/network-tiers/docs/using-network-service-tiers and https://cloud.google.com/network-tiers.
-    default_network_tier = lookup(project, "default_network_tier", "")
+    default_network_tier = lookup(local.all.project, "default_network_tier", "")
     # default_service_account - Project default service account setting: can be one of `delete`, `deprivilege`, `disable`, or `keep`.
-    default_service_account = lookup(project, "default_service_account", "disable")
+    default_service_account = lookup(local.all.project, "default_service_account", "disable")
     # disable_dependent_services - Whether services that are enabled and which depend on this service should also be disabled when this service is destroyed.
-    disable_dependent_services = lookup(project, "disable_dependent_services", true)
+    disable_dependent_services = lookup(local.all.project, "disable_dependent_services", true)
     # disable_services_on_destroy - Whether project services will be disabled when the resources are destroyed
-    disable_services_on_destroy = lookup(project, "disable_services_on_destroy", true)
+    disable_services_on_destroy = lookup(local.all.project, "disable_services_on_destroy", true)
     # domain - The domain name (optional).
-    domain = lookup(project, "domain", "")
+    domain = lookup(local.all.project, "domain", "")
     # enable_shared_vpc_host_project - If this project is a shared VPC host project. If true, you must *not* set svpc_host_project_id variable. Default is false.
-    enable_shared_vpc_host_project = lookup(project, "enable_shared_vpc_host_project", false)
+    enable_shared_vpc_host_project = lookup(local.all.project, "enable_shared_vpc_host_project", false)
     # essential_contacts - A mapping of users or groups to be assigned as Essential Contacts to the project, specifying a notification category
-    essential_contacts = lookup(project, "essential_contacts", {})
+    essential_contacts = lookup(local.all.project, "essential_contacts", {})
     # folder_id - The ID of a folder to host this project
-    folder_id = lookup(project, "folder_id", "")
+    folder_id = lookup(local.all.project, "folder_id", "")
     # grant_network_role - Whether or not to grant networkUser role on the host project/subnets
-    grant_network_role = lookup(project, "grant_network_role", true)
+    grant_network_role = lookup(local.all.project, "grant_network_role", true)
     # grant_services_security_admin_role - Whether or not to grant Kubernetes Engine Service Agent the Security Admin role on the host project so it can manage firewall rules
-    grant_services_security_admin_role = lookup(project, "grant_services_security_admin_role", false)
+    grant_services_security_admin_role = lookup(local.all.project, "grant_services_security_admin_role", false)
     # group_name - A group to control the project by being assigned group_role (defaults to project editor)
-    group_name = lookup(project, "group_name", "")
+    group_name = lookup(local.all.project, "group_name", "")
     # group_role - The role to give the controlling group (group_name) over the project (defaults to project editor)
-    group_role = lookup(project, "group_role", "roles/editor")
+    group_role = lookup(local.all.project, "group_role", "roles/editor")
     # labels - Map of labels for project
-    labels = lookup(project, "labels", {})
+    labels = lookup(local.all.project, "labels", {})
     # language_tag - Language code to be used for essential contacts notifications
-    language_tag = lookup(project, "language_tag", "en-US")
+    language_tag = lookup(local.all.project, "language_tag", "en-US")
     # lien - Add a lien on the project to prevent accidental deletion
-    lien = lookup(project, "lien", false)
+    lien = lookup(local.all.project, "lien", false)
     # project_id - The ID to give the project. If not provided, the `name` will be used.
-    project_id = lookup(project, "project_id", "")
+    project_id = lookup(local.all.project, "project_id", "")
     # project_sa_name - Default service account name for the project.
-    project_sa_name = lookup(project, "project_sa_name", "project-service-account")
+    project_sa_name = lookup(local.all.project, "project_sa_name", "project-service-account")
     # random_project_id - Adds a suffix of 4 random characters to the `project_id`.
-    random_project_id = lookup(project, "random_project_id", false)
+    random_project_id = lookup(local.all.project, "random_project_id", false)
     # sa_role - A role to give the default Service Account for the project (defaults to none)
-    sa_role = lookup(project, "sa_role", "")
+    sa_role = lookup(local.all.project, "sa_role", "")
     # shared_vpc_subnets - List of subnets fully qualified subnet IDs (ie. projects/$project_id/regions/$region/subnetworks/$subnet_id)
-    shared_vpc_subnets = lookup(project, "shared_vpc_subnets", [])
+    shared_vpc_subnets = lookup(local.all.project, "shared_vpc_subnets", [])
     # svpc_host_project_id - The ID of the host project which hosts the shared VPC
-    svpc_host_project_id = lookup(project, "svpc_host_project_id", "")
+    svpc_host_project_id = lookup(local.all.project, "svpc_host_project_id", "")
     # usage_bucket_name - Name of a GCS bucket to store GCE usage reports in (optional)
-    usage_bucket_name = lookup(project, "usage_bucket_name", "")
+    usage_bucket_name = lookup(local.all.project, "usage_bucket_name", "")
     # usage_bucket_prefix - Prefix in the GCS bucket to store GCE usage reports in (optional)
-    usage_bucket_prefix = lookup(project, "usage_bucket_prefix", "")
+    usage_bucket_prefix = lookup(local.all.project, "usage_bucket_prefix", "")
     # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
-    vpc_service_control_attach_enabled = lookup(project, "vpc_service_control_attach_enabled", false)
+    vpc_service_control_attach_enabled = lookup(local.all.project, "vpc_service_control_attach_enabled", false)
     # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
-    vpc_service_control_sleep_duration = lookup(project, "vpc_service_control_sleep_duration", "5s")
+    vpc_service_control_sleep_duration = lookup(local.all.project, "vpc_service_control_sleep_duration", "5s")
 },
   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
   (lookup(project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(project, "budget_alert_pubsub_topic") }),
   # budget_amount - The amount to use for a budget alert
   (lookup(project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(project, "budget_amount") }),
   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
   (lookup(project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(project, "budget_calendar_period") }),
   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
   (lookup(project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(project, "budget_custom_period_end_date") }),
   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
   (lookup(project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(project, "budget_custom_period_start_date") }),
-  # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>` 
+  # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
   (lookup(project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(project, "budget_display_name") }),
   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
   (lookup(project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(project, "random_project_id_length") }),
   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
   (lookup(project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(project, "vpc_service_control_perimeter_name") })
 )
+
 ```
```

### Comparing `terragrunt-generator-0.6.3/terragrunt_generator.egg-info/SOURCES.txt` & `terragrunt-generator-0.6.4/terragrunt_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.3/tests/test_generate.py` & `terragrunt-generator-0.6.4/tests/test_generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,30 +25,29 @@
     assert '' in results
 
 
 def test_generate_locals():
     # Scenario 1
     # Given the generate_locals function is called with filename="", url="https://gitserver.com/test/test.git", path="modules/test", and version="0.1.0"
     # When the function is executed
-    filename = ''
     url: str = 'https://gitserver.com/test/test.git'
     path: str = 'modules/test'
     version: str = '0.1.0'
-    results = generate_locals(filename, url, path, version)
+    results = generate_locals(url, path, version)
 
     # Then it should return a string that includes the expected "locals" block
     expected = """
 locals {
     module = {
         repository = "gitserver.com/test/test.git"
         path = "//modules/test"
         version = "0.1.0"
         source =  "${local.module.repository}${local.module.path != null ? local.module.path : ''}?ref=${local.module.version}"
     }
-    environment = get_env("ENV", "development")
+    environment = get_env("CONFIG", "test")
     all = merge(
         yamldecode(file(find_in_parent_folders(format("config.%s.yaml", local.environment)))),
     )
 }
 """
 
     assert results == expected
@@ -57,15 +56,15 @@
 def test_generate_terraform():
     # Scenario 1
     # Given the generate_terraform function is called with url="https://gitserver.com/test/test.git", path="modules/test", version="0.1.0", and lookup="local.all[\"test\"]"
     # When the function is executed
     url: str = 'https://gitserver.com/test/test.git'
     path: str = 'modules/test'
     version: str = '0.1.0'
-    lookup: str = 'local.all.test'
+    lookup: str = 'test'
     results = generate_terraform(url, path, version, lookup)
 
     # Then it should return a string that includes the expected "terraform" block
     expected = """
 terraform {
     source = lookup(local.all.test, "enabled", true) == true ? local.module.source : null
 }
@@ -82,15 +81,15 @@
         {
             'name': 'test',
             'description': 'A',
             'type': 'string',
             'default': 'hello',
         }
     ]
-    lookup: str = 'local.all.test'
+    lookup: str = 'test'
     results = generate_inputs(variables, lookup)
 
     # Then it should return a string that includes the expected "inputs" block
     expected = """
 inputs = {
     # test - A
     test = lookup(local.all.test, "test", "hello")
```

### Comparing `terragrunt-generator-0.6.3/tests/test_reader.py` & `terragrunt-generator-0.6.4/tests/test_reader.py`

 * *Files identical despite different names*

