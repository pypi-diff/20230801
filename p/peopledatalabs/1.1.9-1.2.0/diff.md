# Comparing `tmp/peopledatalabs-1.1.9.tar.gz` & `tmp/peopledatalabs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopledatalabs-1.1.9.tar", max compression
+gzip compressed data, was "peopledatalabs-1.2.0.tar", max compression
```

## Comparing `peopledatalabs-1.1.9.tar` & `peopledatalabs-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-07-17 18:03:42.940434 peopledatalabs-1.1.9/LICENSE
--rw-r--r--   0        0        0    12222 2023-07-17 18:03:42.940434 peopledatalabs-1.1.9/README.md
--rw-r--r--   0        0        0     1637 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/__init__.py
--rw-r--r--   0        0        0     5754 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/__init__.py
--rw-r--r--   0        0        0     1635 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/company.py
--rw-r--r--   0        0        0      762 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/location.py
--rw-r--r--   0        0        0     2812 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/person.py
--rw-r--r--   0        0        0      744 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/school.py
--rw-r--r--   0        0        0      314 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/errors.py
--rw-r--r--   0        0        0      984 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/logger.py
--rw-r--r--   0        0        0     5048 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/main.py
--rw-r--r--   0        0        0     2445 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/__init__.py
--rw-r--r--   0        0        0     2198 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/company.py
--rw-r--r--   0        0        0      215 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/location.py
--rw-r--r--   0        0        0     4349 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/person.py
--rw-r--r--   0        0        0      783 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/school.py
--rw-r--r--   0        0        0     2241 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/requests.py
--rw-r--r--   0        0        0     1139 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/settings.py
--rw-r--r--   0        0        0      460 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/utils.py
--rw-r--r--   0        0        0    13628 1970-01-01 00:00:00.000000 peopledatalabs-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-01 20:29:45.706542 peopledatalabs-1.2.0/LICENSE
+-rw-r--r--   0        0        0    12608 2023-08-01 20:29:45.706542 peopledatalabs-1.2.0/README.md
+-rw-r--r--   0        0        0     1637 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/__init__.py
+-rw-r--r--   0        0        0     5754 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/endpoints/__init__.py
+-rw-r--r--   0        0        0     1635 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/endpoints/company.py
+-rw-r--r--   0        0        0      762 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/endpoints/location.py
+-rw-r--r--   0        0        0     2812 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/endpoints/person.py
+-rw-r--r--   0        0        0      744 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/endpoints/school.py
+-rw-r--r--   0        0        0      314 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/errors.py
+-rw-r--r--   0        0        0      984 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/logger.py
+-rw-r--r--   0        0        0     5825 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/main.py
+-rw-r--r--   0        0        0     2703 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/models/__init__.py
+-rw-r--r--   0        0        0     2198 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/models/company.py
+-rw-r--r--   0        0        0      215 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/models/location.py
+-rw-r--r--   0        0        0     4349 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/models/person.py
+-rw-r--r--   0        0        0      783 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/models/school.py
+-rw-r--r--   0        0        0     2241 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/requests.py
+-rw-r--r--   0        0        0     1139 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/settings.py
+-rw-r--r--   0        0        0      460 2023-08-01 20:29:45.710542 peopledatalabs-1.2.0/src/peopledatalabs/utils.py
+-rw-r--r--   0        0        0    14014 1970-01-01 00:00:00.000000 peopledatalabs-1.2.0/PKG-INFO
```

### Comparing `peopledatalabs-1.1.9/LICENSE` & `peopledatalabs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/README.md` & `peopledatalabs-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,30 @@
     print(
         f"Status: {result.status_code}"
         f"\nReason: {result.reason}"
         f"\nMessage: {result.json()['error']['message']}"
     )
 ```
 
+#### Get IP Enrichment
+
+```python
+result = client.ip(
+    ip="72.212.42.169",
+)
+if result.ok:
+    print(result.text)
+else:
+    print(
+        f"Status: {result.status_code};"
+        f"\nReason: {result.reason};"
+        f"\nMessage: {result.json()['error']['message']};"
+    )
+```
+
 ## 🏝 Sandbox Usage <a name="sandbox"></a>
 #### To enable sandbox usage, use the sandbox flag on PDLPY
 
 ```python
 PDLPY(sandbox=True)
 ```
 
@@ -411,14 +427,15 @@
 | --------------------------------------------------------------------------------------- | ---------------------------------- |
 | [Autocomplete API](https://docs.peopledatalabs.com/docs/autocomplete-api)               | `PDLPY.autocomplete(**params)`     |
 | [Company Cleaner API](https://docs.peopledatalabs.com/docs/cleaner-apis#companyclean)   | `PDLPY.company.cleaner(**params)`  |
 | [Location Cleaner API](https://docs.peopledatalabs.com/docs/cleaner-apis#locationclean) | `PDLPY.location.cleaner(**params)` |
 | [School Cleaner API](https://docs.peopledatalabs.com/docs/cleaner-apis#schoolclean)     | `PDLPY.school.cleaner(**params)`   |
 | [Job Title Enrichment API](https://docs.peopledatalabs.com/docs/job-title-enrichment-api) | `PDLPY.job_title(**params)` |
 | [Skill Enrichment API](https://docs.peopledatalabs.com/docs/skill-enrichment-api) | `PDLPY.skill(**params)` |
+| [IP Enrichment API](https://docs.peopledatalabs.com/docs/ip-enrichment-api) | `PDLPY.ip(**params)` |
 
 ## 📘 Documentation <a name="documentation"></a>
 
 All of our API endpoints are documented at: https://docs.peopledatalabs.com/
 
 These docs describe the supported input parameters, output responses and also provide additional technical context.
```

#### html2text {}

```diff
@@ -81,20 +81,23 @@
 f"\nReason: {result.reason}" f"\nMessage: {result.json()['error']['message']}"
 ) ``` #### Get Job Title Enrichment ```python result = client.job_title
 ( job_title="data scientist", ) if result.ok: print(result.text) else: print
 ( f"Status: {result.status_code}" f"\nReason: {result.reason}" f"\nMessage:
 {result.json()['error']['message']}" ) ``` #### Get Skill Enrichment ```python
 result = client.skill( skill="c++", ) if result.ok: print(result.text) else:
 print( f"Status: {result.status_code}" f"\nReason: {result.reason}"
-f"\nMessage: {result.json()['error']['message']}" ) ``` ## ð Sandbox Usage
-#### To enable sandbox usage, use the sandbox flag on PDLPY ```python PDLPY
-(sandbox=True) ``` ## ð Endpoints  **Person Endpoints** | API Endpoint |
-PDLPY Function | | ------------------------------------------------------------
--------------------------- | ----------------------------------- | | [Person
-Enrichment API](https://docs.peopledatalabs.com/docs/enrichment-api) |
+f"\nMessage: {result.json()['error']['message']}" ) ``` #### Get IP Enrichment
+```python result = client.ip( ip="72.212.42.169", ) if result.ok: print
+(result.text) else: print( f"Status: {result.status_code};" f"\nReason:
+{result.reason};" f"\nMessage: {result.json()['error']['message']};" ) ``` ##
+ð Sandbox Usage  #### To enable sandbox usage, use the sandbox flag on PDLPY
+```python PDLPY(sandbox=True) ``` ## ð Endpoints  **Person Endpoints** | API
+Endpoint | PDLPY Function | | -------------------------------------------------
+------------------------------------- | ----------------------------------- | |
+[Person Enrichment API](https://docs.peopledatalabs.com/docs/enrichment-api) |
 `PDLPY.person.enrichment(**params)` | | [Person Bulk Enrichment API](https://
 docs.peopledatalabs.com/docs/bulk-enrichment-api) | `PDLPY.person.bulk
 (**params)` | | [Person Search API](https://docs.peopledatalabs.com/docs/
 search-api) | `PDLPY.person.search(**params)` | | [Person Retrieve API](https:/
 /docs.peopledatalabs.com/docs/person-retrieve-api) | `PDLPY.person.retrieve
 (**params)` | | [Person Identify API](https://docs.peopledatalabs.com/docs/
 identify-api) | `PDLPY.person.identify(**params)` | **Company Endpoints** | API
@@ -112,21 +115,23 @@
 `PDLPY.company.cleaner(**params)` | | [Location Cleaner API](https://
 docs.peopledatalabs.com/docs/cleaner-apis#locationclean) |
 `PDLPY.location.cleaner(**params)` | | [School Cleaner API](https://
 docs.peopledatalabs.com/docs/cleaner-apis#schoolclean) | `PDLPY.school.cleaner
 (**params)` | | [Job Title Enrichment API](https://docs.peopledatalabs.com/
 docs/job-title-enrichment-api) | `PDLPY.job_title(**params)` | | [Skill
 Enrichment API](https://docs.peopledatalabs.com/docs/skill-enrichment-api) |
-`PDLPY.skill(**params)` | ## ð Documentation  All of our API endpoints are
-documented at: https://docs.peopledatalabs.com/ These docs describe the
-supported input parameters, output responses and also provide additional
-technical context. As illustrated in the [Endpoints](#endpoints) section above,
-each of our API endpoints is mapped to a specific method in the PDLPY class.
-For each of these class methods, **all function inputs are mapped as input
-parameters to the respective API endpoint**, meaning that you can use the API
-documentation linked above to determine the input parameters for each endpoint.
-As an example: The following is **valid** because `name` is a [supported input
-parameter to the Person Identify API](https://docs.peopledatalabs.com/docs/
-identify-api-reference#input-parameters): ```python PDLPY().person.identify(
-{"name": "sean thorne"}) ``` Conversely, this would be **invalid** because
-`fake_parameter` is not an input parameter to the Person Identify API:
-```python PDLPY().person.identify({"fake_parameter": "anything"}) ```
+`PDLPY.skill(**params)` | | [IP Enrichment API](https://
+docs.peopledatalabs.com/docs/ip-enrichment-api) | `PDLPY.ip(**params)` | ##
+ð Documentation  All of our API endpoints are documented at: https://
+docs.peopledatalabs.com/ These docs describe the supported input parameters,
+output responses and also provide additional technical context. As illustrated
+in the [Endpoints](#endpoints) section above, each of our API endpoints is
+mapped to a specific method in the PDLPY class. For each of these class
+methods, **all function inputs are mapped as input parameters to the respective
+API endpoint**, meaning that you can use the API documentation linked above to
+determine the input parameters for each endpoint. As an example: The following
+is **valid** because `name` is a [supported input parameter to the Person
+Identify API](https://docs.peopledatalabs.com/docs/identify-api-
+reference#input-parameters): ```python PDLPY().person.identify({"name": "sean
+thorne"}) ``` Conversely, this would be **invalid** because `fake_parameter` is
+not an input parameter to the Person Identify API: ```python PDLPY
+().person.identify({"fake_parameter": "anything"}) ```
```

### Comparing `peopledatalabs-1.1.9/pyproject.toml` & `peopledatalabs-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peopledatalabs"
-version = "1.1.9"
+version = "1.2.0"
 description = "Official Python client for the People Data Labs API"
 homepage = "https://www.peopledatalabs.com"
 repository = "https://github.com/peopledatalabs/peopledatalabs-python"
 documentation = "https://docs.peopledatalabs.com"
 keywords = [
   "data enrichment",
   "people data labs",
@@ -36,15 +36,15 @@
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.7"
 black = "^23.3.0"
 coverage = "^7.2.7"
 docformatter = "^1.7"
 flake8 = "^5.0.4"
-pylint = "^2.17.4"
+pylint = "^2.17.5"
 pytest = "^7.4.0"
 pyupgrade = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/__init__.py` & `peopledatalabs-1.2.0/src/peopledatalabs/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/company.py` & `peopledatalabs-1.2.0/src/peopledatalabs/endpoints/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/location.py` & `peopledatalabs-1.2.0/src/peopledatalabs/endpoints/location.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/person.py` & `peopledatalabs-1.2.0/src/peopledatalabs/endpoints/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/school.py` & `peopledatalabs-1.2.0/src/peopledatalabs/endpoints/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/logger.py` & `peopledatalabs-1.2.0/src/peopledatalabs/logger.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/main.py` & `peopledatalabs-1.2.0/src/peopledatalabs/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .endpoints import Endpoint
 from .endpoints.person import Person
 from .endpoints.company import Company
 from .endpoints.location import Location
 from .endpoints.school import School
 from .logger import get_logger
-from .models import AutocompleteModel, JobTitleModel, SkillModel
+from .models import AutocompleteModel, JobTitleModel, SkillModel, IPModel
 from .requests import Request
 from .settings import settings
 from .utils import check_empty_parameters
 
 
 logger = get_logger()
 
@@ -148,14 +148,41 @@
                 "User-Agent": "PDL-PYTHON-SDK",
                 "Content-Type": "application/json",
             },
             params=kwargs,
             validator=JobTitleModel,
         ).get()
 
+    @check_empty_parameters
+    def ip(self, **kwargs):
+        """
+        Calls PeopleDataLabs' IP Enrichment API.
+
+        Args:
+            **kwargs: Parameters for the API as defined
+                in the documentation.
+
+        Returns:
+            A requests.Response object with the result of the HTTP call.
+        """
+        url = Endpoint(self.api_key, self.base_path).get_url(
+            endpoint="ip/enrich"
+        )
+        return Request(
+            api_key=self.api_key,
+            url=url,
+            headers={
+                "Accept-Encoding": "gzip",
+                "User-Agent": "PDL-PYTHON-SDK",
+                "Content-Type": "application/json",
+            },
+            params=kwargs,
+            validator=IPModel,
+        ).get()
+
     @property
     def company(self):
         """
         Calls API from the company section.
         """
         return Company(self.api_key, self.base_path)
```

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/models/__init__.py` & `peopledatalabs-1.2.0/src/peopledatalabs/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -107,7 +107,20 @@
 
 class JobTitleModel(BaseRequestModel):
     """
     Validator model for job_title API.
     """
 
     job_title: str
+
+
+class IPModel(BaseModel):
+    """
+    Validator model for ip API.
+    """
+
+    ip: str
+    return_ip_metadata: Optional[bool]
+    return_ip_location: Optional[bool]
+    return_person: Optional[bool]
+    pretty: Optional[bool]
+    titlecase: Optional[bool]
```

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/models/company.py` & `peopledatalabs-1.2.0/src/peopledatalabs/models/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/models/person.py` & `peopledatalabs-1.2.0/src/peopledatalabs/models/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/models/school.py` & `peopledatalabs-1.2.0/src/peopledatalabs/models/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/requests.py` & `peopledatalabs-1.2.0/src/peopledatalabs/requests.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/src/peopledatalabs/settings.py` & `peopledatalabs-1.2.0/src/peopledatalabs/settings.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.9/PKG-INFO` & `peopledatalabs-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peopledatalabs
-Version: 1.1.9
+Version: 1.2.0
 Summary: Official Python client for the People Data Labs API
 Home-page: https://www.peopledatalabs.com
 License: MIT
 Keywords: data enrichment,people data labs,person enrichment,company enrichment,search
 Author: People Data Labs
 Author-email: hello@peopledatalabs.com
 Requires-Python: >=3.7.2,<4.0.0
@@ -405,14 +405,30 @@
     print(
         f"Status: {result.status_code}"
         f"\nReason: {result.reason}"
         f"\nMessage: {result.json()['error']['message']}"
     )
 ```
 
+#### Get IP Enrichment
+
+```python
+result = client.ip(
+    ip="72.212.42.169",
+)
+if result.ok:
+    print(result.text)
+else:
+    print(
+        f"Status: {result.status_code};"
+        f"\nReason: {result.reason};"
+        f"\nMessage: {result.json()['error']['message']};"
+    )
+```
+
 ## 🏝 Sandbox Usage <a name="sandbox"></a>
 #### To enable sandbox usage, use the sandbox flag on PDLPY
 
 ```python
 PDLPY(sandbox=True)
 ```
 
@@ -441,14 +457,15 @@
 | --------------------------------------------------------------------------------------- | ---------------------------------- |
 | [Autocomplete API](https://docs.peopledatalabs.com/docs/autocomplete-api)               | `PDLPY.autocomplete(**params)`     |
 | [Company Cleaner API](https://docs.peopledatalabs.com/docs/cleaner-apis#companyclean)   | `PDLPY.company.cleaner(**params)`  |
 | [Location Cleaner API](https://docs.peopledatalabs.com/docs/cleaner-apis#locationclean) | `PDLPY.location.cleaner(**params)` |
 | [School Cleaner API](https://docs.peopledatalabs.com/docs/cleaner-apis#schoolclean)     | `PDLPY.school.cleaner(**params)`   |
 | [Job Title Enrichment API](https://docs.peopledatalabs.com/docs/job-title-enrichment-api) | `PDLPY.job_title(**params)` |
 | [Skill Enrichment API](https://docs.peopledatalabs.com/docs/skill-enrichment-api) | `PDLPY.skill(**params)` |
+| [IP Enrichment API](https://docs.peopledatalabs.com/docs/ip-enrichment-api) | `PDLPY.ip(**params)` |
 
 ## 📘 Documentation <a name="documentation"></a>
 
 All of our API endpoints are documented at: https://docs.peopledatalabs.com/
 
 These docs describe the supported input parameters, output responses and also provide additional technical context.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.9 Summary: Official
+Metadata-Version: 2.1 Name: peopledatalabs Version: 1.2.0 Summary: Official
 Python client for the People Data Labs API Home-page: https://
 www.peopledatalabs.com License: MIT Keywords: data enrichment,people data
 labs,person enrichment,company enrichment,search Author: People Data Labs
 Author-email: hello@peopledatalabs.com Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -101,20 +101,23 @@
 f"\nReason: {result.reason}" f"\nMessage: {result.json()['error']['message']}"
 ) ``` #### Get Job Title Enrichment ```python result = client.job_title
 ( job_title="data scientist", ) if result.ok: print(result.text) else: print
 ( f"Status: {result.status_code}" f"\nReason: {result.reason}" f"\nMessage:
 {result.json()['error']['message']}" ) ``` #### Get Skill Enrichment ```python
 result = client.skill( skill="c++", ) if result.ok: print(result.text) else:
 print( f"Status: {result.status_code}" f"\nReason: {result.reason}"
-f"\nMessage: {result.json()['error']['message']}" ) ``` ## ð Sandbox Usage
-#### To enable sandbox usage, use the sandbox flag on PDLPY ```python PDLPY
-(sandbox=True) ``` ## ð Endpoints  **Person Endpoints** | API Endpoint |
-PDLPY Function | | ------------------------------------------------------------
--------------------------- | ----------------------------------- | | [Person
-Enrichment API](https://docs.peopledatalabs.com/docs/enrichment-api) |
+f"\nMessage: {result.json()['error']['message']}" ) ``` #### Get IP Enrichment
+```python result = client.ip( ip="72.212.42.169", ) if result.ok: print
+(result.text) else: print( f"Status: {result.status_code};" f"\nReason:
+{result.reason};" f"\nMessage: {result.json()['error']['message']};" ) ``` ##
+ð Sandbox Usage  #### To enable sandbox usage, use the sandbox flag on PDLPY
+```python PDLPY(sandbox=True) ``` ## ð Endpoints  **Person Endpoints** | API
+Endpoint | PDLPY Function | | -------------------------------------------------
+------------------------------------- | ----------------------------------- | |
+[Person Enrichment API](https://docs.peopledatalabs.com/docs/enrichment-api) |
 `PDLPY.person.enrichment(**params)` | | [Person Bulk Enrichment API](https://
 docs.peopledatalabs.com/docs/bulk-enrichment-api) | `PDLPY.person.bulk
 (**params)` | | [Person Search API](https://docs.peopledatalabs.com/docs/
 search-api) | `PDLPY.person.search(**params)` | | [Person Retrieve API](https:/
 /docs.peopledatalabs.com/docs/person-retrieve-api) | `PDLPY.person.retrieve
 (**params)` | | [Person Identify API](https://docs.peopledatalabs.com/docs/
 identify-api) | `PDLPY.person.identify(**params)` | **Company Endpoints** | API
@@ -132,21 +135,23 @@
 `PDLPY.company.cleaner(**params)` | | [Location Cleaner API](https://
 docs.peopledatalabs.com/docs/cleaner-apis#locationclean) |
 `PDLPY.location.cleaner(**params)` | | [School Cleaner API](https://
 docs.peopledatalabs.com/docs/cleaner-apis#schoolclean) | `PDLPY.school.cleaner
 (**params)` | | [Job Title Enrichment API](https://docs.peopledatalabs.com/
 docs/job-title-enrichment-api) | `PDLPY.job_title(**params)` | | [Skill
 Enrichment API](https://docs.peopledatalabs.com/docs/skill-enrichment-api) |
-`PDLPY.skill(**params)` | ## ð Documentation  All of our API endpoints are
-documented at: https://docs.peopledatalabs.com/ These docs describe the
-supported input parameters, output responses and also provide additional
-technical context. As illustrated in the [Endpoints](#endpoints) section above,
-each of our API endpoints is mapped to a specific method in the PDLPY class.
-For each of these class methods, **all function inputs are mapped as input
-parameters to the respective API endpoint**, meaning that you can use the API
-documentation linked above to determine the input parameters for each endpoint.
-As an example: The following is **valid** because `name` is a [supported input
-parameter to the Person Identify API](https://docs.peopledatalabs.com/docs/
-identify-api-reference#input-parameters): ```python PDLPY().person.identify(
-{"name": "sean thorne"}) ``` Conversely, this would be **invalid** because
-`fake_parameter` is not an input parameter to the Person Identify API:
-```python PDLPY().person.identify({"fake_parameter": "anything"}) ```
+`PDLPY.skill(**params)` | | [IP Enrichment API](https://
+docs.peopledatalabs.com/docs/ip-enrichment-api) | `PDLPY.ip(**params)` | ##
+ð Documentation  All of our API endpoints are documented at: https://
+docs.peopledatalabs.com/ These docs describe the supported input parameters,
+output responses and also provide additional technical context. As illustrated
+in the [Endpoints](#endpoints) section above, each of our API endpoints is
+mapped to a specific method in the PDLPY class. For each of these class
+methods, **all function inputs are mapped as input parameters to the respective
+API endpoint**, meaning that you can use the API documentation linked above to
+determine the input parameters for each endpoint. As an example: The following
+is **valid** because `name` is a [supported input parameter to the Person
+Identify API](https://docs.peopledatalabs.com/docs/identify-api-
+reference#input-parameters): ```python PDLPY().person.identify({"name": "sean
+thorne"}) ``` Conversely, this would be **invalid** because `fake_parameter` is
+not an input parameter to the Person Identify API: ```python PDLPY
+().person.identify({"fake_parameter": "anything"}) ```
```

