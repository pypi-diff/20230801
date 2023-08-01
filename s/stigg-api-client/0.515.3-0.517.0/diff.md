# Comparing `tmp/stigg_api_client-0.515.3.tar.gz` & `tmp/stigg_api_client-0.517.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.515.3.tar", max compression
+gzip compressed data, was "stigg_api_client-0.517.0.tar", max compression
```

## Comparing `stigg_api_client-0.515.3.tar` & `stigg_api_client-0.517.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-31 10:12:28.144694 stigg_api_client-0.515.3/README.md
--rw-r--r--   0        0        0      480 2023-07-31 10:13:03.168762 stigg_api_client-0.515.3/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-31 10:12:28.144694 stigg_api_client-0.515.3/stigg/__init__.py
--rw-r--r--   0        0        0     3699 2023-07-31 10:12:28.144694 stigg_api_client-0.515.3/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-31 10:13:01.252756 stigg_api_client-0.515.3/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-07-31 10:13:01.680757 stigg_api_client-0.515.3/stigg/generated/operations.py
--rw-r--r--   0        0        0   467319 2023-07-31 10:13:01.512757 stigg_api_client-0.515.3/stigg/generated/schema.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.515.3/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-08-01 07:10:16.828104 stigg_api_client-0.517.0/README.md
+-rw-r--r--   0        0        0      480 2023-08-01 07:10:51.584442 stigg_api_client-0.517.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-08-01 07:10:16.828104 stigg_api_client-0.517.0/stigg/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-01 07:10:16.828104 stigg_api_client-0.517.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-08-01 07:10:49.652430 stigg_api_client-0.517.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-08-01 07:10:50.068433 stigg_api_client-0.517.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   468257 2023-08-01 07:10:49.916432 stigg_api_client-0.517.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.517.0/PKG-INFO
```

### Comparing `stigg_api_client-0.515.3/README.md` & `stigg_api_client-0.517.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.515.3/stigg/client.py` & `stigg_api_client-0.517.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.515.3/stigg/generated/operations.py` & `stigg_api_client-0.517.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.515.3/stigg/generated/schema.py` & `stigg_api_client-0.517.0/stigg/generated/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,19 @@
 
 
 class SubscriptionEntitlementSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'environmentId', 'id', 'subscriptionId', 'updatedAt')
 
 
+class SubscriptionInvoiceStatus(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('CANCELED', 'OPEN', 'PAID')
+
+
 class SubscriptionMigrationTaskSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'environmentId', 'id', 'status', 'taskType')
 
 
 class SubscriptionMigrationTime(sgqlc.types.Enum):
     __schema__ = schema
@@ -4078,15 +4083,15 @@
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
 
 
 class CustomerSubscription(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'billing_id', 'billing_link_url', 'cancel_reason', 'cancellation_date', 'coupon', 'created_at', 'crm_id', 'crm_link_url', 'current_billing_period_end', 'customer', 'effective_end_date', 'end_date', 'environment', 'environment_id', 'experiment', 'experiment_info', 'future_updates', 'id', 'is_custom_price_subscription', 'old_billing_id', 'outdated_price_packages', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'scheduled_updates', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'sync_states', 'total_price', 'trial_end_date', 'was_in_trial')
+    __field_names__ = ('additional_meta_data', 'addons', 'billing_id', 'billing_link_url', 'cancel_reason', 'cancellation_date', 'coupon', 'created_at', 'crm_id', 'crm_link_url', 'current_billing_period_end', 'customer', 'effective_end_date', 'end_date', 'environment', 'environment_id', 'experiment', 'experiment_info', 'future_updates', 'id', 'is_custom_price_subscription', 'latest_invoice', 'old_billing_id', 'outdated_price_packages', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'scheduled_updates', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'sync_states', 'total_price', 'trial_end_date', 'was_in_trial')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddon')), graphql_name='addons', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(SubscriptionAddonFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionAddonSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
@@ -4104,14 +4109,15 @@
     environment = sgqlc.types.Field(sgqlc.types.non_null('Environment'), graphql_name='environment')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     experiment = sgqlc.types.Field('Experiment', graphql_name='experiment')
     experiment_info = sgqlc.types.Field('experimentInfo', graphql_name='experimentInfo')
     future_updates = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionFutureUpdate'))), graphql_name='futureUpdates')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     is_custom_price_subscription = sgqlc.types.Field(Boolean, graphql_name='isCustomPriceSubscription')
+    latest_invoice = sgqlc.types.Field('SubscriptionInvoice', graphql_name='latestInvoice')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
     outdated_price_packages = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='outdatedPricePackages')
     plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='plan')
     prices = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPrice')), graphql_name='prices', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(SubscriptionPriceFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionPriceSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
@@ -6985,14 +6991,25 @@
     schedule_status = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionScheduleStatus), graphql_name='scheduleStatus')
     schedule_variables = sgqlc.types.Field('ScheduleVariables', graphql_name='scheduleVariables')
     scheduled_execution_time = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='scheduledExecutionTime')
     subscription_schedule_type = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionScheduleType), graphql_name='subscriptionScheduleType')
     target_package = sgqlc.types.Field(PackageDTO, graphql_name='targetPackage')
 
 
+class SubscriptionInvoice(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('billing_id', 'created_at', 'error_message', 'payment_url', 'status', 'updated_at')
+    billing_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='billingId')
+    created_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='createdAt')
+    error_message = sgqlc.types.Field(String, graphql_name='errorMessage')
+    payment_url = sgqlc.types.Field(String, graphql_name='paymentUrl')
+    status = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionInvoiceStatus), graphql_name='status')
+    updated_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='updatedAt')
+
+
 class SubscriptionMigrationTask(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('affected_customers_count', 'created_at', 'end_date', 'environment_id', 'id', 'initiated_package_id', 'packages', 'progress', 'start_date', 'status', 'task_type')
     affected_customers_count = sgqlc.types.Field(Int, graphql_name='affectedCustomersCount')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
```

### Comparing `stigg_api_client-0.515.3/PKG-INFO` & `stigg_api_client-0.517.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.515.3
+Version: 0.517.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

