# Comparing `tmp/async_nec_beamer-0.2.0.tar.gz` & `tmp/async_nec_beamer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_nec_beamer-0.2.0.tar", last modified: Mon Jul 31 12:22:24 2023, max compression
+gzip compressed data, was "async_nec_beamer-0.2.1.tar", last modified: Tue Aug  1 09:58:26 2023, max compression
```

## Comparing `async_nec_beamer-0.2.0.tar` & `async_nec_beamer-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/async_nec_beamer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/async_nec_beamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19795 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/async_nec_beamer/nec_beamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:22:23.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/bin/async_nec_beamer
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:58:26.463853 async_nec_beamer-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 09:58:14.000000 async_nec_beamer-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-01 09:58:26.463853 async_nec_beamer-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-01 09:58:14.000000 async_nec_beamer-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:58:26.463853 async_nec_beamer-0.2.1/async_nec_beamer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 09:58:14.000000 async_nec_beamer-0.2.1/async_nec_beamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-08-01 09:58:14.000000 async_nec_beamer-0.2.1/async_nec_beamer/nec_beamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:58:26.463853 async_nec_beamer-0.2.1/async_nec_beamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-01 09:58:26.000000 async_nec_beamer-0.2.1/async_nec_beamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 09:58:26.000000 async_nec_beamer-0.2.1/async_nec_beamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:58:26.000000 async_nec_beamer-0.2.1/async_nec_beamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:58:26.000000 async_nec_beamer-0.2.1/async_nec_beamer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 09:58:26.000000 async_nec_beamer-0.2.1/async_nec_beamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 09:58:26.000000 async_nec_beamer-0.2.1/async_nec_beamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:58:26.463853 async_nec_beamer-0.2.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-08-01 09:58:14.000000 async_nec_beamer-0.2.1/bin/async_nec_beamer
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:58:26.463853 async_nec_beamer-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-01 09:58:14.000000 async_nec_beamer-0.2.1/setup.py
```

### Comparing `async_nec_beamer-0.2.0/LICENSE` & `async_nec_beamer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_nec_beamer-0.2.0/PKG-INFO` & `async_nec_beamer-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_nec_beamer
-Version: 0.2.0
+Version: 0.2.1
 Summary: NEC Beamer Web Interface Wrapper (Async)
 Home-page: https://github.com/heinrich-foto/async_nec_beamer
 Author: Heinrich-Foto
 Author-email: async_nec_beamer@heinrich-foto.de
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `async_nec_beamer-0.2.0/async_nec_beamer/nec_beamer.py` & `async_nec_beamer-0.2.1/async_nec_beamer/nec_beamer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 #!/usr/bin/env python
-
+import inspect
+import ipaddress
 import logging
 import re
 from datetime import datetime
 import json as json_lib
 
 import aiohttp
 import asyncio
 
 _logger = logging.getLogger("async_nec_beamer")
 # Default values for the NEC Beamer
 NAME = "NEC Beamer"
 IP_ADDRESS = "192.168.0.175"
+TIMEOUT = 5*60  # 5 minutes
+
+
+class DummyResponse:
+    def __init__(self, status):
+        self.status = status
 
 
 class Nec_Beamer:
-    def __init__(self, ip_address, name) -> None:
+    def __init__(self, ip_address=IP_ADDRESS, name=NAME, timeout=TIMEOUT) -> None:
+        # check if ip_address is a valid IP Address (v4 and v6)
+        if not ipaddress.ip_address(ip_address):
+            raise ValueError("ip_address is not a valid IP Address")
+        # check if name is a string
+        if not isinstance(name, str):
+            raise ValueError("name is not a string")
+        # check if timeout is an integer
+        if not isinstance(timeout, int) and timeout >= 0:
+            raise ValueError("timeout is not an integer")
 
-        self._ip_address = ip_address if ip_address else IP_ADDRESS
+        self._ip_address = ip_address
+        self._timeout = aiohttp.ClientTimeout(total=timeout)
         self._is_on = False
-        self._name = name if isinstance(name, str) else "NEC Beamer"
+        self._name = name
         self._is_available = False
         self._lamp_life_remaining = 0  # top.statusF.document.stat.textfield.value='81';
         self._lamp_hours = 0  # top.statusF.document.stat.textfield2.value='0390';
         self._filter_hours = 0  # top.statusF.document.stat.textfield4.value='0396';
-        self._projektor_hours_used = (
-            0  # top.statusF.document.stat.textfield6.value='0019';
-        )
+        self._message_error_status = ""  # top.statusF.document.stat.textfield5.value='0000';
+        self._projektor_hours_used = 0  # top.statusF.document.stat.textfield6.value='0019';
+
         self.__json = False
 
         self._muted = {
             "snd": False,
             "pic": False,
             "osd": False,
         }
@@ -93,39 +110,59 @@
             _logger.error(f"Command %s not found", command)
             return
         _logger.info(f"Sending command to NEC Beamer: %s", command)
         command = self._commands[command] if command in self._commands else command
         url = f"http://{self._ip_address}{command}"
         _logger.info(f"with this URL: %s", url)
 
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as response:
-                _logger.debug("Response Status: %s", response.status)
-                _logger.debug("Response Headers: %s", response.headers)
-                html = await response.text()
-                # response = requests.get(url, timeout=5)
-                _logger.debug(f"Response from NEC Beamer: %s", html[:15])
-
+        try:
+            async with aiohttp.ClientSession(timeout=self._timeout) as session:
+                async with session.get(url) as response:
+                    _logger.debug("Response Status: %s", response.status)
+                    _logger.debug("Response Headers: %s", response.headers)
+                    html = await response.text()
+                    # response = requests.get(url, timeout=5)
+                    _logger.debug(f"Response from NEC Beamer: %s", html[:15])
+        except (aiohttp.ServerTimeoutError, aiohttp.ClientConnectorError) as e:
+            _logger.error(f"Connection timed out: %s", e)
+            # AttributeError: 'NoneType' object has no attribute 'status'
+            # create a dummy response object with only a status attribute
+            response = DummyResponse(status=408)
+            return response
         self._is_available = True
         _logger.debug(f"set is_available to %s", self._is_available)
         return response
 
-    async def __check_response_status_and_update(self, response):
+    async def __check_response_status_and_update(self, response) -> bool:
         if response.status != 200:
             _logger.error(
                 f"Error sending command to NEC Beamer: %s", response.status
             )
+            _logger.debug(f"  called from %s", inspect.stack()[1].function)
             return False
         html = await response.text()
         if "power_on_b.gif" and "power_off_g.gif" in html:
             self._is_on = False
         elif "power_on_g.gif" and "power_off_b.gif" in html:
             self._is_on = True
         else:
             _logger.error(f"Error updating NEC Beamer: %s", response.status)
+            _logger.error("power_on*.gif not found in response.")
+            if _logger.level == logging.DEBUG:
+                _logger.debug(f"  called from %s", inspect.stack()[1].function)
+                # get all "gif" from response.text
+                all_gif = re.findall("gif", html)
+                if len(all_gif) > 0:
+                    _logger.debug(f"all gif from response: %s", all_gif)
+                else:
+                    _logger.debug(f"no gif from response\n=====================")
+                    # indent the logging html output by 4 spaces
+                    _logger.debug(
+                        "\n".join(["HTML    " + i for i in html.split("\n")])
+                    )
             return False
 
         # parse response.text for lamp life remaining, lamp hours, filter hours, projector hours used
         # get line from response.text that contains "top.statusF.document.stat.textfield.value= and extract the value
 
         if "top.statusF.document.stat.textfield.value=" in html:
             self._lamp_life_remaining = html.split(
@@ -149,14 +186,19 @@
         # get line from response.text that contains "top.statusF.document.stat.textfield6.value= and extract the value
 
         if "top.statusF.document.stat.textfield6.value=" in html:
             self._projektor_hours_used = html.split(
                 "top.statusF.document.stat.textfield6.value="
             )[1].split(";")[0]
 
+        if "top.statusF.document.stat.textfield5.value=" in html:
+            self._message_error_status = html.split(
+                "top.statusF.document.stat.textfield5.value="
+            )[1].split(";")[0]
+
         # clean up values and convert to int if possible (values are like: '81')
 
         # get all /images/*_a.gif files and check if they are in the response.text
         # if yes this means the corresponding source is active
         # if no this means the corresponding source is not active
         # set the corresponding source to active or not active
 
@@ -185,15 +227,17 @@
                 self._muted[muted_source_name] = True
             else:
                 _logger.error(f"muted source name not found in sources list: %s", muted_source_name)
                 _logger.debug(f"image_name: %s", image)
 
         def __clean_value(value):
             if isinstance(value, str):
-                value = value.replace("'", "").replace(" ", "")
+                value = value.replace("'", "").replace('"', "")
+                # remove leading and trailing spaces
+                value = value.strip()
             if value == "true" or value == "True":
                 return True
             elif value == "false" or value == "False":
                 return False
             elif isinstance(value, bool):
                 return value
             elif value.isnumeric():
@@ -204,15 +248,19 @@
 
         self._lamp_life_remaining = __clean_value(self._lamp_life_remaining)
         self._lamp_hours = __clean_value(self._lamp_hours)
         self._filter_hours = __clean_value(self._filter_hours)
         self._projektor_hours_used = __clean_value(self._projektor_hours_used)
         self._is_available = __clean_value(self._is_available)
         self._is_on = __clean_value(self._is_on)
+        self._message_error_status = __clean_value(self._message_error_status)
 
+        # if message_error_status is not "Normal operation" (or empty) log it as critical
+        if self._message_error_status != "Normal operation" and self._message_error_status != "":
+            _logger.critical(f"NEC Beamer has an Error status message: %s", self._message_error_status)
         return True
 
     @property
     def name(self):
         return self._name
 
     @property
@@ -220,25 +268,27 @@
         return self._is_on
 
     @property
     def is_available(self):
         return self._is_available
 
     async def turn_on(self):
+        """Turn the device on."""
         response = await self.__send_command("power_on")
         _logger.debug(f"Response from NEC Beamer: %s", response)
 
         if response.status == 200:
             self._is_on = True
             await self.update()
         else:
             self._is_on = False
             _logger.error(f"Error turning on NEC Beamer: %s", response.status)
 
     async def turn_off(self):
+        """Turn the device off."""
         response = await self.__send_command("power_off")
 
         if response.status == 200:
             await self.update()
             self._is_on = False
         else:
             self._is_on = True
@@ -249,21 +299,25 @@
         response = await self.__send_command("update")
         try:
             if response.status == 200:
                 await self.__check_response_status_and_update(response)
             else:
                 self._is_on = False
                 self._is_available = False
-                _logger.error(f"Error updating NEC Beamer: %s", response.status)
+                _logger.error(f"Error in updating NEC Beamer with HTTP-Status Code %s."
+                              f" Beamer is not available.", response.status)
+                _logger.debug(f"Response: %s", response)
+                _logger.debug(f"  called from: %s", inspect.stack()[1].function)
         except AttributeError as e:
             self._is_on = False
             self._is_available = False
             _logger.error(f"Error in updating NEC Beamer. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
+            _logger.debug(f"  called from: %s", inspect.stack()[1].function)
 
     @property
     def lamp_life_remaining(self):
         return self._lamp_life_remaining
 
     @property
     def lamp_hours(self):
@@ -274,50 +328,54 @@
         return self._filter_hours
 
     @property
     def projektor_hours_used(self):
         return self._projektor_hours_used
 
     async def source_rgb1(self):
+        """Switch to VGA-Input"""
         response = await self.__send_command("source_rgb1")
         try:
             if response.status == 200:
                 await self.update()
             else:
                 _logger.error(f"Error switching to source_rgb1: %s", response.status)
         except AttributeError as e:
             _logger.error(f"Error in switching to source_rgb1. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
 
     async def source_rgb2(self):
+        """Switch to BNC-Input"""
         response = await self.__send_command("source_rgb2")
         try:
             if response.status == 200:
                 await self.update()
             else:
                 _logger.error(f"Error switching to source_rgb2: %s", response.status)
         except AttributeError as e:
             _logger.error(f"Error in switching to source_rgb2. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
 
     async def source_rgb3(self):
+        """Switch to DVI-Input"""
         response = await self.__send_command("source_rgb3")
         try:
             if response.status == 200:
                 await self.update()
             else:
                 _logger.error(f"Error switching to source_rgb3: %s", response.status)
         except AttributeError as e:
             _logger.error(f"Error in switching to source_rgb3. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
 
     async def source_comp(self):
+        """Switch to Component-Input"""
         response = await self.__send_command("source_comp")
         try:
             if response.status == 200:
                 await self.update()
             else:
                 _logger.error(f"Error switching to source_comp: %s", response.status)
         except AttributeError as e:
@@ -370,14 +428,15 @@
     async def vol_up(self):
         response = await self.__send_command("vol_up")
 
     async def vol_dw(self):
         response = await self.__send_command("vol_dw")
 
     async def mute(self):
+        """Mute/Unmute all output of NEC Beamer"""
         await self.update()
         if self._all_muted:
             _logger.debug(f"Unmute")
             response = await self.__send_command("unmuteAll")
         else:
             _logger.debug(f"Mute")
             response = await self.__send_command("muteAll")
@@ -388,14 +447,15 @@
                 _logger.error(f"Error muting All of NEC Beamer: %s", response.status)
         except AttributeError as e:
             _logger.error(f"Error muting All of NEC Beamer. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
 
     async def mute_picture(self):
+        """Mute/Unmute Picture (and Sound?) of NEC Beamer"""
         await self.update()
         if self._muted["pic"]:
             _logger.debug(f"Unmute Picture")
             response = await self.__send_command("unmutePic")
         else:
             _logger.debug(f"Mute Picture")
             response = await self.__send_command("mutePic")
@@ -406,14 +466,15 @@
                 _logger.error(f"Error muting Picture of NEC Beamer: %s", response.status)
         except AttributeError as e:
             _logger.error(f"Error muting Picture of NEC Beamer. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
 
     async def mute_osd(self):
+        """Mute/Unmute OSD of NEC Beamer"""
         await self.update()
         if self._muted["osd"]:
             _logger.debug(f"Unmute OSD")
             response = await self.__send_command("unmuteOSD")
         else:
             _logger.debug(f"Mute OSD")
             response = await self.__send_command("muteOSD")
@@ -424,14 +485,15 @@
                 _logger.error(f"Error muting OSD of NEC Beamer: %s", response.status)
         except AttributeError as e:
             _logger.error(f"Error muting OSD of NEC Beamer. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
 
     async def mute_audio(self):
+        """Mute/Unmute Audio of NEC Beamer"""
         await self.update()
         if self._muted["snd"]:
             _logger.debug(f"Unmute Audio")
             response = await self.__send_command("unmuteSnd")
         else:
             _logger.debug(f"Mute Audio")
             response = await self.__send_command("muteSnd")
@@ -442,20 +504,24 @@
                 _logger.error(f"Error muting Audio of NEC Beamer: %s", response.status)
         except AttributeError as e:
             _logger.error(f"Error muting Audio of NEC Beamer. Cannot connect.")
             _logger.debug(f"AttributeError: %s", e)
             _logger.debug(f"Response: %s", response)
 
     def __repr__(self) -> str:
-        return f"Nec_Beamer({self._ip_address}, {self._name})"
+        return f"Nec_Beamer(\'{self._ip_address}\', \'{self._name}\')"
 
     def __str__(self) -> str:
-        return f"Nec_Beamer({self._ip_address}, {self._name})"
+        if self.__json:
+            return f"{self.__json_dict()}"
+        else:
+            return f"{self.__text()}"
 
     def __json_dict(self) -> dict:
+        """Returns the status of the beamer in a JSON format"""
         try:
             selected_source = [key for key, value in self._sources.items() if value is True][0]
         except IndexError:
             selected_source = None
 
         json_dict = {
             "name": self._name,
@@ -463,33 +529,39 @@
             "is_on": self._is_on,
             "is_available": self._is_available,
             "status": {
                 "lamp_life_remaining": self._lamp_life_remaining,
                 "lamp_hours": self._lamp_hours,
                 "filter_hours": self._filter_hours,
                 "projektor_hours_used": self._projektor_hours_used,
+                "error_status": self._message_error_status,
             },
             "muted": self._muted,
             "selected-source": selected_source,
         }
         return json_dict
 
-    def print_status(self, json=False):
+    def __text(self):
+        """Prints the status of the beamer in a human-readable format"""
+        return f"""Name: {self._name}
+IP Address: {self._ip_address}
+Is On: {self._is_on}
+Is Available: {self._is_available}
+    Lamp Life Remaining: {self._lamp_life_remaining}
+    Lamp Hours: {self._lamp_hours}
+    Filter Hours: {self._filter_hours}
+    Projektor Hours Used: {self._projektor_hours_used}
+    Message: {self._message_error_status}
+Is Muted All: {self._all_muted}
+    Is Muted Picture: {self._muted["pic"]}
+    Is Muted OSD: {self._muted["osd"]}
+    Is Muted Audio: {self._muted["snd"]}
+Selected Source: {self._selected_source}"""
 
+    def print_status(self, json=False):
+        """Prints the status of the beamer in a human-readable format or in a JSON format"""
         if json or self.__json:
             print(json_lib.dumps(self.__json_dict(), indent=4))
             _logger.debug(json_lib.dumps(self.__json_dict(), indent=4, sort_keys=True))
             return
-        print(f"Name: {self._name}")
-        print(f"IP Address: {self._ip_address}")
-        print(f"Is On: {self._is_on}")
-        print(f"Is Available: {self._is_available}")
-        print(f"Lamp Life Remaining: {self._lamp_life_remaining}")
-        print(f"Lamp Hours: {self._lamp_hours}")
-        print(f"Filter Hours: {self._filter_hours}")
-        print(f"Projektor Hours Used: {self._projektor_hours_used}")
-        print(f"Is Muted All: {self._all_muted}")
-        print(f"Is Muted Picture: {self._muted['pic']}")
-        print(f"Is Muted OSD: {self._muted['osd']}")
-        print(f"Is Muted Audio: {self._muted['snd']}")
-        print(f"Selected Source: {self._selected_source}")
-
+        print(self.__text())
+        _logger.debug(self.__text())
```

### Comparing `async_nec_beamer-0.2.0/async_nec_beamer.egg-info/PKG-INFO` & `async_nec_beamer-0.2.1/async_nec_beamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-nec-beamer
-Version: 0.2.0
+Version: 0.2.1
 Summary: NEC Beamer Web Interface Wrapper (Async)
 Home-page: https://github.com/heinrich-foto/async_nec_beamer
 Author: Heinrich-Foto
 Author-email: async_nec_beamer@heinrich-foto.de
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `async_nec_beamer-0.2.0/bin/async_nec_beamer` & `async_nec_beamer-0.2.1/bin/async_nec_beamer`

 * *Files identical despite different names*

### Comparing `async_nec_beamer-0.2.0/setup.py` & `async_nec_beamer-0.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='async_nec_beamer',
-      version='0.2.0',
+      version='0.2.1',
       description='NEC Beamer Web Interface Wrapper (Async)',
       url='https://github.com/heinrich-foto/async_nec_beamer',
       author='Heinrich-Foto',
       author_email='async_nec_beamer@heinrich-foto.de',
       license='MIT',
       packages=['async_nec_beamer'],
       install_requires=[
```

