# Comparing `tmp/threemystic_cloud_data_client-0.1.64.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.65.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.64.tar` & `threemystic_cloud_data_client-0.1.65.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0    17768 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23536 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/hatch.toml
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/pyproject.toml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    25671 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13576 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.65/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,21 @@
 
         year_data[cost_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
         year_data[cost_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
         year_data[cost_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
         if data_dt >= fiscal_start and data_dt <= fiscal_end:
           year_data[cost_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
 
+  def get_total_cost_data(self, cost_data, cost_metric, *args, **kwargs):
+    if cost_data["Total"].get(cost_metric) is not None:
+      if cost_data["Total"][cost_metric].get("Unit") is not None:
+        return cost_data["Total"][cost_metric]["Unit"]
+    
+    return 0
+      
   def get_currency_cost_data(self, cost_data, cost_metric, *args, **kwargs):
     if cost_data["Total"].get(cost_metric) is not None:
       if cost_data["Total"][cost_metric].get("Unit") is not None:
         return cost_data["Total"][cost_metric]["Unit"]
     
     if len(cost_data["Groups"]) > 0:
       if cost_data["Groups"][0]["Metrics"].get(cost_metric) is not None:
@@ -174,41 +181,24 @@
 
         day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
         if year_data[cost_metric].get(by_month_key) is None:
           year_data[cost_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
         
         if year_data[cost_metric][by_month_key]["days"].get(day_key) is None:
           year_data[cost_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= self.get_currency_cost_data(cost_data= cost_data, cost_metric= cost_metric))
-        
-        raw_row_data_cost = (cost_data["Total"][cost_metric]["Amount"])
-        row_data_cost = (cost_data["Total"][cost_metric]["Amount"])
-        
-        if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"]:
-          row_data_cost = self.get_common().helper_currency().convert(
-            ammount= row_data_cost,
-            currency_from= year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"],
-            currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
-            conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
-              dt_string= self.get_common().helper_type().datetime().datetime_as_string(
-                dt= data_dt,
-                dt_format= "%Y%m01"
-              ),
-              dt_format= "%Y%m%d"
-            )).date()
-          )
 
-        year_data[cost_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
-        year_data[cost_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
-        year_data[cost_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
-        if data_dt >= fiscal_start and data_dt <= fiscal_end:
-          year_data[cost_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
+        raw_row_data_cost = self.get_total_cost_data(cost_data= cost_data, cost_metric= cost_metric)
+        total_attribute_empty = False if raw_row_data_cost > 0 else True
 
         for cost_data_group in cost_data["Groups"]:
           raw_row_data_cost_group = cost_data_group["Metrics"][cost_metric]["Amount"]
           row_data_cost_group = raw_row_data_cost_group
+
+          if total_attribute_empty:
+            raw_row_data_cost += raw_row_data_cost_group
           
           if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != cost_data_group["Metrics"][cost_metric]["Unit"]:
             row_data_cost_group = self.get_common().helper_currency().convert(
               ammount= row_data_cost_group,
               currency_from= cost_data_group["Metrics"][cost_metric]["Unit"],
               currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
               conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
@@ -230,14 +220,36 @@
               year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] = Decimal(0)
               year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data_group_key] = Decimal(0)
 
             year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] += Decimal(raw_row_data_cost_group)
             year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data_group_key] += Decimal(row_data_cost_group)
             year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] += Decimal(raw_row_data_cost_group)
             year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data_group_key] += Decimal(row_data_cost_group)
+        
+        row_data_cost = raw_row_data_cost
+        
+        if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"]:
+          row_data_cost = self.get_common().helper_currency().convert(
+            ammount= row_data_cost,
+            currency_from= year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"],
+            currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
+            conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
+              dt_string= self.get_common().helper_type().datetime().datetime_as_string(
+                dt= data_dt,
+                dt_format= "%Y%m01"
+              ),
+              dt_format= "%Y%m%d"
+            )).date()
+          )
+
+        year_data[cost_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
+        year_data[cost_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
+        if data_dt >= fiscal_start and data_dt <= fiscal_end:
+          year_data[cost_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
 
 
   async def __process_get_cost_data(self, account, client, fiscal_year_start, loop, *args, **kwargs):
     fiscal_year_start_date = self.get_common().helper_type().datetime().datetime_from_string(
       dt_string= f"{self.get_data_start().year}/{fiscal_year_start}",
       dt_format= "%Y/%m/%d"
     )
```

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,77 @@
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.base_class.base import cloud_data_client_azure_client_action_base as base
 import asyncio
+from requests import post as request_post
 from decimal import Decimal, ROUND_HALF_UP
 from azure.mgmt.costmanagement import CostManagementClient
-from azure.mgmt.costmanagement.models import GranularityType,ForecastDefinition,ForecastType,ForecastTimeframe,ForecastTimePeriod,QueryDefinition,TimeframeType,ExportType,QueryTimePeriod
+from azure.mgmt.costmanagement.models import GranularityType,ForecastDefinition,ForecastType,ForecastTimeframe,ForecastTimePeriod,QueryDefinition,TimeframeType,ExportType,QueryTimePeriod,QueryResult
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="budget", 
       logger_name= "cloud_data_client_azure_client_action_budget",
       *args, **kwargs)
   
   def __process_get_cost_generate_data(self, account, client, cost_filter, is_forcast = False, *args, **kwargs):
     if not is_forcast:
-      return self.get_cloud_client().sdk_request(
+      cost_filter = QueryDefinition(**cost_filter)
+      cost_response = self.get_cloud_client().sdk_request(
         tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
         lambda_sdk_command=lambda: client.query.usage(
           scope= f'{self.get_cloud_client().get_account_prefix()}{self.get_cloud_client().get_account_id(account= account)}',
-          parameters= QueryDefinition(**cost_filter)
+          parameters= cost_filter
         )
       )
-
-    return self.get_cloud_client().sdk_request(
-        tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True),
-        lambda_sdk_command=lambda: client.forecast.usage(
-          scope= f'{self.get_cloud_client().get_account_prefix()}{self.get_cloud_client().get_account_id(account= account)}',
-          parameters= ForecastDefinition(**cost_filter),
+    else:
+      cost_filter = ForecastDefinition(**cost_filter)
+      cost_response = self.get_cloud_client().sdk_request(
+          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True),
+          lambda_sdk_command=lambda: client.forecast.usage(
+            scope= f'{self.get_cloud_client().get_account_prefix()}{self.get_cloud_client().get_account_id(account= account)}',
+            parameters= ForecastDefinition(**cost_filter),
+          )
         )
+    
+    
+    next_link = getattr(cost_response, "next_link", None)
+    
+    next_cost_page = 1
+    cost_filter = cost_filter.serialize()
+    if self.get_common().helper_type().general().is_type(obj= cost_filter, type_check= dict):
+      cost_filter = self.get_common().helper_json().dumps(data= cost_filter)
+
+    while not self.get_common().helper_type().string().is_null_or_whitespace(string_value= next_link):
+      cost_api_resquest = request_post(
+        url= next_link,
+        headers= {
+          "Authorization": f"Bearer {self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)).get_token('https://management.azure.com/.default').token}",
+          "Content-Type": "application/json"
+        },
+        data= cost_filter,
+        timeout= 10,
       )
+
+      if cost_api_resquest.status_code == 429:
+        self.get_common().helper_type().requests().expodential_backoff_wait(attempt= next_cost_page, auto_sleep= True)
+        next_cost_page += 1
+        continue
+
+      cost_api_response = cost_api_resquest.json()
+      next_link = cost_api_response["properties"].get("nextLink")
+      next_cost_page = 1
+
+      cost_response.rows += cost_api_response["properties"].get("rows")
+
+    return cost_response
    
-  async def __process_get_cost_data_forcast_time_range(self, account, start_date, end_date, fiscal_start, fiscal_end, query_grouping = [], *args, **kwargs):
+  async def __process_get_cost_data_forcast_time_range(self, account, year_data, cost_metric, start_date, end_date, fiscal_start, fiscal_end, query_grouping = [], *args, **kwargs):
     
     cost_filter = {
-      'type': ForecastType.AMORTIZED_COST,
+      'type': getattr(ForecastType, cost_metric),
       'timeframe': ForecastTimeframe.CUSTOM,
       'time_period': ForecastTimePeriod(
         from_property= self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= f"{self.get_common().helper_type().datetime().datetime_as_string(dt_format='%Y-%m-%d', dt= start_date)}T00:00:00+00:00"),
         to= self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= f"{self.get_common().helper_type().datetime().datetime_as_string(dt_format='%Y-%m-%d', dt= end_date)}T23:59:59+00:00")
       ),
       'dataset': {
         'granularity': GranularityType.DAILY,
@@ -54,24 +89,24 @@
 
     try:
       usage = self.__process_get_cost_generate_data(account= account, cost_filter= cost_filter, is_forcast= True, *args, **kwargs)
 
       if usage is None:
         return usage
 
-      return await self.__process_get_cost_data_daily_data(usage= usage, fiscal_start= fiscal_start, fiscal_end= fiscal_end,  is_forcast= True, query_grouping= query_grouping)
+      return await self.__process_get_cost_data_daily_data(usage= usage, year_data= year_data, cost_metric= cost_metric, fiscal_start= fiscal_start, fiscal_end= fiscal_end,  is_forcast= True, query_grouping= query_grouping)
     except Exception as err:
       self.get_common().get_logger().exception(msg= f"{self.get_cloud_client().get_account_id(account= account)} - {str(err)}", extra={"exception": err})
       return {}
 
     
-  async def __process_get_cost_data_time_range(self, account, start_date, end_date, fiscal_start, fiscal_end, query_grouping = [], *args, **kwargs):
+  async def __process_get_cost_data_time_range(self, account, year_data, cost_metric, start_date, end_date, fiscal_start, fiscal_end, query_grouping = [], *args, **kwargs):
     
     cost_filter = {
-      'type': ExportType.AMORTIZED_COST,
+      'type': getattr(ExportType, cost_metric),
       'timeframe': TimeframeType.CUSTOM,
       'time_period': QueryTimePeriod(
         from_property= self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= f"{self.get_common().helper_type().datetime().datetime_as_string(dt_format='%Y-%m-%d', dt= start_date)}T00:00:00+00:00"),
         to=  self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= f"{self.get_common().helper_type().datetime().datetime_as_string(dt_format='%Y-%m-%d', dt= end_date)}T23:59:59+00:00")
       ),
       'dataset': {
         'granularity': GranularityType.DAILY,
@@ -85,19 +120,19 @@
           {"type": "Dimension", "name": dimension} for dimension in query_grouping
         ]        
       }
     }
     
     try:
       usage = self.__process_get_cost_generate_data(account= account, cost_filter= cost_filter, is_forcast= False, *args, **kwargs)
-
+      
       if usage is None:
         return {}
 
-      return await self.__process_get_cost_data_daily_data(account= account, usage= usage, fiscal_start= fiscal_start, fiscal_end= fiscal_end, is_forcast= False, query_grouping= query_grouping)
+      return await self.__process_get_cost_data_daily_data(account= account, year_data= year_data, cost_metric= cost_metric, usage= usage, fiscal_start= fiscal_start, fiscal_end= fiscal_end, is_forcast= False, query_grouping= query_grouping)
     except Exception as err:
       self.get_common().get_logger().exception(msg= f"{self.get_cloud_client().get_account_id(account= account)} - {str(err)}", extra={"exception": err})
       return {}
     
   def __init_costdata_month(self, data_dt, *args, **kwargs):
     return {
       "currency": self.get_common().helper_type().string().set_case(self.get_cloud_data_client().get_default_currency(), case= "upper"),
@@ -143,16 +178,20 @@
         "total":{},
         "forcast_total":{},
         "origional_currency_total":{},
         "origional_currency_forcast_total":{},
       }
     }
     
-  async def __process_get_cost_data_daily_data(self, usage, fiscal_start, fiscal_end, query_grouping, is_forcast = False, *args, **kwargs):
-    by_month = { }
+  async def __process_get_cost_data_daily_data(self, usage, year_data, cost_metric, fiscal_start, fiscal_end, query_grouping, is_forcast = False, *args, **kwargs):
+    
+    if year_data is None:
+      year_data = {}
+    if year_data.get(cost_metric) is None:
+      year_data[cost_metric] = {}
 
     column_indexs = {
       self.get_common().helper_type().string().set_case(string_value= dimension, case= "lower"):-1 for dimension in query_grouping
     }
     if column_indexs.get("resourcegroup") is None:
       column_indexs["resourcegroup"] = -1
     if column_indexs.get("resourcetype") is None:
@@ -178,79 +217,76 @@
       cost_key = f"cost{self.get_common().helper_type().string().set_case(self.get_cloud_data_client().get_default_currency(), case= 'lower')}"
 
     for cost_data in usage.rows:
       data_dt = self.get_common().helper_type().datetime().datetime_from_string(dt_string= str(cost_data[column_indexs["usagedate"]]), dt_format= "%Y%m%d")
       by_month_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m", dt= data_dt)
         
       day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
-      if by_month.get(by_month_key) is None:
-        by_month[by_month_key] = self.__init_costdata_month(data_dt= data_dt)
+      if year_data[cost_metric].get(by_month_key) is None:
+        year_data[cost_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
       
-      if by_month[by_month_key]["days"].get(day_key) is None:
-        by_month[by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= cost_data[column_indexs["currency"]])
+      if year_data[cost_metric][by_month_key]["days"].get(day_key) is None:
+        year_data[cost_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= cost_data[column_indexs["currency"]])
 
       
       raw_row_data_cost = (cost_data[column_indexs[cost_key]])
       row_data_cost = (cost_data[column_indexs[cost_key]])
       
-      if by_month[by_month_key]["days"][day_key]["currency"] != by_month[by_month_key]["days"][day_key]["origional_currency"]:
+      if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"]:
         row_data_cost = self.get_common().helper_currency().convert(
           ammount= row_data_cost,
-          currency_from= by_month[by_month_key]["days"][day_key]["origional_currency"],
-          currency_to= by_month[by_month_key]["days"][day_key]["currency"],
+          currency_from= year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"],
+          currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
           conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
             dt_string= self.get_common().helper_type().datetime().datetime_as_string(
               dt= data_dt,
               dt_format= "%Y%m01"
             ),
             dt_format= "%Y%m%d"
           )).date()
         )
 
-      by_month[by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
-      by_month[by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
-      by_month[by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
+      year_data[cost_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
+      year_data[cost_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
+      year_data[cost_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
       if data_dt >= fiscal_start and data_dt <= fiscal_end:
-        by_month[by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
 
       if column_indexs["resourcegroup"] > -1:
-        if (by_month[by_month_key]["days"][day_key]["resource_group"][f'{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None or
-            by_month[by_month_key]["days"][day_key]["resource_group"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None):
-          by_month[by_month_key]["days"][day_key]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
-          by_month[by_month_key]["days"][day_key]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
+        if (year_data[cost_metric][by_month_key]["days"][day_key]["resource_group"][f'{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None or
+            year_data[cost_metric][by_month_key]["days"][day_key]["resource_group"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None):
+          year_data[cost_metric][by_month_key]["days"][day_key]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
+          year_data[cost_metric][by_month_key]["days"][day_key]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
         
-        if (by_month[by_month_key]["totals"]["resource_group"][f'{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None or
-            by_month[by_month_key]["totals"]["resource_group"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None):
-          by_month[by_month_key]["totals"]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
-          by_month[by_month_key]["totals"]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
-
-        by_month[by_month_key]["days"][day_key]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(raw_row_data_cost)
-        by_month[by_month_key]["days"][day_key]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(row_data_cost)
-        by_month[by_month_key]["totals"]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(raw_row_data_cost)
-        by_month[by_month_key]["totals"]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(row_data_cost)
+        if (year_data[cost_metric][by_month_key]["totals"]["resource_group"][f'{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None or
+            year_data[cost_metric][by_month_key]["totals"]["resource_group"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcegroup"]]) is None):
+          year_data[cost_metric][by_month_key]["totals"]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
+          year_data[cost_metric][by_month_key]["totals"]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] = Decimal(0)
+
+        year_data[cost_metric][by_month_key]["days"][day_key]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(raw_row_data_cost)
+        year_data[cost_metric][by_month_key]["days"][day_key]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"]["resource_group"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(raw_row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"]["resource_group"][f'{total_key}'][cost_data[column_indexs["resourcegroup"]]] += Decimal(row_data_cost)
 
       if column_indexs["resourcetype"] > -1:
-        if (by_month[by_month_key]["days"][day_key]["resource_type"][f'{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None or
-            by_month[by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None):
-          by_month[by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
-          by_month[by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
+        if (year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None or
+            year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None):
+          year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
+          year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
         
-        if (by_month[by_month_key]["totals"]["resource_type"][f'{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None or
-            by_month[by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None):
-          by_month[by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
-          by_month[by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
-
+        if (year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None or
+            year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'].get(cost_data[column_indexs["resourcetype"]]) is None):
+          year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
+          year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] = Decimal(0)
 
-        by_month[by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(raw_row_data_cost)
-        by_month[by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(row_data_cost)
-        by_month[by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(raw_row_data_cost)
-        by_month[by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(row_data_cost)
 
-
-    return by_month
+        year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(raw_row_data_cost)
+        year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(raw_row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data[column_indexs["resourcetype"]]] += Decimal(row_data_cost)
 
   async def __process_get_cost_data_sum_year_forcast_data(self, year_month_data, forcast_month_data, *args, **kwargs):
     key_list = self.get_common().helper_type().list().unique_list(data= list(year_month_data.keys()) + list(forcast_month_data.keys()))
 
     for key in key_list:
       year_month_key_data = year_month_data.get(key)
       forcast_month_key_data = forcast_month_data.get(key)
@@ -266,57 +302,45 @@
         forcast_month_key_data = Decimal(0)
       
       if self.get_common().helper_type().general().is_numeric(year_month_key_data) and year_month_key_data is None:
         year_month_key_data = Decimal(0)
       
       year_month_data[key] = (year_month_key_data + forcast_month_key_data)
         
-      
 
-  async def __process_get_cost_data_process_year_data_range_data(self, year_data, processed_time_range_data, *args, **kwargs):
-    
-    while len(processed_time_range_data.keys()) > 0:
-        month_key, month_data = processed_time_range_data.popitem()
-        if year_data.get(month_key) is None:
-          year_data[month_key] = month_data
-          continue
-        
-        await self.__process_get_cost_data_sum_year_forcast_data(
-          year_month_data= year_data[month_key],
-          forcast_month_data= month_data
-        )
-
-  async def __process_get_cost_data_process_forcast_year_data(self, year_data, start_date, end_date, fiscal_start, fiscal_end, *args, **kwargs):
+  async def __process_get_cost_data_process_forcast_year_data(self, year_data, cost_metric, start_date, end_date, fiscal_start, fiscal_end, *args, **kwargs):
      end_date += self.get_common().helper_type().datetime().time_delta(months= 1, dt= end_date)
      while start_date < end_date:
-      await self.__process_get_cost_data_process_year_data_range_data(
-        year_data= year_data,
-        processed_time_range_data= await self.__process_get_cost_data_forcast_time_range(
+      await self.__process_get_cost_data_forcast_time_range(
+          year_data= year_data,
+          cost_metric= cost_metric,
           start_date= start_date,
           end_date= self.get_common().helper_type().datetime().yesterday(dt=(start_date + self.get_common().helper_type().datetime().time_delta(months= 3, dt= start_date))),
           fiscal_start= fiscal_start, fiscal_end= fiscal_end, 
           query_grouping= ["SubscriptionId"],
           *args, **kwargs )
-      )
 
       start_date = start_date + self.get_common().helper_type().datetime().time_delta(months= 3, dt= start_date)
 
-  async def __process_get_cost_data_process_year_data(self, year_data, start_date, end_date, fiscal_start, fiscal_end, *args, **kwargs):
+  async def __process_get_cost_data_process_year_data(self, year_data, cost_metric, start_date, end_date, fiscal_start, fiscal_end, *args, **kwargs):
      end_date += self.get_common().helper_type().datetime().time_delta(months= 1, dt= end_date)
-     while start_date < end_date:
-      
-      await self.__process_get_cost_data_process_year_data_range_data(
+     while start_date < end_date and start_date <  self.get_data_start():
+      adjusted_enddate = self.get_common().helper_type().datetime().yesterday(dt=(start_date + self.get_common().helper_type().datetime().time_delta(months= 3, dt= start_date)))
+      if adjusted_enddate > self.get_data_start():
+        adjusted_enddate = self.get_data_start()
+
+      await self.__process_get_cost_data_time_range(
         year_data= year_data,
-        processed_time_range_data= await self.__process_get_cost_data_time_range(
-          start_date= start_date,
-          end_date= self.get_common().helper_type().datetime().yesterday(dt=(start_date + self.get_common().helper_type().datetime().time_delta(months= 3, dt= start_date))),
-          fiscal_start= fiscal_start, fiscal_end= fiscal_end, 
-          query_grouping= ["SubscriptionId"],
-          *args, **kwargs )
-      )
+        cost_metric= cost_metric,
+        start_date= start_date,
+        end_date= adjusted_enddate,
+        fiscal_start= fiscal_start, fiscal_end= fiscal_end, 
+        query_grouping= ["SubscriptionId"],
+        *args, **kwargs )
+      
 
       start_date = start_date + self.get_common().helper_type().datetime().time_delta(months= 3, dt= start_date)
 
       
 
   async def __process_get_cost_data(self, loop, fiscal_year_start, *args, **kwargs):
     fiscal_year_start_date = self.get_common().helper_type().datetime().datetime_from_string(
@@ -333,26 +357,29 @@
     
     start_date = (fiscal_year_start_date
                  + self.get_common().helper_type().datetime().time_delta(months= -1, dt= fiscal_year_start_date))
     
     forecast_end = (fiscal_year_end
                  + self.get_common().helper_type().datetime().time_delta(months= 3, dt= fiscal_year_end))
     year_data = {}
-    #__process_get_cost_data_forcast_time_range
-    cost_metric = ExportType.AMORTIZED_COST
+    cost_metric = "AMORTIZED_COST"
+
     await self.__process_get_cost_data_process_year_data(
       year_data= year_data,
+      cost_metric= cost_metric,
       start_date= start_date,
       end_date= self.get_data_start(),
       fiscal_start= fiscal_year_start_date,
       fiscal_end= fiscal_year_end, *args, **kwargs
     )
+
     
     await self.__process_get_cost_data_process_forcast_year_data(
       year_data= year_data,
+      cost_metric= cost_metric,
       start_date= self.get_data_start(),
       end_date= forecast_end,
       fiscal_start= fiscal_year_start_date,
       fiscal_end= fiscal_year_end, *args, **kwargs
     )
     
     month_key = self.get_common().helper_type().datetime().datetime_as_string(
@@ -373,76 +400,80 @@
       "month_forecast": Decimal(0),
       "last_seven_days": Decimal(0),
       "raw_last_14_days": {},
       "last_month": Decimal(0),
     }
 
     last14_days = {}
-    await self.__process_get_cost_data_process_year_data_range_data(
+    await self.__process_get_cost_data_time_range(
       year_data= last14_days,
-      processed_time_range_data= await self.__process_get_cost_data_time_range(
-        start_date= (self.get_data_start() + self.get_common().helper_type().datetime().time_delta(days= -14)),
-        end_date= self.get_data_start(),
-        fiscal_start= fiscal_year_start_date, fiscal_end= fiscal_year_start_date, 
-        query_grouping= ["SubscriptionId", "ResourceGroup", "ResourceType"],
-        *args, **kwargs )
-    )
+      cost_metric= cost_metric,
+      start_date= (self.get_data_start() + self.get_common().helper_type().datetime().time_delta(days= -14)),
+      end_date= self.get_data_start(),
+      fiscal_start= fiscal_year_start_date, fiscal_end= fiscal_year_start_date, 
+      query_grouping= ["SubscriptionId", "ResourceGroup", "ResourceType"],
+      *args, **kwargs )
 
     day_count = 0
-    if last14_days.get(month_key) is not None:
+    if last14_days.get(cost_metric) is not None:
+
       for i in range(0,9):
         if day_count >= 7:
           break
         
         month_key_last14 = self.get_common().helper_type().datetime().datetime_as_string(
           dt= (self.get_data_start() - self.get_common().helper_type().datetime().time_delta(days= i)),
           dt_format= "%Y%m"
         )
         day_key = self.get_common().helper_type().datetime().datetime_as_string(
           dt= (self.get_data_start() - self.get_common().helper_type().datetime().time_delta(days= i)),
           dt_format= "%Y%m%d"
         )
         
-
-        if last14_days[month_key_last14]["days"].get(day_key) is None:
+        if last14_days[cost_metric].get(month_key_last14) is None:
+          continue
+        if last14_days[cost_metric][month_key_last14]["days"].get(day_key) is None:
           continue
         
         day_count += 1
-        return_data["last_seven_days"] += last14_days[month_key_last14]["days"][day_key]["total"]
-    
-    return_data["raw_last_14_days"] = last14_days[month_key_last14]["days"]
-    
+        return_data["last_seven_days"] += last14_days[cost_metric][month_key_last14]["days"][day_key]["total"]
 
+      return_data["raw_last_14_days"] = {}
+      for month_key in last14_days[cost_metric].keys():
+        for day_key, day_data in last14_days[cost_metric][month_key]["days"].items():
+          return_data["raw_last_14_days"][day_key]= day_data
     
 
-    for data in year_data.values():
-      return_data["fiscal_year_to_date"] += data["totals"].get("fiscal_total")
-      return_data["fiscal_year_forecast"] += (data["totals"].get("fiscal_total") + data["totals"].get("fiscal_forcast_total"))
-      if data["year"] == self.get_data_start().year:
-        return_data["year_to_date"] += data["totals"].get("total")
-        return_data["year_forecast"] += (data["totals"].get("total") + data["totals"].get("forcast_total"))
-
     
-    if year_data.get(month_key) is not None:
-      return_data["month_to_date"] = year_data[month_key]["totals"]["total"]
-      return_data["month_forecast"] = year_data[month_key]["totals"]["total"] + year_data[month_key]["totals"]["forcast_total"]
-    
-    if year_data.get(last_month_key) is not None:
-      return_data["last_month"] = year_data[last_month_key]["totals"]["total"]
+    if year_data.get(cost_metric) is not None:
+      for data in year_data.get(cost_metric).values():
+        return_data["fiscal_year_to_date"] += data["totals"].get("fiscal_total")
+        return_data["fiscal_year_forecast"] += (data["totals"].get("fiscal_total") + data["totals"].get("fiscal_forcast_total"))
+        if data["year"] == self.get_data_start().year:
+          return_data["year_to_date"] += data["totals"].get("total")
+          return_data["year_forecast"] += (data["totals"].get("total") + data["totals"].get("forcast_total"))
+
+      
+      if year_data[cost_metric].get(month_key) is not None:
+        return_data["month_to_date"] = year_data[cost_metric][month_key]["totals"]["total"]
+        return_data["month_forecast"] = year_data[cost_metric][month_key]["totals"]["total"] + year_data[cost_metric][month_key]["totals"]["forcast_total"]
+      
+      if year_data[cost_metric].get(last_month_key) is not None:
+        return_data["last_month"] = year_data[cost_metric][last_month_key]["totals"]["total"]
 
 
     return return_data
 
   async def _process_account_data(self, account, loop, *args, **kwargs):
     
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= kwargs.get("fiscal_year_start")):
       kwargs["fiscal_year_start"] = self.get_cloud_data_client().get_default_fiscal_year_start()
     
     costmanagement_client = CostManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
-  
+    
     return {
       "account": account,
       "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
         {},
         await self.get_base_return_data(
           account= self.get_cloud_client().serialize_resource(resource= account),
           resource_id =  f'{self.get_cloud_client().get_account_prefix()}{self.get_cloud_client().get_account_id(account= account)}',
```

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
           string_value= status.get("code"),
           separator= "[/]"
         )[-1], case= "upper")
       
     return None
   async def _process_account_data(self, account, loop, *args, **kwargs):
     client = ComputeManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
-
+    
     public_ips = await self.__process_get_resources_vm_public_ips(account= account)
     tasks = {
         "resource": loop.create_task(self.__process_get_resources_vm(account= account)),
         "vm_statuses": loop.create_task(self.__process_get_resources_vm_statuses(account= account, client= client)),
         "availability_sets": loop.create_task(self.__process_get_resources_vm_availability_sets(client= client, account= account)),
         "nics": loop.create_task(self.__process_get_resources_vm_nics(account= account, public_ips= public_ips)),
         "load_balancers": loop.create_task(self.__process_get_resources_vm_load_balancers(account= account, public_ips= public_ips)),
```

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     super().__init__(provider= "azure", *args, **kwargs)  
 
   def get_accounts(self, *args, **kwargs):
 
     if len(self.get_runparam_key(data_key= "data_accounts", default_value= [])) < 1:
       return [ 
         account for account in self.get_cloud_client().get_accounts() 
-        if account.resource_container ]
+        if account.resource_container and account.subscription_id == "5c49443f-ce4b-470d-8ba8-c9571c1de06d" ]
     
     return [ 
         account for account in self.get_cloud_client().get_accounts() 
         if( account.resource_container and 
             self.get_cloud_client().get_account_id(account= account) in self.get_runparam_key(data_key= "data_accounts", default_value= []) and 
             not f'-{self.get_cloud_client().get_account_id(account= account)}' in self.get_runparam_key(data_key= "data_accounts", default_value= [])
           )
```

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.65/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/.gitignore` & `threemystic_cloud_data_client-0.1.65/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/LICENSE` & `threemystic_cloud_data_client-0.1.65/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/README.md` & `threemystic_cloud_data_client-0.1.65/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/hatch.toml` & `threemystic_cloud_data_client-0.1.65/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.64/pyproject.toml` & `threemystic_cloud_data_client-0.1.65/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.17",
-  "threemystic-cloud-client >= 0.1.59",
+  "threemystic-cloud-client >= 0.1.60",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-compute >= 29",
   "azure-mgmt-cosmosdb >= 9",
   "azure-mgmt-costmanagement >= 4",
   "azure-mgmt-dns >= 8",
```

### Comparing `threemystic_cloud_data_client-0.1.64/PKG-INFO` & `threemystic_cloud_data_client-0.1.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.64
+Version: 0.1.65
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 Requires-Dist: azure-mgmt-redis>=14
 Requires-Dist: azure-mgmt-resourcegraph>=8
 Requires-Dist: azure-mgmt-sql>=3
 Requires-Dist: azure-mgmt-sqlvirtualmachine>=0.6
 Requires-Dist: azure-mgmt-subscription>=3
 Requires-Dist: azure-mgmt-synapse>=2
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.59
+Requires-Dist: threemystic-cloud-client>=0.1.60
 Requires-Dist: threemystic-common>=0.1.17
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
```

