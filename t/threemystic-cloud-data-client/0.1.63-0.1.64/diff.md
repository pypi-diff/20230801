# Comparing `tmp/threemystic_cloud_data_client-0.1.63.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.64.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.63.tar` & `threemystic_cloud_data_client-0.1.64.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0    17385 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23458 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/hatch.toml
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/pyproject.toml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.63/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0    17768 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23536 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.64/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,86 +58,98 @@
         "total":{},
         "forcast_total":{},
         "origional_currency_total":{},
         "origional_currency_forcast_total":{},
       }
     }
   
-  async def __process_get_cost_data_process_forcast(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, forecast_metrics, *args, **kwargs):
+  async def __process_get_cost_data_process_forcast(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, cost_metrics, *args, **kwargs):
     
-    results_by_time_forcast = self.get_cloud_client().general_boto_call_array(
-      boto_call=lambda: client.get_cost_and_usage(
-        TimePeriod={
-          'Start': start_date.strftime("%Y-%m-%d"),
-          'End': end_date.strftime("%Y-%m-%d"),
-        },
-        Granularity='DAILY',
-        Metrics=forecast_metrics,
-        Filter={
-          "Dimensions":{
-            "Key":"LINKED_ACCOUNT",
-            "Values":[self.get_cloud_client().get_account_id(account= account)]
-          }
-        },
-      ),
-      boto_params= None,
-      boto_nextkey = None,
-      boto_key= None
-    )
+    for cost_metric in cost_metrics:
+      results_by_time_forcast = self.get_cloud_client().general_boto_call_array(
+        boto_call=lambda: client.get_cost_forecast(
+          TimePeriod={
+            'Start': start_date.strftime("%Y-%m-%d"),
+            'End': end_date.strftime("%Y-%m-%d"),
+          },
+          Granularity='DAILY',
+          Metric=cost_metric,
+          Filter={
+            "Dimensions":{
+              "Key":"LINKED_ACCOUNT",
+              "Values":[self.get_cloud_client().get_account_id(account= account)]
+            }
+          },
+        ),
+        boto_params= None,
+        boto_nextkey = None,
+        boto_key= None
+      )
+      
+      total_key = "forcast_total"
+      currency = results_by_time_forcast["Total"]["Unit"]
     
-    total_key = "forcast_total"
-    currency = results_by_time_forcast["Total"]["Unit"]
     
-    for forecast_metric in forecast_metrics:
-      year_data[forecast_metric] = {}
+      year_data[cost_metric] = {}
       for cost_data in results_by_time_forcast["ForecastResultsByTime"]:
         data_dt = self.get_common().helper_type().datetime().datetime_from_string(dt_string= str(cost_data["TimePeriod"]["Start"]), dt_format= "%Y-%m-%d")
         by_month_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m", dt= data_dt)
 
         day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
         if year_data.get(by_month_key) is None:
-          year_data[forecast_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
+          year_data[cost_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
         
-        if year_data[forecast_metric][by_month_key]["days"].get(day_key) is None:
-          year_data[forecast_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= currency)
+        if year_data[cost_metric][by_month_key]["days"].get(day_key) is None:
+          year_data[cost_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= currency)
         
         raw_row_data_cost = (cost_data["MeanValue"])
         row_data_cost = (cost_data["MeanValue"])
         
-        if year_data[forecast_metric][by_month_key]["days"][day_key]["currency"] != year_data[forecast_metric][by_month_key]["days"][day_key]["origional_currency"]:
+        if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"]:
           row_data_cost = self.get_common().helper_currency().convert(
             ammount= row_data_cost,
             currency_from= currency,
-            currency_to= year_data[forecast_metric][by_month_key]["days"][day_key]["currency"],
+            currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
             conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
               dt_string= self.get_common().helper_type().datetime().datetime_as_string(
                 dt= data_dt,
                 dt_format= "%Y%m01"
               ),
               dt_format= "%Y%m%d"
             )).date()
           )
 
-        year_data[forecast_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
-        year_data[forecast_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
-        year_data[forecast_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
+        year_data[cost_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
         if data_dt >= fiscal_start and data_dt <= fiscal_end:
-          year_data[forecast_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
+          year_data[cost_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
 
-
-  async def __process_get_cost_data_process_year_data(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, forecast_metrics, *args, **kwargs):
+  def get_currency_cost_data(self, cost_data, cost_metric, *args, **kwargs):
+    if cost_data["Total"].get(cost_metric) is not None:
+      if cost_data["Total"][cost_metric].get("Unit") is not None:
+        return cost_data["Total"][cost_metric]["Unit"]
+    
+    if len(cost_data["Groups"]) > 0:
+      if cost_data["Groups"][0]["Metrics"].get(cost_metric) is not None:
+        if cost_data["Groups"][0]["Metrics"][cost_metric].get("Unit") is not None:
+          return cost_data["Groups"][0]["Metrics"][cost_metric]["Unit"]
+        
+    return self.get_cloud_data_client().get_default_currency()
+      
+  async def __process_get_cost_data_process_year_data(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, cost_metrics, *args, **kwargs):
 
     results_by_time = self.get_cloud_client().general_boto_call_array(
       boto_call=lambda: client.get_cost_and_usage(
         TimePeriod={
           'Start': start_date.strftime("%Y-%m-%d"),
           'End': end_date.strftime("%Y-%m-%d"),
         },
         Granularity='DAILY',
-        Metrics=forecast_metrics,
+        Metrics=cost_metrics,
         Filter={
           "Dimensions":{
             "Key":"LINKED_ACCOUNT",
             "Values":[self.get_cloud_client().get_account_id(account= account)]
           }
         },
         GroupBy= [
@@ -150,84 +162,82 @@
       boto_params= None,
       boto_nextkey = "NextPageToken",
       boto_nextkey_param = "NextPageToken",
       boto_key="ResultsByTime"
     )
     
     total_key = "total"
-    for forecast_metric in forecast_metrics:
-      year_data[forecast_metric] = {}
+    for cost_metric in cost_metrics:
+      year_data[cost_metric] = {}
       for cost_data in results_by_time:
         data_dt = self.get_common().helper_type().datetime().datetime_from_string(dt_string= str(cost_data["TimePeriod"]["Start"]), dt_format= "%Y-%m-%d")
         by_month_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m", dt= data_dt)
 
         day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
-        if year_data[forecast_metric].get(by_month_key) is None:
-          year_data[forecast_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
+        if year_data[cost_metric].get(by_month_key) is None:
+          year_data[cost_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
         
-        if year_data[forecast_metric][by_month_key]["days"].get(day_key) is None:
-          year_data[forecast_metric][by_month_key]["days"][day_key] = cost_data
-          return 
-          year_data[forecast_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= cost_data["Total"][forecast_metric]["Unit"])
+        if year_data[cost_metric][by_month_key]["days"].get(day_key) is None:
+          year_data[cost_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= self.get_currency_cost_data(cost_data= cost_data, cost_metric= cost_metric))
         
-        raw_row_data_cost = (cost_data["Total"][forecast_metric]["Amount"])
-        row_data_cost = (cost_data["Total"][forecast_metric]["Amount"])
+        raw_row_data_cost = (cost_data["Total"][cost_metric]["Amount"])
+        row_data_cost = (cost_data["Total"][cost_metric]["Amount"])
         
-        if year_data[forecast_metric][by_month_key]["days"][day_key]["currency"] != year_data[forecast_metric][by_month_key]["days"][day_key]["origional_currency"]:
+        if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"]:
           row_data_cost = self.get_common().helper_currency().convert(
             ammount= row_data_cost,
-            currency_from= year_data[forecast_metric][by_month_key]["days"][day_key]["origional_currency"],
-            currency_to= year_data[forecast_metric][by_month_key]["days"][day_key]["currency"],
+            currency_from= year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"],
+            currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
             conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
               dt_string= self.get_common().helper_type().datetime().datetime_as_string(
                 dt= data_dt,
                 dt_format= "%Y%m01"
               ),
               dt_format= "%Y%m%d"
             )).date()
           )
 
-        year_data[forecast_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
-        year_data[forecast_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
-        year_data[forecast_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
+        year_data[cost_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
+        year_data[cost_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
         if data_dt >= fiscal_start and data_dt <= fiscal_end:
-          year_data[forecast_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
+          year_data[cost_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
 
         for cost_data_group in cost_data["Groups"]:
-          raw_row_data_cost_group = cost_data_group["Metrics"][forecast_metric]["Amount"]
+          raw_row_data_cost_group = cost_data_group["Metrics"][cost_metric]["Amount"]
           row_data_cost_group = raw_row_data_cost_group
           
-          if year_data[forecast_metric][by_month_key]["days"][day_key]["currency"] != cost_data_group["Metrics"][forecast_metric]["Unit"]:
+          if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != cost_data_group["Metrics"][cost_metric]["Unit"]:
             row_data_cost_group = self.get_common().helper_currency().convert(
               ammount= row_data_cost_group,
-              currency_from= cost_data_group["Metrics"][forecast_metric]["Unit"],
-              currency_to= year_data[forecast_metric][by_month_key]["days"][day_key]["currency"],
+              currency_from= cost_data_group["Metrics"][cost_metric]["Unit"],
+              currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
               conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
                 dt_string= self.get_common().helper_type().datetime().datetime_as_string(
                   dt= data_dt,
                   dt_format= "%Y%m01"
                 ),
                 dt_format= "%Y%m%d"
               )).date()
             )
           for cost_data_group_key in cost_data_group["Keys"]:
-            if (year_data[forecast_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'].get(cost_data_group_key) is None or
-                year_data[forecast_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'].get(cost_data_group_key) is None):
-              year_data[forecast_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] = Decimal(0)
-              year_data[forecast_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data_group_key] = Decimal(0)
+            if (year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'].get(cost_data_group_key) is None or
+                year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'].get(cost_data_group_key) is None):
+              year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] = Decimal(0)
+              year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data_group_key] = Decimal(0)
             
-            if (year_data[forecast_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'].get(cost_data_group_key) is None or
-                year_data[forecast_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'].get(cost_data_group_key) is None):
-              year_data[forecast_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] = Decimal(0)
-              year_data[forecast_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data_group_key] = Decimal(0)
-
-            year_data[forecast_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] += Decimal(raw_row_data_cost_group)
-            year_data[forecast_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data_group_key] += Decimal(row_data_cost_group)
-            year_data[forecast_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] += Decimal(raw_row_data_cost_group)
-            year_data[forecast_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data_group_key] += Decimal(row_data_cost_group)
+            if (year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'].get(cost_data_group_key) is None or
+                year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'].get(cost_data_group_key) is None):
+              year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] = Decimal(0)
+              year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data_group_key] = Decimal(0)
+
+            year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] += Decimal(raw_row_data_cost_group)
+            year_data[cost_metric][by_month_key]["days"][day_key]["resource_type"][f'{total_key}'][cost_data_group_key] += Decimal(row_data_cost_group)
+            year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'origional_currency_{total_key}'][cost_data_group_key] += Decimal(raw_row_data_cost_group)
+            year_data[cost_metric][by_month_key]["totals"]["resource_type"][f'{total_key}'][cost_data_group_key] += Decimal(row_data_cost_group)
 
 
   async def __process_get_cost_data(self, account, client, fiscal_year_start, loop, *args, **kwargs):
     fiscal_year_start_date = self.get_common().helper_type().datetime().datetime_from_string(
       dt_string= f"{self.get_data_start().year}/{fiscal_year_start}",
       dt_format= "%Y/%m/%d"
     )
@@ -243,48 +253,49 @@
                  + self.get_common().helper_type().datetime().time_delta(months= -1, dt= fiscal_year_start_date))
     
     forecast_end = (fiscal_year_end
                  + self.get_common().helper_type().datetime().time_delta(months= 3, dt= fiscal_year_end))
     
 
     year_data = {}
-    forcast_metric = "NetUnblendedCost"
+    cost_metric = "NetUnblendedCost"
     await self.__process_get_cost_data_process_year_data(
       year_data= year_data,
       client= client,
       account= account,
       start_date= start_date,
       end_date= self.get_data_start() if forecast_end > self.get_data_start() else forecast_end,
       fiscal_start= fiscal_year_start_date, 
       fiscal_end= fiscal_year_end,
-      forecast_metrics = [forcast_metric]
+      cost_metrics = [cost_metric]
     )
-    return year_data
 
-    await self.__process_get_cost_data_process_forcast(
-      year_data= year_data,
-      client= client,
-      account= account,
-      start_date= start_date,
-      end_date= self.get_data_start() if forecast_end > self.get_data_start() else forecast_end,
-      fiscal_start= fiscal_year_start_date, 
-      fiscal_end= fiscal_year_end,
-      forecast_metrics = [forcast_metric]
-    )
+    if forecast_end > self.get_data_start():
+      await self.__process_get_cost_data_process_forcast(
+        year_data= year_data,
+        client= client,
+        account= account,
+        start_date= self.get_data_start(),
+        end_date= forecast_end,
+        fiscal_start= fiscal_year_start_date, 
+        fiscal_end= fiscal_year_end,
+        cost_metrics = [cost_metric]
+      )
 
     month_key = self.get_common().helper_type().datetime().datetime_as_string(
       dt= self.get_data_start(),
       dt_format= "%Y%m"
     )
     last_month_key = self.get_common().helper_type().datetime().datetime_as_string(
       dt= (self.get_data_start() - self.get_common().helper_type().datetime().time_delta(days= (self.get_data_start().day + 1))),
       dt_format= "%Y%m"
     )
     
     return_data = {
+      "cost_metric": cost_metric,
       "year_to_date": Decimal(0),  
       "year_forecast": Decimal(0),
       "fiscal_year_to_date": Decimal(0),  
       "fiscal_year_forecast": Decimal(0),
       "month_to_date": Decimal(0),  
       "month_forecast": Decimal(0),
       "last_seven_days": Decimal(0),
```

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,15 @@
     start_date = (fiscal_year_start_date
                  + self.get_common().helper_type().datetime().time_delta(months= -1, dt= fiscal_year_start_date))
     
     forecast_end = (fiscal_year_end
                  + self.get_common().helper_type().datetime().time_delta(months= 3, dt= fiscal_year_end))
     year_data = {}
     #__process_get_cost_data_forcast_time_range
+    cost_metric = ExportType.AMORTIZED_COST
     await self.__process_get_cost_data_process_year_data(
       year_data= year_data,
       start_date= start_date,
       end_date= self.get_data_start(),
       fiscal_start= fiscal_year_start_date,
       fiscal_end= fiscal_year_end, *args, **kwargs
     )
@@ -359,14 +360,15 @@
       dt_format= "%Y%m"
     )
     last_month_key = self.get_common().helper_type().datetime().datetime_as_string(
       dt= (self.get_data_start() - self.get_common().helper_type().datetime().time_delta(days= (self.get_data_start().day + 1))),
       dt_format= "%Y%m"
     )
     return_data = {
+      "cost_metric": cost_metric,
       "year_to_date": Decimal(0),  
       "year_forecast": Decimal(0),
       "fiscal_year_to_date": Decimal(0),  
       "fiscal_year_forecast": Decimal(0),
       "month_to_date": Decimal(0),  
       "month_forecast": Decimal(0),
       "last_seven_days": Decimal(0),
```

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.64/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/.gitignore` & `threemystic_cloud_data_client-0.1.64/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/LICENSE` & `threemystic_cloud_data_client-0.1.64/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/README.md` & `threemystic_cloud_data_client-0.1.64/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/hatch.toml` & `threemystic_cloud_data_client-0.1.64/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/pyproject.toml` & `threemystic_cloud_data_client-0.1.64/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.63/PKG-INFO` & `threemystic_cloud_data_client-0.1.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.63
+Version: 0.1.64
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

