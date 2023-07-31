# Comparing `tmp/opet-0.0.8.tar.gz` & `tmp/opet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opet-0.0.8.tar", last modified: Sun Jul 30 21:36:16 2023, max compression
+gzip compressed data, was "opet-0.0.9.tar", last modified: Mon Jul 31 22:59:33 2023, max compression
```

## Comparing `opet-0.0.8.tar` & `opet-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 21:36:16.073233 opet-0.0.8/
--rw-r--r--   0 btcyz255   (501) staff       (20)     1069 2023-07-30 14:59:51.000000 opet-0.0.8/LICENSE
--rw-r--r--   0 btcyz255   (501) staff       (20)     1384 2023-07-30 21:36:16.072978 opet-0.0.8/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)      910 2023-07-30 21:35:55.000000 opet-0.0.8/README.md
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 21:36:16.069039 opet-0.0.8/opet/
--rw-r--r--   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:11:51.000000 opet-0.0.8/opet/__init__.py
--rw-r--r--   0 btcyz255   (501) staff       (20)     1448 2023-07-30 21:25:02.000000 opet-0.0.8/opet/api.py
--rw-r--r--   0 btcyz255   (501) staff       (20)      130 2023-07-30 21:13:49.000000 opet-0.0.8/opet/exceptions.py
--rw-r--r--   0 btcyz255   (501) staff       (20)      310 2023-07-30 21:35:26.000000 opet-0.0.8/opet/main.py
--rw-r--r--   0 btcyz255   (501) staff       (20)     1005 2023-07-30 21:26:13.000000 opet-0.0.8/opet/utils.py
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 21:36:16.072505 opet-0.0.8/opet.egg-info/
--rw-r--r--   0 btcyz255   (501) staff       (20)     1384 2023-07-30 21:36:15.000000 opet-0.0.8/opet.egg-info/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)      271 2023-07-30 21:36:15.000000 opet-0.0.8/opet.egg-info/SOURCES.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 21:36:15.000000 opet-0.0.8/opet.egg-info/dependency_links.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)       43 2023-07-30 21:36:15.000000 opet-0.0.8/opet.egg-info/entry_points.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)       15 2023-07-30 21:36:15.000000 opet-0.0.8/opet.egg-info/requires.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        5 2023-07-30 21:36:15.000000 opet-0.0.8/opet.egg-info/top_level.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)       38 2023-07-30 21:36:16.073297 opet-0.0.8/setup.cfg
--rw-r--r--   0 btcyz255   (501) staff       (20)      892 2023-07-30 21:36:07.000000 opet-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:59:33.461540 opet-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 22:59:21.000000 opet-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-31 22:59:33.461540 opet-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 22:59:21.000000 opet-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:59:33.461540 opet-0.0.9/opet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:59:21.000000 opet-0.0.9/opet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-31 22:59:21.000000 opet-0.0.9/opet/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 22:59:21.000000 opet-0.0.9/opet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 22:59:21.000000 opet-0.0.9/opet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 22:59:21.000000 opet-0.0.9/opet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:59:33.461540 opet-0.0.9/opet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-31 22:59:33.000000 opet-0.0.9/opet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 22:59:33.000000 opet-0.0.9/opet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:59:33.000000 opet-0.0.9/opet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 22:59:33.000000 opet-0.0.9/opet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 22:59:33.000000 opet-0.0.9/opet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 22:59:33.000000 opet-0.0.9/opet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:59:33.461540 opet-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-31 22:59:21.000000 opet-0.0.9/setup.py
```

### Comparing `opet-0.0.8/LICENSE` & `opet-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opet-0.0.8/PKG-INFO` & `opet-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opet
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package that allows you to view fuel prices in Turkey based on cities.
 Home-page: https://github.com/sinanerdinc/opet
 Author: Sinan Erdinc
 Author-email: hello@sinanerdinc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,26 +23,24 @@
 
 Projeyi isterseniz aşağıdaki şekilde bir kütüphane olarak kullanabilirsiniz, veya opet-cli üzerinden terminalden kullanabilirsiniz.
 
 ```
 client = OpetApiClient()
 
 print(client.get_provinces())
-print(client.get_districts(28))
-print(client.get_price("028002"))
+print(client.get_price("55"))
 ```
+### get_last_update
+En son güncellemenin ne zaman olduğunu görebilirsiniz.
 
 ### get_provinces
 Sistemde yakıt fiyatlarını çekmek için kullanabileceğiniz il ve kodlarını getirir.
 
-### get_districts
-Parametre olarak vereceğiniz il kodu sonrasında o ildeki ilçeleri getirir.
-
-### get_price
-Parametre olarak vereceğiniz ilçe kodu ile o ilçedeki yakıt fiyatlarına ulaşabilirsiniz.
+### price
+Parametre olarak vereceğiniz il kodu ile o ildeki yakıt fiyatlarına ulaşabilirsiniz.
 
 ## opet-cli
 Terminal üzerinden plaka kodu parametresi geçerek yakıt fiyatlarını json formatında görebilirsiniz.
 
 ```
 opet-cli --il 34
 ```
```

### Comparing `opet-0.0.8/README.md` & `opet-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 
 Projeyi isterseniz aşağıdaki şekilde bir kütüphane olarak kullanabilirsiniz, veya opet-cli üzerinden terminalden kullanabilirsiniz.
 
 ```
 client = OpetApiClient()
 
 print(client.get_provinces())
-print(client.get_districts(28))
-print(client.get_price("028002"))
+print(client.get_price("55"))
 ```
+### get_last_update
+En son güncellemenin ne zaman olduğunu görebilirsiniz.
 
 ### get_provinces
 Sistemde yakıt fiyatlarını çekmek için kullanabileceğiniz il ve kodlarını getirir.
 
-### get_districts
-Parametre olarak vereceğiniz il kodu sonrasında o ildeki ilçeleri getirir.
-
-### get_price
-Parametre olarak vereceğiniz ilçe kodu ile o ilçedeki yakıt fiyatlarına ulaşabilirsiniz.
+### price
+Parametre olarak vereceğiniz il kodu ile o ildeki yakıt fiyatlarına ulaşabilirsiniz.
 
 ## opet-cli
 Terminal üzerinden plaka kodu parametresi geçerek yakıt fiyatlarını json formatında görebilirsiniz.
 
 ```
 opet-cli --il 34
 ```
```

### Comparing `opet-0.0.8/opet/api.py` & `opet-0.0.9/opet/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-from opet.utils import yesterday, http_get, to_json
+from opet.utils import http_get, to_json
 from opet.exceptions import ProvinceNotFoundError
 
 class OpetApiClient:
     def __init__(self):
         self.url = "https://api.opet.com.tr/api/fuelprices"
 
+    def get_last_update(self):
+        return http_get(f"{self.url}/lastupdate")
+
     def get_provinces(self):
         return http_get(f"{self.url}/provinces")
 
-    def get_districts(self, province_id):
-        return http_get(f"{self.url}/provinces/{province_id}/districts")
-
-    def get_price(self, district_id: str):
-        date = yesterday()
-        url = f"{self.url}/prices/archive?DistrictCode={district_id}&StartDate={date}&EndDate={date}&IncludeAllProducts=true"
+    def get_price(self, province_id: str):
+        url = f"{self.url}/prices?ProvinceCode={province_id}&IncludeAllProducts=true"
         r = http_get(url)
         response = list(map(lambda x: dict(name=x["productName"], amount=x["amount"]), r[0]["prices"]))
         return response
 
     def price(self, province_id: str):
         _provinces = self.get_provinces()
         formatted_provinces = {str(item['code']): item['name'] for item in _provinces}
         province_name = formatted_provinces.get(f"{province_id}", None)
         if province_name is None:
             raise ProvinceNotFoundError(f"Sistemde {province_id} plaka koduna ait bir il bulunamadı.")
 
         result = dict(
             results=dict(
                 province=province_name,
-                prices=self.get_price(self.get_districts(province_id)[0]["code"])
+                lastUpdate=self.get_last_update()["lastUpdateDate"],
+                prices=self.get_price(province_id)
             )
         )
         return to_json(result)
 
 
 if __name__ == '__main__':
     client = OpetApiClient()
+    print(client.get_provinces())
+    print(client.get_price("28"))
     print(client.price("28"))
```

### Comparing `opet-0.0.8/opet.egg-info/PKG-INFO` & `opet-0.0.9/opet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opet
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package that allows you to view fuel prices in Turkey based on cities.
 Home-page: https://github.com/sinanerdinc/opet
 Author: Sinan Erdinc
 Author-email: hello@sinanerdinc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,26 +23,24 @@
 
 Projeyi isterseniz aşağıdaki şekilde bir kütüphane olarak kullanabilirsiniz, veya opet-cli üzerinden terminalden kullanabilirsiniz.
 
 ```
 client = OpetApiClient()
 
 print(client.get_provinces())
-print(client.get_districts(28))
-print(client.get_price("028002"))
+print(client.get_price("55"))
 ```
+### get_last_update
+En son güncellemenin ne zaman olduğunu görebilirsiniz.
 
 ### get_provinces
 Sistemde yakıt fiyatlarını çekmek için kullanabileceğiniz il ve kodlarını getirir.
 
-### get_districts
-Parametre olarak vereceğiniz il kodu sonrasında o ildeki ilçeleri getirir.
-
-### get_price
-Parametre olarak vereceğiniz ilçe kodu ile o ilçedeki yakıt fiyatlarına ulaşabilirsiniz.
+### price
+Parametre olarak vereceğiniz il kodu ile o ildeki yakıt fiyatlarına ulaşabilirsiniz.
 
 ## opet-cli
 Terminal üzerinden plaka kodu parametresi geçerek yakıt fiyatlarını json formatında görebilirsiniz.
 
 ```
 opet-cli --il 34
 ```
```

### Comparing `opet-0.0.8/setup.py` & `opet-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="opet",
     author="Sinan Erdinc",
     author_email="hello@sinanerdinc.com",
-    version="0.0.8",
+    version="0.0.9",
     install_requires=["requests", "click"],
     description="A Python package that allows you to view fuel prices in Turkey based on cities.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sinanerdinc/opet",
     classifiers=[
         "Programming Language :: Python :: 3",
```

