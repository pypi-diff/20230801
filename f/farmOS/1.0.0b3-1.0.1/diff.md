# Comparing `tmp/farmOS-1.0.0b3.tar.gz` & `tmp/farmOS-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pcw/Development/farmOS-development/farmOS.py/dist/tmp2m0wwidj/farmOS-1.0.0b3.tar", last modified: Mon Jul 26 17:08:44 2021, max compression
+gzip compressed data, was "farmOS-1.0.1.tar", last modified: Tue Aug  1 18:39:13 2023, max compression
```

## Comparing `farmOS-1.0.0b3.tar` & `farmOS-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pcw       (1000) pcw       (1000)        0 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/
--rw-r--r--   0 pcw       (1000) pcw       (1000)    35149 2019-10-08 04:15:52.000000 farmOS-1.0.0b3/LICENSE
--rw-r--r--   0 pcw       (1000) pcw       (1000)     7982 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/PKG-INFO
--rw-r--r--   0 pcw       (1000) pcw       (1000)     7472 2021-07-20 22:50:33.000000 farmOS-1.0.0b3/README.md
-drwxr-xr-x   0 pcw       (1000) pcw       (1000)        0 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/farmOS/
--rw-r--r--   0 pcw       (1000) pcw       (1000)     5922 2021-07-26 17:01:26.000000 farmOS-1.0.0b3/farmOS/__init__.py
--rw-r--r--   0 pcw       (1000) pcw       (1000)     8465 2021-07-20 18:45:12.000000 farmOS-1.0.0b3/farmOS/client.py
--rw-r--r--   0 pcw       (1000) pcw       (1000)     7333 2021-07-20 18:45:12.000000 farmOS-1.0.0b3/farmOS/client_2.py
--rw-r--r--   0 pcw       (1000) pcw       (1000)     5401 2021-07-26 16:57:23.000000 farmOS-1.0.0b3/farmOS/session.py
--rw-r--r--   0 pcw       (1000) pcw       (1000)     4132 2021-07-20 18:45:12.000000 farmOS-1.0.0b3/farmOS/subrequests.py
-drwxr-xr-x   0 pcw       (1000) pcw       (1000)        0 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/farmOS.egg-info/
--rw-r--r--   0 pcw       (1000) pcw       (1000)     7982 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/farmOS.egg-info/PKG-INFO
--rw-r--r--   0 pcw       (1000) pcw       (1000)      316 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/farmOS.egg-info/SOURCES.txt
--rw-r--r--   0 pcw       (1000) pcw       (1000)        1 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/farmOS.egg-info/dependency_links.txt
--rw-r--r--   0 pcw       (1000) pcw       (1000)       34 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/farmOS.egg-info/requires.txt
--rw-r--r--   0 pcw       (1000) pcw       (1000)       13 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/farmOS.egg-info/top_level.txt
--rw-r--r--   0 pcw       (1000) pcw       (1000)       63 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/setup.cfg
--rw-r--r--   0 pcw       (1000) pcw       (1000)      946 2021-07-26 17:08:02.000000 farmOS-1.0.0b3/setup.py
-drwxr-xr-x   0 pcw       (1000) pcw       (1000)        0 2021-07-26 17:08:44.000000 farmOS-1.0.0b3/tests/
--rw-r--r--   0 pcw       (1000) pcw       (1000)        0 2019-10-08 04:15:52.000000 farmOS-1.0.0b3/tests/__init__.py
--rw-r--r--   0 pcw       (1000) pcw       (1000)     2367 2021-07-20 22:28:57.000000 farmOS-1.0.0b3/tests/conftest.py
+drwxrwxr-x   0 paul121   (1000) paul121   (1000)        0 2023-08-01 18:39:13.473562 farmOS-1.0.1/
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)    35149 2021-12-10 18:08:16.000000 farmOS-1.0.1/LICENSE
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     2151 2023-08-01 18:39:13.473562 farmOS-1.0.1/PKG-INFO
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     1680 2023-03-11 01:56:12.000000 farmOS-1.0.1/README.md
+drwxrwxr-x   0 paul121   (1000) paul121   (1000)        0 2023-08-01 18:39:13.469562 farmOS-1.0.1/farmOS/
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     5922 2022-11-28 17:32:34.000000 farmOS-1.0.1/farmOS/__init__.py
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     8465 2022-11-28 17:32:34.000000 farmOS-1.0.1/farmOS/client.py
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     7494 2023-08-01 18:30:26.000000 farmOS-1.0.1/farmOS/client_2.py
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     5399 2023-08-01 18:30:26.000000 farmOS-1.0.1/farmOS/session.py
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     4217 2023-08-01 18:30:26.000000 farmOS-1.0.1/farmOS/subrequests.py
+drwxrwxr-x   0 paul121   (1000) paul121   (1000)        0 2023-08-01 18:39:13.473562 farmOS-1.0.1/farmOS.egg-info/
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     2151 2023-08-01 18:39:13.000000 farmOS-1.0.1/farmOS.egg-info/PKG-INFO
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)      316 2023-08-01 18:39:13.000000 farmOS-1.0.1/farmOS.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)        1 2023-08-01 18:39:13.000000 farmOS-1.0.1/farmOS.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)       41 2023-08-01 18:39:13.000000 farmOS-1.0.1/farmOS.egg-info/requires.txt
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)       13 2023-08-01 18:39:13.000000 farmOS-1.0.1/farmOS.egg-info/top_level.txt
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)       63 2023-08-01 18:39:13.473562 farmOS-1.0.1/setup.cfg
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)      968 2023-08-01 18:30:26.000000 farmOS-1.0.1/setup.py
+drwxrwxr-x   0 paul121   (1000) paul121   (1000)        0 2023-08-01 18:39:13.473562 farmOS-1.0.1/tests/
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)        0 2021-12-10 18:08:16.000000 farmOS-1.0.1/tests/__init__.py
+-rw-rw-r--   0 paul121   (1000) paul121   (1000)     2367 2022-11-28 17:32:34.000000 farmOS-1.0.1/tests/conftest.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `farmOS-1.0.0b3/LICENSE` & `farmOS-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `farmOS-1.0.0b3/farmOS/__init__.py` & `farmOS-1.0.1/farmOS/__init__.py`

 * *Files identical despite different names*

### Comparing `farmOS-1.0.0b3/farmOS/client.py` & `farmOS-1.0.1/farmOS/client.py`

 * *Files identical despite different names*

### Comparing `farmOS-1.0.0b3/farmOS/client_2.py` & `farmOS-1.0.1/farmOS/client_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from urllib.parse import urlparse
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class ResourceBase:
     """Base class for JSONAPI resource methods."""
@@ -40,21 +41,22 @@
         )
         more = True
         while more:
             # TODO: Should we merge in the "includes" info here?
             yield from response["data"]
             try:
                 next_url = response["links"]["next"]["href"]
-                response = self.session._http_request(url=next_url)
+                parsed_url = urlparse(next_url)
+                next_path = parsed_url._replace(scheme="", netloc="").geturl()
+                response = self.session.http_request(path=next_path)
                 response = response.json()
             except KeyError:
                 more = False
 
     def send(self, entity_type, bundle=None, payload=None):
-
         # Default to empty payload dict.
         if payload is None:
             payload = {}
 
         # Set the resource type.
         payload["type"] = self._get_resource_type(entity_type, bundle)
         json_payload = {
```

### Comparing `farmOS-1.0.0b3/farmOS/session.py` & `farmOS-1.0.1/farmOS/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         token_url=None,
         authorization_url=None,
         content_type="application/vnd.api+json",
         token_updater=None,
         *args,
         **kwargs,
     ):
-
         # Default to the "farm_manager" scope.
         if scope is None:
             scope = "farm_manager"
 
         # Create a dictionary of credentials required to pass along with Refresh Tokens
         # Required to generate a new access token
         auto_refresh_kwargs = {"client_id": client_id, "client_secret": client_secret}
@@ -109,15 +108,14 @@
         # Assemble the URL.
         url = f"{self.hostname}/{path}"
         return self._http_request(
             url=url, method=method, options=options, params=params, headers=headers
         )
 
     def _http_request(self, url, method="GET", options=None, params=None, headers=None):
-
         # Automatically follow redirects, unless this is a POST request.
         # The Python requests library converts POST to GET during a redirect.
         # Allow this to be overridden in options.
         allow_redirects = True
         if method in ["POST", "PUT"]:
             allow_redirects = False
         if options and "allow_redirects" in options:
```

### Comparing `farmOS-1.0.0b3/farmOS/subrequests.py` & `farmOS-1.0.1/farmOS/subrequests.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,39 +90,41 @@
         self.session = session
 
     def send(
         self,
         blueprint: Union[SubrequestsBlueprint, List],
         format: Optional[Union[Format, str]] = Format.json,
     ):
-
         if isinstance(blueprint, List):
             blueprint = SubrequestsBlueprint.parse_obj(blueprint)
 
         # Modify each sub-request as needed.
         for sub in blueprint.__root__:
             # Build the URI if an endpoint is provided.
             if sub.uri is None and sub.endpoint is not None:
                 sub.uri = f"{self.session.hostname}/{sub.endpoint}"
 
+            # Set the endpoint to None so it is not included in the serialized subrequest.
+            sub.endpoint = None
+
             # Auto populate headers for each sub-request.
             if "Accept" not in sub.headers:
                 sub.headers["Accept"] = "application/vnd.api+json"
             if sub.body is not None and "Content-Type" not in sub.headers:
                 sub.headers["Content-Type"] = "application/vnd.api+json"
 
         headers = {"Content-Type": "application/json"}
 
         params = {}
         if format == Format.json.value:
             params = {"_format": "json"}
 
         # Generate the json to send. It is important to use the .json() method
         # of the model for correct serialization.
-        json = blueprint.json(exclude={"subrequest": {"endpoint"}}, exclude_none=True)
+        json = blueprint.json(exclude_none=True)
         options = {"data": json}
 
         response = self.session.http_request(
             method="POST",
             path=self.subrequest_path,
             options=options,
             params=params,
```

### Comparing `farmOS-1.0.0b3/setup.py` & `farmOS-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import setuptools
 
 setup_requires = [
     "pytest-runner",
 ]
 
-install_requires = ["requests-oauthlib", "pydantic>=1.7.3"]
+install_requires = ["requests-oauthlib~=1.3.1", "pydantic~=1.7.3"]
 
-tests_require = ["pytest", "black>=20"]
+tests_require = ["pytest", "black~=23.0", "setuptools~=68.0"]
 
 with open("README.md") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="farmOS",
-    version="1.0.0-beta.3",
+    version="1.0.1",
     author="farmOS team",
     author_email="mike@mstenta.net",
     description="A Python library for interacting with farmOS over API. ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/farmOS/farmOS.py",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     setup_requires=setup_requires,
     install_requires=install_requires,
     tests_require=tests_require,
     test_suite="pytest",
 )
```

### Comparing `farmOS-1.0.0b3/tests/conftest.py` & `farmOS-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

