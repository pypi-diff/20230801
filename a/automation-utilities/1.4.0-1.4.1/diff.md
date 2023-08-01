# Comparing `tmp/automation-utilities-1.4.0.tar.gz` & `tmp/automation-utilities-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.4.0.tar", last modified: Mon Jul 31 01:13:11 2023, max compression
+gzip compressed data, was "automation-utilities-1.4.1.tar", last modified: Tue Aug  1 18:46:12 2023, max compression
```

## Comparing `automation-utilities-1.4.0.tar` & `automation-utilities-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 01:13:11.734111 automation-utilities-1.4.0/
-drwxrwxrwx   0        0        0        0 2023-07-31 01:13:11.731839 automation-utilities-1.4.0/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-07-31 01:13:11.732969 automation-utilities-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 01:13:11.723885 automation-utilities-1.4.0/automation_utilities/
--rw-rw-rw-   0        0        0      186 2023-07-19 17:03:31.000000 automation-utilities-1.4.0/automation_utilities/Control.py
--rw-rw-rw-   0        0        0     1628 2023-07-28 20:33:25.000000 automation-utilities-1.4.0/automation_utilities/Data.py
--rw-rw-rw-   0        0        0       82 2023-07-20 19:25:23.000000 automation-utilities-1.4.0/automation_utilities/Exceptions.py
--rw-rw-rw-   0        0        0      936 2023-07-18 19:42:13.000000 automation-utilities-1.4.0/automation_utilities/Files.py
--rw-rw-rw-   0        0        0     1918 2023-07-30 08:46:44.000000 automation-utilities-1.4.0/automation_utilities/FiveSim.py
--rw-rw-rw-   0        0        0        0 2023-07-20 19:11:30.000000 automation-utilities-1.4.0/automation_utilities/Generator.py
--rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.4.0/automation_utilities/Input.py
--rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.4.0/automation_utilities/PhoneNumbers.py
--rw-rw-rw-   0        0        0      525 2023-07-20 19:11:30.000000 automation-utilities-1.4.0/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0     2195 2023-07-21 18:11:32.000000 automation-utilities-1.4.0/automation_utilities/mailtm.py
--rw-rw-rw-   0        0        0       42 2023-07-31 01:13:11.734111 automation-utilities-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      307 2023-07-31 01:13:06.000000 automation-utilities-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:46:12.033702 automation-utilities-1.4.1/
+drwxrwxrwx   0        0        0        0 2023-08-01 18:46:12.031069 automation-utilities-1.4.1/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-08-01 18:46:11.000000 automation-utilities-1.4.1/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-08-01 18:46:11.000000 automation-utilities-1.4.1/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 18:46:11.000000 automation-utilities-1.4.1/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-01 18:46:11.000000 automation-utilities-1.4.1/Automation_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-01 18:46:11.000000 automation-utilities-1.4.1/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-08-01 18:46:12.033196 automation-utilities-1.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 18:46:12.024377 automation-utilities-1.4.1/automation_utilities/
+-rw-rw-rw-   0        0        0      186 2023-07-19 17:03:31.000000 automation-utilities-1.4.1/automation_utilities/Control.py
+-rw-rw-rw-   0        0        0     1628 2023-07-28 20:33:25.000000 automation-utilities-1.4.1/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:25:23.000000 automation-utilities-1.4.1/automation_utilities/Exceptions.py
+-rw-rw-rw-   0        0        0      936 2023-07-18 19:42:13.000000 automation-utilities-1.4.1/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0     2045 2023-08-01 18:30:38.000000 automation-utilities-1.4.1/automation_utilities/FiveSim.py
+-rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.4.1/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0     2392 2023-08-01 17:45:22.000000 automation-utilities-1.4.1/automation_utilities/MailTM.py
+-rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.4.1/automation_utilities/PhoneNumbers.py
+-rw-rw-rw-   0        0        0      525 2023-07-20 19:11:30.000000 automation-utilities-1.4.1/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 18:46:12.033702 automation-utilities-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      307 2023-08-01 18:45:55.000000 automation-utilities-1.4.1/setup.py
```

### Comparing `automation-utilities-1.4.0/Automation_Utilities.egg-info/SOURCES.txt` & `automation-utilities-1.4.1/Automation_Utilities.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 Automation_Utilities.egg-info/dependency_links.txt
 Automation_Utilities.egg-info/top_level.txt
 automation_utilities/Control.py
 automation_utilities/Data.py
 automation_utilities/Exceptions.py
 automation_utilities/Files.py
 automation_utilities/FiveSim.py
-automation_utilities/Generator.py
 automation_utilities/Input.py
+automation_utilities/MailTM.py
 automation_utilities/PhoneNumbers.py
 automation_utilities/__init__.py
 automation_utilities/mailtm.py
 automation_utilities.egg-info/PKG-INFO
 automation_utilities.egg-info/SOURCES.txt
 automation_utilities.egg-info/dependency_links.txt
 automation_utilities.egg-info/requires.txt
```

### Comparing `automation-utilities-1.4.0/automation_utilities/Data.py` & `automation-utilities-1.4.1/automation_utilities/Data.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.4.0/automation_utilities/Files.py` & `automation-utilities-1.4.1/automation_utilities/Files.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.4.0/automation_utilities/FiveSim.py` & `automation-utilities-1.4.1/automation_utilities/FiveSim.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 DOMAIN = "5sim.net"
 
 
 class Phone:
     def __init__(self, number_id, phone):
         self.id = number_id
-        self.phone = phone
+        self.number = phone
 
 
 class FiveSim:
     def __init__(self, token):
         self.headers = {
             'Authorization': 'Bearer ' + token,
             'Accept': 'application/json',
@@ -22,21 +22,25 @@
         return response.json()['balance']
 
     def buy_activation_number(self, country: str, operator: str, product: str):
         url = f'https://{DOMAIN}/v1/user/buy/activation/{country}/{operator}/{product}'
         response = requests.get(url, headers=self.headers).json()
         return Phone(response['id'], response['phone'][1:])
 
-    def get_codes(self, phone: Phone):
+    def get_codes(self, phone: Phone, timeout: float = 30):
+        start = time.time()
         while True:
             try:
                 response = requests.get(f'https://{DOMAIN}/v1/user/check/{phone.id}', headers=self.headers).json()
                 return [sms['code'] for sms in response['sms']]
             except (ValueError, IndexError):
-                time.sleep(1)
+                pass
+
+            if time.time() - start > timeout:
+                raise TimeoutError
 
 
 def min_cost_providers(country: str, product: str):
     response = requests.get(f'https://{DOMAIN}/v1/guest/prices?country={country}&product={product}').json()
     operators0 = []
     for operator in response[country][product]:
         if response[country][product][operator]['count'] != 0:
```

### Comparing `automation-utilities-1.4.0/automation_utilities/PhoneNumbers.py` & `automation-utilities-1.4.1/automation_utilities/PhoneNumbers.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.4.0/automation_utilities/__init__.py` & `automation-utilities-1.4.1/automation_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.4.0/automation_utilities/mailtm.py` & `automation-utilities-1.4.1/automation_utilities/MailTM.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,30 +32,34 @@
             try:
                 token = requests.post('https://api.mail.tm/token', json=data).json()['token']
                 break
             except JSONDecodeError:
                 pass
         self.headers = {'Authorization': f"Bearer {token}"}
 
-    def messages(self):
+    def messages(self, timeout: float = 30):
+        start = time.time()
         while True:
             while True:
                 try:
                     resoponse = requests.get('https://api.mail.tm/messages', headers=self.headers).json()
                     break
                 except JSONDecodeError:
                     pass
+                if time.time() - start > timeout:
+                    raise TimeoutError
             if resoponse['hydra:totalItems'] > 0:
                 messages = []
                 for member in resoponse['hydra:member']:
                     url = f'https://api.mail.tm/messages/{member["id"]}'
                     while True:
                         try:
                             messages.append(requests.get(url, headers=self.headers).json()['html'])
                             break
                         except JSONDecodeError:
                             pass
                 if resoponse['hydra:totalItems'] == 1:
                     return messages[0][0]
                 else:
                     return messages[0]
-            time.sleep(1)
+            if time.time() - start > timeout:
+                raise TimeoutError
```

