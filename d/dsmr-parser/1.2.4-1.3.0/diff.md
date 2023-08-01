# Comparing `tmp/dsmr-parser-1.2.4.tar.gz` & `tmp/dsmr-parser-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmr-parser-1.2.4.tar", last modified: Tue Jul 11 20:04:44 2023, max compression
+gzip compressed data, was "dsmr-parser-1.3.0.tar", last modified: Tue Aug  1 07:27:43 2023, max compression
```

## Comparing `dsmr-parser-1.2.4.tar` & `dsmr-parser-1.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/
--rw-r--r--   0 nigel     (1000) nigel     (1000)     1089 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/LICENSE
--rw-r--r--   0 nigel     (1000) nigel     (1000)      269 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/PKG-INFO
--rw-r--r--   0 nigel     (1000) nigel     (1000)    10844 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/README.rst
-drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.146406 dsmr-parser-1.2.4/dsmr_parser/
--rw-r--r--   0 nigel     (1000) nigel     (1000)        0 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/__init__.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     2406 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/__main__.py
-drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.146406 dsmr-parser-1.2.4/dsmr_parser/clients/
--rw-r--r--   0 nigel     (1000) nigel     (1000)      345 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/clients/__init__.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     6147 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/clients/filereader.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     6287 2023-02-12 17:32:14.000000 dsmr-parser-1.2.4/dsmr_parser/clients/protocol.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     2168 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/clients/rfxtrx_protocol.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     4520 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/clients/serial_.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)      639 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/clients/settings.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     2738 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/clients/socket_.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     1543 2023-04-12 08:58:40.000000 dsmr-parser-1.2.4/dsmr_parser/clients/telegram_buffer.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)       89 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/exceptions.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     6268 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/obis_name_mapping.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     6201 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/dsmr_parser/obis_references.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)    11887 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/objects.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)    14128 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/dsmr_parser/parsers.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)      340 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/profile_generic_specifications.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)    19034 2023-07-11 19:56:39.000000 dsmr-parser-1.2.4/dsmr_parser/telegram_specifications.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)      755 2023-02-12 17:32:14.000000 dsmr-parser-1.2.4/dsmr_parser/value_types.py
-drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.146406 dsmr-parser-1.2.4/dsmr_parser.egg-info/
--rw-r--r--   0 nigel     (1000) nigel     (1000)      269 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/PKG-INFO
--rw-r--r--   0 nigel     (1000) nigel     (1000)     1093 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/SOURCES.txt
--rw-r--r--   0 nigel     (1000) nigel     (1000)        1 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/dependency_links.txt
--rw-r--r--   0 nigel     (1000) nigel     (1000)       62 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/entry_points.txt
--rw-r--r--   0 nigel     (1000) nigel     (1000)       72 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/requires.txt
--rw-r--r--   0 nigel     (1000) nigel     (1000)       12 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/top_level.txt
--rw-r--r--   0 nigel     (1000) nigel     (1000)       38 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/setup.cfg
--rw-r--r--   0 nigel     (1000) nigel     (1000)      630 2023-07-11 19:58:20.000000 dsmr-parser-1.2.4/setup.py
-drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/test/
--rw-r--r--   0 nigel     (1000) nigel     (1000)      663 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/test/test_filereader.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)    16710 2023-07-11 19:56:39.000000 dsmr-parser-1.2.4/test/test_parse_fluvius.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     9825 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_iskra_ie.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     4788 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/test/test_parse_sagemcom_t210_d_r.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     4845 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v2_2.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     5305 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v3.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)    13023 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v4_2.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)    14431 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v5.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     2327 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/test/test_protocol.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     2436 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/test/test_rfxtrx_protocol.py
--rw-r--r--   0 nigel     (1000) nigel     (1000)     3535 2023-04-12 08:39:00.000000 dsmr-parser-1.2.4/test/test_telegram_buffer.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-08-01 07:27:43.370122 dsmr-parser-1.3.0/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     1089 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/LICENSE
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      269 2023-08-01 07:27:43.369122 dsmr-parser-1.3.0/PKG-INFO
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    10844 2023-02-19 11:25:41.000000 dsmr-parser-1.3.0/README.rst
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-08-01 07:27:43.368122 dsmr-parser-1.3.0/dsmr_parser/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)        0 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/dsmr_parser/__init__.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2406 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/dsmr_parser/__main__.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-08-01 07:27:43.369122 dsmr-parser-1.3.0/dsmr_parser/clients/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      345 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/dsmr_parser/clients/__init__.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     6147 2023-02-19 11:25:41.000000 dsmr-parser-1.3.0/dsmr_parser/clients/filereader.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     6563 2023-08-01 07:23:53.000000 dsmr-parser-1.3.0/dsmr_parser/clients/protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2168 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/dsmr_parser/clients/rfxtrx_protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     4520 2023-02-19 11:25:41.000000 dsmr-parser-1.3.0/dsmr_parser/clients/serial_.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      639 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/dsmr_parser/clients/settings.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     3069 2023-08-01 07:23:53.000000 dsmr-parser-1.3.0/dsmr_parser/clients/socket_.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     1543 2023-04-12 08:58:40.000000 dsmr-parser-1.3.0/dsmr_parser/clients/telegram_buffer.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       89 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/dsmr_parser/exceptions.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     7424 2023-08-01 07:23:53.000000 dsmr-parser-1.3.0/dsmr_parser/obis_references.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    11785 2023-08-01 07:23:53.000000 dsmr-parser-1.3.0/dsmr_parser/objects.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    14353 2023-08-01 07:23:53.000000 dsmr-parser-1.3.0/dsmr_parser/parsers.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      340 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/dsmr_parser/profile_generic_specifications.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    57291 2023-08-01 07:23:53.000000 dsmr-parser-1.3.0/dsmr_parser/telegram_specifications.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      755 2023-02-12 17:32:14.000000 dsmr-parser-1.3.0/dsmr_parser/value_types.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-08-01 07:27:43.369122 dsmr-parser-1.3.0/dsmr_parser.egg-info/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      269 2023-08-01 07:27:43.000000 dsmr-parser-1.3.0/dsmr_parser.egg-info/PKG-INFO
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     1094 2023-08-01 07:27:43.000000 dsmr-parser-1.3.0/dsmr_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)        1 2023-08-01 07:27:43.000000 dsmr-parser-1.3.0/dsmr_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       62 2023-08-01 07:27:43.000000 dsmr-parser-1.3.0/dsmr_parser.egg-info/entry_points.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       72 2023-08-01 07:27:43.000000 dsmr-parser-1.3.0/dsmr_parser.egg-info/requires.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       12 2023-08-01 07:27:43.000000 dsmr-parser-1.3.0/dsmr_parser.egg-info/top_level.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       38 2023-08-01 07:27:43.370122 dsmr-parser-1.3.0/setup.cfg
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      630 2023-08-01 07:24:37.000000 dsmr-parser-1.3.0/setup.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-08-01 07:27:43.369122 dsmr-parser-1.3.0/test/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      663 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/test/test_filereader.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    16710 2023-07-11 19:56:39.000000 dsmr-parser-1.3.0/test/test_parse_fluvius.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     9825 2023-04-18 18:46:02.000000 dsmr-parser-1.3.0/test/test_parse_iskra_ie.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     4788 2023-01-28 10:18:52.000000 dsmr-parser-1.3.0/test/test_parse_sagemcom_t210_d_r.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     4845 2023-04-18 18:46:02.000000 dsmr-parser-1.3.0/test/test_parse_v2_2.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     5305 2023-04-18 18:46:02.000000 dsmr-parser-1.3.0/test/test_parse_v3.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    13023 2023-04-18 18:46:02.000000 dsmr-parser-1.3.0/test/test_parse_v4_2.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    14525 2023-08-01 07:18:54.000000 dsmr-parser-1.3.0/test/test_parse_v5.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    16926 2023-08-01 07:23:53.000000 dsmr-parser-1.3.0/test/test_parse_v5_eon_hungary.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2327 2023-02-19 11:25:41.000000 dsmr-parser-1.3.0/test/test_protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2436 2023-02-19 11:25:41.000000 dsmr-parser-1.3.0/test/test_rfxtrx_protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     3535 2023-04-12 08:39:00.000000 dsmr-parser-1.3.0/test/test_telegram_buffer.py
```

### Comparing `dsmr-parser-1.2.4/LICENSE` & `dsmr-parser-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/README.rst` & `dsmr-parser-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser/__main__.py` & `dsmr-parser-1.3.0/dsmr_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser/clients/filereader.py` & `dsmr-parser-1.3.0/dsmr_parser/clients/filereader.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser/clients/protocol.py` & `dsmr-parser-1.3.0/dsmr_parser/clients/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 def create_dsmr_protocol(dsmr_version, telegram_callback, loop=None, **kwargs):
     """Creates a DSMR asyncio protocol."""
     protocol = _create_dsmr_protocol(dsmr_version, telegram_callback,
                                      DSMRProtocol, loop, **kwargs)
     return protocol
 
 
-def _create_dsmr_protocol(dsmr_version, telegram_callback, protocol, loop=None, **kwargs):
+# pylama noqa - because of "complex" (too long) if-elif-else.
+# Match - case might be a solution but it is not available in <3.10
+def _create_dsmr_protocol(dsmr_version, telegram_callback, protocol, loop=None, **kwargs): #noqa
     """Creates a DSMR asyncio protocol."""
 
     if dsmr_version == '2.2':
         specification = telegram_specifications.V2_2
         serial_settings = SERIAL_SETTINGS_V2_2
     elif dsmr_version == '4':
         specification = telegram_specifications.V4
@@ -47,14 +49,17 @@
         serial_settings = SERIAL_SETTINGS_V5
     elif dsmr_version == "Q3D":
         specification = telegram_specifications.Q3D
         serial_settings = SERIAL_SETTINGS_V5
     elif dsmr_version == 'ISKRA_IE':
         specification = telegram_specifications.ISKRA_IE
         serial_settings = SERIAL_SETTINGS_V5
+    elif dsmr_version == '5EONHU':
+        specification = telegram_specifications.EON_HUNGARY
+        serial_settings = SERIAL_SETTINGS_V5
     else:
         raise NotImplementedError("No telegram parser found for version: %s",
                                   dsmr_version)
 
     protocol = partial(protocol, loop, TelegramParser(specification),
                        telegram_callback=telegram_callback, **kwargs)
```

### Comparing `dsmr-parser-1.2.4/dsmr_parser/clients/rfxtrx_protocol.py` & `dsmr-parser-1.3.0/dsmr_parser/clients/rfxtrx_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser/clients/serial_.py` & `dsmr-parser-1.3.0/dsmr_parser/clients/serial_.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser/clients/settings.py` & `dsmr-parser-1.3.0/dsmr_parser/clients/settings.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser/clients/socket_.py` & `dsmr-parser-1.3.0/dsmr_parser/clients/socket_.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,15 +39,20 @@
 
                 lines = buffer.splitlines(keepends=True)
 
                 if len(lines) == 0:
                     continue
 
                 for data in lines:
-                    self.telegram_buffer.append(data.decode('ascii'))
+                    try:
+                        self.telegram_buffer.append(data.decode('ascii'))
+                    except UnicodeDecodeError:
+                        # Some garbage came through the channel
+                        # E.g.: Happens at EON_HUNGARY, but only once at the start of the socket.
+                        logger.error('Failed to parse telegram due to unicode decode error')
 
                 for telegram in self.telegram_buffer.get_all():
                     try:
                         yield self.telegram_parser.parse(telegram)
                     except InvalidChecksumError as e:
                         logger.warning(str(e))
                     except ParseError as e:
```

### Comparing `dsmr-parser-1.2.4/dsmr_parser/clients/telegram_buffer.py` & `dsmr-parser-1.3.0/dsmr_parser/clients/telegram_buffer.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser/obis_references.py` & `dsmr-parser-1.3.0/dsmr_parser/obis_references.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 Might be refactored in a backwards incompatible way as soon as proper telegram
 objects are introduced.
 """
 P1_MESSAGE_HEADER = r'^\d-\d:0\.2\.8.+?\r\n'
 P1_MESSAGE_TIMESTAMP = r'^\d-\d:1\.0\.0.+?\r\n'
 ELECTRICITY_USED_TARIFF_1 = r'^\d-\d:1\.8\.1.+?\r\n'
 ELECTRICITY_USED_TARIFF_2 = r'^\d-\d:1\.8\.2.+?\r\n'
+ELECTRICITY_USED_TARIFF_3 = r'^\d-\d:1\.8\.3.+?\r\n'
+ELECTRICITY_USED_TARIFF_4 = r'^\d-\d:1\.8\.4.+?\r\n'
 ELECTRICITY_DELIVERED_TARIFF_1 = r'^\d-\d:2\.8\.1.+?\r\n'
 ELECTRICITY_DELIVERED_TARIFF_2 = r'^\d-\d:2\.8\.2.+?\r\n'
+ELECTRICITY_DELIVERED_TARIFF_3 = r'^\d-\d:2\.8\.3.+?\r\n'
+ELECTRICITY_DELIVERED_TARIFF_4 = r'^\d-\d:2\.8\.4.+?\r\n'
 CURRENT_REACTIVE_IMPORTED = r'^\d-\d:3\.7\.0.+?\r\n'
 ELECTRICITY_REACTIVE_IMPORTED_TOTAL = r'^\d-\d:3\.8\.0.+?\r\n'
 ELECTRICITY_REACTIVE_IMPORTED_TARIFF_1 = r'^\d-\d:3\.8\.1.+?\r\n'
 ELECTRICITY_REACTIVE_IMPORTED_TARIFF_2 = r'^\d-\d:3\.8\.2.+?\r\n'
 CURRENT_REACTIVE_EXPORTED = r'^\d-\d:4\.7\.0.+?\r\n'
 ELECTRICITY_REACTIVE_EXPORTED_TOTAL = r'^\d-\d:4\.8\.0.+?\r\n'
 ELECTRICITY_REACTIVE_EXPORTED_TARIFF_1 = r'^\d-\d:4\.8\.1.+?\r\n'
@@ -118,7 +122,25 @@
 
 
 LUXEMBOURG_EQUIPMENT_IDENTIFIER = r'^\d-\d:42\.0\.0.+?\r\n'  # Logical device name
 
 Q3D_EQUIPMENT_IDENTIFIER = r'^\d-\d:0\.0\.0.+?\r\n'  # Logical device name
 Q3D_EQUIPMENT_STATE = r'^\d-\d:96\.5\.5.+?\r\n'  # Device state (hexadecimal)
 Q3D_EQUIPMENT_SERIALNUMBER = r'^\d-\d:96\.1\.255.+?\r\n'  # Device Serialnumber
+
+# EON Hungary
+EON_HU_ELECTRICITY_REACTIVE_TOTAL_Q1 = r'^\d-\d:5\.8\.0.+?\r\n'
+EON_HU_ELECTRICITY_REACTIVE_TOTAL_Q2 = r'^\d-\d:6\.8\.0.+?\r\n'
+EON_HU_ELECTRICITY_REACTIVE_TOTAL_Q3 = r'^\d-\d:7\.8\.0.+?\r\n'
+EON_HU_ELECTRICITY_REACTIVE_TOTAL_Q4 = r'^\d-\d:8\.8\.0.+?\r\n'
+EON_HU_ELECTRICITY_COMBINED = r'^\d-\d:15\.8\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_POWER_FACTOR_TOTAL = r'^\d-\d:13\.7\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_POWER_FACTOR_L1 = r'^\d-\d:33\.7\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_POWER_FACTOR_L2 = r'^\d-\d:53\.7\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_POWER_FACTOR_L3 = r'^\d-\d:73\.7\.0.+?\r\n'
+EON_HU_FREQUENCY = r'^\d-\d:14\.7\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_REACTIVE_POWER_Q1 = r'^\d-\d:5\.7\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_REACTIVE_POWER_Q2 = r'^\d-\d:6\.7\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_REACTIVE_POWER_Q3 = r'^\d-\d:7\.7\.0.+?\r\n'
+EON_HU_INSTANTANEOUS_REACTIVE_POWER_Q4 = r'^\d-\d:8\.7\.0.+?\r\n'
+EON_HU_MAX_POWER_ON_L2 = r'^\d-\d:51\.4\.0.+?\r\n'
+EON_HU_MAX_POWER_ON_L3 = r'^\d-\d:71\.4\.0.+?\r\n'
```

### Comparing `dsmr-parser-1.2.4/dsmr_parser/objects.py` & `dsmr-parser-1.3.0/dsmr_parser/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from decimal import Decimal
 
 import datetime
 import json
 
 import pytz
 
-from dsmr_parser import obis_name_mapping
-
 
 class Telegram(dict):
     """
     Container for parsed telegram data.
 
     Attributes can be accessed on a telegram object by addressing by their english name, for example:
         telegram.ELECTRICITY_USED_TARIFF_1
@@ -23,43 +21,42 @@
     Note: Dict like usage is deprecated. The inheritance from dict is because of backwards compatibility.
     """
     def __init__(self, *args, **kwargs):
         self._item_names = []
         self._mbus_devices = []
         super().__init__(*args, **kwargs)
 
-    def add(self, obis_reference, dsmr_object):
+    def add(self, obis_reference, dsmr_object, obis_name):
         # Update name mapping used to get value by attribute. Example: telegram.P1_MESSAGE_HEADER
-        obis_name = obis_name_mapping.EN[obis_reference]
         setattr(self, obis_name, dsmr_object)
         if obis_name not in self._item_names:  # TODO repeating obis references
             self._item_names.append(obis_name)
 
         # TODO isinstance check: MaxDemandParser (BELGIUM_MAXIMUM_DEMAND_13_MONTHS) returns a list
         if isinstance(dsmr_object, DSMRObject) and dsmr_object.is_mbus_reading:
-            self._add_mbus(obis_reference, dsmr_object)
+            self._add_mbus(obis_reference, dsmr_object, obis_name)
 
         # Fill dict which is only used for backwards compatibility
         if obis_reference not in self:
             self[obis_reference] = dsmr_object
 
-    def _add_mbus(self, obis_reference, dsmr_object):
+    def _add_mbus(self, obis_reference, dsmr_object, obis_name):
         """
         The given DsmrObject is assumed to be Mbus related and will be grouped into a MbusDevice.
         Grouping is done by the DsmrObject channel ID.
         """
         channel_id = dsmr_object.obis_id_code[1]
 
         # Create new MbusDevice or update existing one as it's records are being added one by one.
         mbus_device = self.get_mbus_device_by_channel(channel_id)
         if not mbus_device:
             mbus_device = MbusDevice(channel_id=channel_id)
             self._mbus_devices.append(mbus_device)
 
-        mbus_device.add(obis_reference, dsmr_object)
+        mbus_device.add(obis_reference, dsmr_object, obis_name)
 
         if not hasattr(self, 'MBUS_DEVICES'):
             setattr(self, 'MBUS_DEVICES', self._mbus_devices)
             self._item_names.append('MBUS_DEVICES')
 
     def get_mbus_device_by_channel(self, channel_id):
         """
@@ -327,18 +324,17 @@
     This object is similar to the Telegram except that it only contains readings related to the same mbus device.
     """
 
     def __init__(self, channel_id):
         self.channel_id = channel_id
         self._item_names = []
 
-    def add(self, obis_reference, dsmr_object):
+    def add(self, obis_reference, dsmr_object, obis_name):
         # Update name mapping used to get value by attribute. Example: telegram.P1_MESSAGE_HEADER
         # Also keep track of the added names internally
-        obis_name = obis_name_mapping.EN[obis_reference]
         setattr(self, obis_name, dsmr_object)
         self._item_names.append(obis_name)
 
     def __len__(self):
         return len(self._item_names)
 
     def __iter__(self):
```

### Comparing `dsmr-parser-1.2.4/dsmr_parser/parsers.py` & `dsmr-parser-1.3.0/dsmr_parser/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             telegram DSMR version (v4 and up).
         :type telegram_specification: dict
         """
         self.apply_checksum_validation = apply_checksum_validation
         self.telegram_specification = telegram_specification
         # Regexes are compiled once to improve performance
         self.telegram_specification_regexes = {
-            signature: re.compile(signature, re.DOTALL | re.MULTILINE)
-            for signature in self.telegram_specification['objects'].keys()
+            object["obis_reference"]: re.compile(object["obis_reference"], re.DOTALL | re.MULTILINE)
+            for object in self.telegram_specification['objects']
         }
 
     def parse(self, telegram_data, encryption_key="", authentication_key="", throw_ex=False):  # noqa: C901
         """
         Parse telegram from string to dict.
         The telegram str type makes python 2.x integration easier.
 
@@ -80,33 +80,39 @@
                 pass
 
         if self.apply_checksum_validation and self.telegram_specification['checksum_support']:
             self.validate_checksum(telegram_data)
 
         telegram = Telegram()
 
-        for signature, parser in self.telegram_specification['objects'].items():
-            pattern = self.telegram_specification_regexes[signature]
+        for object in self.telegram_specification['objects']:
+            pattern = self.telegram_specification_regexes[object["obis_reference"]]
             matches = pattern.findall(telegram_data)
 
             # Some signatures are optional and may not be present,
             # so only parse lines that match
             for match in matches:
                 try:
-                    dsmr_object = parser.parse(match)
+                    dsmr_object = object["value_parser"].parse(match)
                 except ParseError:
-                    logger.error("ignore line with signature {}, because parsing failed.".format(signature),
-                                 exc_info=True)
+                    logger.error(
+                        "ignore line with signature {}, because parsing failed.".format(object["obis_reference"]),
+                        exc_info=True
+                    )
                     if throw_ex:
                         raise
                 except Exception as err:
                     logger.error("Unexpected {}: {}".format(type(err), err))
                     raise
                 else:
-                    telegram.add(obis_reference=signature, dsmr_object=dsmr_object)
+                    telegram.add(
+                        obis_reference=object["obis_reference"],
+                        dsmr_object=dsmr_object,
+                        obis_name=object["value_name"]
+                    )
 
         return telegram
 
     @staticmethod
     def validate_checksum(telegram):
         """
         :param str telegram:
```

### Comparing `dsmr-parser-1.2.4/dsmr_parser/value_types.py` & `dsmr-parser-1.3.0/dsmr_parser/value_types.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/dsmr_parser.egg-info/SOURCES.txt` & `dsmr-parser-1.3.0/dsmr_parser.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.rst
 setup.py
 dsmr_parser/__init__.py
 dsmr_parser/__main__.py
 dsmr_parser/exceptions.py
-dsmr_parser/obis_name_mapping.py
 dsmr_parser/obis_references.py
 dsmr_parser/objects.py
 dsmr_parser/parsers.py
 dsmr_parser/profile_generic_specifications.py
 dsmr_parser/telegram_specifications.py
 dsmr_parser/value_types.py
 dsmr_parser.egg-info/PKG-INFO
@@ -29,10 +28,11 @@
 test/test_parse_fluvius.py
 test/test_parse_iskra_ie.py
 test/test_parse_sagemcom_t210_d_r.py
 test/test_parse_v2_2.py
 test/test_parse_v3.py
 test/test_parse_v4_2.py
 test/test_parse_v5.py
+test/test_parse_v5_eon_hungary.py
 test/test_protocol.py
 test/test_rfxtrx_protocol.py
 test/test_telegram_buffer.py
```

### Comparing `dsmr-parser-1.2.4/setup.py` & `dsmr-parser-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(
     name='dsmr-parser',
     description='Library to parse Dutch Smart Meter Requirements (DSMR)',
     author='Nigel Dokter and many others',
     author_email='mail@nldr.net',
     license='MIT',
     url='https://github.com/ndokter/dsmr_parser',
-    version='1.2.4',
+    version='1.3.0',
     packages=find_packages(exclude=('test', 'test.*')),
     install_requires=[
         'pyserial>=3,<4',
         'pyserial-asyncio<1',
         'pytz',
         'Tailer==0.4.1',
         'dlms_cosem==21.3.2'
```

### Comparing `dsmr-parser-1.2.4/test/test_filereader.py` & `dsmr-parser-1.3.0/test/test_filereader.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_parse_fluvius.py` & `dsmr-parser-1.3.0/test/test_parse_fluvius.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_parse_iskra_ie.py` & `dsmr-parser-1.3.0/test/test_parse_iskra_ie.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_parse_sagemcom_t210_d_r.py` & `dsmr-parser-1.3.0/test/test_parse_sagemcom_t210_d_r.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_parse_v2_2.py` & `dsmr-parser-1.3.0/test/test_parse_v2_2.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_parse_v3.py` & `dsmr-parser-1.3.0/test/test_parse_v3.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_parse_v4_2.py` & `dsmr-parser-1.3.0/test/test_parse_v4_2.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_parse_v5.py` & `dsmr-parser-1.3.0/test/test_parse_v5.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def test_parse(self):
         parser = TelegramParser(telegram_specifications.V5)
         try:
             telegram = parser.parse(TELEGRAM_V5, throw_ex=True)
         except Exception as ex:
             assert False, f"parse trigged an exception {ex}"
-
+        print('test: ', type(telegram.P1_MESSAGE_HEADER), telegram.P1_MESSAGE_HEADER.__dict__)
         # P1_MESSAGE_HEADER (1-3:0.2.8)
         assert isinstance(telegram.P1_MESSAGE_HEADER, CosemObject)
         assert telegram.P1_MESSAGE_HEADER.unit is None
         assert isinstance(telegram.P1_MESSAGE_HEADER.value, str)
         assert telegram.P1_MESSAGE_HEADER.value == '50'
 
         # P1_MESSAGE_TIMESTAMP (0-0:1.0.0)
```

### Comparing `dsmr-parser-1.2.4/test/test_protocol.py` & `dsmr-parser-1.3.0/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_rfxtrx_protocol.py` & `dsmr-parser-1.3.0/test/test_rfxtrx_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.4/test/test_telegram_buffer.py` & `dsmr-parser-1.3.0/test/test_telegram_buffer.py`

 * *Files identical despite different names*

