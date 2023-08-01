# Comparing `tmp/fyers_sdk-2.0.4.tar.gz` & `tmp/fyers_sdk-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.0.4.tar", last modified: Mon Jul 31 10:39:01 2023, max compression
+gzip compressed data, was "fyers_sdk-2.0.6.tar", last modified: Tue Aug  1 07:08:10 2023, max compression
```

## Comparing `fyers_sdk-2.0.4.tar` & `fyers_sdk-2.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.0.4/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.0.4/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.187518 fyers_sdk-2.0.4/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    58588 2023-07-31 10:36:58.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 10:17:48.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.0.4/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.0.4/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.0.4/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.207518 fyers_sdk-2.0.4/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 10:37:07.000000 fyers_sdk-2.0.4/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.207900 fyers_sdk-2.0.6/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.0.6/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:08:10.203900 fyers_sdk-2.0.6/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.0.6/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.179900 fyers_sdk-2.0.6/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.203900 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    59613 2023-08-01 06:57:51.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7508 2023-08-01 07:05:48.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.0.6/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.0.6/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.0.6/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.203900 fyers_sdk-2.0.6/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-01 07:08:10.207900 fyers_sdk-2.0.6/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-01 07:08:05.000000 fyers_sdk-2.0.6/setup.py
```

### Comparing `fyers_sdk-2.0.4/LICENSE.txt` & `fyers_sdk-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.4/PKG-INFO` & `fyers_sdk-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.0.4
+Version: 2.0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.0.4/README.md` & `fyers_sdk-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,18 @@
     def __init__(
         self,
         access_token: str,
         write_to_file: bool = False,
         log_path: Optional[str] = None,
         litemode: bool = False,
         reconnect: bool = False,
-        OnMessage: Optional[Callable] = None,
-        OnError: Optional[Callable] = None,
-        OnOpen: Optional[Callable] = None,
-        OnClose: Optional[Callable] = None,
+        on_message: Optional[Callable] = None,
+        on_error: Optional[Callable] = None,
+        on_connect: Optional[Callable] = None,
+        on_close: Optional[Callable] = None,
     ):
 
         """
         Initialize YourClass instance.
 
         Args:
             access_token (str): The access token used for authentication.
@@ -172,18 +172,18 @@
         self.log_path = log_path
         self.lite = litemode
         self.source = "PythonSDK-1.0.0"
         self.channel_num = 1
         self.channels = []
         self.running_channels = set()
         self.data_type = None
-        self.OnMessage = OnMessage
-        self.OnError = OnError
-        self.OnOpen = OnOpen
-        self.OnClose = OnClose
+        self.OnMessage = on_message
+        self.OnError = on_error
+        self.OnOpen = on_connect
+        self.OnClose = on_close
         self.ack_count = 0
         self.__ws_run = None
         self.write_to_file = write_to_file
         self.background_flag = False
         self.update_count = 0
         self.literesp = {}
         self.channel_symbol = []
@@ -634,23 +634,23 @@
             offset += 2
             string_val = data[offset : offset + field_length].decode("utf-8")
             offset += field_length
 
             if string_val == "K":
 
                 self.On_message(
-                    {
+                    {   "type": defines.AUTH_TYPE,
                         "code": defines.SUCCESS_CODE,
                         "message": defines.AUTH_SUCCESS,
                         "s": defines.SUCCESS,
                     }
                 )
             else:
                 self.On_error(
-                    {
+                    {   "type": defines.AUTH_TYPE,
                         "code": defines.AUTH_ERROR_CODE,
                         "message": defines.AUTH_FAIL,
                         "s": defines.ERROR,
                     }
                 )
 
             offset += 1
@@ -679,23 +679,25 @@
             field_length = struct.unpack("H", data[offset : offset + 2])[0]
             offset += 2
             string_val = data[offset : offset + 1].decode("latin-1")
             offset += field_length
             if string_val == "K":
 
                 self.On_message(
-                    {
+                    {   
+                        "type": defines.SUBS_TYPE,
                         "code": defines.SUCCESS_CODE,
                         "message": defines.SUBSCRIBE_SUCCESS,
                         "s": defines.SUCCESS,
                     }
                 )
             else:
                 self.On_error(
                     {
+                        "type": defines.SUBS_TYPE,
                         "code": defines.SUBS_ERROR_CODE,
                         "message": defines.SUBSCRIBE_FAIL,
                         "s": defines.ERROR,
                     }
                 )
 
         except Exception as e:
@@ -720,14 +722,15 @@
             offset += 2
             string_val = data[offset : offset + 1].decode("latin-1")
             offset += field_length
             if string_val == "K":
 
                 self.On_message(
                     {
+                        "type": defines.UNSUBS_TYPE,
                         "code": defines.SUCCESS_CODE,
                         "message": defines.UNSUBSCRIBE_SUCCESS,
                         "s": defines.SUCCESS,
                     }
                 )
                 for symbol in self.unsub_symbol:
                     count = 0
@@ -740,14 +743,15 @@
                         self.scrips_per_channel[self.active_channel].remove(symbol)
                     if count == 1:
                         self.symbol_token.pop(symbol)
                             
             else:
                 self.On_error(
                     {
+                        "type": defines.UNSUBS_TYPE,
                         "code": defines.UNSUBS_ERROR_CODE,
                         "message": defines.UNSUBSCRIBE_FAIL,
                         "s": defines.ERROR,
                     }
                 )
 
         except Exception as e:
@@ -784,22 +788,24 @@
                 string_val = data[offset : offset + field_length].decode("utf-8")
                 offset += field_length
 
                 if string_val == "K":
                     if self.lite:
                         self.On_message(
                             {
+                                "type": defines.LITE_MODE_TYPE,
                                 "code": defines.SUCCESS_CODE,
                                 "message": defines.LITE_MODE,
                                 "s": defines.SUCCESS,
                             }
                         )
                     else:
                         self.On_message(
                             {
+                                "type": defines.FULL_MODE_TYPE,
                                 "code": defines.SUCCESS_CODE,
                                 "message": defines.FULL_MODE,
                                 "s": defines.SUCCESS,
                             }
                         )
                 else:
                     self.On_error(
@@ -808,14 +814,78 @@
                             "message": defines.MODE_CHANGE_ERROR,
                             "s": defines.ERROR,
                         }
                     )
 
         except Exception as e:
             self.data_logger.exception(e)
+        
+    def __resume_pause_resp(self, data: bytearray, channeltype: int) -> dict:
+        """
+        Unpacks and processes the resume/pause response data based on the channel type.
+
+        Args:
+            data (bytearray): The response data.
+            channeltype (int): The channel type. 7 for pause and 8 for resume.
+
+        Returns:
+            dict: The resume/pause response as a dictionary with keys 'code', 'message', and 's'.
+        """
+        try:
+            offset = 5
+
+            # Unpack the field length
+            field_length = struct.unpack("!H", data[offset : offset + 2])[0]
+            offset += 2
+
+            # Extract the string value and decode it
+            string_val = data[offset : offset + field_length].decode("utf-8")
+            offset += field_length
+
+            if string_val == "K":
+                if channeltype == 7:
+                    self.On_message(
+                        {
+                            "type": defines.CH_PAUSE_TYPE,
+                            "code": defines.SUCCESS_CODE,
+                            "message": defines.CHANNEL_PAUSED,
+                            "s": defines.SUCCESS,
+                        }
+                    )
+                else:
+                    self.On_message(
+                        {
+                            "type": defines.CH_RESUME_TYPE,
+                            "code": defines.SUCCESS_CODE,
+                            "message": defines.CHANNEL_RESUMED,
+                            "s": defines.SUCCESS,
+                        }
+                    )
+            else:
+                if channeltype == 7:
+                    self.On_error(
+                        {
+                            "type": defines.CH_PAUSE_TYPE,
+                            "code": defines.PAUSE_ERROR_CODE,
+                            "message": defines.CHANNEL_CHANGE_FAIL,
+                            "s": defines.ERROR,
+                        }
+                    )
+                else:
+                    self.On_error(
+                        {
+                            "type": defines.CH_RESUME_TYPE,
+                            "code": defines.RESUME_ERROR_CODE,
+                            "message": defines.CHANNEL_CHANGE_FAIL,
+                            "s": defines.ERROR,
+                        }
+                    )
+
+        except Exception as e:
+            self.data_logger.exception(e)
 
     def __response_output(self, data: str, data_type: str) -> object:
 
         """
         Processes the response data and returns the output based on the specified data_type.
 
         Args:
@@ -863,17 +933,17 @@
                             20
                         ]:
                             response[val] = data_resp[val] / (
                                 10 ** data_resp["precision"]
                             )
                         elif val in data_resp:
                             response[val] = data_resp[val]
-                    if "close_price" in response and "ltp" in response:
-                        response["ch"] = round((response['ltp']  - response['close_price']),2) 
-                        response["chp"] = round((response["ch"]  / response['close_price'] * 100) , 2)
+                    if "prev_close_price" in response and "ltp" in response:
+                        response["ch"] = round((response['ltp']  - response['prev_close_price']),2) 
+                        response["chp"] = round((response["ch"]  / response['prev_close_price'] * 100) , 2)
                     if "OI" in response:
                         response.pop("OI")
                     if "Yhigh" in response:
                         response.pop("Yhigh")
                     if "Ylow" in response:
                         response.pop("Ylow")
                 else:
@@ -959,14 +1029,15 @@
                             ]
                             offset += 1
                             string_data = data[offset : offset + string_len].decode(
                                 "utf-8"
                             )
                             self.resp[self.dp_sym[topic_id]][val[i]] = string_data
                             offset += string_len
+                        self.resp[self.dp_sym[topic_id]]["type"] = "dp"
                         self.resp[topic_name]["symbol"] = self.symbol_token[topic_name]
                         self.__response_output(
                             self.resp[self.dp_sym[topic_id]], "depth"
                         )
 
                     elif topic_name[:2] == "if":
 
@@ -1003,15 +1074,15 @@
                             offset += 1
                             string_data = data[offset : offset + string_len].decode(
                                 "utf-8"
                             )
                             self.resp[self.index_sym[topic_id]][val[i]] = string_data
                             offset += string_len
                         self.resp[topic_name]["symbol"] = self.symbol_token[topic_name]
-
+                        self.resp[self.index_sym[topic_id]]["type"] = "if"
                         self.__response_output(
                             self.resp[self.index_sym[topic_id]], "index"
                         )
 
                     elif topic_name[:2] == "sf":
                         self.scrips_sym[topic_id] = topic_name
                         self.resp[self.scrips_sym[topic_id]] = {}
@@ -1044,14 +1115,15 @@
                             offset += 1
                             string_data = data[offset : offset + string_len].decode(
                                 "utf-8"
                             )
                             self.resp[self.scrips_sym[topic_id]][val[i]] = string_data
                             offset += string_len
                         self.resp[topic_name]["symbol"] = self.symbol_token[topic_name]
+                        self.resp[self.scrips_sym[topic_id]]["type"] = "sf"
                         self.__response_output(
                             self.resp[self.scrips_sym[topic_id]], "scrips"
                         )
 
                 elif data_type == 85:  # Full mode datafeed
                     offset += 1
                     topic_id = struct.unpack("H", data[offset : offset + 2])[0]
@@ -1122,73 +1194,14 @@
                         self.__response_output(
                             self.resp[self.index_sym[topic_id]], "index"
                         )
 
         except Exception as e:
             self.data_logger.exception(e)
 
-    def __resume_pause_resp(self, data: bytearray, channeltype: int) -> dict:
-        """
-        Unpacks and processes the resume/pause response data based on the channel type.
-
-        Args:
-            data (bytearray): The response data.
-            channeltype (int): The channel type. 7 for pause and 8 for resume.
-
-        Returns:
-            dict: The resume/pause response as a dictionary with keys 'code', 'message', and 's'.
-        """
-        try:
-            offset = 5
-
-            # Unpack the field length
-            field_length = struct.unpack("!H", data[offset : offset + 2])[0]
-            offset += 2
-
-            # Extract the string value and decode it
-            string_val = data[offset : offset + field_length].decode("utf-8")
-            offset += field_length
-
-            if string_val == "K":
-                if channeltype == 7:
-                    self.On_message(
-                        {
-                            "code": defines.SUCCESS_CODE,
-                            "message": defines.CHANNEL_PAUSED,
-                            "s": defines.SUCCESS,
-                        }
-                    )
-                else:
-                    self.On_message(
-                        {
-                            "code": defines.SUCCESS_CODE,
-                            "message": defines.CHANNEL_RESUMED,
-                            "s": defines.SUCCESS,
-                        }
-                    )
-            else:
-                if channeltype == 7:
-                    self.On_error(
-                        {
-                            "code": defines.PAUSE_ERROR_CODE,
-                            "message": defines.CHANNEL_CHANGE_FAIL,
-                            "s": defines.ERROR,
-                        }
-                    )
-                else:
-                    self.On_error(
-                        {
-                            "code": defines.RESUME_ERROR_CODE,
-                            "message": defines.CHANNEL_CHANGE_FAIL,
-                            "s": defines.ERROR,
-                        }
-                    )
-
-        except Exception as e:
-            self.data_logger.exception(e)
 
     def __response_msg(self, data: bytearray):
         """
         Processes the response message based on the response type and calls the corresponding function.
 
         Args:
             data (bytearray): The response data.
@@ -1261,15 +1274,15 @@
                     flag = True
             if flag:
                 self.On_error(
                     {
                         "code": defines.INVALID_CODE,
                         "message": defines.INVALID_SYMBOLS,
                         "s": defines.ERROR,
-                        "symbols": wrong_symbols,
+                        "invalid_symbols": wrong_symbols,
                     }
                 )
 
             return symbol_dict
 
         except Exception as e:
             self.data_logger.exception(e)
@@ -1525,14 +1538,21 @@
         t = Thread(target=self.infinite_loop)
         t.start()
 
     def infinite_loop(self):
         while self.__ws_run:
             pass
 
+
+    def is_connected(self):
+        if self.__ws_object:
+            return True
+        else:
+            return False
+
     def unsubscribe(
         self, symbols: list, data_type: str = "SymbolUpdate", channel: int = 1
     ):
         """
         Unsubscribes from real-time data updates for the specified symbols.
 
         Args:
```

### Comparing `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/defines.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 SUCCESS_CODE = 200
 INVALID_CODE = -300
 TOKEN_EXPIRED = -99
 LIMIT_EXCEED_CODE = -99
 LIMIT_EXCEED_MSG_200 = "Please provide less than 200 symbols"
 LIMIT_EXCEED_MSG_500 = "Please provide less than 500 symbols"
 TOKEN_EXPIRED_MSG = "Token is expired"
-WRONG_CHANNEL_MSG = (
-    "Please provide valid symbol"
-)
 INVALID_TOKEN = "Please provide valid token"
-SUCCESS = "Ok"
+SUCCESS = "ok"
 ERROR = "error"
 AUTH_SUCCESS = "Authentication done"
 AUTH_FAIL = "Authentication failed"
 SUBSCRIBE_SUCCESS = "Subscribed"
 SUBSCRIBE_FAIL = "subscription failed"
 UNSUBSCRIBE_SUCCESS = "Unsubscribed"
 UNSUBSCRIBE_FAIL = "unsubscription failed"
@@ -27,7 +24,14 @@
 FULL_MODE = "Full Mode On"
 MODE_CHANGE_ERROR = "Mode change failed"
 CHANNEL_PAUSED = "Channel Paused"
 CHANNEL_RESUMED = "Channel Resumed"
 CHANNEL_CHANGE_FAIL = "Mode change failed"
 INVALID_SYMBOLS = "Please provide a valid symbol"
 CONNECTION_CLOSED = "Connection Closed"
+AUTH_TYPE = "cn"
+SUBS_TYPE = "sub"
+UNSUBS_TYPE = "unsub"
+LITE_MODE_TYPE = "lit"
+FULL_MODE_TYPE = "ful"
+CH_PAUSE_TYPE = "cp"
+CH_RESUME_TYPE = "cr"
```

### Comparing `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/map.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9390625%*

 * *Differences: {"'data_val'": "{insert: [(3, 'exch_feed_time'), (20, 'prev_close_price'), (21, 'type')], delete: "*

 * *               '[20, 3]}',*

 * * "'depthvalue'": "{insert: [(30, 'type')]}",*

 * * "'index_val'": "{insert: [(1, 'prev_close_price'), (2, 'exch_feed_time'), (6, 'type')], delete: "*

 * *                '[2, 1]}'}*

```diff
@@ -1,13 +1,13 @@
 {
     "data_val": [
         "ltp",
         "vol_traded_today",
         "last_traded_time",
-        "ExFeedTime",
+        "exch_feed_time",
         "bidSize",
         "askSize",
         "bidPrice",
         "askPrice",
         "last_traded_qty",
         "tot_buy_qty",
         "tot_sell_qty",
@@ -16,15 +16,16 @@
         "low_price",
         "high_price",
         "Yhigh",
         "Ylow",
         "lowCircuit",
         "upCircuit",
         "open_price",
-        "close_price",
+        "prev_close_price",
+        "type",
         "symbol"
     ],
     "depthvalue": [
         "bidPrice1",
         "bidPrice2",
         "bidPrice3",
         "bidPrice4",
@@ -50,14 +51,15 @@
         "bidorder4",
         "bidorder5",
         "askorder1",
         "askorder2",
         "askorder3",
         "askorder4",
         "askorder5",
+        "type",
         "symbol"
     ],
     "exch_seg_dict": {
         "1010": "nse_cm",
         "1011": "nse_fo",
         "1012": "cde_fo",
         "1120": "mcx_fo",
@@ -189,19 +191,20 @@
         "NSE:NIFTYSMLCAP100-INDEX": "NIFTY SMLCAP 100",
         "NSE:NIFTYSMLCAP250-INDEX": "NIFTY SMLCAP 250",
         "NSE:NIFTYSMLCAP50-INDEX": "NIFTY SMLCAP 50",
         "NSE:NIFTYTOTALMKT-INDEX": "NIFTY TOTAL MKT"
     },
     "index_val": [
         "ltp",
-        "close_price",
-        "ExFeedTime",
+        "prev_close_price",
+        "exch_feed_time",
         "high_price",
         "low_price",
         "open_price",
+        "type",
         "symbol"
     ],
     "lite_val": [
         "ltp",
         "symbol"
     ]
 }
```

### Comparing `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.4/fyers_sdk/fyersModel.py` & `fyers_sdk-2.0.6/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.4/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.0.6/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.4/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.0.6/fyers_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.0.4
+Version: 2.0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.0.4/setup.py` & `fyers_sdk-2.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.0.4',
+     version='2.0.6',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
@@ -18,15 +18,16 @@
      },
      include_package_data=True,
      install_requires=[
                 'requests==2.31.0',
                 'asyncio==3.4.3',
                 'aiohttp==3.8.4',
                 'aws_lambda_powertools==1.25.5',
-                'websocket-client==1.6.1'
+                'websocket-client==1.6.1',
+                'pkg_resources'
           ],
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
  )
```

