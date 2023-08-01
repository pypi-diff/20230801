# Comparing `tmp/macrometa-target-mongo-0.0.9.tar.gz` & `tmp/macrometa-target-mongo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mongo-0.0.9.tar", max compression
+gzip compressed data, was "macrometa-target-mongo-1.0.0.tar", max compression
```

## Comparing `macrometa-target-mongo-0.0.9.tar` & `macrometa-target-mongo-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    32393 2023-02-07 07:10:24.954189 macrometa-target-mongo-0.0.9/LICENSE
--rw-r--r--   0        0        0     6076 2023-02-07 07:10:24.954189 macrometa-target-mongo-0.0.9/macrometa_target_mongo/__init__.py
--rw-r--r--   0        0        0     9350 2023-02-07 07:10:24.954189 macrometa-target-mongo-0.0.9/macrometa_target_mongo/main.py
--rw-r--r--   0        0        0     1591 2023-02-07 07:10:25.198192 macrometa-target-mongo-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 macrometa-target-mongo-0.0.9/setup.py
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 macrometa-target-mongo-0.0.9/PKG-INFO
+-rwxr-xr-x   0        0        0    11905 2023-08-01 08:30:17.813788 macrometa-target-mongo-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7479 2023-08-01 08:30:17.813788 macrometa-target-mongo-1.0.0/macrometa_target_mongo/__init__.py
+-rw-r--r--   0        0        0    17446 2023-08-01 08:30:17.813788 macrometa-target-mongo-1.0.0/macrometa_target_mongo/main.py
+-rw-r--r--   0        0        0     1622 2023-08-01 08:30:18.061787 macrometa-target-mongo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 macrometa-target-mongo-1.0.0/setup.py
+-rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 macrometa-target-mongo-1.0.0/PKG-INFO
```

### Comparing `macrometa-target-mongo-0.0.9/macrometa_target_mongo/__init__.py` & `macrometa-target-mongo-1.0.0/macrometa_target_mongo/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -44,33 +44,37 @@
         """Fetch sample data using the given configurations."""
         return []
 
     def schemas(self, integration: dict) -> list[Schema]:
         """Get supported schemas using the given configurations."""
         return []
 
+    def reserved_keys(self) -> list[str]:
+        """List of reserved keys for the connector."""
+        return []
+
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('host', 'Host', ConfigAttributeType.STRING, True, False,
                            description='MongoDB host.',
                            placeholder_value='mongodb_host'),
             ConfigProperty('port', 'Port', ConfigAttributeType.INT, False, False,
                            description='MongoDB port.',
                            default_value='27017'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='MongoDB user.',
                            placeholder_value='mongo'),
-            ConfigProperty('password', 'Password', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='MongoDB password.',
                            placeholder_value='password'),
             ConfigProperty('auth_database', 'Auth Database', ConfigAttributeType.STRING, True, False,
                            description='MongoDB authentication database.',
                            default_value='admin'),
-            ConfigProperty('database', 'Database', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('database', 'Database', ConfigAttributeType.STRING, True, True,
                            description='MongoDB database name.',
                            placeholder_value='mongo'),
             ConfigProperty('target_collection', 'Target Collection', ConfigAttributeType.STRING, True, True,
                            description="Target collection name.",
                            placeholder_value='my_collection'),
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When `hard_delete` option is true then the documents which are deleted from '
@@ -90,17 +94,29 @@
                            default_value='false'),
             ConfigProperty('ssl', 'Use SSL', ConfigAttributeType.BOOLEAN, False, False,
                            description='Can be set to true to connect using SSL.',
                            default_value='false'),
             ConfigProperty('verify_mode', 'Verify Mode', ConfigAttributeType.BOOLEAN, False, False,
                            description='Default SSL verify mode.',
                            default_value='true'),
+            ConfigProperty('tls_ca_file', 'SSL/TLS CA Certificate', ConfigAttributeType.FILE, False, False,
+                           description='Specific CA certificate in PEM string format. This is most often the case '
+                                       'when using `self-signed` server certificate.',
+                           placeholder_value="my_ca_certificate"),
+            ConfigProperty('tls_certificate_key_file', 'SSL/TLS Client Certificate', ConfigAttributeType.FILE, False, False,
+                           description='Specific client certificate in PEM string format. If the private key for the client '
+                                       'certificate is stored in a separate file, it should be concatenated with the certificate file.',
+                           placeholder_value="my_client_certificate"),
+            ConfigProperty('tls_certificate_key_file_password', 'SSL/TLS Client Key Password', ConfigAttributeType.PASSWORD, False, False,
+                           description='If the private key contained in the certificate keyfile is encrypted, users can provide a '
+                                       'password or passphrase to decrypt the encrypted private keys.',
+                           placeholder_value="my_client_key_password"),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows inserted per batch.',
-                           default_value='50'),
+                           default_value='1000'),
             ConfigProperty('batch_flush_interval', 'Batch Flush Interval (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Time between batch flush executions.',
                            default_value='60'),
             ConfigProperty('batch_flush_min_time_gap', 'Batch Flush Minimum Time Gap (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Minimum time gap between two batch flush tasks.',
```

### Comparing `macrometa-target-mongo-0.0.9/pyproject.toml` & `macrometa-target-mongo-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core==1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mongo"
-version='0.0.9'
+version='1.0.0'
 description = "Macrometa connector for writing data into MongoDB, can be used as a target for any Data Mesh Integration."
 license = "Apache-2.0"
 authors = ["Macrometa <product@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -25,17 +25,18 @@
     { include = "macrometa_target_mongo" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 requests = "^2.25.1"
 pipelinewise-singer-python = "1.2.0"
-c8connector = "0.0.14"
+c8connector = ">=0.0.29"
 pymongo = {version = "^4.0",extras = ["srv"]}
 adjust-precision-for-schema = "0.3.4"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 macrometa-target-mongo = "macrometa_target_mongo.main:main"
 
 [tool.poetry.urls]
 "Homepage" = "https://www.macrometa.com/"
 "Bug Tracker" = "https://github.com/Macrometacorp/macrometa-target-mongo/issues"
```

### Comparing `macrometa-target-mongo-0.0.9/setup.py` & `macrometa-target-mongo-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 ['macrometa_target_mongo']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['adjust-precision-for-schema==0.3.4',
- 'c8connector==0.0.14',
+ 'c8connector>=0.0.29',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'pymongo[srv]>=4.0,<5.0',
  'requests>=2.25.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mongo = '
                      'macrometa_target_mongo.main:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mongo',
-    'version': '0.0.9',
+    'version': '1.0.0',
     'description': 'Macrometa connector for writing data into MongoDB, can be used as a target for any Data Mesh Integration.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'product@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mongo-0.0.9/PKG-INFO` & `macrometa-target-mongo-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mongo
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa connector for writing data into MongoDB, can be used as a target for any Data Mesh Integration.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MongoDB
 Author: Macrometa
 Author-email: product@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: adjust-precision-for-schema (==0.3.4)
-Requires-Dist: c8connector (==0.0.14)
+Requires-Dist: c8connector (>=0.0.29)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pymongo[srv] (>=4.0,<5.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-target-mongo/issues
 Project-URL: Homepage, https://www.macrometa.com/
```

