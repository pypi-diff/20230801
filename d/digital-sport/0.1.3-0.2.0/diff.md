# Comparing `tmp/digital-sport-0.1.3.tar.gz` & `tmp/digital-sport-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-sport-0.1.3.tar", last modified: Sun May  1 06:57:39 2022, max compression
+gzip compressed data, was "digital-sport-0.2.0.tar", last modified: Tue Aug  1 11:55:22 2023, max compression
```

## Comparing `digital-sport-0.1.3.tar` & `digital-sport-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-05-01 06:57:39.438819 digital-sport-0.1.3/
--rw-rw-r--   0 repente   (1000) repente   (1000)       13 2022-04-30 18:44:35.000000 digital-sport-0.1.3/MANIFEST.in
--rw-rw-r--   0 repente   (1000) repente   (1000)     2183 2022-05-01 06:57:39.438819 digital-sport-0.1.3/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)     1888 2021-09-18 18:41:50.000000 digital-sport-0.1.3/README.md
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-05-01 06:57:39.406812 digital-sport-0.1.3/digital_sport.egg-info/
--rw-rw-r--   0 repente   (1000) repente   (1000)     2183 2022-05-01 06:57:39.000000 digital-sport-0.1.3/digital_sport.egg-info/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      325 2022-05-01 06:57:39.000000 digital-sport-0.1.3/digital_sport.egg-info/SOURCES.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        1 2022-05-01 06:57:39.000000 digital-sport-0.1.3/digital_sport.egg-info/dependency_links.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        9 2022-05-01 06:57:39.000000 digital-sport-0.1.3/digital_sport.egg-info/requires.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        6 2022-05-01 06:57:39.000000 digital-sport-0.1.3/digital_sport.egg-info/top_level.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       38 2022-05-01 06:57:39.438819 digital-sport-0.1.3/setup.cfg
--rw-rw-r--   0 repente   (1000) repente   (1000)     2456 2022-04-30 20:38:35.000000 digital-sport-0.1.3/setup.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-05-01 06:57:39.438819 digital-sport-0.1.3/sport/
--rw-rw-r--   0 repente   (1000) repente   (1000)      678 2022-04-30 18:33:06.000000 digital-sport-0.1.3/sport/abstract.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     9209 2022-04-30 20:12:59.000000 digital-sport-0.1.3/sport/api.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     2992 2022-04-30 18:33:06.000000 digital-sport-0.1.3/sport/interface.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      982 2022-04-30 18:33:06.000000 digital-sport-0.1.3/sport/report_service.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     4267 2022-04-30 18:33:06.000000 digital-sport-0.1.3/sport/search_center.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1172 2022-04-30 18:33:06.000000 digital-sport-0.1.3/sport/tool.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-08-01 11:55:22.005082 digital-sport-0.2.0/
+-rw-rw-r--   0 repente   (1000) repente   (1000)       13 2022-04-30 18:44:35.000000 digital-sport-0.2.0/MANIFEST.in
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2139 2023-08-01 11:55:22.005082 digital-sport-0.2.0/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1844 2023-08-01 10:36:21.000000 digital-sport-0.2.0/README.md
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-08-01 11:55:22.005082 digital-sport-0.2.0/digital_sport.egg-info/
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2139 2023-08-01 11:55:21.000000 digital-sport-0.2.0/digital_sport.egg-info/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      343 2023-08-01 11:55:21.000000 digital-sport-0.2.0/digital_sport.egg-info/SOURCES.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        1 2023-08-01 11:55:21.000000 digital-sport-0.2.0/digital_sport.egg-info/dependency_links.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        9 2023-08-01 11:55:21.000000 digital-sport-0.2.0/digital_sport.egg-info/requires.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        6 2023-08-01 11:55:21.000000 digital-sport-0.2.0/digital_sport.egg-info/top_level.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       38 2023-08-01 11:55:22.005082 digital-sport-0.2.0/setup.cfg
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2453 2023-08-01 11:55:17.000000 digital-sport-0.2.0/setup.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-08-01 11:55:22.005082 digital-sport-0.2.0/sport/
+-rw-rw-r--   0 repente   (1000) repente   (1000)       99 2023-08-01 10:45:10.000000 digital-sport-0.2.0/sport/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      678 2022-04-30 18:33:06.000000 digital-sport-0.2.0/sport/abstract.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     9345 2023-08-01 10:41:32.000000 digital-sport-0.2.0/sport/api.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     7290 2023-08-01 11:10:06.000000 digital-sport-0.2.0/sport/interface.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      982 2023-08-01 10:41:32.000000 digital-sport-0.2.0/sport/report_service.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     4267 2023-08-01 10:41:32.000000 digital-sport-0.2.0/sport/search_center.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1172 2022-04-30 18:33:06.000000 digital-sport-0.2.0/sport/tool.py
```

### Comparing `digital-sport-0.1.3/PKG-INFO` & `digital-sport-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 Metadata-Version: 2.1
 Name: digital-sport
-Version: 0.1.3
+Version: 0.2.0
 Summary: Sport Api - structured data.
 Home-page: https://github.com/repen/digital-sport
 Author: Andrey Plugin
 Author-email: 9keepa@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### Описание
 
 Получение структурированной информации по спортивным  live событиям.
 
-Очень важно, все данные доступны в live режиме. 
+Очень важно, все данные доступны в live режиме. Данные только по футболу.
 
 Нельзя получать данные по матчам которые уже:
 - сыграны
 - запланированы
 
+
 ### Установка
 
 1. `pip install digital-sport`
 
-2. Для работы библиотеки нужен апи токен, который дает доступ к информации.
-	
 
-Апи токен можно получить:
-    
-- в телеграм боте @sport_api_bot (/help).
-- на сайте [data-provider.ru](https://data-provider.ru).
+Вопросы по работе библиотеки:
 
-#### Установить токен
+- help in telegram `@sport_user`
+    
 
-```
-from sport.api import FootballSport
+#### Получить live матчи.
 
-token = "Your token"
-football = FootballSport(token, debug=True)
 ```
+from sport import FootballSport
 
-#### Получить live матчи.
+football = FootballSport()
 
-```
 fixtures = football.live()
+
 print(fixtures)
 ```
 
 #### Получить статистику по мачту.
 
 Необходим id матча.
 
@@ -81,7 +76,13 @@
 Работа в многопоточном режиме.
 Необходимо передать в метод список live матчей. 
 
 ```
 fixtures = football.add_statistics(fixtures)
 ```
 
+#### Цели
+
+- [ ] Реализовать интерфейс к live событиям по теннису.
+- [ ] Реализовать интерфейс к live событиям по баскетболу.
+
+
```

### Comparing `digital-sport-0.1.3/README.md` & `digital-sport-0.2.0/digital_sport.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,49 @@
+Metadata-Version: 2.1
+Name: digital-sport
+Version: 0.2.0
+Summary: Sport Api - structured data.
+Home-page: https://github.com/repen/digital-sport
+Author: Andrey Plugin
+Author-email: 9keepa@gmail.com
+License: MIT
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 ### Описание
 
 Получение структурированной информации по спортивным  live событиям.
 
-Очень важно, все данные доступны в live режиме. 
+Очень важно, все данные доступны в live режиме. Данные только по футболу.
 
 Нельзя получать данные по матчам которые уже:
 - сыграны
 - запланированы
 
+
 ### Установка
 
 1. `pip install digital-sport`
 
-2. Для работы библиотеки нужен апи токен, который дает доступ к информации.
-	
 
-Апи токен можно получить:
-    
-- в телеграм боте @sport_api_bot (/help).
-- на сайте [data-provider.ru](https://data-provider.ru).
+Вопросы по работе библиотеки:
 
-#### Установить токен
+- help in telegram `@sport_user`
+    
 
-```
-from sport.api import FootballSport
+#### Получить live матчи.
 
-token = "Your token"
-football = FootballSport(token, debug=True)
 ```
+from sport import FootballSport
 
-#### Получить live матчи.
+football = FootballSport()
 
-```
 fixtures = football.live()
+
 print(fixtures)
 ```
 
 #### Получить статистику по мачту.
 
 Необходим id матча.
 
@@ -67,8 +74,15 @@
 
 Для матчей у которых имеется статистика к этим объектам добавится их статистика.
 Работа в многопоточном режиме.
 Необходимо передать в метод список live матчей. 
 
 ```
 fixtures = football.add_statistics(fixtures)
-```
+```
+
+#### Цели
+
+- [ ] Реализовать интерфейс к live событиям по теннису.
+- [ ] Реализовать интерфейс к live событиям по баскетболу.
+
+
```

### Comparing `digital-sport-0.1.3/setup.py` & `digital-sport-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Импорт недавно установленного пакета setuptools.
 # Upload package to PyPi.
-# python3 setup.py sdist bdist_wheel
-# python3 -m twine upload --repository testpypi dist/*
-# python3 -m twine upload --repository pypi dist/*
+# python setup.py sdist bdist_wheel
+# python -m twine upload --repository testpypi dist/*
+# python -m twine upload --repository pypi dist/*
 from setuptools import setup
 
 # Открытие README.md и присвоение его long_description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Функция, которая принимает несколько аргументов. Она присваивает эти значения пакету.
 setup(
     # Имя дистрибутива пакета. Оно должно быть уникальным, поэтому добавление вашего имени пользователя в конце является обычным делом.
     name="digital-sport",
     # Номер версии вашего пакета. Обычно используется семантическое управление версиями.
-    version="0.1.3",
+    version="0.2.0",
     # Имя автора.
     author="Andrey Plugin",
     # Его почта.
     author_email="9keepa@gmail.com",
     # Краткое описание, которое будет показано на странице PyPi.
     description="Sport Api - structured data.",
     # Длинное описание, которое будет отображаться на странице PyPi. Использует README.md репозитория для заполнения.
```

### Comparing `digital-sport-0.1.3/sport/abstract.py` & `digital-sport-0.2.0/sport/abstract.py`

 * *Files identical despite different names*

### Comparing `digital-sport-0.1.3/sport/api.py` & `digital-sport-0.2.0/sport/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 Copyright (c) 2022 Plugin Andrey (9keepa@gmail.com)
 Licensed under the MIT License
 """
+import re
+import requests
 from typing import List
+from functools import partial
+from concurrent.futures import ThreadPoolExecutor
 from .abstract import AbstractSport
-import requests
 from .tool import log
 from .search_center import H2hSearch, SearchStatistics
 from .report_service import ReportService
 from .interface import IStatistics
-from concurrent.futures import ThreadPoolExecutor
-import re
-from functools import partial
 
 
 logger = log(__name__)
-_FOOTBALL_URL = "https://static.data-provider.ru/api/v1/fsfootball"
-_BASKETBALL_URL = "https://static.data-provider.ru/api/v1/fsbasketball"
-_TENNIS_URL = "https://static.data-provider.ru/api/v1/fstennis"
+_FOOTBALL_URL = "http://82.146.63.207:1080/api/v1/flashscore_football"
+_BASKETBALL_URL = None
+_TENNIS_URL = None
+
 
+class TemporaryNotAvailableError(Exception):
+    pass
 
 class ListWrapper(list):
     def __init__(self, ll, method_name, cls):
         super(ListWrapper, self).__init__(ll)
         self.method_name = method_name
         self.cls: FootballSport = cls
 
@@ -166,15 +169,15 @@
         return wrapper
 
     return _list_wrapper
 
 
 class FootballSport(AbstractSport):
 
-    def __init__(self, token: str, debug=False, requests_params=None):
+    def __init__(self, token: str="Free-token", debug=False, requests_params=None):
         self.request_limit = None
         self.reset_limit = None
         self.token = token
         self.debug = debug
         self.headers = {
             'X-Service-Key': self.token
         }
@@ -189,16 +192,16 @@
                                 headers=self.headers, **self.requests_params)
         if response.status_code == 404:
             raise ValueError(f"Resource [{route}] not found!")
         if response.status_code == 401:
             raise ValueError(f"{response.headers.get('WWW-Authenticate')}")
         self.request_limit = response.headers.get("X-Day-Limit-Value")
         self.reset_limit = response.headers.get("X-Day-Limit-Reset")
-        if self.debug:
-            logger.info(f"Requests limit: {self.request_limit}")
+        if False:
+            logger.debug(f"Requests limit: {self.request_limit}")
         return response
 
     @list_wrapper("statistics")
     def statistics(self, match_id: str):
         route = "/statistics/" + match_id
         response = self._request(route)
         return response.json()
@@ -243,13 +246,15 @@
         return fixtures
 
 
 class BasketballSport(FootballSport):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.base_url = _BASKETBALL_URL
+        raise TemporaryNotAvailableError("the class is temporarily unavailable")
 
 
 class TennisSport(FootballSport):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.base_url = _TENNIS_URL
+        self.base_url = _TENNIS_URL
+        raise TemporaryNotAvailableError("the class is temporarily unavailable")
```

### Comparing `digital-sport-0.1.3/sport/report_service.py` & `digital-sport-0.2.0/sport/report_service.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Copyright (c) 2022 Plugin Andrey (9keepa@gmail.com)
 Licensed under the MIT License
 """
-from typing import List, Any
 import csv
 import json
+from typing import List, Any
 
 class ReportService:
 
     def __init__(self, objects_list: List[Any]):
         self.objects_list = objects_list
 
     def csv_dump(self, path, encoding="utf8"):
```

### Comparing `digital-sport-0.1.3/sport/search_center.py` & `digital-sport-0.2.0/sport/search_center.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Copyright (c) 2022 Plugin Andrey (9keepa@gmail.com)
 Licensed under the MIT License
 """
 from typing import Callable, List
-from .interface import Ih2h, IStatistics
 from functools import partial
+from .interface import Ih2h, IStatistics
 
 
 def pprint(string, match_id:str):
     if match_id:
         string = f"{match_id}: {string}"
     print(string)
```

### Comparing `digital-sport-0.1.3/sport/tool.py` & `digital-sport-0.2.0/sport/tool.py`

 * *Files identical despite different names*

