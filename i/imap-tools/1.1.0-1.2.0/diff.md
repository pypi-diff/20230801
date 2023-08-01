# Comparing `tmp/imap-tools-1.1.0.tar.gz` & `tmp/imap-tools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imap-tools-1.1.0.tar", last modified: Tue Jul 25 09:15:33 2023, max compression
+gzip compressed data, was "dist\imap-tools-1.2.0.tar", last modified: Tue Aug  1 05:50:27 2023, max compression
```

## Comparing `imap-tools-1.1.0.tar` & `imap-tools-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 09:15:33.000000 imap-tools-1.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools/
--rw-rw-rw-   0        0        0     1209 2022-03-06 11:54:23.000000 imap-tools-1.1.0/imap_tools/consts.py
--rw-rw-rw-   0        0        0     2109 2022-02-15 11:27:46.000000 imap-tools-1.1.0/imap_tools/errors.py
--rw-rw-rw-   0        0        0     7084 2022-03-14 10:53:53.000000 imap-tools-1.1.0/imap_tools/folder.py
--rw-rw-rw-   0        0        0     4465 2022-11-21 11:14:06.000000 imap-tools-1.1.0/imap_tools/idle.py
--rw-rw-rw-   0        0        0     2059 2021-09-20 07:00:52.000000 imap-tools-1.1.0/imap_tools/imap_utf7.py
--rw-rw-rw-   0        0        0    15852 2023-07-25 09:13:31.000000 imap-tools-1.1.0/imap_tools/mailbox.py
--rw-rw-rw-   0        0        0     9662 2021-11-25 11:36:59.000000 imap-tools-1.1.0/imap_tools/message.py
--rw-rw-rw-   0        0        0    16320 2022-08-31 05:00:37.000000 imap-tools-1.1.0/imap_tools/query.py
--rw-rw-rw-   0        0        0     7386 2022-08-31 05:00:37.000000 imap-tools-1.1.0/imap_tools/utils.py
--rw-rw-rw-   0        0        0      522 2023-07-25 09:13:31.000000 imap-tools-1.1.0/imap_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    20633 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11548 2019-10-23 05:52:39.000000 imap-tools-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       56 2021-01-28 06:25:19.000000 imap-tools-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    20633 2023-07-25 09:15:33.000000 imap-tools-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    20123 2023-07-25 09:13:31.000000 imap-tools-1.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-25 09:15:33.000000 imap-tools-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1125 2021-08-06 04:21:06.000000 imap-tools-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:50:27.000000 imap-tools-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-08-01 05:50:27.000000 imap-tools-1.2.0/imap_tools/
+-rw-rw-rw-   0        0        0     1209 2022-03-06 11:54:23.000000 imap-tools-1.2.0/imap_tools/consts.py
+-rw-rw-rw-   0        0        0     2109 2022-02-15 11:27:46.000000 imap-tools-1.2.0/imap_tools/errors.py
+-rw-rw-rw-   0        0        0     7085 2023-07-31 05:50:43.000000 imap-tools-1.2.0/imap_tools/folder.py
+-rw-rw-rw-   0        0        0     4465 2022-11-21 11:14:06.000000 imap-tools-1.2.0/imap_tools/idle.py
+-rw-rw-rw-   0        0        0     2059 2021-09-20 07:00:52.000000 imap-tools-1.2.0/imap_tools/imap_utf7.py
+-rw-rw-rw-   0        0        0    15852 2023-07-25 09:13:31.000000 imap-tools-1.2.0/imap_tools/mailbox.py
+-rw-rw-rw-   0        0        0     9662 2021-11-25 11:36:59.000000 imap-tools-1.2.0/imap_tools/message.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:49:19.000000 imap-tools-1.2.0/imap_tools/py.typed
+-rw-rw-rw-   0        0        0    16320 2022-08-31 05:00:37.000000 imap-tools-1.2.0/imap_tools/query.py
+-rw-rw-rw-   0        0        0     7386 2022-08-31 05:00:37.000000 imap-tools-1.2.0/imap_tools/utils.py
+-rw-rw-rw-   0        0        0      522 2023-07-31 05:52:54.000000 imap-tools-1.2.0/imap_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:50:27.000000 imap-tools-1.2.0/imap_tools.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:50:26.000000 imap-tools-1.2.0/imap_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    20677 2023-08-01 05:50:26.000000 imap-tools-1.2.0/imap_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-08-01 05:50:26.000000 imap-tools-1.2.0/imap_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 05:50:26.000000 imap-tools-1.2.0/imap_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11548 2019-10-23 05:52:39.000000 imap-tools-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       56 2021-01-28 06:25:19.000000 imap-tools-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    20677 2023-08-01 05:50:27.000000 imap-tools-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20167 2023-07-31 05:48:03.000000 imap-tools-1.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-01 05:50:27.000000 imap-tools-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-08-01 05:49:19.000000 imap-tools-1.2.0/setup.py
```

### Comparing `imap-tools-1.1.0/imap_tools/consts.py` & `imap-tools-1.2.0/imap_tools/consts.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/errors.py` & `imap-tools-1.2.0/imap_tools/errors.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/folder.py` & `imap-tools-1.2.0/imap_tools/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 raise MailboxFolderStatusValueError(str(opt))
         status_result = self.mailbox.client._simple_command(
             command, encode_folder(folder), '({})'.format(' '.join(options)))
         check_command_status(status_result, MailboxFolderStatusError)
         result = self.mailbox.client._untagged_response(status_result[0], status_result[1], command)
         check_command_status(result, MailboxFolderStatusError)
         status_data = [i for i in result[1] if type(i) is bytes][0]  # may contain tuples with encoded names
-        values = status_data.decode().split('(')[1].split(')')[0].split(' ')
+        values = status_data.decode().split('(')[-1].split(')')[0].split(' ')
         return {k: int(v) for k, v in pairs_to_dict(values).items() if str(v).isdigit()}
 
     def list(self, folder: AnyStr = '', search_args: str = '*', subscribed_only: bool = False) -> List[FolderInfo]:
         """
         Get a listing of folders on the server
         :param folder: mailbox folder, if empty - get from root
         :param search_args: search arguments, is case-sensitive mailbox name with possible wildcards
```

### Comparing `imap-tools-1.1.0/imap_tools/idle.py` & `imap-tools-1.2.0/imap_tools/idle.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/imap_utf7.py` & `imap-tools-1.2.0/imap_tools/imap_utf7.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/mailbox.py` & `imap-tools-1.2.0/imap_tools/mailbox.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/message.py` & `imap-tools-1.2.0/imap_tools/message.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/query.py` & `imap-tools-1.2.0/imap_tools/query.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/utils.py` & `imap-tools-1.2.0/imap_tools/utils.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/imap_tools/__init__.py` & `imap-tools-1.2.0/imap_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 from .mailbox import BaseMailBox, MailBox, MailBoxUnencrypted, MailBoxTls
 from .message import MailMessage, MailAttachment
 from .folder import MailBoxFolderManager, FolderInfo
 from .consts import MailMessageFlags, MailBoxFolderStatusOptions
 from .utils import EmailAddress
 from .errors import *
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
```

### Comparing `imap-tools-1.1.0/imap_tools.egg-info/PKG-INFO` & `imap-tools-1.2.0/imap_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-tools
-Version: 1.1.0
+Version: 1.2.0
 Summary: Work with email by IMAP
 Home-page: https://github.com/ikvk/imap_tools
 Author: Vladimir Kaukin
 Author-email: KaukinVK@ya.ru
 License: Apache-2.0
 Keywords: imap,imap-client,python3,python,email
 Platform: UNKNOWN
@@ -418,15 +418,16 @@
 `Nicarex <https://github.com/Nicarex>`_,
 `RanjithNair1980 <https://github.com/RanjithNair1980>`_,
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
 `stumpylog <https://github.com/stumpylog>`_,
-`dimitrisstr <https://github.com/dimitrisstr>`_
+`dimitrisstr <https://github.com/dimitrisstr>`_,
+`abionics <https://github.com/abionics>`_
 
 Help the project
 ----------------
 1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
 2. Do not know how to improve library - try to help other open projects that you use ✋
 3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
 4. Star the project ⭐
```

### Comparing `imap-tools-1.1.0/LICENSE` & `imap-tools-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imap-tools-1.1.0/PKG-INFO` & `imap-tools-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-tools
-Version: 1.1.0
+Version: 1.2.0
 Summary: Work with email by IMAP
 Home-page: https://github.com/ikvk/imap_tools
 Author: Vladimir Kaukin
 Author-email: KaukinVK@ya.ru
 License: Apache-2.0
 Keywords: imap,imap-client,python3,python,email
 Platform: UNKNOWN
@@ -418,15 +418,16 @@
 `Nicarex <https://github.com/Nicarex>`_,
 `RanjithNair1980 <https://github.com/RanjithNair1980>`_,
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
 `stumpylog <https://github.com/stumpylog>`_,
-`dimitrisstr <https://github.com/dimitrisstr>`_
+`dimitrisstr <https://github.com/dimitrisstr>`_,
+`abionics <https://github.com/abionics>`_
 
 Help the project
 ----------------
 1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
 2. Do not know how to improve library - try to help other open projects that you use ✋
 3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
 4. Star the project ⭐
```

### Comparing `imap-tools-1.1.0/README.rst` & `imap-tools-1.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,16 @@
 `Nicarex <https://github.com/Nicarex>`_,
 `RanjithNair1980 <https://github.com/RanjithNair1980>`_,
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
 `stumpylog <https://github.com/stumpylog>`_,
-`dimitrisstr <https://github.com/dimitrisstr>`_
+`dimitrisstr <https://github.com/dimitrisstr>`_,
+`abionics <https://github.com/abionics>`_
 
 Help the project
 ----------------
 1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
 2. Do not know how to improve library - try to help other open projects that you use ✋
 3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
 4. Star the project ⭐
```

### Comparing `imap-tools-1.1.0/setup.py` & `imap-tools-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     license='Apache-2.0',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='Vladimir Kaukin',
     author_email='KaukinVK@ya.ru',
     description='Work with email by IMAP',
     keywords=['imap', 'imap-client', 'python3', 'python', 'email'],
+    package_data={"imap_tools": ["py.typed"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     # install_requires=['typing>=3.6.2'],
 )
```

