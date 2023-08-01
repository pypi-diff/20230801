# Comparing `tmp/callbackin-0.8.0.tar.gz` & `tmp/callbackin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callbackin-0.8.0.tar", max compression
+gzip compressed data, was "callbackin-0.9.0.tar", max compression
```

## Comparing `callbackin-0.8.0.tar` & `callbackin-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.8.0/README.md
--rw-r--r--   0        0        0       21 2023-06-18 07:21:15.268375 callbackin-0.8.0/callbackin/__init__.py
--rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.8.0/callbackin/__main__.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.8.0/callbackin/handler/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-17 12:25:13.371198 callbackin-0.8.0/callbackin/handler/callback.py
--rw-r--r--   0        0        0     1954 2023-06-18 07:09:18.773367 callbackin-0.8.0/callbackin/handler/login.py
--rw-r--r--   0        0        0     4829 2023-06-18 07:21:02.539144 callbackin-0.8.0/callbackin/main.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.8.0/callbackin/schemas/__init__.py
--rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.8.0/callbackin/schemas/callback.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.8.0/callbackin/utils/__init__.py
--rw-r--r--   0        0        0     1607 2023-06-18 07:12:34.471642 callbackin-0.8.0/callbackin/utils/config.py
--rw-r--r--   0        0        0     1708 2023-06-18 07:11:10.976813 callbackin-0.8.0/callbackin/utils/request.py
--rw-r--r--   0        0        0      440 2023-06-18 07:21:08.146358 callbackin-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.9.0/README.md
+-rw-r--r--   0        0        0       21 2023-08-01 16:04:17.507618 callbackin-0.9.0/callbackin/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.9.0/callbackin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.9.0/callbackin/handler/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-17 12:25:13.371198 callbackin-0.9.0/callbackin/handler/callback.py
+-rw-r--r--   0        0        0     1954 2023-06-18 07:09:18.773367 callbackin-0.9.0/callbackin/handler/login.py
+-rw-r--r--   0        0        0     4915 2023-08-01 16:04:19.782017 callbackin-0.9.0/callbackin/main.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.9.0/callbackin/schemas/__init__.py
+-rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.9.0/callbackin/schemas/callback.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.9.0/callbackin/utils/__init__.py
+-rw-r--r--   0        0        0     1607 2023-06-18 07:12:34.471642 callbackin-0.9.0/callbackin/utils/config.py
+-rw-r--r--   0        0        0     1708 2023-06-18 07:11:10.976813 callbackin-0.9.0/callbackin/utils/request.py
+-rw-r--r--   0        0        0      440 2023-08-01 16:04:45.041248 callbackin-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.9.0/PKG-INFO
```

### Comparing `callbackin-0.8.0/README.md` & `callbackin-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `callbackin-0.8.0/callbackin/handler/callback.py` & `callbackin-0.9.0/callbackin/handler/callback.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.8.0/callbackin/handler/login.py` & `callbackin-0.9.0/callbackin/handler/login.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.8.0/callbackin/main.py` & `callbackin-0.9.0/callbackin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         "name": name,
         "local_endpoint": local_endpoint,
         "description": description,
     })
     if response.status_code == 200:
         callback = Callback(**response.json())
         typer.echo(f"Using This URL to use your endpoint: {get_base_url()}/handle/{callback.path}")
+        typer.echo(f"Start callback with this command: callbackin run {callback.id}")
     else:
         typer.echo("Error creating callback")
 
 @app.command("list")
 def list_callbacks():
     typer.echo("Listing callbacks")
     response = get("/callbacks")
```

### Comparing `callbackin-0.8.0/callbackin/utils/config.py` & `callbackin-0.9.0/callbackin/utils/config.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.8.0/callbackin/utils/request.py` & `callbackin-0.9.0/callbackin/utils/request.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.8.0/PKG-INFO` & `callbackin-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callbackin
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Author: ibrahim4529
 Author-email: ibrahim.hanif4529@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

