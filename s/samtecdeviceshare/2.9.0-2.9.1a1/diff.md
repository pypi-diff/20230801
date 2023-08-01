# Comparing `tmp/samtecdeviceshare-2.9.0.tar.gz` & `tmp/samtecdeviceshare-2.9.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samtecdeviceshare-2.9.0.tar", max compression
+gzip compressed data, was "samtecdeviceshare-2.9.1a1.tar", max compression
```

## Comparing `samtecdeviceshare-2.9.0.tar` & `samtecdeviceshare-2.9.1a1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1068 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/LICENSE.md
--rw-r--r--   0        0        0     5895 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/README.md
--rw-r--r--   0        0        0      732 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      128 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/__init__.py
--rw-r--r--   0        0        0    12249 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/aiofilelock.py
--rw-r--r--   0        0        0    12915 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/balena/__init__.py
--rw-r--r--   0        0        0     6517 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/balena/api.py
--rw-r--r--   0        0        0        0 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/emulation/__init__.py
--rw-r--r--   0        0        0      924 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/emulation/networkmanager.py
--rw-r--r--   0        0        0     3561 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/fastapi_utils.py
--rw-r--r--   0        0        0     2305 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/helper.py
--rw-r--r--   0        0        0     1872 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/logger.py
--rw-r--r--   0        0        0     8743 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/nm_utils.py
--rw-r--r--   0        0        0     9989 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/sdshare.py
--rw-r--r--   0        0        0     6396 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/server.py
--rw-r--r--   0        0        0     6892 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/types.py
--rw-r--r--   0        0        0     8445 2022-05-11 23:41:32.646454 samtecdeviceshare-2.9.0/samtecdeviceshare/wiredhandler.py
--rw-r--r--   0        0        0     7072 2022-05-11 23:41:41.722788 samtecdeviceshare-2.9.0/setup.py
--rw-r--r--   0        0        0     6856 2022-05-11 23:41:41.724017 samtecdeviceshare-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-01 16:37:57.817474 samtecdeviceshare-2.9.1a1/LICENSE.md
+-rw-r--r--   0        0        0     5895 2023-08-01 16:37:57.817474 samtecdeviceshare-2.9.1a1/README.md
+-rw-r--r--   0        0        0      740 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/__init__.py
+-rw-r--r--   0        0        0    12224 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/aiofilelock.py
+-rw-r--r--   0        0        0    12915 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/balena/__init__.py
+-rw-r--r--   0        0        0     6523 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/balena/api.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/emulation/__init__.py
+-rw-r--r--   0        0        0      924 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/emulation/networkmanager.py
+-rw-r--r--   0        0        0     3561 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/fastapi_utils.py
+-rw-r--r--   0        0        0     2305 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/helper.py
+-rw-r--r--   0        0        0     1872 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/logger.py
+-rw-r--r--   0        0        0     8925 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/nm_utils.py
+-rw-r--r--   0        0        0    10018 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/sdshare.py
+-rw-r--r--   0        0        0     6342 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/server.py
+-rw-r--r--   0        0        0     6910 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/types.py
+-rw-r--r--   0        0        0     8412 2023-08-01 16:37:57.821474 samtecdeviceshare-2.9.1a1/samtecdeviceshare/wiredhandler.py
+-rw-r--r--   0        0        0     6911 1970-01-01 00:00:00.000000 samtecdeviceshare-2.9.1a1/PKG-INFO
```

### Comparing `samtecdeviceshare-2.9.0/LICENSE.md` & `samtecdeviceshare-2.9.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `samtecdeviceshare-2.9.0/README.md` & `samtecdeviceshare-2.9.1a1/README.md`

 * *Files identical despite different names*

### Comparing `samtecdeviceshare-2.9.0/pyproject.toml` & `samtecdeviceshare-2.9.1a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "samtecdeviceshare"
-version = "2.9.0"
+version = "2.9.1a1"
 description = "Handles a variety of common routines for SDC-based applications"
 readme = "README.md"
 authors = ["Adam Page <adam.page@samtec.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = "^0.63.0"
 uvicorn = "^0.13.3"
 pydantic = "^1.7.3"
 pyhumps = "^1.6.1"
 python-networkmanager = { version = "*",  platform = "linux"}
 dbus-python = { version = "*",  platform = "linux"}
 httpx = "^0.16.1"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.1"
 aiofiles = "^0.6.0"
 pyaml-env = "^1.1.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^6.2.1"
 pylint = "^2.6.0"
 twine = "^3.3.0"
 watchgod = "^0.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/aiofilelock.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/aiofilelock.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,15 @@
     """ Raised when the lock could not be acquired in *timeout* seconds. """
     def __init__(self, lock_file):
         #: The path of the file lock.
         super().__init__()
         self.lock_file = lock_file
 
     def __str__(self):
-        temp = "The file lock '{}' could not be acquired."\
-               .format(self.lock_file)
+        temp = f"The file lock '{self.lock_file}' could not be acquired."
         return temp
 
 
 # Classes
 # ------------------------------------------------
 
 # This is a helper class which is returned by :meth:`BaseFileLock.acquire`
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/balena/__init__.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/balena/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,31 +191,31 @@
 
 async def update_check(force: bool = False, delay: int = 0) -> bool:
     if delay:
         await asyncio.sleep(delay)
     async with httpx.AsyncClient() as client:
         r = await client.post(
             supervisor_address()+'/v1/update',
-            params={'apikey': supervisor_api_key()}, json=dict(force=force)
+            params={'apikey': supervisor_api_key()}, json={'force': force}
         )
     return r.status_code == httpx.codes.NO_CONTENT
 
 async def reboot(force: bool = False) -> bool:
     async with httpx.AsyncClient() as client:
         r = await client.post(
             supervisor_address()+'/v1/reboot',
-            params={'apikey': supervisor_api_key()}, json=dict(force=force)
+            params={'apikey': supervisor_api_key()}, json={'force': force}
         )
     return r.status_code == httpx.codes.ACCEPTED
 
 async def shutdown(force: bool = False) -> bool:
     async with httpx.AsyncClient() as client:
         r = await client.post(
             supervisor_address()+'/v1/shutdown',
-            params={'apikey': supervisor_api_key()}, json=dict(force=force)
+            params={'apikey': supervisor_api_key()}, json={'force': force}
         )
     return r.status_code == httpx.codes.ACCEPTED
 
 async def purge() -> bool:
     async with httpx.AsyncClient() as client:
         r = await client.post(
             supervisor_address()+'/v1/purge', params={'apikey': supervisor_api_key()}
@@ -223,15 +223,15 @@
     return r.status_code == httpx.codes.OK
 
 async def restart(app_id: Optional[int] = None) -> bool:
     app_id = get_app_id() if app_id is None else app_id
     async with httpx.AsyncClient() as client:
         r = await client.post(
             supervisor_address()+'/v1/restart',
-            params={'apikey': supervisor_api_key()}, json=dict(appId=app_id)
+            params={'apikey': supervisor_api_key()}, json={'appId': app_id}
         )
     return r.status_code == httpx.codes.OK
 
 async def regenerate_api_key() -> str:
     async with httpx.AsyncClient() as client:
         r = await client.post(
             supervisor_address()+'/v1/regenerate-api-key', params={'apikey': supervisor_api_key()}
@@ -305,48 +305,48 @@
 
 async def restart_service(service: str, app_id: Optional[int] = None, force: bool = False) -> bool:
     if app_id is None:
         app_id = get_app_id()
     async with httpx.AsyncClient() as client:
         r = await client.get(
             supervisor_address()+f'/v2/applications/{app_id}/restart-service',
-            params={'apikey': supervisor_api_key()}, json=dict(serviceName=service, force=force)
+            params={'apikey': supervisor_api_key()}, json={'serviceName': service, 'force': force}
         )
     return r.status_code == httpx.codes.OK
 
 async def stop_service(service: str, app_id: Optional[int] = None, force: bool = False) -> bool:
     if app_id is None:
         app_id = get_app_id()
     async with httpx.AsyncClient() as client:
         r = await client.get(
             supervisor_address()+f'/v2/applications/{app_id}/stop-service',
-            params={'apikey': supervisor_api_key()}, json=dict(serviceName=service, force=force)
+            params={'apikey': supervisor_api_key()}, json={'serviceName': service, 'force': force}
         )
     return r.status_code == httpx.codes.OK
 
 async def start_service(service: str, app_id: Optional[int] = None, force: bool = False) -> bool:
     if app_id is None:
         app_id = get_app_id()
     async with httpx.AsyncClient() as client:
         r = await client.get(
             supervisor_address()+f'/v2/applications/{app_id}/start-service',
-            params={'apikey': supervisor_api_key()}, json=dict(serviceName=service, force=force)
+            params={'apikey': supervisor_api_key()}, json={'serviceName': service, 'force': force}
         )
     return r.status_code == httpx.codes.OK
 
 async def restart_services(app_id: Optional[int] = None, force: bool = False) -> bool:
     app_id = get_app_id() if app_id is None else app_id
     async with httpx.AsyncClient() as client:
         r = await client.get(
             supervisor_address()+f'/v2/applications/{app_id}/restart',
-            params={'apikey': supervisor_api_key()}, json=dict(force=force)
+            params={'apikey': supervisor_api_key()}, json={'force': force}
         )
     return r.status_code == httpx.codes.OK
 
 async def purge_all_user_data(app_id: Optional[int] = None, force: bool = False) -> bool:
     app_id = get_app_id() if app_id is None else app_id
     async with httpx.AsyncClient() as client:
         r = await client.get(
             supervisor_address()+f'/v2/applications/{app_id}/purge',
-            params={'apikey': supervisor_api_key()}, json=dict(force=force)
+            params={'apikey': supervisor_api_key()}, json={'force': force}
         )
     return r.status_code == httpx.codes.OK
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/balena/api.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/balena/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,29 @@
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 @router.post('/v1/reboot', status_code=status.HTTP_202_ACCEPTED)
 async def route_reboot(force: Optional[bool] = None):
     success = await reboot(force=force or False)
     if not success:
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST)
-    return JSONResponse(dict(Data='OK', Error=''))
+    return JSONResponse({'Data': 'OK', 'Error': ''})
 
 @router.post('/v1/shutdown', status_code=status.HTTP_202_ACCEPTED)
 async def route_shutdown(force: Optional[bool] = None):
     success = await shutdown(force=force or False)
     if not success:
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST)
-    return JSONResponse(dict(Data='OK', Error=''))
+    return JSONResponse({'Data': 'OK', 'Error': ''})
 
 @router.post('/v1/purge', status_code=status.HTTP_200_OK)
 async def route_purge():
     success = await purge()
     if not success:
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST)
-    return JSONResponse(dict(Data='OK', Error=''))
+    return JSONResponse({'Data': 'OK', 'Error': ''})
 
 @router.post('/v1/restart', status_code=status.HTTP_200_OK)
 async def route_restart():
     success = await restart()
     if not success:
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST)
     return "OK"
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/emulation/networkmanager.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/emulation/networkmanager.py`

 * *Files identical despite different names*

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/fastapi_utils.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/helper.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/helper.py`

 * *Files identical despite different names*

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/logger.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/logger.py`

 * *Files identical despite different names*

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/nm_utils.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/nm_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import asyncio
 import logging
 from typing import Dict, List, Optional, Any, Union, Pattern
 from .types import NetworkCredentials
 
 logger = logging.getLogger('sdc.helper')
 
+
+class UnsupportedActionError(Exception):
+    def __init__(self, message="Unsupported action"):
+        self.message = message
+        super().__init__(self.message)
+
+
 try:
     import NetworkManager as nm  # type: ignore
     from dbus.mainloop.glib import DBusGMainLoop  # type: ignore
     DBusGMainLoop(set_as_default=True)
 except Exception:
     if os.getenv('PYTHON_ENV') == 'development':
         logger.warning('Failed to load NetworkManager. Using emulator in development.')
@@ -98,19 +105,19 @@
         raise TypeError('Invalid wifi credentials: Passphrase incorrect.')
     # https://developer-old.gnome.org/NetworkManager/stable/settings-802-11-wireless-security.html
     if passphrase:
         s_wsec = {'key-mgmt': 'wpa-psk', 'proto': ['rsn'], 'psk': passphrase, 'wps-method': 1}
     else:
         s_wsec = {'key-mgmt': 'none', 'auth-alg': 'open'}
     conn = {
-        'connection': dict(type='802-11-wireless', uuid=conn_uuid or str(uuid.uuid4()), id=ssid),
-        '802-11-wireless': dict(ssid=ssid.encode("utf-8"), mode='ap', band='bg', channel=1),
+        'connection': {'type': '802-11-wireless', 'uuid': conn_uuid or str(uuid.uuid4()), 'id': ssid},
+        '802-11-wireless': {'ssid': ssid.encode("utf-8"), 'mode': 'ap', 'band': 'bg', 'channel': 1},
         '802-11-wireless-security': s_wsec,
-        'ipv4': dict(method='shared'),
-        'ipv6': dict(method='ignore')
+        'ipv4': {'method': 'shared'},
+        'ipv6': {'method': 'ignore'}
     }
     return conn
 
 def create_wifi_client_connection(ssid: str, passphrase: Optional[str] = None, identity: Optional[str] = None, conn_uuid: Optional[str] = None):
     if not isinstance(ssid, str):
         raise TypeError('Invalid wifi credentials: SSID missing or incorrect.')
     if passphrase and not valid_wpa_passphrase(passphrase):
@@ -125,16 +132,16 @@
         s_eap = None
     # WEP open
     else:
         s_wsec = {'key-mgmt': 'none', 'auth-alg': 'open'}
         s_eap = None
 
     conn = {
-        'connection': dict(type='802-11-wireless', uuid=conn_uuid or str(uuid.uuid4()), id=ssid),
-        '802-11-wireless': dict(ssid=ssid.encode("utf-8"), security='802-11-wireless-security'),
+        'connection': {'type': '802-11-wireless', 'uuid': conn_uuid or str(uuid.uuid4()), 'id': ssid},
+        '802-11-wireless': {'ssid': ssid.encode("utf-8"), 'security': '802-11-wireless-security'},
         '802-11-wireless-security': s_wsec,
         'ipv4': {'method': 'auto'},
         'ipv6': {'method': 'auto'}
     }
     if s_eap:
         conn['802-1x'] = s_eap
     return conn
@@ -164,19 +171,19 @@
             time.sleep(0.5)
             # Wait for the connection to start up
             start = time.time()
             while time.time() < start + int(timeout):
                 if act_conn.State == nm.NM_ACTIVE_CONNECTION_STATE_ACTIVATED:
                     return
                 await asyncio.sleep(1)
-            raise Exception('Failed to start wifi connection due to timeout')
+            raise TimeoutError('Failed to start wifi connection due to timeout')
         if str(action).upper() == 'DOWN':
             dev.Disconnect()
             return
-        raise Exception('Unsupported action')
+        raise UnsupportedActionError()
     except Exception as err:
         logger.exception(err)
         raise
 
 async def setup_wifi_hotspot(credentials: NetworkCredentials, conn_uuid: Optional[uuid.UUID] = None, action: Optional[str] = None, timeout: float = 10):
     conn_settings = create_wifi_hotspot_connection(ssid=credentials.ssid, passphrase=credentials.passphrase, conn_uuid=conn_uuid)
     await setup_wifi_connection(conn_settings=conn_settings, iface=credentials.iface_regex or credentials.iface, action=action, timeout=timeout)
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/sdshare.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/sdshare.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,16 @@
         zip_fp.close()
         bf.seek(0)
         return bf.read()
 
     async def get_log_zip_data(self):
         return await run_in_threadpool(self.get_log_zip_data_sync)
 
-    async def blink_device(self):
+    @staticmethod
+    async def blink_device():
         if is_on_balena():
             return await balena.blink()
         return True
 
     async def enable_update_lock(self, timeout: int = 6):
         if self.update_lock.is_locked:
             return
@@ -161,15 +162,16 @@
         try:
             await self.update_lock.release()
         except LockTimeout:
             logger.warning('Forcefully breaking update lock file.')
             await self.update_lock.release(force=True)
         logger.info('Update lock successfully removed.')
 
-    async def restart_device(self, force: bool = False):
+    @staticmethod
+    async def restart_device(force: bool = False):
         if not is_on_balena():
             return
         return await balena.reboot(force=force)
 
     async def update_application(self) -> bool:
         if not is_on_balena():
             return True
@@ -201,25 +203,25 @@
             if await is_online_async():
                 await shield(balena.update_check(force=False))
                 await asyncio.sleep(1)
                 return
 
             # Must provide wifi credentials
             if credentials is None:
-                raise Exception('No internet access and no Wi-Fi credentials provided.')
+                raise TypeError('No internet access and no Wi-Fi credentials provided.')
             await self.launch_wifi(credentials=credentials)
             # Wait 20 seconds for internet access
             num_attempts = 0
             online = False
             while num_attempts < 20 and not online:
                 await asyncio.sleep(1)
                 online = await is_online_async()
                 num_attempts += 1
             if not online:
-                raise Exception('Timeout reached trying to contact server.')
+                raise TimeoutError('Timeout reached trying to contact server.')
 
             # Trigger supervisor to check for an update
             logger.info('OTA Update Check: Started')
             await balena.update_check(force=False)
             await asyncio.sleep(20)
             tic = time.time()
             app_state = await balena.get_application_state()
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/server.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,49 +72,49 @@
     return await sds.get_device_state()
 
 @app.get("/api/v2/app/logs", description='Download all app logs as a zip.')
 async def get_app_logs() -> Response:
     try:
         return Response(content=await sds.get_log_zip_data(), media_type="application/octet-stream", status_code=status.HTTP_200_OK)
     except Exception as err:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail='Failed to get app logs w/ error: {0}'.format(err)) from err
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f'Failed to get app logs w/ error: {err}') from err
 
 @app.post('/api/v2/device/blink', status_code=status.HTTP_200_OK, description='''
 Have the device blink for 15 seconds.''')
 async def blink_device() -> TextResponseEnum:
     try:
         return TextResponseEnum.from_bool(await sds.blink_device())
     except Exception as err:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail='Failed to get app state w/ error: {0}'.format(err)) from err
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f'Failed to get app state w/ error: {err}') from err
 
 @app.post('/api/v2/device/restart', status_code=status.HTTP_202_ACCEPTED, description='''
 Performs a full reboot of the device.''')
 async def restart_device() -> TextResponseEnum:
     return TextResponseEnum.from_bool(await sds.restart_device())
 
 @app.post('/api/v2/app/update/check', status_code=status.HTTP_204_NO_CONTENT, description='''
 Checks if an app update exists and if so downloads it. ''')
 async def app_update_check(background_tasks: BackgroundTasks, credentials: Optional[NetworkCredentials] = None) -> TextResponseEnum:
     try:
         background_tasks.add_task(sds.perform_ota_update_check, credentials)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
     except (CancelledError, ConnectionResetError) as err:
         logger.exception('Request cancelled or reset (error: %s)', err)
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail='Failed to perform update check w/ error: {0}'.format(err)) from err
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f'Failed to perform update check w/ error: {err}') from err
     except Exception as err:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail='Failed to perform update check w/ error: {0}'.format(err)) from err
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f'Failed to perform update check w/ error: {err}') from err
 
 @app.post('/api/v2/app/update/install', status_code=status.HTTP_204_NO_CONTENT, description='''
 Installs update if downloaded and restarts app.''')
 async def app_update_install(background_tasks: BackgroundTasks) -> TextResponseEnum:
     try:
         background_tasks.add_task(sds.update_application)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
     except Exception as err:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail='Failed to perform update w/ error: {0}'.format(err)) from err
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f'Failed to perform update w/ error: {err}') from err
 
 #######################################################################################################################
 # Optional WiFi REST Routes
 #######################################################################################################################
 
 @app.get('/api/v2/network/wifi/credentials', response_model=Optional[NetworkCredentialCleaned], status_code=status.HTTP_200_OK, description='''
 Get WiFi connection information. __NOTE__: Only gets stored default connection for now.''')
@@ -124,11 +124,11 @@
 @app.post('/api/v2/network/wifi/credentials', status_code=status.HTTP_200_OK, description='''
 Temporarily connect to supplied WiFi network. Connection is cleared on reboot or app restart.''')
 async def set_wifi_network(credentials: NetworkCredentials) -> TextResponseEnum:
     try:
         await sds.launch_wifi(credentials)
         return TextResponseEnum.Success
     except Exception as err:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail='Failed to update WiFi credentials w/ error: {0}'.format(err)) from err
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f'Failed to update WiFi credentials w/ error: {err}') from err
 
 if __name__ == "__main__":
     uvicorn.run(app, host=sds.config.rest_address, port=sds.config.rest_port)
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/types.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     @classmethod
     def load_default(cls):
         config_path = os.getenv('SDC_CONFIGURATION_PATH')
         if config_path and os.path.isfile(config_path):
             # If JSON, convert to yaml to support env var replacement
             if os.path.splitext(config_path)[1].lower() == '.json':
-                with open(config_path, 'r') as fp:
+                with open(config_path, 'r', encoding='utf-8') as fp:
                     config = parse_config(data=yaml.dump(json.load(fp)), raise_if_na=True)
                 return cls(**config)
 
             if os.path.splitext(config_path)[1].lower() in ('.yml', '.yaml'):
                 config = parse_config(config_path, raise_if_na=True)
                 return cls(**config)
         return cls()
```

### Comparing `samtecdeviceshare-2.9.0/samtecdeviceshare/wiredhandler.py` & `samtecdeviceshare-2.9.1a1/samtecdeviceshare/wiredhandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,25 +151,25 @@
             next_fsm.con_counter = 0
             next_fsm.con_state = WiredConnectionState.DISCONNECTED
             next_fsm.con_method = self.config.method
         else:
             next_fsm.con_method = con_method
 
         if next_fsm.dev_iface != self.fsm.dev_iface:
-            logger.info('Wired device iface changed to {0}'.format(next_fsm.dev_iface))
+            logger.info('Wired device iface changed to %s', next_fsm.dev_iface)
         if next_fsm.con_name != self.fsm.con_name:
-            logger.info('Wired connection name changed to {0}'.format(next_fsm.con_name))
+            logger.info('Wired connection name changed to %s', next_fsm.con_name)
         if next_fsm.con_state != self.fsm.con_state:
-            logger.info('Wired connection state changed to {0}'.format(next_fsm.con_state))
+            logger.info('Wired connection state changed to %s', next_fsm.con_state)
 
         # If have connection and want method to change or needs initialization
         if next_fsm.con_needs_init or (next_fsm.con_method != con_method):
             # IMPORTANT: On init we must start with primary method
             next_con_method = self.config.method if next_fsm.con_needs_init else next_fsm.con_method
-            logger.info('Setting connection {0} to method {1}'.format(next_fsm.con_name, next_con_method))
+            logger.info('Setting connection %s to method %s', next_fsm.con_name, next_con_method)
             success = update_active_conn_ipv4_method(con, dev, next_con_method)
             # NOTE: If failed to activate, restart process
             if not success:
                 next_fsm.con_needs_init = True
                 logger.error('Failed setting active connection method.')
             else:
                 next_fsm.con_needs_init = False
```

### Comparing `samtecdeviceshare-2.9.0/setup.py` & `samtecdeviceshare-2.9.1a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,159 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: samtecdeviceshare
+Version: 2.9.1a1
+Summary: Handles a variety of common routines for SDC-based applications
+License: MIT
+Author: Adam Page
+Author-email: adam.page@samtec.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: aiofiles (>=0.6.0,<0.7.0)
+Requires-Dist: dbus-python ; sys_platform == "linux"
+Requires-Dist: fastapi (>=0.63.0,<0.64.0)
+Requires-Dist: httpx (>=0.16.1,<0.17.0)
+Requires-Dist: pyaml-env (>=1.1.0,<2.0.0)
+Requires-Dist: pydantic (>=1.7.3,<2.0.0)
+Requires-Dist: pyhumps (>=1.6.1,<2.0.0)
+Requires-Dist: python-networkmanager ; sys_platform == "linux"
+Requires-Dist: uvicorn (>=0.13.3,<0.14.0)
+Description-Content-Type: text/markdown
+
+# Samtec Device Connect Service
+
+A Python 3 SDC conforming REST API to run on IoT devices that enables user discovery, viewing, and management.
+
+## Installation
+
+```bash
+pip install samtecdeviceshare
+```
+
+## Running
+
+First ensure all environment variables are set correctly.
+Note: To test locally for development ensure EMULATION and PYTHON_ENV are set.
+
+```bash
+python -m samtecdeviceshare.server
+```
+
+## Environment Variables
+
+A number of environment variables are supported for configuration. These configurations can also be contained in a yaml/json configuration file specified using `SDC_CONFIGURATION_PATH`. Env vars take precedence over the configuration file.
+
+### SDC Server / General
+
+These variables are specific to this SDC service. The variables can also start with prefix `SDC_`.
+
+| Name              | Description                   | Default                                     |
+| ----------------- | ----------------------------- | ------------------------------------------- |
+| REST_ADDRESS      | Rest API Address              | 0.0.0.0                                     |
+| REST_PORT         | Rest port                     | 47546                                       |
+| ROOT_PATH         | API root path                 | ''                                          |
+| PYTHON_ENV        | enum: development production  | production                                  |
+| EMULATION         | Use emulated devices/io       | null                                        |
+| LOG_VERBOSE       | boolean verbose logs          | false                                       |
+
+### Application
+
+These variables are used to provide app info that will be shared by SDC.
+
+| Name              | Description                   | Default                                     |
+| ----------------- | ----------------------------- | ------------------------------------------- |
+| APP_NAME          | Name of app                   | SDC App                                     |
+| APP_VERSION       | SemVer of app                 | 0.0.0                                       |
+| APP_WEB_PORT      | Embedded web app port         | 80                                          |
+| APP_IMG_PATH      | app icon path                 | {CURDIR}../static/img.png                   |
+| APP_LOG_PATH      | Path to store log files       | default tempdir()                           |
+| APP_LOCK_PATH     | Path to update lock file      | .__sdc.lock                                 |
+
+### Wireless Networks
+
+SDC can handle configuring N wireless networks. Prefix *SDC_* is required. Us integer `i` in prefix for defining multiple networks.
+A network can optionally be defined default. This will be primary method used to handle updates and will be exposed through REST API.
+
+| Name                     | Description                   | Default                         |
+| ------------------------ | ----------------------------- | ------------------------------- |
+| SDC_WIFI[i]_SSID         | WiFi SSID                     | null*                           |
+| SDC_WIFI[i]_MODE         | enum: HOTSPOT CLIENT DISABLED | DISABLED                        |
+| SDC_WIFI[i]_PASS         | WiFi passphrase               | null                            |
+| SDC_WIFI[i]_IFACE        | WiFi hardware interface       | null                            |
+| SDC_WIFI[i]_DEFAULT      | Use as default for updates    | False                           |
+
+### Wired Networks
+
+SDC can handle configuring N wired networks. Prefix *SDC_* is required. Us integer `i` in prefix for defining multiple networks.
+`SDC_ETH[i]_IFACE` or `SDC_ETH[i]_REGEX_IFACE` is required with the latter supporting regex matching. Be careful defining multiple networks with generic regular expression.
+[Most Linux distros follow a predictable naming scheme for interfaces.](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/networking_guide/sec-understanding_the_predictable_network_interface_device_names). When searching for interfaces, a fullmatch is required `re.fullmatch()`.
+
+| Name                        | Description                   | Default                      |
+| --------------------------- | ----------------------------- | ---------------------------- |
+| SDC_ETH[i]_IFACE            | Interface name (str)          | null                         |
+| SDC_ETH[i]_REGEX_IFACE      | Interface name (regex)        | null                         |
+| SDC_ETH[i]_METHOD           | Primary method                | WiredConnectionMethod.auto   |
+| SDC_ETH[i]_TIMEOUT          | Timeout of primary            | 15                           |
+| SDC_ETH[i]_FALLBACK         | Fallback method               | null                         |
+| SDC_ETH[i]_FALLBACK_TIMEOUT | Timeout to get DHCP address   | -1                           |
+
+### Balena
+
+Refer to Balena [documentation](https://www.balena.io/docs/learn/develop/runtime/) for list and description of variables.
+
+- BALENA_SUPERVISOR_API_KEY
+- BALENA_APP_ID
+- BALENA_DEVICE_TYPE
+- BALENA
+- BALENA_SUPERVISOR_ADDRESS
+- BALENA_SUPERVISOR_HOST
+- BALENA_DEVICE_UUID
+- BALENA_API_KEY
+- BALENA_APP_RELEASE
+- BALENA_SUPERVISOR_VERSION
+- BALENA_APP_NAME
+- BALENA_DEVICE_NAME_AT_INIT
+- BALENA_HOST_OS_VERSION
+- BALENA_SUPERVISOR_PORT
+
+## Development
+
+### Installing
+
+```bash
+git clone git@bitbucket.org:samteccmd/samtecdeviceshare.git samtecdeviceshare
+cd samtecdeviceshare
+poetry install --dev
+poetry shell
+```
+
+### Testing
+
+First, run dummy Balena supervisor:
+
+```bash
+bash ./tests/dummy-supervisor.sh
+```
+
+Next, fire up REST server using uvicorn:
+
+```bash
+EMULATION=1 \
+PYTHON_ENV="development" \
+DEBUG=1 \
+uvicorn samtecdeviceshare.server:app --reload --reload-dir ./samtecdeviceshare
+```
+
+**Interactive API docs** will be available: <http://127.0.0.1:8000/docs>
+
+### Unit Tests
+
+```bash
+pylint --rcfile .pylintrc samtecdeviceshare
+pytest
+```
 
-packages = \
-['samtecdeviceshare', 'samtecdeviceshare.balena', 'samtecdeviceshare.emulation']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=5.4.1,<6.0.0',
- 'aiofiles>=0.6.0,<0.7.0',
- 'fastapi>=0.63.0,<0.64.0',
- 'httpx>=0.16.1,<0.17.0',
- 'pyaml-env>=1.1.0,<2.0.0',
- 'pydantic>=1.7.3,<2.0.0',
- 'pyhumps>=1.6.1,<2.0.0',
- 'uvicorn>=0.13.3,<0.14.0']
-
-extras_require = \
-{':sys_platform == "linux"': ['python-networkmanager', 'dbus-python']}
-
-setup_kwargs = {
-    'name': 'samtecdeviceshare',
-    'version': '2.9.0',
-    'description': 'Handles a variety of common routines for SDC-based applications',
-    'long_description': '# Samtec Device Connect Service\n\nA Python 3 SDC conforming REST API to run on IoT devices that enables user discovery, viewing, and management.\n\n## Installation\n\n```bash\npip install samtecdeviceshare\n```\n\n## Running\n\nFirst ensure all environment variables are set correctly.\nNote: To test locally for development ensure EMULATION and PYTHON_ENV are set.\n\n```bash\npython -m samtecdeviceshare.server\n```\n\n## Environment Variables\n\nA number of environment variables are supported for configuration. These configurations can also be contained in a yaml/json configuration file specified using `SDC_CONFIGURATION_PATH`. Env vars take precedence over the configuration file.\n\n### SDC Server / General\n\nThese variables are specific to this SDC service. The variables can also start with prefix `SDC_`.\n\n| Name              | Description                   | Default                                     |\n| ----------------- | ----------------------------- | ------------------------------------------- |\n| REST_ADDRESS      | Rest API Address              | 0.0.0.0                                     |\n| REST_PORT         | Rest port                     | 47546                                       |\n| ROOT_PATH         | API root path                 | \'\'                                          |\n| PYTHON_ENV        | enum: development production  | production                                  |\n| EMULATION         | Use emulated devices/io       | null                                        |\n| LOG_VERBOSE       | boolean verbose logs          | false                                       |\n\n### Application\n\nThese variables are used to provide app info that will be shared by SDC.\n\n| Name              | Description                   | Default                                     |\n| ----------------- | ----------------------------- | ------------------------------------------- |\n| APP_NAME          | Name of app                   | SDC App                                     |\n| APP_VERSION       | SemVer of app                 | 0.0.0                                       |\n| APP_WEB_PORT      | Embedded web app port         | 80                                          |\n| APP_IMG_PATH      | app icon path                 | {CURDIR}../static/img.png                   |\n| APP_LOG_PATH      | Path to store log files       | default tempdir()                           |\n| APP_LOCK_PATH     | Path to update lock file      | .__sdc.lock                                 |\n\n### Wireless Networks\n\nSDC can handle configuring N wireless networks. Prefix *SDC_* is required. Us integer `i` in prefix for defining multiple networks.\nA network can optionally be defined default. This will be primary method used to handle updates and will be exposed through REST API.\n\n| Name                     | Description                   | Default                         |\n| ------------------------ | ----------------------------- | ------------------------------- |\n| SDC_WIFI[i]_SSID         | WiFi SSID                     | null*                           |\n| SDC_WIFI[i]_MODE         | enum: HOTSPOT CLIENT DISABLED | DISABLED                        |\n| SDC_WIFI[i]_PASS         | WiFi passphrase               | null                            |\n| SDC_WIFI[i]_IFACE        | WiFi hardware interface       | null                            |\n| SDC_WIFI[i]_DEFAULT      | Use as default for updates    | False                           |\n\n### Wired Networks\n\nSDC can handle configuring N wired networks. Prefix *SDC_* is required. Us integer `i` in prefix for defining multiple networks.\n`SDC_ETH[i]_IFACE` or `SDC_ETH[i]_REGEX_IFACE` is required with the latter supporting regex matching. Be careful defining multiple networks with generic regular expression.\n[Most Linux distros follow a predictable naming scheme for interfaces.](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/networking_guide/sec-understanding_the_predictable_network_interface_device_names). When searching for interfaces, a fullmatch is required `re.fullmatch()`.\n\n| Name                        | Description                   | Default                      |\n| --------------------------- | ----------------------------- | ---------------------------- |\n| SDC_ETH[i]_IFACE            | Interface name (str)          | null                         |\n| SDC_ETH[i]_REGEX_IFACE      | Interface name (regex)        | null                         |\n| SDC_ETH[i]_METHOD           | Primary method                | WiredConnectionMethod.auto   |\n| SDC_ETH[i]_TIMEOUT          | Timeout of primary            | 15                           |\n| SDC_ETH[i]_FALLBACK         | Fallback method               | null                         |\n| SDC_ETH[i]_FALLBACK_TIMEOUT | Timeout to get DHCP address   | -1                           |\n\n### Balena\n\nRefer to Balena [documentation](https://www.balena.io/docs/learn/develop/runtime/) for list and description of variables.\n\n- BALENA_SUPERVISOR_API_KEY\n- BALENA_APP_ID\n- BALENA_DEVICE_TYPE\n- BALENA\n- BALENA_SUPERVISOR_ADDRESS\n- BALENA_SUPERVISOR_HOST\n- BALENA_DEVICE_UUID\n- BALENA_API_KEY\n- BALENA_APP_RELEASE\n- BALENA_SUPERVISOR_VERSION\n- BALENA_APP_NAME\n- BALENA_DEVICE_NAME_AT_INIT\n- BALENA_HOST_OS_VERSION\n- BALENA_SUPERVISOR_PORT\n\n## Development\n\n### Installing\n\n```bash\ngit clone git@bitbucket.org:samteccmd/samtecdeviceshare.git samtecdeviceshare\ncd samtecdeviceshare\npoetry install --dev\npoetry shell\n```\n\n### Testing\n\nFirst, run dummy Balena supervisor:\n\n```bash\nbash ./tests/dummy-supervisor.sh\n```\n\nNext, fire up REST server using uvicorn:\n\n```bash\nEMULATION=1 \\\nPYTHON_ENV="development" \\\nDEBUG=1 \\\nuvicorn samtecdeviceshare.server:app --reload --reload-dir ./samtecdeviceshare\n```\n\n**Interactive API docs** will be available: <http://127.0.0.1:8000/docs>\n\n### Unit Tests\n\n```bash\npylint --rcfile .pylintrc samtecdeviceshare\npytest\n```\n',
-    'author': 'Adam Page',
-    'author_email': 'adam.page@samtec.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

