# Comparing `tmp/sanicargs-2.1.0.tar.gz` & `tmp/sanicargs-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanicargs-2.1.0.tar", last modified: Mon Dec 21 08:26:58 2020, max compression
+gzip compressed data, was "sanicargs-3.0.0.tar", max compression
```

## Comparing `sanicargs-2.1.0.tar` & `sanicargs-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1049 2020-12-21 08:26:10.849383 sanicargs-2.1.0/LICENSE
--rw-r--r--   0        0        0     3098 2020-12-21 08:26:10.849383 sanicargs-2.1.0/README.md
--rw-r--r--   0        0        0      929 2020-12-21 08:26:10.849383 sanicargs-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4345 2020-12-21 08:26:10.849383 sanicargs-2.1.0/sanicargs/__init__.py
--rw-r--r--   0        0        0       24 2020-12-21 08:26:10.849383 sanicargs-2.1.0/sanicargs/fields.py
--rw-r--r--   0        0        0     3909 2020-12-21 08:26:58.073006 sanicargs-2.1.0/setup.py
--rw-r--r--   0        0        0     4003 2020-12-21 08:26:58.073311 sanicargs-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-08-01 12:50:39.785228 sanicargs-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2922 2023-08-01 14:45:23.859602 sanicargs-3.0.0/README.md
+-rw-r--r--   0        0        0     1008 2023-08-01 14:45:23.865739 sanicargs-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3594 2023-08-01 14:45:23.868646 sanicargs-3.0.0/sanicargs/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-01 12:50:39.787169 sanicargs-3.0.0/sanicargs/fields.py
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 sanicargs-3.0.0/PKG-INFO
```

### Comparing `sanicargs-2.1.0/LICENSE` & `sanicargs-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanicargs-2.1.0/README.md` & `sanicargs-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -70,13 +70,8 @@
 
 You need to apply the `parse_parameters` decorator as the first one executed which means closest to the `def`.
 
 ### `request` is mandatory!
 
 You should always have request as the first argument in your function in order to use `parse_parameters`.
 
-**Note** that `request` arg can be renamed and even type-annotated as long as it is the first arg.
-
-### `parse_query_args` deprecation
-
-`parse_query_args` will be deprecated in future version in favor of `parse_parameters`
-Currently it is still usable as a legacy decorator
+**Note** that `request` arg can be renamed and even type-annotated as long as it is the first arg.
```

### Comparing `sanicargs-2.1.0/sanicargs/__init__.py` & `sanicargs-3.0.0/sanicargs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+import datetime
 import inspect
+import json
 from functools import wraps
+from logging import getLogger
+
 import ciso8601
-import datetime
-import json
-import warnings
+from sanic.exceptions import BadRequest
 
-from sanic import response
-from sanic.exceptions import abort
 from sanicargs.fields import List
 
-from logging import getLogger
-
 __logger = getLogger("sanicargs")
 
 
 def __parse_datetime(date_string):
     return ciso8601.parse_datetime_as_naive(date_string)
 
 
@@ -44,42 +42,23 @@
     str: str,
     datetime.datetime: __parse_datetime,
     datetime.date: __parse_date,
     List[str]: __parse_list,
 }
 
 
-def parse_query_args(func):
-    """parses query args and validates, deserializes them
-    VERY IMPORTANT!:
-    to use this decorator it must be used in a Sanic endpoint and used BEFORE the 
-    sanic blueprint decorator like so:
-        @blueprint.route("/foo/<businessunitid>/bar")
-        @authorize_business_unit
-        @parse_query_args
-    and the signature of the function needs to start with request and the rest of 
-    the parameters need type hints like so:
-        async def generate_csv(request, query: str, businessunitid: str):
-    """
-    warnings.warn(
-        "This decorator will be deprecated in the next major release",
-        DeprecationWarning,
-    )
-    return __parse(func, True)
-
-
 def parse_parameters(func):
     """parses query or body parameters depending on http method, validates and deserializes them
     VERY IMPORTANT!:
-    to use this decorator it must be used in a Sanic endpoint and used BEFORE the 
+    to use this decorator it must be used in a Sanic endpoint and used BEFORE the
     sanic blueprint decorator like so:
         @blueprint.route("/foo/<businessunitid>/bar")
         @authorize_business_unit
         @parse_parameters
-    and the signature of the function needs to start with request and the rest of 
+    and the signature of the function needs to start with request and the rest of
     the parameters need type hints like so:
         async def generate_csv(request, query: str, businessunitid: str):
     """
     return __parse(func)
 
 
 def __parse(func, legacy=False):
@@ -130,11 +109,11 @@
                 {
                     "message": f"Request {'args' if legacy else 'parameters'} not validated",
                     "name": name,
                     "raw_value": raw_value,
                     "stacktrace": str(err),
                 }
             )
-            return abort(400, "Bad or missing value for %s" % name)
+            raise BadRequest(f"Bad or missing value for {name}")
         return await func(request, **kwargs)
 
     return inner
```

### Comparing `sanicargs-2.1.0/setup.py` & `sanicargs-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,99 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sanicargs
+Version: 3.0.0
+Summary: Parses query args or body parameters in sanic using type annotations
+Home-page: https://github.com/trustpilot/python-sanicargs
+Keywords: sanicargs,sanic,query,args,type annotations
+Author: John Sutherland
+Author-email: johns@trustpilot.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ciso8601 (>=2.3.0,<3.0.0)
+Requires-Dist: sanic (>=23.6.0,<24.0.0)
+Project-URL: Repository, https://github.com/trustpilot/python-sanicargs
+Description-Content-Type: text/markdown
+
+[![Build Status](https://travis-ci.org/trustpilot/python-sanicargs.svg?branch=master)](https://travis-ci.org/trustpilot/python-sanicargs) [![Latest Version](https://img.shields.io/pypi/v/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs) [![Python Support](https://img.shields.io/pypi/pyversions/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs)
+
+# Sanicargs
+Parses query parameters and json body parameters for [Sanic](https://github.com/channelcat/sanic) using type annotations.
+
+## Survey
+Please fill out [this survey](https://docs.google.com/forms/d/e/1FAIpQLSdNLvB7NEJQhUyVdaZpBAgS0f1k9OywZp8xDqhaNY0rl-unZA/viewform?usp=sf_link) if you are using Sanicargs, we are gathering feedback :-)
+
+## Install
+Install with pip
+```
+$ pip install sanicargs
+```
+
+## Usage
+
+Use the `parse_parameters` decorator to parse query parameters (GET) or body parameters (POST) and type cast them together with path params in [Sanic](https://github.com/channelcat/sanic)'s routes or blueprints like in this [example](https://github.com/trustpilot/python-sanicargs/tree/master/examples/simple.py) below:
+
+```python
+import datetime
+from sanic import Sanic, response
+from sanicargs import parse_parameters
+
+app = Sanic("test_sanic_app")
+
+@app.route("/me/<id>/birthdate", methods=['GET'])
+@parse_parameters
+async def test_datetime(req, id: str, birthdate: datetime.datetime):
+    return response.json({
+        'id': id, 
+        'birthdate': birthdate.isoformat()
+    })
+
+if __name__ == "__main__":
+  app.run(host="0.0.0.0", port=8080, access_log=False, debug=False)
+```
+
+Test it running with 
+```bash
+$ curl 'http://0.0.0.0:8080/me/123/birthdate?birthdate=2017-10-30'
+```
+
+### Query parameters
+
+* **str** : `ex: ?message=hello world`
+* **int** : `ex: ?age=100`
+* **bool** : `ex: ?missing=false`
+* **datetime.datetime** : `ex: ?currentdate=2017-10-30T10:10:30 or 2017-10-30`
+* **datetime.date** : `ex: ?birthdate=2017-10-30`
+* **List[str]** : `ex: ?words=you,me,them,we`
+
+### JSON body parameters
+
+{
+  "message": "hello word",
+  "age": 100,
+  "missing": false,
+  "currentDate": "2017-10-30",
+  "currentDateTime": "2017-10-30T10:10:30",
+  "words": ["you", "me", "them", "we"]
+}
 
-packages = \
-['sanicargs']
+### Note about datetimes
 
-package_data = \
-{'': ['*']}
+Dates and datetimes are parsed without timezone information giving you a "naive datetime" object. See the note on [datetime.timestamp()](https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp) about handling timezones if you require epoch format timestamps.
 
-install_requires = \
-['ciso8601>=2.1.3,<3.0.0', 'sanic>=18.12']
-
-setup_kwargs = {
-    'name': 'sanicargs',
-    'version': '2.1.0',
-    'description': 'Parses query args or body parameters in sanic using type annotations',
-    'long_description': '[![Build Status](https://travis-ci.org/trustpilot/python-sanicargs.svg?branch=master)](https://travis-ci.org/trustpilot/python-sanicargs) [![Latest Version](https://img.shields.io/pypi/v/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs) [![Python Support](https://img.shields.io/pypi/pyversions/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs)\n\n# Sanicargs\nParses query parameters and json body parameters for [Sanic](https://github.com/channelcat/sanic) using type annotations.\n\n## Survey\nPlease fill out [this survey](https://docs.google.com/forms/d/e/1FAIpQLSdNLvB7NEJQhUyVdaZpBAgS0f1k9OywZp8xDqhaNY0rl-unZA/viewform?usp=sf_link) if you are using Sanicargs, we are gathering feedback :-)\n\n## Install\nInstall with pip\n```\n$ pip install sanicargs\n```\n\n## Usage\n\nUse the `parse_parameters` decorator to parse query parameters (GET) or body parameters (POST) and type cast them together with path params in [Sanic](https://github.com/channelcat/sanic)\'s routes or blueprints like in this [example](https://github.com/trustpilot/python-sanicargs/tree/master/examples/simple.py) below:\n\n```python\nimport datetime\nfrom sanic import Sanic, response\nfrom sanicargs import parse_parameters\n\napp = Sanic("test_sanic_app")\n\n@app.route("/me/<id>/birthdate", methods=[\'GET\'])\n@parse_parameters\nasync def test_datetime(req, id: str, birthdate: datetime.datetime):\n    return response.json({\n        \'id\': id, \n        \'birthdate\': birthdate.isoformat()\n    })\n\nif __name__ == "__main__":\n  app.run(host="0.0.0.0", port=8080, access_log=False, debug=False)\n```\n\nTest it running with \n```bash\n$ curl \'http://0.0.0.0:8080/me/123/birthdate?birthdate=2017-10-30\'\n```\n\n### Query parameters\n\n* **str** : `ex: ?message=hello world`\n* **int** : `ex: ?age=100`\n* **bool** : `ex: ?missing=false`\n* **datetime.datetime** : `ex: ?currentdate=2017-10-30T10:10:30 or 2017-10-30`\n* **datetime.date** : `ex: ?birthdate=2017-10-30`\n* **List[str]** : `ex: ?words=you,me,them,we`\n\n### JSON body parameters\n\n{\n  "message": "hello word",\n  "age": 100,\n  "missing": false,\n  "currentDate": "2017-10-30",\n  "currentDateTime": "2017-10-30T10:10:30",\n  "words": ["you", "me", "them", "we"]\n}\n\n### Note about datetimes\n\nDates and datetimes are parsed without timezone information giving you a "naive datetime" object. See the note on [datetime.timestamp()](https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp) about handling timezones if you require epoch format timestamps.\n\n### Important notice about decorators\n\nThe sequence of decorators is, as usual, important in Python.\n\nYou need to apply the `parse_parameters` decorator as the first one executed which means closest to the `def`.\n\n### `request` is mandatory!\n\nYou should always have request as the first argument in your function in order to use `parse_parameters`.\n\n**Note** that `request` arg can be renamed and even type-annotated as long as it is the first arg.\n\n### `parse_query_args` deprecation\n\n`parse_query_args` will be deprecated in future version in favor of `parse_parameters`\nCurrently it is still usable as a legacy decorator\n',
-    'author': 'Johannes Valbjørn',
-    'author_email': 'jgv@trustpilot.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/trustpilot/python-sanicargs',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+### Important notice about decorators
+
+The sequence of decorators is, as usual, important in Python.
+
+You need to apply the `parse_parameters` decorator as the first one executed which means closest to the `def`.
+
+### `request` is mandatory!
 
+You should always have request as the first argument in your function in order to use `parse_parameters`.
 
-setup(**setup_kwargs)
+**Note** that `request` arg can be renamed and even type-annotated as long as it is the first arg.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

