# Comparing `tmp/stigg_api_client_v2-0.515.3.tar.gz` & `tmp/stigg_api_client_v2-0.517.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.515.3.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.517.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.515.3.tar` & `stigg_api_client_v2-0.517.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1644 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/README.md
--rw-r--r--   0        0        0      452 2023-07-31 10:13:08.553031 stigg_api_client_v2-0.515.3/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/stigg/__init__.py
--rw-r--r--   0        0        0     4711 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/stigg/client.py
--rw-r--r--   0        0        0      932 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/stigg/edge_utils.py
--rw-r--r--   0        0        0    40986 2023-07-31 10:13:06.896977 stigg_api_client_v2-0.515.3/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-31 10:13:05.508933 stigg_api_client_v2-0.515.3/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-31 10:13:06.412962 stigg_api_client_v2-0.515.3/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    70891 2023-07-31 10:13:06.632969 stigg_api_client_v2-0.515.3/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-31 10:13:01.336801 stigg_api_client_v2-0.515.3/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-31 10:13:06.412962 stigg_api_client_v2-0.515.3/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-31 10:13:05.452931 stigg_api_client_v2-0.515.3/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-31 10:13:05.468932 stigg_api_client_v2-0.515.3/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70464 2023-07-31 10:13:01.556808 stigg_api_client_v2-0.515.3/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-31 10:13:05.496933 stigg_api_client_v2-0.515.3/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24198 2023-07-31 10:13:03.152859 stigg_api_client_v2-0.515.3/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-31 10:13:05.456931 stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-31 10:13:05.464932 stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-31 10:13:06.412962 stigg_api_client_v2-0.515.3/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    58974 2023-07-31 10:13:06.408961 stigg_api_client_v2-0.515.3/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-31 10:13:05.524933 stigg_api_client_v2-0.515.3/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-31 10:13:05.532934 stigg_api_client_v2-0.515.3/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-31 10:13:05.512933 stigg_api_client_v2-0.515.3/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-31 10:13:05.572935 stigg_api_client_v2-0.515.3/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-31 10:13:05.548934 stigg_api_client_v2-0.515.3/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-31 10:13:05.544934 stigg_api_client_v2-0.515.3/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-31 10:13:05.580935 stigg_api_client_v2-0.515.3/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-31 10:13:05.536934 stigg_api_client_v2-0.515.3/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-31 10:13:05.556934 stigg_api_client_v2-0.515.3/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-31 10:13:05.568935 stigg_api_client_v2-0.515.3/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-31 10:13:05.416930 stigg_api_client_v2-0.515.3/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-31 10:13:05.408930 stigg_api_client_v2-0.515.3/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-31 10:13:05.440931 stigg_api_client_v2-0.515.3/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   127287 2023-07-31 10:13:05.392929 stigg_api_client_v2-0.515.3/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-31 10:13:05.500933 stigg_api_client_v2-0.515.3/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-31 10:13:05.404930 stigg_api_client_v2-0.515.3/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-31 10:13:05.432931 stigg_api_client_v2-0.515.3/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-31 10:13:05.488932 stigg_api_client_v2-0.515.3/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-31 10:13:05.484932 stigg_api_client_v2-0.515.3/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-31 10:13:05.480932 stigg_api_client_v2-0.515.3/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-31 10:13:06.416962 stigg_api_client_v2-0.515.3/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-31 10:13:05.424930 stigg_api_client_v2-0.515.3/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-31 10:13:05.444931 stigg_api_client_v2-0.515.3/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-31 10:13:05.588935 stigg_api_client_v2-0.515.3/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.515.3/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/README.md
+-rw-r--r--   0        0        0      452 2023-08-01 07:11:23.019905 stigg_api_client_v2-0.517.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/stigg/__init__.py
+-rw-r--r--   0        0        0     4711 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/stigg/client.py
+-rw-r--r--   0        0        0      932 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/stigg/edge_utils.py
+-rw-r--r--   0        0        0    41050 2023-08-01 07:11:20.699898 stigg_api_client_v2-0.517.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-08-01 07:11:18.759895 stigg_api_client_v2-0.517.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-08-01 07:11:20.019897 stigg_api_client_v2-0.517.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    70891 2023-08-01 07:11:20.339897 stigg_api_client_v2-0.517.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-08-01 07:11:12.779851 stigg_api_client_v2-0.517.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-08-01 07:11:20.019897 stigg_api_client_v2-0.517.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-08-01 07:11:18.679895 stigg_api_client_v2-0.517.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-08-01 07:11:18.707895 stigg_api_client_v2-0.517.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70464 2023-08-01 07:11:13.095853 stigg_api_client_v2-0.517.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-08-01 07:11:18.743895 stigg_api_client_v2-0.517.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24306 2023-08-01 07:11:15.315870 stigg_api_client_v2-0.517.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-08-01 07:11:18.691895 stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-08-01 07:11:18.703895 stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-08-01 07:11:20.019897 stigg_api_client_v2-0.517.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    58974 2023-08-01 07:11:20.015897 stigg_api_client_v2-0.517.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-08-01 07:11:18.783895 stigg_api_client_v2-0.517.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-08-01 07:11:18.791895 stigg_api_client_v2-0.517.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-08-01 07:11:18.771895 stigg_api_client_v2-0.517.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-08-01 07:11:18.851896 stigg_api_client_v2-0.517.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-08-01 07:11:18.815895 stigg_api_client_v2-0.517.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-08-01 07:11:18.807895 stigg_api_client_v2-0.517.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-08-01 07:11:18.863896 stigg_api_client_v2-0.517.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-08-01 07:11:18.799895 stigg_api_client_v2-0.517.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-08-01 07:11:18.827895 stigg_api_client_v2-0.517.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-08-01 07:11:18.843896 stigg_api_client_v2-0.517.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-08-01 07:11:18.627894 stigg_api_client_v2-0.517.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-08-01 07:11:18.619894 stigg_api_client_v2-0.517.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-08-01 07:11:18.659894 stigg_api_client_v2-0.517.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   127287 2023-08-01 07:11:18.599894 stigg_api_client_v2-0.517.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-08-01 07:11:18.751895 stigg_api_client_v2-0.517.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-08-01 07:11:18.615894 stigg_api_client_v2-0.517.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-08-01 07:11:18.655894 stigg_api_client_v2-0.517.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-08-01 07:11:18.735895 stigg_api_client_v2-0.517.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-08-01 07:11:18.727895 stigg_api_client_v2-0.517.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-08-01 07:11:18.719895 stigg_api_client_v2-0.517.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-08-01 07:11:20.027897 stigg_api_client_v2-0.517.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-08-01 07:11:18.639894 stigg_api_client_v2-0.517.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-08-01 07:11:18.671894 stigg_api_client_v2-0.517.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-08-01 07:11:18.875896 stigg_api_client_v2-0.517.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.517.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.515.3/README.md` & `stigg_api_client_v2-0.517.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.515.3/stigg/client.py` & `stigg_api_client_v2-0.517.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.515.3/stigg/edge_utils.py` & `stigg_api_client_v2-0.517.0/stigg/edge_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/__init__.py` & `stigg_api_client_v2-0.517.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
@@ -75,14 +75,15 @@
     SourceType,
     SubscriptionAddonSortFields,
     SubscriptionCancellationTime,
     SubscriptionCancelReason,
     SubscriptionDecisionStrategy,
     SubscriptionEndSetup,
     SubscriptionEntitlementSortFields,
+    SubscriptionInvoiceStatus,
     SubscriptionMigrationTaskSortFields,
     SubscriptionMigrationTime,
     SubscriptionPriceSortFields,
     SubscriptionScheduleStatus,
     SubscriptionScheduleType,
     SubscriptionStartSetup,
     SubscriptionStatus,
@@ -1099,14 +1100,15 @@
     "SubscriptionFragmentTotalPrice",
     "SubscriptionFutureUpdateData",
     "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
     "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
     "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
     "SubscriptionFutureUpdateDataTargetPackage",
     "SubscriptionInput",
+    "SubscriptionInvoiceStatus",
     "SubscriptionMigrationInput",
     "SubscriptionMigrationTaskFilter",
     "SubscriptionMigrationTaskSort",
     "SubscriptionMigrationTaskSortFields",
     "SubscriptionMigrationTime",
     "SubscriptionPreviewFragment",
     "SubscriptionPreviewFragmentBillingPeriodRange",
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.517.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/async_client.py` & `stigg_api_client_v2-0.517.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/base_client.py` & `stigg_api_client_v2-0.517.0/stigg/generated/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/base_model.py` & `stigg_api_client_v2-0.517.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.517.0/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/client.py` & `stigg_api_client_v2-0.517.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.517.0/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/enums.py` & `stigg_api_client_v2-0.517.0/stigg/generated/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
@@ -754,14 +754,20 @@
     createdAt = "createdAt"
     environmentId = "environmentId"
     id = "id"
     subscriptionId = "subscriptionId"
     updatedAt = "updatedAt"
 
 
+class SubscriptionInvoiceStatus(str, Enum):
+    CANCELED = "CANCELED"
+    OPEN = "OPEN"
+    PAID = "PAID"
+
+
 class SubscriptionMigrationTaskSortFields(str, Enum):
     createdAt = "createdAt"
     environmentId = "environmentId"
     id = "id"
     status = "status"
     taskType = "taskType"
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.517.0/stigg/generated/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/fragments.py` & `stigg_api_client_v2-0.517.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,14 +32,36 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -56,36 +78,14 @@
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -329,47 +329,14 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
-class CustomerPortalSubscriptionPriceFragment(BaseModel):
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    billing_model: Optional[BillingModel] = Field(alias="billingModel")
-    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
-    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
-
-
-class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-
-
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -414,14 +381,34 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
+
+
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+
+
 class CustomerPortalSubscriptionAddon(BaseModel):
     addon_id: str = Field(alias="addonId")
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     quantity: int
 
 
@@ -506,14 +493,27 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -548,65 +548,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class SubscriptionFutureUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
@@ -719,14 +668,65 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class TotalPriceFragment(BaseModel):
     sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
     total: "TotalPriceFragmentTotal"
 
 
 class TotalPriceFragmentSubTotal(BaseModel):
     amount: float
@@ -899,34 +899,14 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -942,14 +922,34 @@
 class MockPaywallPriceFragmentFeature(BaseModel):
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1396,19 +1396,19 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
 SlimCustomerFragment.update_forward_refs()
@@ -1431,49 +1431,44 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionPriceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateData.update_forward_refs()
 SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
@@ -1482,14 +1477,19 @@
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
@@ -1509,19 +1509,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.517.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.517.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.517.0/stigg/generated/get_customer_by_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.517.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.517.0/stigg/generated/get_mock_paywall.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/get_products.py` & `stigg_api_client_v2-0.517.0/stigg/generated/get_products.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.517.0/stigg/generated/get_sdk_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/input_types.py` & `stigg_api_client_v2-0.517.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.517.0/stigg/generated/provision_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.517.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.517.0/stigg/generated/report_usage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.515.3/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.517.0/stigg/generated/update_subscription.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 10:13
+# Generated by ariadne-codegen on 2023-08-01 07:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.515.3/PKG-INFO` & `stigg_api_client_v2-0.517.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.515.3
+Version: 0.517.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

