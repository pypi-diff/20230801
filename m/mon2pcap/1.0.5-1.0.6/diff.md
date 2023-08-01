# Comparing `tmp/mon2pcap-1.0.5.tar.gz` & `tmp/mon2pcap-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mon2pcap-1.0.5.tar", max compression
+gzip compressed data, was "mon2pcap-1.0.6.tar", max compression
```

## Comparing `mon2pcap-1.0.5.tar` & `mon2pcap-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.5/LICENSE
--rw-r--r--   0        0        0     3378 2023-06-05 14:39:35.620745 mon2pcap-1.0.5/README.md
--rw-r--r--   0        0        0      230 2023-06-05 07:10:39.716916 mon2pcap-1.0.5/mon2pcap/__init__.py
--rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.5/mon2pcap/common.py
--rw-r--r--   0        0        0     2850 2023-06-04 11:23:50.048354 mon2pcap-1.0.5/mon2pcap/console.py
--rw-r--r--   0        0        0     3261 2023-06-05 14:05:37.872613 mon2pcap-1.0.5/mon2pcap/constants.py
--rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.5/mon2pcap/errors.py
--rw-r--r--   0        0        0     1928 2023-06-04 10:03:27.787298 mon2pcap-1.0.5/mon2pcap/helpers.py
--rw-r--r--   0        0        0     7537 2023-06-05 14:36:44.763690 mon2pcap-1.0.5/mon2pcap/mon2pcap.py
--rw-r--r--   0        0        0    60553 2023-06-05 14:29:47.705500 mon2pcap-1.0.5/mon2pcap/packets.py
--rw-r--r--   0        0        0     1017 2023-06-05 14:37:31.916503 mon2pcap-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 mon2pcap-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.6/LICENSE
+-rw-r--r--   0        0        0     3414 2023-06-06 07:07:44.299547 mon2pcap-1.0.6/README.md
+-rw-r--r--   0        0        0      230 2023-06-05 07:10:39.716916 mon2pcap-1.0.6/mon2pcap/__init__.py
+-rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.6/mon2pcap/common.py
+-rw-r--r--   0        0        0     2850 2023-06-04 11:23:50.048354 mon2pcap-1.0.6/mon2pcap/console.py
+-rw-r--r--   0        0        0     3261 2023-06-05 14:05:37.872613 mon2pcap-1.0.6/mon2pcap/constants.py
+-rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.6/mon2pcap/errors.py
+-rw-r--r--   0        0        0     1893 2023-08-01 21:34:26.261970 mon2pcap-1.0.6/mon2pcap/helpers.py
+-rw-r--r--   0        0        0     7537 2023-08-01 21:35:32.691800 mon2pcap-1.0.6/mon2pcap/mon2pcap.py
+-rw-r--r--   0        0        0    60553 2023-06-05 14:29:47.705500 mon2pcap-1.0.6/mon2pcap/packets.py
+-rw-r--r--   0        0        0     1017 2023-08-01 21:45:34.698798 mon2pcap-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4375 1970-01-01 00:00:00.000000 mon2pcap-1.0.6/PKG-INFO
```

### Comparing `mon2pcap-1.0.5/LICENSE` & `mon2pcap-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.5/README.md` & `mon2pcap-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,9 +85,12 @@
   - `RANAP      (56)` OFF by default
   - `BSSGP      (59)` OFF by default
   - `TCAP       (54)` OFF by default
   - `SCCP       (53)` OFF by default
   - `SLS        (94)` ON  by default
   - `SCTP       (51)` OFF by default
 
+## Changelog
+[CHANGELOG](CHANGELOG.md)
+
 ## License
-[GPLv3]('./LICENSE')
+[GPLv3](LICENSE)
```

### Comparing `mon2pcap-1.0.5/mon2pcap/console.py` & `mon2pcap-1.0.6/mon2pcap/console.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.5/mon2pcap/constants.py` & `mon2pcap-1.0.6/mon2pcap/constants.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.5/mon2pcap/helpers.py` & `mon2pcap-1.0.6/mon2pcap/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     num = 0
     for lnum, line in enumerate(file, 1):
         try:
             line = line.replace("\t", "    ").replace(
                 "\x00", ""
             )  # replace `NUL` character seen in some files
             if not line.strip():
-                chunk.append(line)
                 continue
             if line.strip().split()[0] in days_of_week and num > 2:
                 num = 0
                 yield chunk
                 chunk.clear()
             if line.strip().split()[0] in days_of_week and num == 0:
                 num += 1
```

### Comparing `mon2pcap-1.0.5/mon2pcap/mon2pcap.py` & `mon2pcap-1.0.6/mon2pcap/mon2pcap.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.5/mon2pcap/packets.py` & `mon2pcap-1.0.6/mon2pcap/packets.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.5/pyproject.toml` & `mon2pcap-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mon2pcap"
-version = "1.0.5"
+version = "1.0.6"
 description = "Convert StarOS \"monitor subscriber\" or \"monitor protocol\" ASCII dump to PCAP"
 authors = ["Artur Russu <arussu@cisco.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/arussu/mon2pcap"
 keywords = ["scapy", "mon2pcap"]
 classifiers = [
```

### Comparing `mon2pcap-1.0.5/PKG-INFO` & `mon2pcap-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mon2pcap
-Version: 1.0.5
+Version: 1.0.6
 Summary: Convert StarOS "monitor subscriber" or "monitor protocol" ASCII dump to PCAP
 Home-page: https://github.com/arussu/mon2pcap
 License: GPL-3.0-only
 Keywords: scapy,mon2pcap
 Author: Artur Russu
 Author-email: arussu@cisco.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -109,10 +109,13 @@
   - `RANAP      (56)` OFF by default
   - `BSSGP      (59)` OFF by default
   - `TCAP       (54)` OFF by default
   - `SCCP       (53)` OFF by default
   - `SLS        (94)` ON  by default
   - `SCTP       (51)` OFF by default
 
+## Changelog
+[CHANGELOG](CHANGELOG.md)
+
 ## License
-[GPLv3]('./LICENSE')
+[GPLv3](LICENSE)
```

