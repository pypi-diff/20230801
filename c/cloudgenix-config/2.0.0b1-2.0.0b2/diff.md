# Comparing `tmp/cloudgenix_config-2.0.0b1.tar.gz` & `tmp/cloudgenix_config-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudgenix_config-2.0.0b1.tar", last modified: Fri Jul 14 20:11:42 2023, max compression
+gzip compressed data, was "cloudgenix_config-2.0.0b2.tar", last modified: Tue Aug  1 15:34:45 2023, max compression
```

## Comparing `cloudgenix_config-2.0.0b1.tar` & `cloudgenix_config-2.0.0b2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-07-14 20:11:42.336189 cloudgenix_config-2.0.0b1/
--rw-r--r--   0 tkamath  (1953533316) 192360288     1066 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/LICENSE
--rw-r--r--   0 tkamath  (1953533316) 192360288    10303 2023-07-14 20:11:42.336323 cloudgenix_config-2.0.0b1/PKG-INFO
--rw-r--r--   0 tkamath  (1953533316) 192360288     9556 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/README.md
-drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-07-14 20:11:42.332246 cloudgenix_config-2.0.0b1/cloudgenix_config/
--rw-r--r--   0 tkamath  (1953533316) 192360288    29548 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/__init__.py
--rw-r--r--   0 tkamath  (1953533316) 192360288   172697 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/default_interfaces.py
--rwxr-xr-x   0 tkamath  (1953533316) 192360288   580626 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/do.py
--rwxr-xr-x   0 tkamath  (1953533316) 192360288   105950 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/pull.py
-drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-07-14 20:11:42.335781 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/
--rw-r--r--   0 tkamath  (1953533316) 192360288    10303 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/PKG-INFO
--rw-r--r--   0 tkamath  (1953533316) 192360288      404 2023-07-14 20:11:42.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/SOURCES.txt
--rw-r--r--   0 tkamath  (1953533316) 192360288        1 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/dependency_links.txt
--rw-r--r--   0 tkamath  (1953533316) 192360288       90 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/entry_points.txt
--rw-r--r--   0 tkamath  (1953533316) 192360288       41 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/requires.txt
--rw-r--r--   0 tkamath  (1953533316) 192360288       18 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/top_level.txt
--rw-r--r--   0 tkamath  (1953533316) 192360288      358 2023-07-14 20:11:42.336827 cloudgenix_config-2.0.0b1/setup.cfg
--rw-r--r--   0 tkamath  (1953533316) 192360288     1324 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/setup.py
+drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-08-01 15:34:45.540356 cloudgenix_config-2.0.0b2/
+-rw-r--r--   0 tkamath  (1953533316) 192360288     1066 2023-08-01 15:33:54.000000 cloudgenix_config-2.0.0b2/LICENSE
+-rw-r--r--   0 tkamath  (1953533316) 192360288    10362 2023-08-01 15:34:45.540536 cloudgenix_config-2.0.0b2/PKG-INFO
+-rw-r--r--   0 tkamath  (1953533316) 192360288     9615 2023-08-01 15:33:54.000000 cloudgenix_config-2.0.0b2/README.md
+drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-08-01 15:34:45.534745 cloudgenix_config-2.0.0b2/cloudgenix_config/
+-rw-r--r--   0 tkamath  (1953533316) 192360288    29548 2023-08-01 15:33:54.000000 cloudgenix_config-2.0.0b2/cloudgenix_config/__init__.py
+-rw-r--r--   0 tkamath  (1953533316) 192360288   172697 2023-08-01 15:33:54.000000 cloudgenix_config-2.0.0b2/cloudgenix_config/default_interfaces.py
+-rwxr-xr-x   0 tkamath  (1953533316) 192360288   580978 2023-08-01 15:33:54.000000 cloudgenix_config-2.0.0b2/cloudgenix_config/do.py
+-rwxr-xr-x   0 tkamath  (1953533316) 192360288   106064 2023-08-01 15:33:54.000000 cloudgenix_config-2.0.0b2/cloudgenix_config/pull.py
+drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-08-01 15:34:45.539678 cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/
+-rw-r--r--   0 tkamath  (1953533316) 192360288    10362 2023-08-01 15:34:44.000000 cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/PKG-INFO
+-rw-r--r--   0 tkamath  (1953533316) 192360288      404 2023-08-01 15:34:45.000000 cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/SOURCES.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288        1 2023-08-01 15:34:44.000000 cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/dependency_links.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288       90 2023-08-01 15:34:44.000000 cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/entry_points.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288       41 2023-08-01 15:34:44.000000 cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/requires.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288       18 2023-08-01 15:34:45.000000 cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/top_level.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288      358 2023-08-01 15:34:45.541358 cloudgenix_config-2.0.0b2/setup.cfg
+-rw-r--r--   0 tkamath  (1953533316) 192360288     1324 2023-08-01 15:33:54.000000 cloudgenix_config-2.0.0b2/setup.py
```

### Comparing `cloudgenix_config-2.0.0b1/LICENSE` & `cloudgenix_config-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudgenix_config-2.0.0b1/PKG-INFO` & `cloudgenix_config-2.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix_config
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Configuration exporting and Continuous Integration (CI) capable configuration importing for the CloudGenix Cloud Controller.
 Home-page: https://github.com/CloudGenix/cloudgenix_config
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -124,15 +124,16 @@
  - For ION 9000, if trying to configure a bypasspair and the port with the same name (12,13,14,15,16), configuration pushes via do_site have to be done in the following two steps:
      - Include only interface configuration of type port and use the do_site utility to push this configuration first.
      - Update the YAML file to remove the interface configuration of type port, include interface configuration of type bypasspair and use the do_site utiltiy to push the bypasspair configuration.
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
-| **2.0.0** | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
+| **2.0.0** | **b2** |  Bug fixes - CGCBL-1436, CGCBL-1925
+|           | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
 | **1.9.0** | **b2** | Bug fixes - CGCBL-1251, CGCBL-1578|
 |           | **b1** | Support for Cloudgenix SDK 6.1.1b1, bug fixes|
 | **1.8.0** | **b1** | Support for Cloudgenix SDK 6.0.2b1, Fix for CGCBL-1399, CGCBL-1347|
 | **1.7.0** | **b3** | Bug fixes|
 |           | **b2** | Fix for CGCBL-336, #73, #74 and CGESC-700|
 |           | **b1** | Support for CloudGenix SDK 6.0.1b1, bug fixes|
 | **1.6.0** | **b2** | Minor bug fixes |
```

### Comparing `cloudgenix_config-2.0.0b1/README.md` & `cloudgenix_config-2.0.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,16 @@
  - For ION 9000, if trying to configure a bypasspair and the port with the same name (12,13,14,15,16), configuration pushes via do_site have to be done in the following two steps:
      - Include only interface configuration of type port and use the do_site utility to push this configuration first.
      - Update the YAML file to remove the interface configuration of type port, include interface configuration of type bypasspair and use the do_site utiltiy to push the bypasspair configuration.
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
-| **2.0.0** | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
+| **2.0.0** | **b2** |  Bug fixes - CGCBL-1436, CGCBL-1925
+|           | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
 | **1.9.0** | **b2** | Bug fixes - CGCBL-1251, CGCBL-1578|
 |           | **b1** | Support for Cloudgenix SDK 6.1.1b1, bug fixes|
 | **1.8.0** | **b1** | Support for Cloudgenix SDK 6.0.2b1, Fix for CGCBL-1399, CGCBL-1347|
 | **1.7.0** | **b3** | Bug fixes|
 |           | **b2** | Fix for CGCBL-336, #73, #74 and CGESC-700|
 |           | **b1** | Support for CloudGenix SDK 6.0.1b1, bug fixes|
 | **1.6.0** | **b2** | Minor bug fixes |
```

### Comparing `cloudgenix_config-2.0.0b1/cloudgenix_config/__init__.py` & `cloudgenix_config-2.0.0b2/cloudgenix_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Configuration IMPORT/EXPORT common functions
 
-**Version:** 2.0.0b1
+**Version:** 2.0.0b2
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017, 2018 CloudGenix, Inc
 
 **License:** MIT
 
@@ -45,15 +45,15 @@
     binary_type = str
 else:
     text_type = str
     binary_type = bytes
 
 
 # Version for reference
-__version__ = "2.0.0b1"
+__version__ = "2.0.0b2"
 version = __version__
 
 __author__ = "CloudGenix Developer Support <developers@cloudgenix.com>"
 __email__ = "developers@cloudgenix.com"
 __copyright__ = "Copyright (c) 2017, 2018 CloudGenix, Inc"
 __license__ = """
     MIT License
```

### Comparing `cloudgenix_config-2.0.0b1/cloudgenix_config/default_interfaces.py` & `cloudgenix_config-2.0.0b2/cloudgenix_config/default_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Configuration IMPORT/EXPORT default device port configurations
 
-**Version:** 2.0.0b1
+**Version:** 2.0.0b2
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017, 2018 CloudGenix, Inc
 
 **License:** MIT
```

### Comparing `cloudgenix_config-2.0.0b1/cloudgenix_config/do.py` & `cloudgenix_config-2.0.0b2/cloudgenix_config/do.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Configuration IMPORT worker/script
 
-**Version:** 2.0.0b1
+**Version:** 2.0.0b2
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017, 2018 CloudGenix, Inc
 
 **License:** MIT
 
@@ -1625,19 +1625,25 @@
     # Update element template with config changes from cleaned copy
     elem_template.update(config_element_copy)
 
     if elem_template.get('cluster_id'):
         elem_template['cluster_id'] = hubclusters_n2id.get(elem_template['cluster_id'])
 
     # Check for changes in cleaned config copy and cleaned template (will finally detect spoke HA changes here):
-    if spoke_ha_config and reset_spoke_ha and element_change_check.get('spoke_ha_config'):
-        if elem_template.get('spoke_ha_config', {}).get('source_interface') != \
-                element_change_check.get('spoke_ha_config', {}).get('source_interface') or \
-                elem_template.get('spoke_ha_config', {}).get('track', {}) != \
-                element_change_check.get('spoke_ha_config', {}).get('track', {}):
+    if reset_spoke_ha:
+        if element_change_check.get('spoke_ha_config') and elem_template.get('spoke_ha_config'):
+            if elem_template.get('spoke_ha_config', {}).get('source_interface') != \
+                    element_change_check.get('spoke_ha_config', {}).get('source_interface') or \
+                    elem_template.get('spoke_ha_config', {}).get('track', {}) != \
+                    element_change_check.get('spoke_ha_config', {}).get('track', {}):
+                output_message("   Resetting Spoke HA in element {0}.".format(element_descriptive_text))
+                elem_template['spoke_ha_config'] = None
+            else:
+                return 1
+        elif element_change_check.get('spoke_ha_config') and not elem_template.get('spoke_ha_config'):
             output_message("   Resetting Spoke HA in element {0}.".format(element_descriptive_text))
             elem_template['spoke_ha_config'] = None
         else:
             return 1
     elif not force_update and elem_template == element_change_check:
         # no change in config, pass.
         output_message("   No Change for Spoke HA in Element {0}.".format(element_descriptive_text))
```

### Comparing `cloudgenix_config-2.0.0b1/cloudgenix_config/pull.py` & `cloudgenix_config-2.0.0b2/cloudgenix_config/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Configuration EXPORT worker/script
 
-**Version:** 2.0.0b1
+**Version:** 2.0.0b2
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017, 2018 CloudGenix, Inc
 
 **License:** MIT
 
@@ -1735,19 +1735,19 @@
 
                     filter_context_id_list, app_def_id_list = [], []
                     if filter_context.get('ipfixfiltercontext_ids', []):
                         for filter_context_id in filter_context.get('ipfixfiltercontext_ids', []):
                             filter_context_id_list.append(id_name_cache.get(filter_context_id, filter_context_id))
                         if filter_context_id_list:
                             filter_context['ipfixfiltercontext_ids'] = filter_context_id_list
-
-                    for app_def_id in filter_context.get('app_def_ids', []):
-                        app_def_id_list.append(id_name_cache.get(app_def_id, app_def_id))
-                    if app_def_id_list:
-                        filter_context['app_def_ids'] = app_def_id_list
+                    if filter_context.get('app_def_ids'):
+                        for app_def_id in filter_context.get('app_def_ids', []):
+                            app_def_id_list.append(id_name_cache.get(app_def_id, app_def_id))
+                        if app_def_id_list:
+                            filter_context['app_def_ids'] = app_def_id_list
 
             strip_meta_attributes(ipfix_template, leave_name=True)
             # names used, but config doesn't index by name for this value currently.
             element[IPFIX_STR].update(ipfix_template)
         delete_if_empty(element, IPFIX_STR)
 
         # Get toolkit
@@ -1812,14 +1812,16 @@
                                                                            site_id))
         # update id name cache in case name changed.
         id_name_cache[element['id']] = checked_element_name
         site[ELEMENTS_STR][checked_element_name] = element_template
         # as always, sanity check for empty element
         delete_if_empty(site[ELEMENTS_STR], checked_element_name)
 
+    delete_if_empty(site, ELEMENTS_STR)
+
     # prep for add to sites dict
     site_template = copy.deepcopy(site)
 
     # replace flat names
     name_lookup_in_template(site_template, 'policy_set_id', id_name_cache)
     name_lookup_in_template(site_template, 'security_policyset_id', id_name_cache)
     name_lookup_in_template(site_template, 'security_policysetstack_id', id_name_cache)
```

### Comparing `cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/PKG-INFO` & `cloudgenix_config-2.0.0b2/cloudgenix_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix-config
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Configuration exporting and Continuous Integration (CI) capable configuration importing for the CloudGenix Cloud Controller.
 Home-page: https://github.com/CloudGenix/cloudgenix_config
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -124,15 +124,16 @@
  - For ION 9000, if trying to configure a bypasspair and the port with the same name (12,13,14,15,16), configuration pushes via do_site have to be done in the following two steps:
      - Include only interface configuration of type port and use the do_site utility to push this configuration first.
      - Update the YAML file to remove the interface configuration of type port, include interface configuration of type bypasspair and use the do_site utiltiy to push the bypasspair configuration.
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
-| **2.0.0** | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
+| **2.0.0** | **b2** |  Bug fixes - CGCBL-1436, CGCBL-1925
+|           | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
 | **1.9.0** | **b2** | Bug fixes - CGCBL-1251, CGCBL-1578|
 |           | **b1** | Support for Cloudgenix SDK 6.1.1b1, bug fixes|
 | **1.8.0** | **b1** | Support for Cloudgenix SDK 6.0.2b1, Fix for CGCBL-1399, CGCBL-1347|
 | **1.7.0** | **b3** | Bug fixes|
 |           | **b2** | Fix for CGCBL-336, #73, #74 and CGESC-700|
 |           | **b1** | Support for CloudGenix SDK 6.0.1b1, bug fixes|
 | **1.6.0** | **b2** | Minor bug fixes |
```

### Comparing `cloudgenix_config-2.0.0b1/setup.py` & `cloudgenix_config-2.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='cloudgenix_config',
-      version='2.0.0b1',
+      version='2.0.0b2',
       description='Configuration exporting and Continuous Integration (CI) capable configuration importing for the '
                   'CloudGenix Cloud Controller.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/CloudGenix/cloudgenix_config',
       author='CloudGenix Developer Support',
       author_email='developers@cloudgenix.com',
```

