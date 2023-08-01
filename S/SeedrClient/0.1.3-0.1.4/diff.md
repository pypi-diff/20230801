# Comparing `tmp/SeedrClient-0.1.3.tar.gz` & `tmp/SeedrClient-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeedrClient-0.1.3.tar", last modified: Sat Jul 29 12:16:26 2023, max compression
+gzip compressed data, was "SeedrClient-0.1.4.tar", last modified: Tue Aug  1 06:35:18 2023, max compression
```

## Comparing `SeedrClient-0.1.3.tar` & `SeedrClient-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/src/SeedrClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/src/seedr_client/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/src/seedr_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/src/seedr_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/src/seedr_client/seedr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/src/SeedrClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/src/seedr_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/src/seedr_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/src/seedr_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/src/seedr_client/seedr_handler.py
```

### Comparing `SeedrClient-0.1.3/PKG-INFO` & `SeedrClient-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,14 +20,19 @@
 SeedrClient is a simple python library that interfaces with Seedr. However, unlike the offical
 rest API, to use SeedrClient you do not need a premium account and even free users can access
 the API.
 
 It is based on [@theabbie](https://github.com/theabbie/seedr-api) and
 [@hemantapkh](https://github.com/hemantapkh/seedrcc) work.
 
+### Installation
+```shell
+pip install SeedrClient
+```
+
 ### Example code
 ```python
 from seedr_client import SeedrHandler
 
 
 seedr = SeedrHandler(email="youremail@example.com", password="your_password")
 print(seedr.get_drive())
```

### Comparing `SeedrClient-0.1.3/README.md` & `SeedrClient-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 SeedrClient is a simple python library that interfaces with Seedr. However, unlike the offical
 rest API, to use SeedrClient you do not need a premium account and even free users can access
 the API.
 
 It is based on [@theabbie](https://github.com/theabbie/seedr-api) and
 [@hemantapkh](https://github.com/hemantapkh/seedrcc) work.
 
+### Installation
+```shell
+pip install SeedrClient
+```
+
 ### Example code
 ```python
 from seedr_client import SeedrHandler
 
 
 seedr = SeedrHandler(email="youremail@example.com", password="your_password")
 print(seedr.get_drive())
```

### Comparing `SeedrClient-0.1.3/setup.py` & `SeedrClient-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `SeedrClient-0.1.3/src/SeedrClient.egg-info/PKG-INFO` & `SeedrClient-0.1.4/src/SeedrClient.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,14 +20,19 @@
 SeedrClient is a simple python library that interfaces with Seedr. However, unlike the offical
 rest API, to use SeedrClient you do not need a premium account and even free users can access
 the API.
 
 It is based on [@theabbie](https://github.com/theabbie/seedr-api) and
 [@hemantapkh](https://github.com/hemantapkh/seedrcc) work.
 
+### Installation
+```shell
+pip install SeedrClient
+```
+
 ### Example code
 ```python
 from seedr_client import SeedrHandler
 
 
 seedr = SeedrHandler(email="youremail@example.com", password="your_password")
 print(seedr.get_drive())
```

### Comparing `SeedrClient-0.1.3/src/seedr_client/seedr_handler.py` & `SeedrClient-0.1.4/src/seedr_client/seedr_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -267,15 +267,17 @@
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_text = response.text
         if not self.is_request_failed(response_text=response_text, requested_on="file"):
             response_json = json.loads(response_text)
             file = {"name": response_json["name"], "download_url": response_json["url"]}
             return file
 
-    def add_torrent(self, torrent=None, wishlist_id=None, folder_id=-1):
+    def add_torrent(
+        self, torrent=None, wishlist_id=None, folder_id=-1, check_size=True
+    ):
         """
         This function allows you to pass either torrent file or magnet uri or a wishlist id, to start downloading
         by Seedr.
 
         Note: If magnet uri is passed instead of a torrent file which is the preferred method, and if the peers in the
         torrent is lower than 3 or if the torrent is completely dead then this function might not be able to add the
         torrent due to the underlying logic which requires the meta info of the torrent. This is a drawback of this
@@ -285,41 +287,56 @@
 
         :param torrent: The torrent file or magnet uri that you want to add to be leeched/downloaded
         :type torrent: str
         :param wishlist_id: The wishlist id that you want to add from your Seedr wishlist
         :type wishlist_id: int
         :param folder_id: The folder you want the torrent to be downloaded to. Defaults to parent.
         :type folder_id: int
+        :param check_size: Used to inform function if checking of Seedr drive space with torrent size is
+            required or not. By default, it checks the torrent size with drive size and raise error if torrent
+            size is larger than drive size.
+        :type check_size: bool
         :return: If successful returns the name and ID of the torrent.
         :rtype: dict
         """
         if torrent:
-            if self.torrent_regex.match(torrent):
-                pass
-            elif self.magnet_regex.match(torrent):
-                # TODO Add a timeout wrapper, which will jump right to adding the torrent instead
-                temp_torrent_file_path = os.path.join(
-                    tempfile.gettempdir(), f"temp{randrange(1, 10**4):04}.torrent"
-                )
-                subprocess.run(
-                    ["ih2torrent", "--file", temp_torrent_file_path, torrent]
-                )
-                torrent = temp_torrent_file_path
+            if check_size:
+                if self.torrent_regex.match(torrent):
+                    pass
+                elif self.magnet_regex.match(torrent):
+                    # TODO Add a timeout wrapper, which will jump right to adding the torrent instead
+                    temp_torrent_file_path = os.path.join(
+                        tempfile.gettempdir(), f"temp{randrange(1, 10**4):04}.torrent"
+                    )
+                    subprocess.run(
+                        ["ih2torrent", "--file", temp_torrent_file_path, torrent]
+                    )
+                    torrent = temp_torrent_file_path
+                else:
+                    raise InvalidTorrent(
+                        f"The torrent passed is invalid, please verify it fix it.\nTorrent/Magnet: {torrent}"
+                    )
+                torrent_info = Torrent.from_file(torrent)
+                if self.drive_size >= torrent_info.total_size:
+                    torrent_magnet_uri = torrent_info.magnet_link
+                else:
+                    print(self.drive_size, torrent_info.total_size)
+                    raise DriveLimit(
+                        "The torrent is larger than the total available space in the drive"
+                    )
             else:
-                raise InvalidTorrent(
-                    f"The torrent passed is invalid, please verify it fix it.\nTorrent/Magnet: {torrent}"
-                )
-            torrent_info = Torrent.from_file(torrent)
-            if self.drive_size >= torrent_info.total_size:
-                torrent_magnet_uri = torrent_info.magnet_link
-            else:
-                print(self.drive_size, torrent_info.total_size)
-                raise DriveLimit(
-                    "The torrent is larger than the total available space in the drive"
-                )
+                if self.torrent_regex.match(torrent):
+                    torrent_info = Torrent.from_file(torrent)
+                    torrent_magnet_uri = torrent_info.magnet_link
+                elif self.magnet_regex.match(torrent):
+                    torrent_magnet_uri = torrent
+                else:
+                    raise InvalidTorrent(
+                        f"The torrent passed is invalid, please verify it fix it.\nTorrent/Magnet: {torrent}"
+                    )
         elif wishlist_id:
             torrent_magnet_uri = None
         else:
             raise TypeError(
                 "add_torrent() is missing an argument. At least one argument needs to be passed"
             )
```

