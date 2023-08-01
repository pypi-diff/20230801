# Comparing `tmp/tortoise-api-0.2.4.tar.gz` & `tmp/tortoise-api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.2.4.tar", last modified: Mon Jul 31 11:51:37 2023, max compression
+gzip compressed data, was "tortoise-api-0.2.5.tar", last modified: Tue Aug  1 10:47:31 2023, max compression
```

## Comparing `tortoise-api-0.2.4.tar` & `tortoise-api-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:51:37.040105 tortoise-api-0.2.4/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.4/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-31 11:51:37.039869 tortoise-api-0.2.4/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.4/README.md
--rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-31 11:50:56.000000 tortoise-api-0.2.4/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 11:51:37.040166 tortoise-api-0.2.4/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:51:37.038347 tortoise-api-0.2.4/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.4/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     3527 2023-07-31 11:49:15.000000 tortoise-api-0.2.4/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)     3069 2023-07-31 11:44:47.000000 tortoise-api-0.2.4/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:51:37.039592 tortoise-api-0.2.4/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-01 10:47:31.836737 tortoise-api-0.2.5/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.5/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-08-01 10:47:31.836489 tortoise-api-0.2.5/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.5/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      686 2023-08-01 10:47:00.000000 tortoise-api-0.2.5/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-08-01 10:47:31.836801 tortoise-api-0.2.5/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-01 10:47:31.832932 tortoise-api-0.2.5/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.5/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     3540 2023-07-31 13:36:53.000000 tortoise-api-0.2.5/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)     3069 2023-07-31 11:44:47.000000 tortoise-api-0.2.5/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-01 10:47:31.836185 tortoise-api-0.2.5/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       66 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.2.4/LICENSE` & `tortoise-api-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.4/PKG-INFO` & `tortoise-api-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `tortoise-api-0.2.4/README.md` & `tortoise-api-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.4/pyproject.toml` & `tortoise-api-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 dependencies = [
     "asyncpg",
     "python-dotenv",
     "starlette",
     "tortoise-api-model>=0.1.0",
     "uvicorn"
 ]
-version = "0.2.4"
+version = "0.2.5"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.2.4/tortoise_api/api.py` & `tortoise-api-0.2.5/tortoise_api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     async def api_menu(self, _: Request):
         return JSONResponse(list(self.models))
 
     async def all_create(self, request: Request):
         model: type[Model] = self._get_model(request)
         if request.method == 'POST':
             data = parse_qs(await request.body())
-            m2ms = {k: data.pop(k) for k in model._meta.m2m_fields}
+            m2ms = {k: data.pop(k) for k in model._meta.m2m_fields if k in data}
             obj: Model = await model.create(**data)
             for k, ids in m2ms.items():
                 m2m_rel: ManyToManyRelation = getattr(obj, k)
                 items = [await m2m_rel.remote_model[i] for i in ids]
                 await m2m_rel.add(*items)
             return RedirectResponse('/'+model.__name__, 303) # create # {True: 201, False: 202}[res[1]]
         objects: [Model] = await model.all().prefetch_related(*model._meta.fetch_fields)
```

### Comparing `tortoise-api-0.2.4/tortoise_api/util.py` & `tortoise-api-0.2.5/tortoise_api/util.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.4/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.2.5/tortoise_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

