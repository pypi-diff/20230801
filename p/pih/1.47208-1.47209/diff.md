# Comparing `tmp/pih-1.47208.tar.gz` & `tmp/pih-1.47209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47208.tar", last modified: Tue Aug  1 00:20:19 2023, max compression
+gzip compressed data, was "pih-1.47209.tar", last modified: Tue Aug  1 00:43:39 2023, max compression
```

## Comparing `pih-1.47208.tar` & `pih-1.47209.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 00:20:18.027718 pih-1.47208/
-drwxrwxrwx   0        0        0        0 2023-08-01 00:20:18.308965 pih-1.47208/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47208/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-1.47208/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47208/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-1.47208/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47208/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      261 2023-08-01 00:20:19.418329 pih-1.47208/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 00:20:19.168326 pih-1.47208/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47208/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47208/pih/collection.py
--rw-rw-rw-   0        0        0    61070 2023-08-01 00:19:29.000000 pih-1.47208/pih/console_api.py
--rw-rw-rw-   0        0        0   111143 2023-07-31 23:11:49.000000 pih-1.47208/pih/const.py
--rw-rw-rw-   0        0        0   316737 2023-08-01 00:20:11.000000 pih-1.47208/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47208/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47208/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47208/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47208/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47208/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47208/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47208/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47208/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 00:20:19.371450 pih-1.47208/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 00:20:16.000000 pih-1.47208/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47208/pih_mio_setup.py
--rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47208/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 00:20:19.465197 pih-1.47208/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 00:43:39.335830 pih-1.47209/
+drwxrwxrwx   0        0        0        0 2023-08-01 00:43:26.379178 pih-1.47209/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47209/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-1.47209/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47209/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-1.47209/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47209/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      261 2023-08-01 00:43:39.288938 pih-1.47209/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 00:43:37.169285 pih-1.47209/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47209/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47209/pih/collection.py
+-rw-rw-rw-   0        0        0    61071 2023-08-01 00:38:40.000000 pih-1.47209/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47209/pih/const.py
+-rw-rw-rw-   0        0        0   317174 2023-08-01 00:40:47.000000 pih-1.47209/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47209/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47209/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47209/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47209/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47209/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47209/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47209/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47209/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 00:43:38.897071 pih-1.47209/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-08-01 00:43:23.000000 pih-1.47209/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47209/pih_mio_setup.py
+-rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47209/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 00:43:39.367074 pih-1.47209/setup.cfg
```

### Comparing `pih-1.47208/MobileHelperCore/api.py` & `pih-1.47209/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/MobileHelperCore/service.py` & `pih-1.47209/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/MobileHelperCore/service_api.py` & `pih-1.47209/MobileHelperCore/service_api.py`

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

### Comparing `pih-1.47208/MobileHelperCore/tools.py` & `pih-1.47209/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/collection.py` & `pih-1.47209/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/console_api.py` & `pih-1.47209/pih/console_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         return self.pih.output
 
     @property
     def input(self) -> Input:
         return self.pih.input
 
     def send_whatsapp_message(self, telephone_number: str, message: str) -> bool:
-        return A.ME_WH_W.send(telephone_number, message, A.CT_ME_WH_W.PROFILE.IT)
+        return A.ME_WH_W.send(telephone_number, message, A.CT_ME_WH_W.Profiles.IT)
 
     def mark_find(self, value: str | None = None) -> None:
         self.output.mark.by_any(value or self.input.mark.any())
 
     def arg(self, index: int = 0, default_value: Any | None = None) -> Any:
         return self.session.arg(index, default_value)
```

### Comparing `pih-1.47208/pih/const.py` & `pih-1.47209/pih/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,15 @@
                 URL_SEND_DOCUMENT: str = f"{URL_MESSAGE}/document/send?{PROFILE_SUFFIX}"
                 URL_SEND_LIST_MESSAGE: str = f"{URL_MESSAGE}/list/send?{PROFILE_SUFFIX}"
                 URL_SEND_BUTTONS_MESSAGE: str = f"{URL_MESSAGE}/buttons/send?{PROFILE_SUFFIX}"
                 URL_GET_MESSAGES: str = f"{URL_MESSAGE}s/get?{PROFILE_SUFFIX}"
                 URL_GET_STATUS: str = f"{URL_API_SYNC}/get/status?{PROFILE_SUFFIX}"
                 CONTACT_SUFFIX: str = "@c.us"
 
-                class PROFILE(Enum):
+                class Profiles(Enum):
                     IT: str = "e6706eaf-ae17"
                     CALL_CENTRE: str = "81b820f8-cd6e"
                     MARKETER: str = "c31db01c-b6d6"
                     DEFAULT: str = CALL_CENTRE
                     
                 AUTHORIZATION: str = "6b356d3f53124af3078707163fdaebca3580dc38"
```

### Comparing `pih-1.47208/pih/pih.py` & `pih-1.47209/pih/pih.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         raise NotImplemented()
 
 class ServiceListener:
     
     def __init__(self):
         self.service: IService | None = None
         self.service_command_list: list[ServiceCommands] = None
-        self.host: str = A.OS.host()
+        self.host: str = PIH.OS.host()
         self.port: int = NetworkTool.next_free_port()
 
     def listen_for(self, service_command_list: list[ServiceCommands], handler: Callable[[ServiceCommands, ParameterList, IClosable], Any]) -> None:     
         self.service_command_list = service_command_list
   
         def service_starts_handler(service: IService) -> None:
             self.service = service
@@ -631,15 +631,15 @@
             if once and self.authenticated:
                 return True
             self.output.green("Инициализация...")
             self.output.clear_screen()
             self.output.pih_title()
             if PIH.SERVICE.check_accessibility(ServiceRoles.AD): 
                 login: str = PIH.OS.get_login()
-                self.output.head1(f"{FullNameTool.to_given_name(A.R_U.by_login(login, cached=False).data.name)}, пожалуйста, пройдите аутентификацию...")
+                self.output.head1(f"{FullNameTool.to_given_name(PIH.RESULT.USER.by_login(login, cached=False).data.name)}, пожалуйста, пройдите аутентификацию...")
                 self.output.new_line()
                 if not self.input.yes_no(f"Использовать логин '{login}'", True):
                     login = PIH.input.login()
                 password: str = PIH.input.password(is_new=False)
                 if DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.authenticate, (login, password))):
                     self.authenticated = True
                     self.start(login, False)
@@ -1605,15 +1605,15 @@
         ANSWER: dict[str, list[str]] = defaultdict(list)
 
         @staticmethod
         def create_output(recipient: str | Enum, say_hello: bool = True) -> Output:
             from MobileHelperCore.api import MobileOutput, MobileSession, Flags, format_given_name
             recipient = recipient if isinstance(recipient, str) else EnumTool.get(recipient)
             session: MobileSession = MobileSession(recipient, EnumTool.get(Flags.SILENCE))
-            recipient_as_whatsapp_group: bool = recipient.endswith(A.CT_ME_WH.GROUP_SUFFIX)
+            recipient_as_whatsapp_group: bool = recipient.endswith(CONST.MESSAGE.WHATSAPP.GROUP_SUFFIX)
             output: MobileOutput = MobileOutput(session)
             session.output = output
             if say_hello and not recipient_as_whatsapp_group:
                 session.say_hello()
             if not recipient_as_whatsapp_group:
                 output.user.get_formatted_given_name = lambda: format_given_name(session, output)
             return output
@@ -1636,15 +1636,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48016"  
 
         @staticmethod
         def local() -> str:
-            return "1.47208"
+            return "1.47209"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -1891,17 +1891,17 @@
                 return PIH.SETTINGS.get(SETTINGS.RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES)
 
 
         class POLIBASE:
 
             @staticmethod
             def test_recipient(sender: Any) -> str | None:
-                if sender == CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.CALL_CENTRE.value:
+                if sender == CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.CALL_CENTRE.value:
                     return PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_VISIT_NOTIFICATION_TEST_TELEPHONE_NUMBER)
-                if sender == CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.MARKETER.value:
+                if sender == CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.MARKETER.value:
                     return PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_TEST_TELEPHONE_NUMBER)
                 return None
             
             class REVIEW_NOTIFICATION:
 
                 @staticmethod
                 def start_time() -> datetime:
@@ -1960,27 +1960,27 @@
                 ["query", "user", "/server:" + host], True, True, False))
             result |= get_login_list(PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
                 ["query", "user", "/server"], host, interactive=None, run_from_system_account=True), True, True, False))
             return list(result)
 
         @staticmethod
         def stop_windows_service(name: str, workstation_name: str) -> bool:
-            output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+            output: str = PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
                 ["sc", "stop", name], workstation_name,  interactive=True, run_from_system_account=True), True, True).stdout
             return output.find("3  STOP_PENDING") != -1
 
         @staticmethod
         def start_windows_service(name: str, workstation_name: str) -> bool:
-            output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+            output: str = PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
             ["sc", "start", name], workstation_name, interactive=True, run_from_system_account=True), True, True).stdout
             return output.find("2  START_PENDING") != -1 
 
         @staticmethod
         def windows_service_running(name: str, workstation_name: str) -> bool:
-            output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+            output: str = PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
             ["sc", "query", name], workstation_name, interactive=True), True, True).stdout
             return output.find("4  RUNNING") != -1
 
         @staticmethod
         def ping(address_or_ip: str, host: str | None = None, count: int = 1, timeout: int = 100):
             command_list: list[str] = ["ping", "-4",  address_or_ip, "-n",
                                        str(count), "-w", str(timeout)]
@@ -2060,15 +2060,15 @@
 
         @staticmethod
         def kill_python_process(host: str, via_taskkill: bool) -> bool:
             return PIH.PSTOOLS.kill_process(CONST.PYTHON.EXECUTOR, host, via_taskkill)
 
         @staticmethod
         def _ws_action(value: str, host: str, show_output: bool = False) -> bool:
-            return PIH.PSTOOLS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+            return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
                 ["shutdown", value, "/t", "0"], host), show_output).returncode == 0
 
         @staticmethod
         def ws_reboot(host: str, show_output: bool = False) -> bool:
             return PIH.PSTOOLS._ws_action("/r", host, show_output)
 
         @staticmethod
@@ -2136,19 +2136,19 @@
             @staticmethod
             def polibase_person_with_inaccessable_email_was_detected(person: PolibasePerson | None = None, registrator_person: PolibasePerson | None = None, actual: bool = False) -> tuple[Events | tuple[Any]] | Events:
                 def get_information() -> tuple[Any]:
                     workstation_name: str = "<не определён>"
                     workstation_description: str = "<не определён>"
                     if actual:
                         try:
-                            user: User = A.R_U.by_polibase_pin(
+                            user: User = PIH.RESULT.USER.by_polibase_pin(
                                 registrator_person.pin).data
-                            workstation: Workstation = A.R.get_first_item(
-                                A.R_WS.by_login(user.samAccountName)) or A.R_WS.by_name(A.CT.TEST.WORKSTATION_MAME).data
-                            if A.D.is_not_none(workstation):
+                            workstation: Workstation = PIH.RESULT.get_first_item(
+                                PIH.RESULT.WORKSTATION.by_login(user.samAccountName)) or PIH.RESULT.WORKSTATION.by_name(CONST.TEST.WORKSTATION_MAME).data
+                            if DataTool.is_not_none(workstation):
                                 workstation_name = workstation.name
                                 workstation_description = workstation.description
                         except NotFound:
                                 pass
                     return (person.FullName, person.pin, person.email, registrator_person.FullName, workstation_name, workstation_description)
                 event: Events = Events.POLIBASE_PERSON_WITH_INACCESSABLE_EMAIL_WAS_DETECTED
                 return PIH.EVENT.BUILDER.create_event(event, registrator_person, get_information, DataTool.check_not_none(person, lambda: (None, person.pin)))
@@ -2433,29 +2433,29 @@
             PIH.EVENT.on_event(internal_handler)
 
 
         @staticmethod
         def on_service_starts(handler_or_service_role_or_information: Callable[[str, Callable[[None], None]], None] | ServiceRoles | ServiceInformationBase) -> None:
             def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
                 event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
-                if event == A.E_B.service_was_started():
+                if event == PIH.EVENT.BUILDER.service_was_started():
                     service_description_name: str = parameters[0]
                     if callable(handler_or_service_role_or_information):
                         handler_or_service_role_or_information(service_description_name, listener.close)
                     elif handler_or_service_role_or_information == service_description_name:
                         listener.close()
             PIH.EVENT.on_event(internal_handler)
         
         @staticmethod
         def on_robocopy_job_complete(handler_or_robocopy_job_name: Callable[[str, int, ServiceListener], None] | str) -> bool | None:
             class DATA_HOLDER:
                 result: bool | None = None
             def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
                 event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
-                if event == A.CT_E.BACKUP_ROBOCOPY_JOB_WAS_COMPLETED:
+                if event == Events.BACKUP_ROBOCOPY_JOB_WAS_COMPLETED:
                     robocopy_job_status_name: str = parameters[0]
                     robocopy_job_status: int = parameters[-1]
                     DATA_HOLDER.result = robocopy_job_status < ROBOCOPY.ERROR_CODE_START
                     if callable(handler_or_robocopy_job_name):
                         handler_or_robocopy_job_name(
                             robocopy_job_status_name, robocopy_job_status, listener)
                     else:
@@ -2530,25 +2530,25 @@
 
         class ADMIN:
 
             SERVICE_INFORMATION_MAP: dict[ServiceInformationBase, ServiceInformation] = {}
 
             @staticmethod
             def change_host_on_local(role_or_information: ServiceRoles | ServiceInformationBase) -> None:
-                ServiceRoles.description(role_or_information).host = A.OS.host()
+                ServiceRoles.description(role_or_information).host = PIH.OS.host()
 
             @staticmethod
             def service_information_list() -> list[ServiceInformation]:
                 return DataTool.to_list(PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP)
 
             @staticmethod
             def kill_all(via_pskill: bool = False, local: bool = False) -> bool:
                 hosts: set[str] = set()
-                for server_role in A.CT_SR:
-                    host: str | None = A.CT_SR.description(server_role).host
+                for server_role in ServiceRoles:
+                    host: str | None = ServiceRoles.description(server_role).host
                     if not DataTool.is_empty(host):
                         hosts.add(host)
                 def kill(host: str, local: bool, via_pskill: bool) -> None:
                     if local:
                         PIH.PSTOOLS.kill_python_process(host, via_pskill)
                     else:
                         PIH.ACTION.WORKSTATION.kill_python_process(host, via_pskill)
@@ -2571,16 +2571,16 @@
             def create_developer_service_description(port: int = None) -> ServiceDescription:
                 if port is None or port == ServiceRoles.DEVELOPER.value.port:
                     return ServiceRoles.DEVELOPER.value
                 return ServiceDescription(f"Developer_{port}", host=CONST.HOST.DEVELOPER.NAME, port=CONST.RPC.PORT(port))
 
             @staticmethod
             def create_support_service_or_master_service_description(master_service_desctiption: ServiceDescription, host: str | None = None) -> ServiceDescription:
-                if A.SRV.check_accessibility(master_service_desctiption):
-                    host = host or A.OS.host()
+                if PIH.SERVICE.check_accessibility(master_service_desctiption):
+                    host = host or PIH.OS.host()
                     if master_service_desctiption.host != host:
                         port: int = PIH.SERVICE.create_port(master_service_desctiption)
                         return ServiceDescription(
                             name=":".join([f"{PIH.SERVICE.SUPPORT_NAME_PREFIX}{master_service_desctiption.name}", host]),
                             description=f"Support service for {master_service_desctiption.name} on {host}",
                             host=host,
                             port=port,
@@ -2651,20 +2651,20 @@
                       call_handler: Callable[[ServiceCommands, ParameterList], Any] | None = None, 
                       starts_handler: Callable[[IService | None], None] | None = None, 
                       max_workers: int | None = None, 
                       stop_before: bool = True, 
                       depends_on_list: list[ServiceDescription | ServiceRoles] | None = None, 
                       isolate: bool = False,
                       show_output: bool = True) -> None:
-                host: str = A.OS.host()
-                service_description: ServiceInformationBase = A.CT_SR.description(role_or_information)
+                host: str = PIH.OS.host()
+                service_description: ServiceInformationBase = ServiceDescription.description(role_or_information)
                 if isolate:
                      PIH.SERVICE.ADMIN.isolate(service_description)
                 else:
-                    if not A.D.contains(host, service_description.host):
+                    if not PIH.DATA.contains(host, service_description.host):
                         if service_description.host_changeable:
                             PIH.SERVICE.ADMIN.change_host_on_local(service_description)
                         else:
                             pass
                     if stop_before:
                         if PIH.SERVICE.check_accessibility(service_description):
                             PIH.SERVICE.ADMIN.stop(service_description)
@@ -2694,19 +2694,19 @@
                               internal_start_handler, max_workers, depends_on_list, show_output)
 
             @staticmethod
             def stop(role_or_information: ServiceRoles | ServiceInformationBase, check_on_started: bool = True, direct_call: bool = False) -> bool:
                 description: ServiceDescription = ServiceRoles.description(role_or_information)
                 if not check_on_started or PIH.SERVICE.check_accessibility(description):
                     if PIH.SERVICE.is_service_as_listener(description) or direct_call:
-                        A.SRV.call(description, ServiceCommands.stop_service)
+                        PIH.SERVICE.call(description, ServiceCommands.stop_service)
                         return True
                     service_information: ServiceInformationBase = DataTool.fill_data_from_source(
                             ServiceInformationBase(), PIH.SERVICE.get_information(description))
-                    A.SRV.call(service_information,
+                    PIH.SERVICE.call(service_information,
                                      ServiceCommands.stop_service)
                     return True
                 return False
 
             @staticmethod
             def update_service_information(list: list[ServiceInformation], add: bool = True, overwrite: bool = False) -> None:
                 if overwrite:
@@ -2718,39 +2718,39 @@
                         if item in PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP:
                             del PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP[item]
 
             @staticmethod
             def validate(cached: bool = False, include_isolated: bool = False) -> tuple[list, list]:
                 if not cached:
                     PIH.SERVICE.ADMIN.request_for_service_information_list()
-                service_information_list: list[ServiceInformation] = A.SRV_A.service_information_list()
+                service_information_list: list[ServiceInformation] = PIH.SERVICE.ADMIN.service_information_list()
                 if not include_isolated:
                     service_information_list = list(filter(lambda item: not item.isolated, service_information_list)) 
                 if not DataTool.is_empty(service_information_list):
                     length: int = len(service_information_list)
                     with ThreadPoolExecutor(max_workers=length) as executor:
                         future_to_bool = {executor.submit(
                             PIH.SERVICE.check_accessibility, service_descroption): service_descroption for service_descroption in service_information_list}
                         offline_service_list: list[ServiceInformation] = []
                         for value in futures.as_completed(future_to_bool):
                             if not value.result():
                                 service_information: ServiceInformation = future_to_bool[value]
                                 offline_service_list.append(service_information)
                                 service_information_list.remove(service_information)
                                 del PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP[service_information]
-                        service_description_list: list[ServiceDescription] = list(filter(lambda item: item.visible_for_admin, map(lambda item: A.CT_SR.description(item), A.CT_SR)))
+                        service_description_list: list[ServiceDescription] = list(filter(lambda item: item.visible_for_admin, map(lambda item: ServiceRoles.description(item), ServiceRoles)))
                         for service_description_item in service_description_list:
                             if service_description_item not in service_information_list:
                                 offline_service_list.append(service_description_item)
                         return offline_service_list, service_information_list
                 return [], []  
 
             @staticmethod
             def request_for_service_information_list() -> None:
-                PIH.SERVICE.ADMIN.update_service_information(list(map(PIH.DATA.EXTRACT.service_information, DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.get_service_information_table, ((RPC.service_information or A.CT_SR.STUB).name), )) or [])), True, True)
+                PIH.SERVICE.ADMIN.update_service_information(list(map(PIH.DATA.EXTRACT.service_information, DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.get_service_information_table, ((RPC.service_information or ServiceRoles.STUB).name), )) or [])), True, True)
                   
         @staticmethod
         def check_accessibility(role_or_information: ServiceRoles | ServiceInformationBase, cached: bool = False) -> bool:
             return not DataTool.is_empty(PIH.SERVICE.get_information(role_or_information, cached))
         
         @staticmethod
         def is_service_as_listener(information: ServiceInformationBase) -> bool:
@@ -2878,15 +2878,15 @@
         @staticmethod
         def get_file_list_by_directory_info(path: str) -> list[str] | None:
             return PIH.PATH.get_file_list(path, DataTool.if_not_empty(PIH.RESULT.DATA_STORAGE.value(PIH.PATH.get_directory_info_name(
                 None, path), DirectoryInfo()).data, lambda info: info.last_created_file_timestamp))
 
         @staticmethod
         def get_directory_info_name(file_path: str | None, directory_path: str | None = None) -> float :
-            return  PIH.PATH.DIRECTORY_INFO_PREFIX + (directory_path or A.PTH.get_file_directory(file_path))
+            return  PIH.PATH.DIRECTORY_INFO_PREFIX + (directory_path or PIH.PATH.get_file_directory(file_path))
 
         @staticmethod
         def save_timestamp_for_directory_info(path: str) -> None:
             PIH.ACTION.DATA_STORAGE.value(DirectoryInfo(path, DateTimeTool.now().timestamp()),
                         PIH.PATH.get_directory_info_name(path))
 
         @staticmethod
@@ -3047,22 +3047,22 @@
                         menu_json = json.loads(manu_text)
                         for menu_json_item in menu_json["menu"]:
                             result.append(CommandMenuItem(menu_json_item["command"], menu_json_item["label"]))
                 return value, result
 
             @staticmethod
             def new_mail_message(value: dict) -> NewMailMessage:
-                return A.D.fill_data_from_source(NewMailMessage(), value)
+                return DataTool.fill_data_from_source(NewMailMessage(), value)
 
             @staticmethod
             def mailbox_info(value: dict | None) -> MailboxInfo | None:
                 if DataTool.is_none(value):
                     return None
-                result: MailboxInfo = A.D.fill_data_from_source(MailboxInfo(), value)
-                result.timestamp = A.D.datetime_from_string(result.timestamp)
+                result: MailboxInfo = DataTool.fill_data_from_source(MailboxInfo(), value)
+                result.timestamp = DataTool.datetime_from_string(result.timestamp)
                 return result
 
             @staticmethod
             def polibase_person(value: dict) -> PolibasePerson:
                 polibase_person: PolibasePerson = DataTool.fill_data_from_source(PolibasePerson(), value)
                 polibase_person.Birth = DateTimeTool.datetime_from_string(polibase_person.Birth)
                 polibase_person.registrationDate = DateTimeTool.datetime_from_string(polibase_person.registrationDate )
@@ -3097,15 +3097,15 @@
                         return True
                     if value == 0:
                         return False
                 return None
             
             @staticmethod
             def service_information(value: dict | ServiceInformation) -> ServiceInformation:
-                service_information: ServiceInformation = A.D.fill_data_from_source(ServiceInformation(), value) if isinstance(value, dict) else value
+                service_information: ServiceInformation = DataTool.fill_data_from_source(ServiceInformation(), value) if isinstance(value, dict) else value
                 if not DataTool.is_empty(service_information.subscribtions):
                     service_information.subscribtions = DataTool.fill_data_from_list_source(Subscribtion, service_information.subscribtions)   
                 return service_information
 
             @staticmethod
             def wappi_telephone_number(value: Any) -> str:
                 if isinstance(value, str):
@@ -3132,15 +3132,15 @@
                 def whatsapp_message(parameter_list: ParameterList) -> WhatsAppMessage | None:
                     allow: bool = PIH.DATA.EXTRACT.subscribtion_result(parameter_list).result
                     message: WhatsAppMessage | None = None
                     if allow:
                         event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
                         if event == Events.WHATSAPP_MESSAGE_RECEIVED:
                             message = DataTool.fill_data_from_source(WhatsAppMessage(), parameters[0])
-                            if not A.D_C.empty(message.message):
+                            if not DataTool.is_empty(message.message):
                                 message.message = urllib.parse.unquote(message.message)
                     return message
                 
                 @staticmethod
                 def action(parameters: dict[str, Any]) -> ActionWasDone:
                     action: ActionWasDone = DataTool.fill_data_from_source(ActionWasDone(), PIH.EVENT.get_parameter(Events.ACTION_WAS_DONE, parameters), copy_by_index=True)
                     action.action = EnumTool.get(Actions, action.action)
@@ -3153,15 +3153,15 @@
                 
                 @staticmethod
                 def with_parameters(parameter_list: ParameterList) -> tuple[Events, list[Any]]:
                     event_data: Any | list[Any] = parameter_list.list[0] if PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else parameter_list.list
                     event: Events = EnumTool.get(Events, event_data[0])
                     in_parameters: dict[str, Any] = event_data[1]
                     out_parameters: list[Any] = []
-                    if not A.D_C.empty(event.value.params):
+                    if not DataTool.is_empty(event.value.params):
                         for event_parameters_description in event.value.params:
                             event_parameters_description: ParamItem = event_parameters_description
                             if event_parameters_description.optional:
                                 if DataTool.is_in(in_parameters, event_parameters_description.name):
                                     out_parameters.append(in_parameters[event_parameters_description.name])
                                 else:
                                     out_parameters.append(None)
@@ -3276,20 +3276,20 @@
             def container_dn_from_dn(dn: str) -> str:
                 return ",".join(dn.split(",")[1:])
             
         class CONVERT:
 
             @staticmethod
             def settings_to_datetime(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> datetime | list[datetime]:
-                settings_value: str | list[str] = A.S.get(item)
+                settings_value: str | list[str] = PIH.SETTINGS.get(item)
                 return  PIH.DATA.CONVERT.settings_to_datetime_list(item, format) if isinstance(settings_value, list) else DateTimeTool.datetime_from_string(settings_value, format)
             
             @staticmethod
             def settings_to_datetime_list(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> list[datetime]:
-                return list(map( lambda item: DateTimeTool.datetime_from_string(item, format), A.S.get(item)))
+                return list(map(lambda item: DateTimeTool.datetime_from_string(item, format), PIH.SETTINGS.get(item)))
 
             @staticmethod
             def file_to_base64(path: str) -> str | None:
                 while True:
                     try:
                         with open(path, "rb") as file:
                             return PIH.DATA.CONVERT.bytes_to_base64(file.read())
@@ -3319,15 +3319,15 @@
                     return EnumTool.get(value).key_name == name or value.name == name
                 if is_equal(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER, value):
                     return PIH.DATA.STATISTICS.for_chiller_filter()
                 return None
 
             @staticmethod
             def for_chiller_filter() -> TimeSeriesStatistics | None:
-                events_result: Result[list[EventDS]] = PIH.RESULT.EVENTS.get(*PIH.EVENT.BUILDER.action_was_done(A.CT_ACT.CHILLER_FILTER_CHANGING))
+                events_result: Result[list[EventDS]] = PIH.RESULT.EVENTS.get(*PIH.EVENT.BUILDER.action_was_done(Actions.CHILLER_FILTER_CHANGING))
                 if ResultTool.is_empty(events_result):
                     return None
                 datetime_list: list[datetime] = ResultTool.map(events_result, lambda event: event.timestamp).data
                 distance: list[timedelta] = []
                 for index, _ in enumerate(datetime_list):
                     if index == len(datetime_list) - 1:
                         break
@@ -3461,15 +3461,15 @@
                     return value
                 return ("" if value.startswith(host_start) else host_start) + value 
 
             @staticmethod
             def get_chiller_indications_value_image_name(datetime: datetime | str) -> str:
                 if isinstance(datetime, str):
                     datetime = PIH.DATA.datetime_from_string(datetime, CONST.ISO_DATETIME_FORMAT)
-                return PIH.PATH.replace_prohibited_symbols_from_path_with_symbol(PIH.DATA.datetime_to_string(datetime, A.CT.DATETIME_FORMAT))
+                return PIH.PATH.replace_prohibited_symbols_from_path_with_symbol(PIH.DATA.datetime_to_string(datetime, CONST.DATETIME_FORMAT))
 
             @staticmethod
             def by_formatter_name(value: Enum | str, data: Any | None) -> str | None:
                 if isinstance(value, str):
                     value = EnumTool.get_by_value(DATA.FORMATTER, value) or value
                 if isinstance(value, str):
                     name: str = j((PIH.DATA.STATISTICS.NAME, "_"))
@@ -3488,15 +3488,15 @@
                     return PIH.DATA.FORMAT.date(data)
                 if value == DATA.FORMATTER.CHILLER_FILTER_COUNT:
                     return str(PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER))
                 if value == DATA.FORMATTER.CHILLER_INDICATIONS_VALUE_INDICATORS:
                     result_list: list[str] = [] 
                     for index in range(len(INDICATIONS.CHILLER.INDICATOR_NAME)):
                         if BM.has_index(data, index):
-                            result_list.append(f"{A.CT_V.BULLET} {INDICATIONS.CHILLER.INDICATOR_NAME[index]}")
+                            result_list.append(f"{CONST.VISUAL.BULLET} {INDICATIONS.CHILLER.INDICATOR_NAME[index]}")
                     return "\n".join(("\n", "\n".join(result_list), ""))
                 return None
 
             @staticmethod
             def polibase_person_card_registry_folder(value: str) -> str:         
                 return value.upper()
 
@@ -3627,15 +3627,15 @@
 
             @staticmethod
             def marketer() -> str:
                 return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.USER.MARKETER)
 
             @staticmethod
             def for_wappi(value: Any) -> str | None:
-                WP = CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE
+                WP = CONST.MESSAGE.WHATSAPP.WAPPI.Profiles
                 value = EnumTool.get_by_value_or_key(WP, value)
                 map: dict = PIH.DATA.TELEPHONE_NUMBER.wappi_profile_to_telephone_number_map
                 if DataTool.is_none(map):
                     map = {
                         WP.CALL_CENTRE: PIH.DATA.TELEPHONE_NUMBER.call_centre_administrator(),
                         WP.IT: PIH.DATA.TELEPHONE_NUMBER.it_administrator(),
                         WP.MARKETER: PIH.DATA.TELEPHONE_NUMBER.marketer(),
@@ -4024,15 +4024,15 @@
                         day_end -= timedelta(days=abs(day_start))
                     else:
                         day_end = start_date.replace(day=day_start)
                 return PIH.RESULT.TIME_TRACKING.create(start_date, end_date, tab_number)
 
             @staticmethod
             def create(start_date: datetime | None = None, end_date: datetime | None = None, tab_number_list: list[str] | None = None) -> Result[list[TimeTrackingResultByPerson]]:
-                now: datetime | None = A.D.check(A.D_C.empty(start_date) or A.D_C.empty(end_date), datetime.now())
+                now: datetime | None = DataTool.check(DataTool.is_empty(start_date) or DataTool.is_empty(end_date), datetime.now())
                 start_date = DateTimeTool.start_date(start_date or now)
                 end_date = DateTimeTool.end_date(end_date or now)
 
                 def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str :
                     return DataTool.check_not_none(entity, lambda: entity.TimeVal.split(CONST.DATETIME_SPLITTER)[not date])
                 result_data: dict = {}
                 full_name_by_tab_number_map: dict = {}
@@ -4497,16 +4497,16 @@
 
             @staticmethod
             def has(value: Events | None, parameters: tuple[Any] | None = None) -> bool:
                 return not ResultTool.is_empty(PIH.RESULT.EVENTS.get(value, parameters))
 
             @staticmethod
             def timeouted(event: Events, parameters: dict | None, timeout_in_seconds: int) -> bool:
-                event_ds: EventDS | None = A.R.get_first_item(
-                    A.R.sort(A.R_E.get(event, parameters), lambda item: item.timestamp, reserve=True))
+                event_ds: EventDS | None = PIH.RESULT.get_first_item(
+                    PIH.RESULT.sort(PIH.RESULT.EVENTS.get(event, parameters), lambda item: item.timestamp, reserve=True))
                 return DataTool.is_none(event_ds) or (
                     DateTimeTool.now() - event_ds.timestamp).total_seconds() > timeout_in_seconds
 
         class SETTINGS:
     
             @staticmethod
             def by_time(current: datetime, settings: SETTINGS) -> bool:
@@ -4546,15 +4546,15 @@
                 return PIH.CHECK.RESOURCE.accessibility_by_ping_with_port(address_or_ip, WINDOWS.PORTS.SMB, host, count, check_for_all)
             
             @staticmethod
             def accessibility_by_ping(address_or_ip: str, host: str | None = None, count: int | None = None, check_for_all: bool = True) -> bool:
                 count = count or 4
                 local_ping_commnad_list: list[str] = [PIH.PSTOOLS.get_executor_path(
                     CONST.PSTOOLS.PS_PING), CONST.PSTOOLS.ACCEPTEULA, "-4", "-n", str(count), address_or_ip]
-                process_result: CompletedProcess = A.PS.execute_command_list(local_ping_commnad_list if host is None else A.PS.create_command_list_for_psexec_command(local_ping_commnad_list, host, interactive=True), True, True)
+                process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(local_ping_commnad_list if host is None else PIH.PSTOOLS.create_command_list_for_psexec_command(local_ping_commnad_list, host, interactive=True), True, True)
                 if process_result.returncode == 0:
                     out: str = process_result.stdout
                     lost_marker: str = "Lost = "
                     index: int = out.find(lost_marker)
                     if index != -1:
                         lost_count: int = int(out[index +
                                                 len(lost_marker): out.find(" (", index)])
@@ -4579,15 +4579,15 @@
             
             @staticmethod
             def pacs_accessibility(count: int = 2) -> bool:
                 return PIH.CHECK.RESOURCE.accessibility_by_ping(RESOURCES.DESCRIPTIONS.PACS_SPB.address, CONST.HOST.WS255.NAME, count)
            
             @staticmethod
             def wappi_profile_accessibility(value: Any, cached: bool = False) -> bool:
-                return PIH.CHECK.RESOURCE.accessibility(PIH.RESULT.RESOURCES.get_resource_status(EnumTool.get_value(value, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value))) if cached else PIH.CHECK.MESSAGE.WHATSAPP.WAPPI.accessibility(value, False)
+                return PIH.CHECK.RESOURCE.accessibility(PIH.RESULT.RESOURCES.get_resource_status(EnumTool.get_value(value, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value))) if cached else PIH.CHECK.MESSAGE.WHATSAPP.WAPPI.accessibility(value, False)
 
             @staticmethod
             def ws_accessibility(name: str) -> bool:
                 result: Result[Workstation] = PIH.RESULT.WORKSTATION.by_name(name)
                 return not ResultTool.is_empty(result) and result.data.accessable
             
             @staticmethod
@@ -4705,15 +4705,15 @@
                     def from_me(value: str) -> bool:
                         value = PIH.DATA.FORMAT.telephone_number(value)
                         return value in [PIH.DATA.TELEPHONE_NUMBER.it_administrator(), PIH.DATA.TELEPHONE_NUMBER.call_centre_administrator(), PIH.DATA.TELEPHONE_NUMBER.marketer()]
 
                     @staticmethod
                     def accessibility(profile: Any, cached: bool = True) -> bool:
                         def internal_accessibility(profile: Any | None = None) -> bool:
-                            profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                            profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                             url: str = f"{CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_STATUS}{profile}"
                             headers: dict = {
                                 "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION,
                                 "Content-Type": "application/json"
                             }
                             response_result: dict = None
                             try:
@@ -5025,17 +5025,17 @@
                                 #dont send message - cause workstation is on but no one user is logged
                             else:
                                 if test:
                                     if workstation_name == CONST.TEST.WORKSTATION_MAME:
                                         PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
                                 else:
                                     PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
-                    result_message: str = f"Сообщение от {session.user_given_name} ({A.D_F.description(session.get_user().description)}):"
+                    result_message: str = f"Сообщение от {session.user_given_name} ({PIH.DATA.FORMAT.description(session.get_user().description)}):"
                     result_message += f" День добрый, "
-                    user: User | None = None if DataTool.is_empty(workstation.samAccountName) else A.R_U.by_login(workstation.samAccountName, True, True).data
+                    user: User | None = None if DataTool.is_empty(workstation.samAccountName) else PIH.RESULT.USER.by_login(workstation.samAccountName, True, True).data
                     result_message += DataTool.if_not_empty(user, lambda user: f"{FullNameTool.to_given_name(user)}, ", "")
                     result_message += message
                     PIH.MESSAGE.WORKSTATION.executor.submit(
                         internal_send_message, workstation.samAccountName, workstation.name.lower(), result_message)
                 ResultTool.every(ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function), every_action)
 
             @staticmethod
@@ -5086,53 +5086,53 @@
         class WHATSAPP:
 
             class WAPPI:
 
                 class QUEUE:
     
                     @staticmethod
-                    def add(message: Message, recipient: str, sender: CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE, high_priority: bool = False) -> bool:
+                    def add(message: Message, recipient: str, sender: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles, high_priority: bool = False) -> bool:
                         return PIH.MESSAGE.WHATSAPP.WAPPI.QUEUE.add_message(Message(message, recipient, sender.value), high_priority)
                     
                     @staticmethod
                     def add_message(message: Message, high_priority: bool = False) -> bool:
                         return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.add_message_to_queue, (message, high_priority)))
 
 
                 WAPPI_PROFILE_MAP: dict | None = None 
 
                 @staticmethod
                 def get_wappi_collection() -> dict:
                     WP = CONST.MESSAGE.WHATSAPP.WAPPI
                     result: dict = PIH.MESSAGE.WHATSAPP.WAPPI.WAPPI_PROFILE_MAP or {
-                        WP.PROFILE.IT: PIH.DATA.TELEPHONE_NUMBER.it_administrator(),
-                        WP.PROFILE.CALL_CENTRE: PIH.DATA.TELEPHONE_NUMBER.call_centre_administrator(),
-                        WP.PROFILE.MARKETER: PIH.DATA.TELEPHONE_NUMBER.marketer()
+                        WP.Profiles.IT: PIH.DATA.TELEPHONE_NUMBER.it_administrator(),
+                        WP.Profiles.CALL_CENTRE: PIH.DATA.TELEPHONE_NUMBER.call_centre_administrator(),
+                        WP.Profiles.MARKETER: PIH.DATA.TELEPHONE_NUMBER.marketer()
                     }
                     if PIH.MESSAGE.WHATSAPP.WAPPI.WAPPI_PROFILE_MAP is None:
                         PIH.MESSAGE.WHATSAPP.WAPPI.WAPPI_PROFILE_MAP = result
                     return result
 
                 @staticmethod
-                def send_to_group(group: CONST.MESSAGE.WHATSAPP.GROUP, message: str, profile: CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE = CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.IT) -> bool:
+                def send_to_group(group: CONST.MESSAGE.WHATSAPP.GROUP, message: str, profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles = CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.IT) -> bool:
                     return PIH.MESSAGE.WHATSAPP.WAPPI.send(group.value, message, profile)
 
                 @staticmethod
-                def get_profile_id(telephone_number: str) -> CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE:
+                def get_profile_id(telephone_number: str) -> CONST.MESSAGE.WHATSAPP.WAPPI.Profiles:
                     if PIH.CHECK.telephone_number_international(telephone_number):
                         telephone_number = PIH.DATA.FORMAT.telephone_number(telephone_number)
                     profile_id_collection = PIH.MESSAGE.WHATSAPP.WAPPI.get_wappi_collection()
                     for item in profile_id_collection:
                         if profile_id_collection[item] == telephone_number:
                             return item
                     return None
 
                 @staticmethod
                 def get_message_list(telephone_number: str, profile: Any | None = None) -> list[WhatsAppMessage]:
-                    profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                    profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                     url: str = f"{CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_MESSAGES}{profile}&chat_id={telephone_number}{CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX}"
                     headers: dict = {
                         "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION,
                         "Content-Type": "application/json"
                     }
                     result: list[WhatsAppMessage] = []
                     try:
@@ -5146,15 +5146,15 @@
                             if message_item["type"] == "chat":
                                 result.append(WhatsAppMessage(message_item["body"], message_item["fromMe"], str(message_item["from"]).split("@")[0], 
                                    str(message_item["to"]).split("@")[0], profile, message_item["time"]))
                     return result 
                 
                 @staticmethod
                 def send(telephone_number: str, message: Any, profile: Any | None = None) -> bool:
-                    profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                    profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                     url: str | None = None
                     payload: dict = {"recipient": telephone_number}
                     if isinstance(message, str):
                         payload["body"] = message
                         url: str = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_MESSAGE
                     elif isinstance(message, (WhatsAppMessageListPayload, WhatsAppMessageButtonsPayload)):
                         for item_name in message.__dataclass_fields__:
@@ -5181,15 +5181,15 @@
                             "Аккаунт Wappi (сервис для отправики сообщений через WhatsApp) не оплачен", LogMessageFlags.ERROR)
                     status_code: int = response.status_code
                     return status_code == 200
 
                 @staticmethod
                 def send_base64_file(url: str, telephone_number: str, caption: str, file_name: str | None, base64_content: str,  profile: Any | None = None) -> bool:
                     profile = EnumTool.get_value(
-                        profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                        profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                     payload: dict = {"recipient": telephone_number,
                                      "caption": caption,
                                      "b64_file": base64_content}
                     if not DataTool.is_empty(file_name):
                         payload["file_name"] = file_name   
                     headers: dict = {"accept": "application/json",
                                      "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION, "Content-Type": "application/json"}
@@ -5232,15 +5232,15 @@
                     pwk.sendwhatmsg_instantly(telephone_number, message)
                 except Exception as уrror:
                     PIH.output.error("Ошибка при отправке сообщения!")
 
             @staticmethod
             def send(telephone_number: str, message: Any, via_wappi: bool = True, use_alternative: bool = True, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
-                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                 result: bool = False
                 telephone_number = PIH.DATA.FORMAT.telephone_number(
                     telephone_number)
                 if via_wappi:
                     result = PIH.MESSAGE.WHATSAPP.WAPPI.send(
                         telephone_number, message, wappi_profile)
                 if result:
@@ -5248,38 +5248,38 @@
                 if use_alternative or not via_wappi:
                     return PIH.MESSAGE.WHATSAPP.send_via_browser(telephone_number, message)
                 return False
 
             @staticmethod
             def send_video(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
-                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                 telephone_number = PIH.DATA.FORMAT.telephone_number(telephone_number)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_video(telephone_number, caption, base64_value, wappi_profile)
 
             @staticmethod
             def send_image(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
-                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                 telephone_number = PIH.DATA.FORMAT.telephone_number(
                     telephone_number)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_image(telephone_number, caption, base64_value, wappi_profile)
         
             @staticmethod
             def send_document(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
-                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value)
                 telephone_number = PIH.DATA.FORMAT.telephone_number(
                     telephone_number)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_document(telephone_number, caption, base64_value, wappi_profile)
 
             @staticmethod
             def send_to_user(user: User, message: Any, via_wappi: bool = True, use_alternative: bool = True, wappi_profile: Any | None = None) -> bool:
                 return PIH.MESSAGE.WHATSAPP.send(user.telephoneNumber, message, via_wappi, use_alternative, EnumTool.get_value(
-                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value))
+                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT.value))
 
         class DELAYED:
 
             @staticmethod
             def register(message: DelayedMessage) -> int:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_delayed_message, PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message)))
 
@@ -5291,15 +5291,15 @@
 
         @staticmethod
         def set_folder_for_person(folder_name: str | None, person_or_pin: PolibasePerson | int, already_set: bool = False) -> bool:
             result: bool = already_set or PIH.ACTION.POLIBASE.set_card_registry_folder(folder_name, person_or_pin)
             event_builder = PIH.EVENT.BUILDER.polibase_person_set_card_registry_folder
             if result:
                 if DataTool.is_empty(folder_name):
-                    A.A_E.remove(*event_builder(None, person_or_pin))
+                    PIH.ACTION.EVENTS.remove(*event_builder(None, person_or_pin))
                     result = True
                 else:
                     event_ds: EventDS | None = ResultTool.get_first_item(PIH.RESULT.EVENTS.get(
                         *event_builder(None, person_or_pin)))
                     allow_to_add: bool = False
                     if DataTool.is_not_none(event_ds):
                         card_registry_folder: str = event_ds.parameters[FIELD_NAME_COLLECTION.CARD_REGISTRY_FOLDER]
@@ -5374,16 +5374,16 @@
         class ACTIONS:
 
             @staticmethod
             def was_done(action: Actions | str, user_login_or_user: str | User | None = None) -> bool | None:
                 user: User | None = None
                 if isinstance(user_login_or_user, User):
                     user = user_login_or_user
-                if A.D_C.empty(user_login_or_user) or isinstance(user_login_or_user, str):
-                    user = A.R_U.by_login(user_login_or_user or AD.USER.ADMINISTRATOR, True, True).data
+                if DataTool.is_empty(user_login_or_user) or isinstance(user_login_or_user, str):
+                    user = PIH.RESULT.USER.by_login(user_login_or_user or AD.USER.ADMINISTRATOR, True, True).data
                 _action: Actions | None = PIH.DATA.ACTIONS.get(action)
                 if DataTool.is_none(_action):
                     return None
                 PIH.EVENT.send(Events.ACTION_WAS_DONE, (EnumTool.get(_action).description, _action.name, user.name, user.samAccountName))
                 return True
 
             @staticmethod
@@ -5459,15 +5459,15 @@
             def send_message(value: str, recipient: str | Enum, flags: int | None = None) -> bool:    
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.send_mobile_helper_message, (value, recipient if isinstance(recipient, str) else EnumTool.get(recipient), flags)))
 
         class BACKUP:
 
             @staticmethod
             def attach_shared_disks() -> bool:
-                output: str = str(PIH.PSTOOLS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+                output: str = str(PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
                     [CONST.POWERSHELL.NAME, PATH_BACKUP.COMMAND.ATTACH_SHARED_DISKS], HOSTS.BACKUP_WORKER.NAME, interactive=None, run_from_system_account=True), True, True).stdout)
                 return output.strip().count("Attached          : True") == 2
 
             @staticmethod
             def start_robocopy_job(name: str | None = None, source: str | None = None, destination: str | None = None, force: bool = False) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.robocopy_start_job, (name, source, destination, force)))
 
@@ -5738,15 +5738,15 @@
             
             @staticmethod
             def kill_process(name_or_pid: str | int, host: str, via_taskkill: bool = True) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.kill_process, (name_or_pid, host, via_taskkill)))
             
             @staticmethod
             def kill_python_process(host: str, via_taskkill: bool = False) -> bool:
-                return PIH.ACTION.WORKSTATION.kill_process(A.CT.PYTHON.EXECUTOR, host, via_taskkill)   
+                return PIH.ACTION.WORKSTATION.kill_process(CONST.PYTHON.EXECUTOR, host, via_taskkill)   
             
             @staticmethod
             def stop_windows_service(name: str, workstation_name: str) -> bool | None:
                 accessable: bool | None = PIH.CHECK.WORKSTATION.accessibility(workstation_name)
                 if DataTool.is_none(accessable):
                     return None
                 return PIH.PSTOOLS.stop_windows_service(name, workstation_name)      
@@ -5757,16 +5757,16 @@
                 if DataTool.is_none(accessable):
                     return None
                 return PIH.PSTOOLS.start_windows_service(name, workstation_name)      
             
             @staticmethod
             def start_windows_service_if_stopped(name: str, workstation_name: str) -> bool | None:
                 windows_service_information = name, workstation_name
-                if not A.C_WS.windows_service_running(*windows_service_information):
-                    return A.A_WS.start_windows_service(*windows_service_information)
+                if not PIH.CHECK.WORKSTATION.windows_service_running(*windows_service_information):
+                    return PIH.ACTION.WORKSTATION.start_windows_service(*windows_service_information)
                 return None
 
 class ActionStack(list):
 
     def __init__(self, caption: str = "", *argv: Callable[[], ActionValue], input: InputBase = None, output: OutputBase = None):
         self.input = input or PIH.input
         self.output = output or PIH.output
```

### Comparing `pih-1.47208/pih/rpc.py` & `pih-1.47209/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/rpcCommandCall_pb2.py` & `pih-1.47209/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47209/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/rpc_collection.py` & `pih-1.47209/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/rpc_const.py` & `pih-1.47209/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/service_example.py` & `pih-1.47209/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/tools.py` & `pih-1.47209/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih/widgets.py` & `pih-1.47209/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih.egg-info/SOURCES.txt` & `pih-1.47209/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih_mio_setup.py` & `pih-1.47209/pih_mio_setup.py`

 * *Files identical despite different names*

### Comparing `pih-1.47208/pih_setup.py` & `pih-1.47209/pih_setup.py`

 * *Files identical despite different names*

