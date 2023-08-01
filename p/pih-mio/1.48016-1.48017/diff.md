# Comparing `tmp/pih-mio-1.48016.tar.gz` & `tmp/pih-mio-1.48017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48016.tar", last modified: Mon Jul 31 08:46:10 2023, max compression
+gzip compressed data, was "pih-mio-1.48017.tar", last modified: Tue Aug  1 02:48:11 2023, max compression
```

## Comparing `pih-mio-1.48016.tar` & `pih-mio-1.48017.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 08:46:09.922616 pih-mio-1.48016/
-drwxrwxrwx   0        0        0        0 2023-07-31 08:46:09.953856 pih-mio-1.48016/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48016/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48016/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-mio-1.48016/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48016/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-mio-1.48016/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48016/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-31 08:46:10.564175 pih-mio-1.48016/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 08:46:10.501675 pih-mio-1.48016/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-31 08:46:08.000000 pih-mio-1.48016/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 08:46:08.000000 pih-mio-1.48016/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48016/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-31 08:46:10.579800 pih-mio-1.48016/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 02:48:10.732291 pih-mio-1.48017/
+drwxrwxrwx   0        0        0        0 2023-08-01 02:48:11.060415 pih-mio-1.48017/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48017/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48017/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-mio-1.48017/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48017/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48017/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48017/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-01 02:48:11.310418 pih-mio-1.48017/PKG-INFO
+-rw-rw-rw-   0        0        0     1624 2023-08-01 02:47:46.000000 pih-mio-1.48017/mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:48:11.279172 pih-mio-1.48017/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-01 02:48:09.000000 pih-mio-1.48017/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-08-01 02:48:10.000000 pih-mio-1.48017/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 02:48:09.000000 pih-mio-1.48017/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-01 02:48:09.000000 pih-mio-1.48017/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 02:48:10.000000 pih-mio-1.48017/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 02:48:10.000000 pih-mio-1.48017/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 02:48:11.326040 pih-mio-1.48017/setup.cfg
```

### Comparing `pih-mio-1.48016/MobileHelperCore/api.py` & `pih-mio-1.48017/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48016/MobileHelperCore/service.py` & `pih-mio-1.48017/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48016/MobileHelperCore/service_api.py` & `pih-mio-1.48017/MobileHelperCore/service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class MobileHelperService():
 
     INIT: bool = False
     INSTANCE: Any | None = None
     NAME: str = "MobileHelper"
    
-    sender_profile_id: A.CT_ME_WH_W.PROFILE = A.ME_WH_W.get_profile_id(A.D_TN.it_administrator())
+    sender_profile_id: A.CT_ME_WH_W.Profiles = A.ME_WH_W.get_profile_id(A.D_TN.it_administrator())
 
     if A.U.update_for_service(ROLE):
         from pih import PIH, Stdin, NotFound, SubscribtionResult
         from pih.tools import ParameterList, BitMask as BM
         from pih.collection import WhatsAppMessage, User
         from MobileHelperCore.api import (MobileHelper as Api, MobileSession, MobileOutput, 
                         MobileInput, MobileUserInput, MobileMarkInput, 
@@ -134,15 +134,15 @@
     def service_call_handler(self, sc: SC, parameter_list: ParameterList, subscribtion_result: SubscribtionResult | None) -> Any:
         if sc == A.CT_SC.send_event:
             if A.D.is_not_none(subscribtion_result) and subscribtion_result.result:
                 if subscribtion_result.type == A.CT_SubT.ON_RESULT_SEQUENTIALLY:
                     message: self.WhatsAppMessage | None = A.D_Ex_E.whatsapp_message(
                         parameter_list)
                     if A.D.is_not_none(message):
-                        if A.D.get_by_value(A.CT_ME_WH_W.PROFILE, message.profile_id) == A.CT_ME_WH_W.PROFILE.IT:
+                        if A.D.get_by_value(A.CT_ME_WH_W.Profiles, message.profile_id) == A.CT_ME_WH_W.Profiles.IT:
                             allow_in_group: bool = not A.D_C.empty(message.chatId) and message.chatId in [A.D.get(A.CT_ME_WH.GROUP.IT)]
                             if A.D.is_none(message.chatId) or allow_in_group:
                                 telephone_number: str = message.chatId if allow_in_group else message.sender
                                 if allow_in_group:
                                     message.chatId = message.sender
                                     message.sender = telephone_number
                                 if A.D.is_none(self.checker) or self.checker(telephone_number):
```

### Comparing `pih-mio-1.48016/MobileHelperCore/tools.py` & `pih-mio-1.48017/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48016/pih_mio_setup.py` & `pih-mio-1.48017/mio_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih import PIH
 from pih.tools import j
 
 #########################################################################################################
 """
-1. python pih_mio_setup.py sdist --dist-dir pih_mio_dist bdist_wheel --dist-dir pih_mio_dist build --build-base pih_mio_build
-2. twine upload --repository pypi pih_mio_dist/*
+1. python mio_setup.py sdist --dist-dir mio_dist bdist_wheel --dist-dir mio_dist build --build-base pih_mio_build
+2. twine upload --repository pypi mio_dist/*
 3. pip install pih_mio -U
 """
-folder = "//pih/facade/pih_mio_dist"
+folder = "//pih/facade/mio_dist"
 for filename in os.listdir(folder):
     file_path = os.path.join(folder, filename)
     try:
         if os.path.isfile(file_path) or os.path.islink(file_path):
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
```

