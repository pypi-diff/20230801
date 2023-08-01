# Comparing `tmp/pih-mio-1.48017.tar.gz` & `tmp/pih-mio-1.48020.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48017.tar", last modified: Tue Aug  1 02:48:11 2023, max compression
+gzip compressed data, was "pih-mio-1.48020.tar", last modified: Tue Aug  1 02:58:53 2023, max compression
```

## Comparing `pih-mio-1.48017.tar` & `pih-mio-1.48020.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:48:10.732291 pih-mio-1.48017/
-drwxrwxrwx   0        0        0        0 2023-08-01 02:48:11.060415 pih-mio-1.48017/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48017/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48017/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-mio-1.48017/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48017/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48017/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48017/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-01 02:48:11.310418 pih-mio-1.48017/PKG-INFO
--rw-rw-rw-   0        0        0     1624 2023-08-01 02:47:46.000000 pih-mio-1.48017/mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:48:11.279172 pih-mio-1.48017/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-01 02:48:09.000000 pih-mio-1.48017/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-08-01 02:48:10.000000 pih-mio-1.48017/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:48:09.000000 pih-mio-1.48017/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-01 02:48:09.000000 pih-mio-1.48017/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-01 02:48:10.000000 pih-mio-1.48017/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 02:48:10.000000 pih-mio-1.48017/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 02:48:11.326040 pih-mio-1.48017/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 02:58:52.647787 pih-mio-1.48020/
+drwxrwxrwx   0        0        0        0 2023-08-01 02:58:48.551481 pih-mio-1.48020/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48020/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48020/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165321 2023-08-01 02:56:27.000000 pih-mio-1.48020/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48020/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48020/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48020/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-01 02:58:52.616531 pih-mio-1.48020/PKG-INFO
+-rw-rw-rw-   0        0        0     1624 2023-08-01 02:47:46.000000 pih-mio-1.48020/mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:58:52.330303 pih-mio-1.48020/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-01 02:58:37.000000 pih-mio-1.48020/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-08-01 02:58:39.000000 pih-mio-1.48020/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 02:58:37.000000 pih-mio-1.48020/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-01 02:58:38.000000 pih-mio-1.48020/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 02:58:38.000000 pih-mio-1.48020/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 02:58:38.000000 pih-mio-1.48020/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 02:58:52.694652 pih-mio-1.48020/setup.cfg
```

### Comparing `pih-mio-1.48017/MobileHelperCore/api.py` & `pih-mio-1.48020/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         self.message_buffer: list[MessageHolder] = []
         self.thread_started: bool = False
         self.session = session
         self.session.output = self
         self.type: int = 0
         self.instant_mode: bool = False
         self.recipient: str | None = None
-        self.profile: int = A.CT.MESSAGE.WHATSAPP.WAPPI.PROFILE.IT
+        self.profile: int = A.CT.MESSAGE.WHATSAPP.WAPPI.Profiles.IT
         self.flags = 0
 
 
     def color_str(self, color: int, text: str, text_before: str | None = None, text_after: str | None = None) -> str:
         return text
 
     def whatsapp_send(self, text: str) -> bool:
```

### Comparing `pih-mio-1.48017/MobileHelperCore/service.py` & `pih-mio-1.48020/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48017/MobileHelperCore/service_api.py` & `pih-mio-1.48020/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48017/MobileHelperCore/tools.py` & `pih-mio-1.48020/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48017/mio_setup.py` & `pih-mio-1.48020/mio_setup.py`

 * *Files identical despite different names*

